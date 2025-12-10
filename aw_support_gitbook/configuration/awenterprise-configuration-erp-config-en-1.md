---
description: "EN-CONFIG-AW_Enterprise_9"
---


After that, only inward goods for purchase orders can be entered that are assigned to the current company. An entry of company-spanning inward goods is not possible.
The rack numbers that are entered on the "Rack assignment" dialog are company-spanning. Thus you cannot enter rack 1 for company 100 and then rack 1 for company 110.
If after the starting of the module you make a company change (^F4 – User configuration – Company change), you will be informed by a message that this company change will only become active after you restart the module.

---
## Call of PPS Webservice methods in the AWE export service

The URL of the PPS Webservice to be called can be stored company-specifically in the env variables `AWC_URL_PPS_WEBSERVICE`. Thus using an export service, it is possible to address several production systems.

## Determination/updating of the AWP registration point in AWE by the export service

By inserting a special record into the table `exportinfo`, the export service can be commanded to determine the current registration points from AWP.

The determination of the registration points can be limited in the registration point types. The limitation is placed via the environment variable `AWC_ALCIMERFSTELLEN_TYP`. The type entries in the variables must be numeric and separated with commas.

If during the determination of the registration point via the PPS Webservice by the production system, the export service does not receive any registration points, the current entries in the table `AWC_ALCIMERFSTELLEN` remain untouched.

If the production system via the PPS Webservice provides at least one registration point, the content of `AWC_ALCIMERFSTELLEN` is deleted completely and the new data record(s) are inserted.

For detailed information about the determination or updating of registration point, please contact your planner.

### Configuration

The determination/'updating of the registration points is started by the entry in the table `EXPORTINFO`.

For the insert, the fields `SCHNITTSTELLE`, `HAUS` and `SHORTWERT1` must be filled:

**SCHNITTSTELLE:**
is assigned the string '`ERFSTELLENALCIM`'

**HAUS:**
Contains the sites for which the registration point determination is done. Using `HAUS` the company-specific env variables `AWC_URL_PPS_WEBSERVICE` und `AWC_ALCIMERFSTELLEN_TYP` that can be stored are evaluated. Thus it is possible via various PPS Webservices to determine registration points from different production systems for different registration points. haus also specifies the site that is entered in `AWC_ALCIMERFSTELLEN` if the determination of the registration points is done company-specifically (see `SHORTWERT1`).

**SHORTWERT1:**
A value of 1 indicates that all registration points determined company-specifically should be written to `AWC_ALCIMERFSTELLEN`. With a value != 1 the company number in the table `AWC_ALCIMERFSTELLEN` is filled with 0 (single-site logic).

### 58.4. External receipt of goods (e.g. SAP)

The detailed description is in the "EN-CONFIG-A+W Enterprise EDI" configuration guide.

## 59. Declaration of performance

As of 1 July 2013, the European Construction Products Regulation prescribes that all manufacturers and intermediate dealers in the EU issue, manage, and provide declarations of performance (DoP for short).

The configuration instructions for the declaration of performance (DOP) is in a separate document "EN-CONFIG-A+W Enterprise DOP".

## 60. Special Intauf types

### 60.1. Cost calculation (KOSTENKALKEK -15)

This intauf type is used in the course of Multi-step cost write-back for suborders. Hereby,

### 60.2. New total (FORALL_SUM -20)

With this intauf type, the item values are recalculated based on the existing price and discounts.
`vorrabatt`, `nachlass`, `rabatt`, `npospreis`, `ekpospreis`

Then the document total values (quantities, prices) are re-totaled based on the item values.
`nettototal`, `ektotal`, `mwstbetrag`, `gesbrutto`, `skontierbar`

For delivery notes, the Delivery surcharge is also re-calculated depending on the configuration.

Since some discounts relate to the re-calculated values, existing discounts are recalculated and distributed.
`kaufrab`, `kposerloes`, `kposekerloes`.

### 60.3. ENERGY SURCHARGE update (-26)

When creating a document, the discounts from the master data are determined and saved within the transaction data.

Now values in the master data can change (e.g. increase of the energy surcharge). If the user wants such a change to affect the existing documents, this can now be implemented with the background process 'intauf'.

In order to re-determine the discounts of a particular method for a document, first the environment variable `RABATTMETHODEN_UPDATE` has to be set. All methods to be updated have to be stored there, separated by a pipe.

**Procedure:**

This logic checks whether the document contains a record of this method. If so, and if this record has not been deleted or changed, the discounts of this method will be recalculated for this document. In sales, the sales and cost sides are handled separately. That is, that for a document that has a manually changed sales record and an unchanged cost record, the purchasing records for this method are determined anew.

In order to communicate to intauf that the discounts should be updated for a particular document, this has to be stored in the database table "aufint".

After the discounts are recalculated as described above, the item revenues and total document values are recalculated.

**CAUTION:** If this is done constantly, e.g. in the vorgangs_sql, attention has to be paid to the adherence to the automatic process chains specified by A+W!

**RABATTMETHODEN_UPDATE (client reference: no)**
If the new discount logic (`RABATTLOGIK_2005`) is activated, it is controlled using this variable which discount methods (table 'rabattmeth') are updated or added by the Intauf types -26 and -28 (case #113069). The individual methods have to be entered here separated by"|".
QR11/2022: Adjustment to the "Sales – Document Change" menu

### 60.4. Adding ENERGY SURCHARGE (-28)

When creating a document, the discounts from the master data are determined and saved within the transaction data.

New surcharges or discounts in the form of new discount methods are being introduced constantly. By default, the discounts for these methods are only present in the documents that are entered after the creation of the associated master data or were changed decisively. The background process 'intauf' now offers a possibility for determining discounts for these new methods also for existing documents.

In order to re-determine the discounts of a particular method for a document, first the environment variable `RABATTMETHODEN_UPDATE` has to be set. All methods to be updated have to be stored there, separated by a pipe.

**Procedure:**

If for this logic within the document, no record of the method exists, the discounts of this method are re-determined for this document. In sales, the sales and cost sides are also separated with this logic. That is, for a document that has only one sales record, the purchasing records for this method have to be determined anew.

After the discounts are recalculated as described above, the item revenues and total document values are recalculated.

**CAUTION:** If this is done constantly, e.g. in the `vorgangs_sql`, attention has to be paid to the adherence to the automatic process chains specified by A+W!

**RABATTMETHODEN_UPDATE (client reference: no)**
If the new discount logic (`RABATTLOGIK_2005`) is activated, it is controlled using this variable which discount methods (table 'rabattmeth') are updated or added by the Intauf types -26 and -28 (case #113069). The individual methods have to be entered here separated by"|".
QR11/2022: Adjustment to the "Sales – Document Change" menu

### 60.5. Book invoice (-33 RECHNUNG_BUCHEN)

#350373
Unbooked invoices are booked.

### 60.6. Recalculate discount (-37)

#174433
There is an Intaufart (-37) recalculates - based on master data - the discounts for cases converted from the old discount logic, and then recalculates the entire case. Unlike former Intauf types, this one takes all discount methods into account. This means that all master data-related discounts will be deleted before they are completely recalculated. Manually added discounts will be kept. Manual changes of master-data related discounts (made at order entry) will be lost however. In the process, only existing discount records are reworked. If discount records in kaufrab are missing because they were deleted or new discounts were created later, they will not be created.

If after recalculation based on the new discounts, the net amount (`kauf.nettototal`) differs from the old one, the following entry will be made in `log rab2005*`:
ATTENTION to case `<kauf.auftrnr>-<kauf.vorgang>-<kauf.subnr>`: Calculated '`kauf.nettototal`' (`<kauf.nettototal>`) differs from the one before recalculating with the new discount logic (`<old kauf.nettototal>`)!

If the environment variable `RABATTERMITTLUNG_NETTO_GLEICH` has been set, cases for which the net total would be changed, will be rejected; in addition to the log entry, the database transaction is reset in Intauf.

These cases should be checked by hand. The differences may result from:
- Rounding errors
- Changed master data entries.
- Discounts no longer exist in master data.

Cases in which the net total has been changed after recalculation, now get - in addition to the log entry in a file - an entry in the database table `CU_DIFFVORGRAB` (if it does not exist, it will be created by the program). This extension was made because information from a database table can be analyzed easier than log file entries.

The table has to have the following structure:

| Column name | Type | Nulls |
| :--- | :--- | :--- |
| auftrnr | integer | yes |
| aufnr | integer | yes |
| vorgang | smallint | yes |
| subnr | smallint | yes |
| neuernettototal | decimal(16) | yes |
| alternettototal | decimal(16) | yes |

In addition to the new function, these three Intauf types (-26,-28,-37) will be checked for data consistency; the following aspects will be checked:
- `kauf.gesnetto` - `<total kaufrab.betrag>` = `kauf.nettototal`
- `kauf.nettototal` + `kauf.mwstbetrag` = `kauf.gesbrutto`
- `kaufrab.grundwert` * `kaufrab.wert` = +/- `kaufrab.betrag` (/100 for `KLEINE_RABATTWERTE`)

If this check fails, the ALCIB - system report id= 2 will be dispatched; the case will be locked (kauf.still -60). The case can be unlocked only by a manual change of database. In this case, a severe error has occurred of which ALCIB service has to be informed. This consistency check can be switched off via environment variable (`NO_CHECK_CONSISTENCY`).

#### 60.6.1. Relevant environment variables:

- **`NO_CHECK_CONSISTENCY` (client reference: no)**
AWDesk #236576: with this environment variable, the consistency check developed with AWDesk #174433 for the Intaufarten -26, -28 and -37 since the check always takes effect even if there are not any problems.

- **`RABATTERMITTLUNG_NETTO_GLEICH` (client reference: no)**
AWDesk #179528: new determination of the discounts with Intaufart -37 is rejected if the net total would change.

### 60.7. Recalculate prices (FORALL_PREISE (-38))

If a document (order or PO) with `still` -38 is presented to `intauf`, then the sales and purchasing conditions and prices are determined anew for all items. Then there is a new totaling of the document total values. An additional call of "intaufart Auftragssummierung" (`FORALL_SUM` (-20 )) is not necessary.
A separate call for PU and SA is currently not possible.
If the talk is of PU here, then this also implies the material cost calculation. For production costs, the order must be transferred to production once again.
If this intaufart is used for POs, it must be heeded that the cost back calculation is not done automatically, but must be initiated with an intauf call -17.

### 60.8. Capacity planning (-39 ALCIM_UEBERGABE)

Here the concern is the transfer of existing order for conversion to the A+W Production capacity planning

# 194130 (alcib 2009 build 4.4.0.4791 / alcib 2011) If you convert the production system from PMS to A+W Production Capacity Planning, it is now possible to transfer the documents already transferred to the PMS to A+W Production. This works only for orders, which have to have been transferred to the production system beforehand. Please note that there is no synchronization between the production systems. This means that this logic can be used to transfer only those orders for which production in PMS has not yet begun. The transfer is made via background processing.

### 60.9. Rack invoices (-40 VORGANG_NEU)

**Note:** The focus here is on -40 in the table "aufint" with document = 7. If in the table kauf still=-40 for document = 4 or 5, then this is a wait state for documents not completely entered in A+W iQuote.

The function for creating the rack invoice is a component of the AWRack module. Via a function in the ERP webservice, invoices for rented racks can be generated.
These rack invoices are generated by the background process "intauf". This functionality that is controlled by AWRck can also be activated directly via customizing.

- The `intauf` process 4 must be configured.
- The table "gestrech" must be filled. The meanings of the fields described here is only for the creation of the invoice by the background process "intauf". It does not apply for the connection to external systems or AWRack. See the table documentation for this.

The fields that are defined here as "Not evaluated" can be used for individual evaluations and control; however, they are not currently evaluated by the background process "intauf". However, this can change them at a later point in time.

| Column | Meaning |
| :--- | :--- |
| group | sequential number per invoice |
| Transid | sequential number per invoice |
| Artnr | Article number for the item in the invoice (artikel.artnr) |
| Gnr | Rack number for which the invoice should be generated (gestell.gnr) |
| Kunr | Customer number for which the invoice should be generated (mp.mpnr) |
| Fakturatage | Number of days that should be invoiced. If the number of days = 0, then it is calculated from fakturabis - fakturavon - mietfreitetage |
| Fakturavon | Date on which the invoice period begins |
| Fakturabis | Date on which the invoice period ends |
| Mietfreietage | Number of days in this invoice period that are rent-free, that is, not to be calculated |
| Steuerflag | -2 – new record to be processed<br>2 - invoice was generated |
| Aufnr | Internal invoice number; it is specified by intauf during the invoice generation (kauf.aufnr) |
| Rechnr | Invoice number; it is assigned by intauf during the invoice generation (kauf.aufnr where vorgang=7) |
| Posnr | Internal item number; it is assigned by intauf during the invoice generation (kpos.posnr) |
| Gsbuchid | Not evaluated |
| Liefdat | Not evaluated |
| Gesliefnr | Not evaluated |
| Auftrnr | Not evaluated |
| Komplett | Not evaluated |

- Then a data record must be written to the table `aufint` with `still` -40 and the background process `intauf 4` started (sctrl).
`insert into aufint values (-1,0,7,0,-40,0,0,-1,<Mandant>).`

The invoice will be booked immediately. Thus, a correction is not currently possible.
Then the invoice is there and the record in `gestrech` as well. Via the record in `gestrech`, you can specify via an individual script the new calculation period for additional invoices.

### 60.10. Copy INTERNAL document (AUFTRAG_NEU (-45))

#101385
This intaufart is absolutely internal ans serves primarily as QS for standard tests. There is no support for this intauf type.
If a document with `still` -45 is presented to `intauf`, the `intauf` creates a copy of the original document.
a. The reference fields in `kauf` are filled with those of the basic document.
b. `Kauf.liefkompl`, `kauf.fakturakz`, `kauf.rechnr` are reset.
c. The entry date (`kauf.edat`) is set to "today."
d. The customer's requested date (`kauf.ltplan`) is set to today + (`ltideal_alt` - `edat_alt`). Thus the difference between the entry and customer's requested date is retained
e. Author, etc. is kept
f. For orders, the `kaufart` (e.g. stock order) is retained.
g. There is no data warehouse booking

A newly generated order is not released. "Orig.`<Refernz Knd Bestnr>`" (`kauf.exaufnr`) is in the remark in the release pool.

### 60.11. Process for transfer of cost calculation (ALCIM_UEBERGABE_KK -47)

The system can now perform a downstream transfer to cost calculation via script call. For this, the orders in question are presented to the background process "intauf" with still -47. It then starts the transfer to cost calculation. During this transfer, the order is locked with still -10.

**Application:** E.g., a script can be started in the evening via Crontab in order to generate stock forecast data. The sample script recognizes that there should be another transfer after order change, however not if the transfer for cost calculation is done and a change was made on the same day.

There is an example under
`$ALCIBPRG/install/xsql/cust/ka/cu_transOrder2CC.sql`
`$ALCIBPRG/cmd/transfertocc`

The script presents the orders with still -47 to `intauf`, which then transfers them for cost calculation to AWP. Here, the stock forecast data, if configured, is generated.

### 60.12. Element exchange (SLKORREKTUR -52)

[AW-221950] / 04/2025 // alcib - 13.04.20016

See also EN-CONFIG-A+W Enterprise Production Interface - "Reporting of an element exchange"

The exchange data is transferred via an entry in the table `zuaufint` with `art=-52`. There is a processing with `still=-52` (element exchange), and directly after this also processing with `still= -38`, via which the costs are calculated and the stock data adjusted.

**Prerequisite.** The structure of the exchanged article must be identical, both with regard to the BOM structure and the definition of the additional data (article dimensioning, variant definition, color definition). For the statement "The structure of the exchanged article must be identical, both with regard to the BOM structure and the definition of the additional data (article dimensioning, variant definition, color definition)" the concern is that an "identical" `poszu` record must exist both for the source article as well as for the target article. If you were to enter the source article and target article manually in the order, the corresponding poszu records must be identical (but for the article number, article name, quantity, etc). Otherwise the exchange will be only rudimentary. Similarly, there is no exchange of the subordinate BOM. Thus, this function is not approved for a production exchange.

Data in the table `zuaufint`:
- `Artnr` = source article number
- `Artnr1` = target article number
- `Poskonr` = BOM number into which exchange should be made
- `Tnr` = tuple number that should be exchanged

### 60.13. EK_RUECKRECH_PLUS -117

[AW-106081]
This intauf type is for internal POs from which via internal EDI an internal order arises in-house (see `IBHAUS` in EN-CONFIG-A+W Enterprise EDI).
The totaled costs including the written-back cost discount (`kpos.ererloes`) from an internal component order (`IBHAUS`) are taken over into the internal PO as PU item price (`kpos.npospreis`) and the PU unit price (`kpos/npospreis/kpos.menge`) are recalculated. With existing written-back discounts, the PU revenue is also recalculated.

## 61. Special process descriptions

### 61.1. Production of patterns/tests

In order to handle internal test production, there is no direct standard procedure. This depends on our customers' special requirements and processes. This special production does not necessarily require special processes in A+W Enterprise

A recommendation can be as follows:
The order is entered for the customer number of one's own branch office. If such orders occur frequently, you can also create a special customer for this. The order type can be set to "free." If configured, the costs are determined normally. With this procedure, you can invoice the orders normally. Otherwise they remain in the system forever. If you don't want to invoice them, you can remove them from the value import (via the customer number) and then complete them manually.

### 61.2. Trade with POs without production

For clients who order all products and do not have their own production, a special configuration with the environment variable `PMSPURCHASETRIGGER` is required. The detailed description is in the "EN-CONFIG-A+W Enterprise EDI" configuration guide. The function is also called "PMSO".

## 62. Customizing

The possibilities for customizing are documented in separate configuration instructions "EN-CONFIG-A+W Enterprise Customizing".

### 62.1. Log

The customizing log can be switched on with system menu (CTRL+F4) – CTRL+K. The level of the log - support or development - can be selected. The log is written to `$PROTOPFAD/cust<pid><mmdd><hhmm>`.

## 63. Late change

### 63.1. Local correction through PO

Environment variable `KAUFUPDATE_BEI_BEST`
A released PO sets the order to the state of LOCAL CORRECTION. Thus a change can no longer be transferred to AWP.
If this variable is active, then despite LOCAL CORRECTION, the changed order can be transferred again to the AWP if the user responds to the subsequent security query appropriately.
This order change is no longer communicated to purchasing. The POs thus remain unchanged.
The variable can inherit the values "On" and "On+AWEIN". If the value is "ON," the setting applies as long as there hasn't been a receipt of goods. If the value is "ON+WAEIN," then the setting also applies if there has already been a receipt of goods.

**Caution:** The environment variable `KAUFUPDATE_BEI_BEST` should only be used with great caution and only activated for individual users.

If for an item in local correction the BOM is changed (e.g. glass exchange), this can mean that the internal part number (tupel number) of the ordered part changes. Later on, this could mean
- That an already ordered part is reported as ordering to A+W Enterprise. PO successions/POs are generated again. If you are not working with the purchase order pool, a new PO is triggered immediately.
- That a goods receipt in A+W Production can no longer be allocated correctly and thus is not removed from the PO pot.

Example: in the present case, the customer orders the glass and then substitutes a more complex frame after the fact. This changes the tupel number of the glass and the glass is ordered again.
You can disarm this scenario by filling the standard frame with a dummy item, so that for an exchange, the number of BOM elements does not change. This isn't a sure thing, but it can help.

In principle, however, the processes that make such a dangerous way of working necessary have to be re-thought.

### 63.2. Transfer of late changes to production

Environment variable:
Three types of changes are classified in A+W Enterprise:
1. Purely commercial change (prices, terms, user data, invoice and printing options, payment options, etc.)
2. Production information changes. (no new scheduling required)
    a) packaging type,
    b) declaration of performance,
    c) file attachments,
    d) delivery address,
    e) customer address,
    f) delivery date (for locked orders)
    g) Route (`KAUF_ROUTE_PRODRELEVANT` not active #394028)

3. Production-relevant changes that require new scheduling.
    h) Change to the product,
    i) Quantity,
    j) Dimensions (also changes to the shape dimensions that do not cause a change in the item dimensions #394028),
    k) Delivery date (for orders that are not locked)
    l) Route (`KAUF_ROUTE_PRODRELEVANT` active #394028)
    m) ...

**Note:** The list of changes is not complete, but should represent a starting point

If you want all changes in the order (except for purely commercial ones) up to the lock of the order in the local correction to be forwarded as production-relevant, you should activate the ENV switch `PRODRELEVANT_BIS_LOKALKORREKTUR`. (#394028)

As a result there are changes that only occur in the individual items and changes that occur on the order header level. Changes on the header level mean that the change type is not transferred to all non-canceled items if the class of the change is higher than any present in the item. If, for example, the quantity is changed in an item and then the delivery address, then all non-changed items receive the status "Info to production (`kpos.aendkz=4`) and the changed position then "production-relevant change" (`kpos.aendkz=5`).

If late changes are transferred to production, the system message 80 ("Production information without scheduling" can be configured for this (see "EN-CONFIG-A+W Enterprise System" section "System messages").

Here is a tabular overview of the effect of the new module logic:

#### 63.2.1. Free orders and transfer to production

| Commercial change (In the question, reference is made that it was only commercial changes) | PROD INFO change (general question) | PRODrel. change (general question) | Treatment |
| :--- | :--- | :--- | :--- |
| YES | | | `kpos.aendkz` = 5 (ALL) |
| NO | | | `kpos.aendkz` = 0 No transfer! |
| | YES | | `kpos.aendkz` = 5 (ALL) |
| | NO | | `kpos.aendkz` = 4 (in item) |
| | | YES | `kpos.aendkz` = 5 (ALL) |
| | | NO | `kpos.aendkz` = 5 (in item) <br> No transfer! |
| | | | No transfer! |

#### 63.2.2. Order by order locking. Transfer to production for lock via PO/GR and `KAUFUPDATE_BEI_BEST` active

`CHECK_KPOSSTAT` = OFF
`MODUL_PROD_SPAETE_AENDERUNGEN` = ON
`KAUFUPDATE BEI BEST` = ON/BEST+WAEIN – caution: dangerous

| Commercial change (In the question, reference is made that it was only commercial changes) | PROD INFO change (In the question, specific reference is made that a PO exists) | PROD-relevant change (In the question, specific reference is made that a PO exists) | Treatment |
| :--- | :--- | :--- | :--- |
| YES | | | `kpos.aendkz` = 5 (ALL) |
| NO | | | `kpos.aendkz` = 0 (ALL) <br> No transfer! |
| | YES | | `kpos.aendkz` = 5 (ALL) |
| | NO | | `kpos.aendkz` = 4 (in item) <br> No transfer! |
| | | YES | `kpos.aendkz` = 5 (ALL) |
| | | NO | `kpos.aendkz` = 5 (in item) <br> No transfer! |

#### 63.2.3. Order by order locking. Transfer to production all other blocks without active `KAUFUPDATE_BEI_BEST`

`MODUL_PROD_SPAETE_AENDERUNGEN` = ON
`KAUFUPDATE_BEI_BEST` = OFF
`CHECK_KPOSSTAT` = OFF

| Commercial change | PROD INFO change (general question) | PROD-relevant change (general question) | Treatment |
| :--- | :--- | :--- | :--- |
| No query. Message that everything remains local | | | `kpos.aendkz` = 0(ALL) |
| | YES (as of 05/22/2017) | | `kpos.aendkz` = 4 (ALL) |
| | NO (as of 05/22/2017) | | `kpos.aendkz` = 4 (in item) <br> No transfer! |
| | | YES (as of 05/22/2017) | `kpos.aendkz` = 4 (ALL) |
| | | NO (as of 05/22/2017) | `kpos.aendkz` = 4 (in item) <br> No transfer! |

#### 63.2.4. Item-by-item locking

`MODUL_PROD_SPAETE_AENDERUNGEN` = ON
`KAUFUPDATE_BEI_BEST` = OFF/ON/BEST+WAEIN (caution!)
`CHECK_KPOSSTAT` = `<date>`

| Commercial change. (In the question, reference is made that it was only commercial changes) | PROD INFO change (general question) With active KAUFUPDATE_BEI_BEST reference is made in the question that a PO exists | PRODrel. Change (general question) With active KAUFUPDATE_BEI_BEST reference is made in the question that a PO exists | Treatment |
| :--- | :--- | :--- | :--- |
| YES | | | `kpos.aendkz` = 5 in all items where it is possible: all free items or ordered with active `KAUFUPDATE_BEI_BEST` <br> Otherwise `kpos.aendkz=4` |
| NO | | | `kpos.aendkz` = 0 |
| | YES | | `kpos.aendkz` = 4 in all or in the individual items (depending on type of change) |
| | NO | | `kpos.aendkz` = 4. <br> No transfer! <br> If data was already in PROD (`kauf.uebertragen=1`), then the data is no longer considered for the next change. |
| | | YES | `kpos.aendkz` = 5 in all items where it is possible. all free items or ordered ones with `KAUFUPDATE_BEI_BEST` <br> Otherwise `kpos.aendkz=4` |
| | | NO | `kpos.aendkz` = 5 in all items where it is possible, otherwise `kpos.aendkz` = 4. <br> No transfer! <br> If data was already in PROD (`kauf.uebertragen=1`), then the data is no longer considered for the next change. |

#### 63.2.5. Comparison OLD/NEW logic.

**Item change (`kpos.aendkz`):**
- 0: no change/changes not transferred (is not evaluated by PROD)
- 1: commercial change (is not evaluated by PROD)
- 2: cancel
- 4: info to production
- 5: Production-relevant -> new scheduling

**Order change (`kauf._angbstatus` nut in `kauf.vorgang=5`)**
- 1: production info change
- 10: production-relevant change
- 11: 1+10

**Free orders (orders not in LOCAL CORRECTION)**

Orders locked by the PO are also affected if `KAUFUPDATE_BEI_BEST` is active (caution: use of the variables is dangerous)
- **OLD:** changes go completely to PROD if the question about release was answered with YES.
- **NEW:** changes go completely (mode = 5) to PROD if the question about release was answered with YES.
- ALL items receive the same status = 5 if they go to production.

**Locked orders (orders in LOCAL CORRECTION) locking order by order**
- **OLD:** commercial changes no longer go to PROD.
- **NEW (AWE 6.3/5.4):** commercial changes no longer go to PROD.
- **NEW: (AWE 6.3/5.4 starting on 05/22/17):** question about release: if YES: all items as INFO. If NO: changes remain local. No longer noticed.
- ALL items always receive the same status = 4 if they go to production.

**Locked orders/locking item by item**
- **OLD:** order goes completely to PROD (if at least 1 free item is there). Always ALL items, also the locked ones.
- **NEW:** changes are transferred item by item. With locked ones, only maximum INFO as change mode. Non-changed items have change mode = 0.

- (+) Due to the new scheduling, only the production-relevant changed items go.
- (-) If the changes in the order are NOT transferred by the user directly to production, the change status is lost and is no longer considered for the next change!
- (-) It is not possible (except via submenu) to transfer all items to production for scheduling if only individual items are changed production-relevant or if in the order there have been global or item-by-item only PROD-INFO changes made. That is, in the place there are fewer possibilities for transfer than with commercial changes.

Items can have different status depending on the type of changes.

#### 63.2.6. Writing back of a changed delivery date from dispatch

If `LAPOOL_TOUR_TO_KAUF` is set, a shift in dispatch is also reported to AWP.

#### 63.2.7. Ignore change of the consignment and the customer item.

[AW-107059]: QR23/08
- Albwir.Alcim.Config.dll - v13.6.5867
- Albwir.Alcim.Orders4Production.dll - v13.6.5746
- Diskset: A+W Production 6 - v13.6.5867
- Diskset: A+W Production 6 Import - v13.6.5746
- Diskset: A+W Planning 6 Import Services - v13.4.9344

**Note. This is a function in the A+W product!**
For the "late takeover of production-relevant data" it can be necessary not to take over changes to the customer consignment and the customer item, such as, for example, if the data has already been created through individual measures (e.g., SP) and does not originate from the transfer file (OrderXML).
For this, there is now the switch `ORDERS4PRODUCTION/IGNORE_COMISSION_CHANGES` in the A+W Production 6 Parameter Administrator.

## 64. VAT adjustment

### 64.1. Concept Overview

With this brief document, we would like to discuss the adjustment of the VAT. For this, the points in A+W Enterprise will be examined at which the user can make this adjustment.

### 64.2. Master data

On the `Master Data > Codes > System > Control` menu, it is possible even before the new VAT rate goes into effect to store the new VAT rate for the customer code "external" with the corresponding start date `Valid from` (07/01/2020). At the same time, a different tax account for the transfer to financial accounting can be stored. If you want to use new accounts in your financial accounting for the new VAT rate, please check in advance whether your transfer interface supports the use of these tax accounts.

*Figure 125: Maintenance of tax records*

No additional master data or configurations are required.

### 64.3. Function Description

In A+W Enterprise, the Entry date of the document is used to determine the VAT rate. The desired or planned delivery date of the document has no effects on the determination of the VAT rate. The only exception from this rule is the creation of a Credit with reference. In this case, the credit is created with the VAT rate of the underlying document.

**Example:**
If you enter an order on 06/25/2020, the order will be calculated with the VAT rate of 19%. And also if the delivery date is planned for 07/02/2020.
If you enter an order on 07/02/2020, the order will be calculated with the VAT rate of 16%.
If on 06/27/2020 you create an invoice for an order or delivery note, then the invoice will include the VAT rate of 19%.
If on 07/02/2020 you create an invoice for an order or delivery note, then the invoice will include the VAT rate of 16%. The invoice will also include a VAT rate of 16% if the document underlying the invoice (order or delivery note) was entered before 07/01/2020.

### 64.4. Action guidelines

Even if according to German tax law the date of service is decisive for the tax determination, A+W Enterprise uses the date on which the document was created.
Therefore, it is necessary that all goods delivered by 06/30/2020 also be invoiced by 06/30/2020.
If individual orders or delivery notes that were created before 07/01/2020 cannot be invoiced before 07/01/2020, the invoices for these can be backdated.
This can be done in 2 ways.

**Creation of manual invoices**
In the Manual invoicing, it is possible to backdate the invoice entry date. For this, in the invoice header in the "Entry Date" field, enter the desired date before 07/01/2020. For security reasons, the date must be entered twice here. The booking date for the invoice is unaffected by this.

*Figure 126: Manual invoice creation*

**Automatic release**
In the automatic invoicing, it is also possible to change the document date. For this, on the Automatic Release dialog, the desired date before 07/01/2020 has to be entered. For security reasons, the date must be entered twice here. The booking date for the invoice is unaffected by this. Thus, in an invoice run, it is possible to invoice all deliveries up to and including 06/30/2020 and then all later deliveries. For this, it is only necessary that the value import used for the invoice run query the delivery date as parameter. Which SQLs are used for the value import is defined in the environment variables `RECHFREI_RELEASE` and `SRCHFREI_RELEASE`. If you need assistance with this, please contact our service or your project employee in timely fashion.

*Figure 127: Automatic invoice creation*

## 65. VAT conversion

With this brief document, we would like to discuss the adjustment of the VAT. For this, the points in A+W Enterprise will be examined at which the user can make this adjustment.

### 65.1. Master data

On the `Master Data > Codes > System > Control` menu, it is possible even before the new VAT rate goes into effect to store the new VAT rate for the customer code "external" with the corresponding start date `Valid from` (07/01/2020). At the same time, a different tax account for the transfer to financial accounting can be stored. If you want to use new accounts in your financial accounting for the new VAT rate, please check in advance whether your transfer interface supports the use of these tax accounts.

*Figure 128: Tax records*

No additional master data or configurations are required.

### 65.2. Function description

In A+W Enterprise, the Entry date of the document is used to determine the VAT rate. The desired or planned delivery date of the document has no effects on the determination of the VAT rate. The only exception from this rule is the creation of a Credit with reference. In this case, the credit is created with the VAT rate of the underlying document.

**Example:**
If you enter an order on 06/25/2020, the order will be calculated with the VAT rate of 19%. And also if the delivery date is planned for 07/02/2020.
If you enter an order on 07/02/2020, the order will be calculated with the VAT rate of 16%.
If on 06/27/2020 you create an invoice for an order or delivery note, then the invoice will include the VAT rate of 19%.
If on 07/02/2020 you create an invoice for an order or delivery note, then the invoice will include the VAT rate of 16%. The invoice will also include a VAT rate of 16% if the document underlying the invoice (order or delivery note) was entered before 07/01/2020.

### 65.3. Action guidelines

Even if according to German tax law the date of service is decisive for the tax determination, A+W Enterprise uses the date on which the document was created.
Therefore, it is necessary that all goods delivered by 06/30/2020 also be invoiced by 06/30/2020.
If individual orders or delivery notes that were created before 07/01/2020 cannot be invoiced before 07/01/2020, the invoices for these can be backdated.

This can be done in 2 ways.

**Creation of manual invoices**
In the Manual invoicing, it is possible to backdate the invoice entry date. For this, in the invoice header in the "Entry Date" field, enter the desired date before 07/01/2020. For security reasons, the date must be entered twice here. The booking date for the invoice is unaffected by this.

*Figure 129: Manual invoice creation*

**Automatic release**
In the automatic invoicing, it is also possible to change the document date. For this, on the Automatic Release dialog, the desired date before 07/01/2020 has to be entered. For security reasons, the date must be entered twice here. The booking date for the invoice is unaffected by this. Thus, in an invoice run, it is possible to invoice all deliveries up to and including 06/30/2020 and then all later deliveries. For this, it is only necessary that the value import used for the invoice run query the delivery date as parameter. Which SQLs are used for the value import is defined in the environment variables `RECHFREI_RELEASE` and `SRCHFREI_RELEASE`. If you need assistance with this, please contact our service or your project employee in timely fashion.

*Figure 130: Automatic invoice creation*

## 66. Rack planning

### 66.1. Master data

#### 66.1.1. Market partner master data

Maximum packing weight in master data - market partners tab: Production
The maximum rack weight in the order is only checked if the one stored in the market partner master data is greater than 0 (null).

#### 66.1.2. Rack types = packaging types

`Logistics` - `Rack management` - `Rack Master Data` - `Rack Types` - `Rack Types`
**Bill of materials (BOM)**
If the environment variables `GESTPLAN_PRIO` or `GESTPLAN_PYRO` are enabled, then BOMs for variable rack types can be stored here (CTRL +F10). The BOMs are stored in the table "gsl". **Only until February 2025 see below**

[AW-124162] - QR November 2022

For transmission of the exterior dimensions of one-way packaging (box) to the OTR, it is now possible to store a new entry on the dialog `Logistics > Rack management > Rack master data > RAck types > Parts list for manufacturing` (CTRL + F10). This record must be marked with the checkbox in the "ED" (exterior dimensions) column. There may be only one record with this code per box type. For this record, the fields length, width, thickness (=height) must be filled out.
The code is not displayed in the packaging planning. Here, it should be possible to see via the parts name that these are the exterior dimensions. In the table `gskistrukt`, the code is taken over, however, so that it can be evaluated there.
During the transfer of the data to the OTR, the record is taken from the table `gskistrukt`, which as `lfdnr` corresponds to the `ordnr` from the box BOM `9table` gsl) to the `aussenmass` flag. If there is no record there, the interior dimensions from the table `vsaufgest` are transferred.

**February 2025 // alcib build 13.04.19463**
Since the evaluation in the box BOM depends on the environment variable `GESTPLAN_STÜCKLISTE`, the entry of the BOM into the rack types is now controlled exclusively via this environment variable.

**Stackability**
[AW-130294] – QR January 2023
For the maintenance of the master data for rack types, it is now possible to mark the stackability of a rack type. This is done in the detailed view of the packaging.
The field is used only for a customer's own evaluations. It is not evaluated further by the system.

### 66.2. Specification for rack planning

#### 66.2.1. Warning in case of forgotten rack planning

[AW-111432] - QR 08/2022 - alcib - 13.04.13805 / ENV

For lites with a particular size, the specifications for the rack planning must absolutely be made in the order. In order to keep the maximum dimension flexible, a separate dummy rack type is stored as dimension master. This rack type is also entered in the environment variables that activate this function.
In the "Dimension master" rack type, the fields "Maximum height" and "Maximum width" are used. When saving the order, it is checked for all items whether the short glass edge exceeds the small maximum dimension and the long glass edge the long maximum dimension of the "dimension master" rack type and if so, whether the specifications for rack planning for this item are stored. If not, the person entering the order is informed and he must do the rack planning.
This check is done exclusively in manual order entry. Within the internal document transfer and for the external order interface, this function is not applied.

**Configuration:** `DIM_MASTER_RACK`

[AW-179404] // 15.05.2024 // alcib - 13.04.17680
Starting with this program version, it is not sufficient only to record the specifications for rackplanning; instead, rackplanning must absolutely be performed in advance.

#### 66.2.2. Individual checking of the rack planning

[AW-135110] // September 2023

An individual checking of the rack planning can be activated. For this, two individual stored procedures (SPs) must be created.

The first SP "`cu_gpl_req()`" receives as parameter the country code of the delivery address (`adr.kfzcode`/`kauf.lkfzcode`) and the dispatch type (`kauf.versandart`). The SP must return whether the rack planning should be checked - FALSE-no check, TRUE - check required.

The second SP "`cu_pm_check ()`" checks the rack planning across all calculated data to see whether it is permitted in this form. As parameter, the SP receives the rack type and the calculated dimensions of the packaging (width/height/depth). Here, two return values (retCode, Fehlertext) are expected. If the `retCode` = TRUE - everything OK, `retCode` = FALSE - not permitted. A note with reason can follow in the error text.

The check is done when saving an order. If the necessity of a check of the rack planning is determined by the first SP and if this has not been done, then the order cannot be saved until the planning has been completed.

The function is not bracketed with any additional environment variables. If the rack planning is configured and the required SPs are present, they will be executed.

- `cu_gpl_req` (`kfzcode`, `versandart`) into `retCode`; `retCode` = 1 - check required.
- `cu_pm_check` (`gtyp`, `maxb`, `maxh`, `maxt`) into `retCode`, `Fehlertext`; `retCode` = 1 - everything OK.

### 66.3. Planning algorithms

Within the packaging planning, there are various planning algorithms available:
- **GA** = Total algorithm
- **PA** = Partial algorithm
- **M** = Manual
- **PA** = Priority algorithm
- **PO** = Cost-based packaging optimization (special configuration and additional tool PMO required)
- **PV** = PO + PackView (special configuration and additional tool PMO required)
- **EA** = Equal Algorithm

**Note:** The abbreviations are used this way in all languages, there is no translation

#### 66.3.1. GA = Total algorithm

GA (= total algorithm): The user specifies for the whole order one Rack main group (configuration-dependent) or one rack type and the program then has the task of distributing the items on this rack.

A rack type or a Rack main group (configuration-dependent) can be predefined for the entire order. Here, the rack main group includes several rack types, that is, various rack types can be combined into a rack main group. (menu: `Logistics > Rack management > Rack master data`)

**Restriction check**

The rack types or rack main types approved for a customer must be stored in the market partner master data (menu: `Master data > Market partner > F4 menu > Rack types`). There, it is either possible to store that particular rack types are approved for this customer or it can be stored that all rack types of a main group are approved for the customer.

#456030: QR 04/20
**Extension of the packaging material planning (sort algorithms: "GA")**

The packaging material planning has been extended so that it is now possible to consider customer-specific restrictions during automatic planning (algorithm "GA"). If the new environment variable `GESTPLAN_KUGEST_RESTRIKT` is switched on, only rack types or main rack groups that are assigned to the market partner are allowed in packaging material planning. For the search for the rack type, this restriction was already active before, whereby it was possible to enter packaging materials manually that were not assigned to the market partner. As long as these were present and appropriate for the order, they could be used. This is no longer possible by switching on the new variable and only the assigned packaging materials are allowed. This restriction applies both to the rack type and to the main rack groups.

If in the specifications a rack type or a main group is entered, it is first checked whether type and main group are approved for the customer of the current order. If this is not the case, then the entry will be rejected with an appropriate message.

If a rack type was entered, then it is checked whether it is appropriate for the dimensions of all order items. That is, it is checked for each order item whether the width is narrower than the maximum width of the rack and wider than the minimum width and whether the height of the item is less than the maximum height of the rack and greater than the minimum height. If this is not the case, then the entry will be rejected with an appropriate message. As width of the item, the larger dimension is always used; that is, if the height is larger than the width, then the lite is "turned."

If a rack main group is input, then it is checked whether there is at least one rack type from this main group on which all lites for the order fit given their dimensions. If this is not the case, then the entry will be rejected with an appropriate message.

If the input of the rack type or main group was accepted, then there is a query as to whether the rack type or main group should be taken over into all items for the setting. If this question is answered with "N" then the value entered is reset to the original value; that is, the change is discarded. If it is answered with "Y", then the rack type/main group entered is taken over in all items of the setting.

#### 66.3.2. PA- Partial algorithm

PA (=partial algorithm): A rack type is specified for an item. The program then has the task of calculating how many racks of this type will be required and of loading these appropriately. In addition, the customer can specify in the "Quantity" field how many lites of an item should be loaded on a rack. Finally, it is possible in the "Group" field to pack several items together on a rack by specifying the same number.

Here, a rack type must be specified for each item. In the process, the same checks are made as in the sorting GA (permissibility for the customer, permissibility for the dimensions). If the type entered is permissible, there is a query as to whether the rack type should be inherited in all other items. Then the master data of the rack type look like this:

- Maximum and minimum dimensions
- Maximum and minimum depth
- Maximum weight
- Own weight
- Identification of fixed/variable (fixed=A-rack or L-rack, variable=boxes)
- Side padding (only for boxes)
- Distance across (in case of several columns next to one another)
- Distance high (in case of packing on top of one another)

read in and displayed in the header area of the screen. If necessary, these fields can be reached and changed from the item area by pressing A5. The following restrictions apply for changes in the header area:
- The maximum weight cannot be changed
- The maximum/minimum dimensions can only be changed for variable boxes so that the maximum dimensions are made smaller and the minimal made larger. The maximum/minimum dimensions for fixed racks can only be changed with special authorization (GERE=rack restrictions). If someone does not have the authorization, a message appears that tells him which employee he must ask or from whom he can receive the authorization. For this, in the environment variable `GEPL_MANR`, the number of the employee must be specified who assigns the authorizations.
- The side padding only exists for variable boxes, not for fixed racks
- The distance across can only be changed if packing next to one another is allowed for the rack type
- The distance high can only be changed if packing above one another is allowed for the rack type.

From the header screen, you return to the item area by pressing A5 or entering "END". In addition to the rack type, now the fields "Quantity" and "Group" can also be specified. In the "Quantity" field, the customer can specify how many lites of an item should be loaded on a rack. By entering any number in the "Group" field, the customer can pack several items together on a rack.

**Example: Order with 3 items**

| Itm | Quantity | Quantity | Group |
| :-- | :--- | :--- | :--- |
| 1 | 21 | 7 | 1 |
| 2 | 15 | 5 | 1 |
| 3 | 30 | 10 | 1 |

Based on these specifications, 3 racks are required in the rack planning:

| Rack | Load |
| :--- | :--- |
| 1000 | 22 pcs. (7 from item 1, 5 from item 2, 10 from item 3) |
| 1001 | 22 pcs. (7 from item 1, 5 from item 2, 10 from item 3) |
| 1002 | 22 pcs. (7 from item 1, 5 from item 2, 10 from item 3) |

If with this breakdown there are leftovers, then they will be planned on another rack of the same type.
**Example:**

| Itm | Quantity | Number | Group |
| :-- | :--- | :--- | :--- |
| 1 | 21 | 7 | 1 |
| 2 | 17 | 5 | 1 |
| 3 | 35 | 10 | 1 |

Based on these specifications, 4 racks are required in the rack planning:

| Rack | Load |
| :--- | :--- |
| 1000 | 22 pcs. (7 from item 1, 5 from item 2, 10 from item 3) |
| 1001 | 22 pcs. (7 from item 1, 5 from item 2, 10 from item 3) |
| 1002 | 22 pcs. (7 from item 1, 5 from item 2, 10 from item 3) |
| 1003 | 7 pcs. (2 from item 2, 5 from item 3) |

If a quantity is specified and a rack type was already specified, there is a check as to whether the specified number of lites even fits on the rack (based on the thickness and weight and the maximum permissible weight for the customer). Here, the total glass thickness of the planned lites is compared to the maximum depth of the rack, and the total weight of the planned lites is compared to the maximum weight of the rack and the maximum permissible weight for the customer.
For boxes, the side padding is not considered for the checking of the total depth, but it is afterwards during the calculation of the total depth. If either maximum depth or maximum weight is exceeded, an appropriate message appears on the screen and the entry is rejected.

#### 66.3.3. M- Manual

M = (manual): The distribution of the items on racks is done manually; that is, the customer specifies exactly how many lites from which items should be together on a rack. If here a value is entered in the "Quantity" field that is smaller than the item quantity, the system immediately generates a new record where the "Quantity" field contains the difference between the item quantity and the quantity previously entered ("Item splitting").

Here, the rack type and quantity per rack must be specified; a group can be entered. With this sorting, the customer specifies in detail how many lites from each item should be packed together on a rack.

If a value is specified in the "Quantity" field that is smaller than the item quantity, then on the screen for this item, another record is attached immediately with the difference between the item quantity and the quantity entered as quantity.

**Example:**

| Itm | Quantity | Quantity |
| :-- | :--- | :--- |
| 1 | 20 | 12 |

This produces 2 records for item 1:

| Itm | Quantity | Quantity |
| :-- | :--- | :--- |
| 1 | 20 | 12 |
| 1 | 20 | 8 |

For this specification, 2 racks are required; on one there are 12 lites, on the other 8 lites. By entering a group, parts of several items can be packed on a rack.

Example for a manual specification:

| Itm | Rtype | Quantity | Quantity | Group |
| :-- | :-- | :--- | :--- | :--- |
| 1 | 1 | 12 | 6 | 1 |
| 1 | 14 | 12 | 6 | 2 |
| 2 | 1 | 25 | 12 | 1 |
| 2 | 14 | 25 | 13 | 2 |
| 3 | 1 | 4 | 2 | 1 |
| 3 | 14 | 4 | 2 | 2 |
| 4 | 1 | 31 | 16 | 1 |
| 4 | 14 | 31 | 15 | 2 |

Based on these specifications, 2 racks will be loaded:

| Rack | Load |
| :--- | :--- |
| 1000 | 36 (6 from item 1, 12 from item 2, 2 from item 3, 16 from item 4) |
| 1001 | 36 (6 from item 1, 13 from item 2, 2 from item 3, 15 from item 4) |

For all 3 sortings, there are additional input fields available in the item area:
- **Intermediate padding between the lites**
This refers to the cork sheets that are placed between the lites so they do not scratch one another. Here, the thickness of these intermediate spaces should be entered in mm.
- **Padding every how many lites**
It is not always said that there must be an intermediate space after each lite. With this field, it is possible to specify every how many lites such distance should be provided. The fields listed under 1 and 2 influence the calculation of the total depth of the lites on the rack.
- **Number across**
If the rack type allows packing next to one another, the number of columns that can be packed next to one another can be entered. This does not apply for the sorting GA and not if an entry was made in the "Group" field. After entry, there is another check whether the dimension restrictions of the rack are not violated (maximum and minimum width). If this is the case, then the entry will be rejected.
- **Number high**
If the rack type allows packing on top of one another, the number of columns that can be packed on top of one another can be entered. This does not apply for the sorting GA and not if an entry was made in the "Group" field. After entry, there is another check whether the dimension restrictions of the rack are not violated (maximum and minimum height). If this is the case, then the entry will be rejected.

#### 66.3.4. PA - Priority algorithm

(starting with Version 2.13): PA = rack planning according to priority list

In the master data (Logistics - Rack management - Rack planning), a priority list of the rack types can be stored. The rack planning then initially tries to plan the items on the rack type with the highest priority. If in the process the dimension restrictions are violated, there is an attempt to fall back on the next rack type in the priority list. If none of the rack types fits, everything will be planned on a "scavenger" rack. (See also case 32755)

#### 66.3.5. EA - equal algorithm

(starting with Version AWE 6 (#384920)): EA = Equal Algorithm

This algorithm always plans an even number of lites of an item in a package. This algorithm has the following restrictions:
- Within an order, all items must be planned with this algorithm. A mixing of different algorithms is not possible.
- The item quantity must be even.
- A rack type or rack main group must be specified.

With this algorithm, it is possible to distribute the quantity of an item across various packaging in advance. For this, you specify the desired quantity in the "Quantity" column. This partial quantity must also be even. The program then automatically creates a new planning item with the residual quantity.

No special configuration is required to use this algorithm. However, it was currently only tested in the configuration GESTPLAN_PILK2. In consultation with the customer, the restrictions of the function were also specified. The fact that all items must be planned with EA and there may be no mixing is related to the internal program logic. It is not a hard restriction from the customer, however it was accepted because a mixing is not currently practically relevant.

With the environment variables `GESTPLAN_EA_DEPARTMENTS` you can define for which departments the EA should be used as default specification. However, it can also be selected manually for other departments or changed for departments defined in the variables.

### 66.4. Rack main group

Within the configuration `GESTPLAN_PYRO`, the packaging type of the order determines the rack main group of the packaging to be used.
#456030: QR 04/20

In addition, the environment variable `GESTPLAN_OHNE_VERPACKART` was created, which with packaging with the configuration `GESTPLAN_PYRO` enables the packaging type stored in the order to be ignored as basis for the rack main group.

### 66.5. Prices

If you are working in rack planning with individually manufactured racks (boxes), you can calculate prices for the packaging within the rack planning.
**Requirement:**
- Box BOM
- Supplier for the box (`cu_gfert`)

#### 66.5.1. Box supplier

The supplier for a special box type is entered in the table `cu_gfert`. This table is a customer-specific table for which there is no maintenance dialog. If the function should be used, a customer-specific maintenance dialog can be created. The table has the structure
- `gtyp` smallint
- `linr` integer

According to the details in the table `cu_gfert` the appropriate supplier is loaded for the box type. If `xhaus.linr` is entered as a supplier number, the box has to be 'produced in-house'; field "supplier" remains empty.
The supplier can be changed per box/rack. Weight and price of a box are calculated on the basis of the data taken from the BOM. (Price details are defined via the articles of the box BOM). The normal price and condition structure from the order item is not applicable.

### 66.6. Costs

If the rack planning is done in an order and these boxes (variable means of packaging with BOM), then the costs of these boxes are totaled and generated as separate cost surcharge (discount type="costs") in the order. This way, the cost side of the order is changed and the contribution margin adjusted.
The calculation is done in the foreground immediately after the rack planning and can be checked in the discount overview right away.
Prerequisite for the calculation are the BOMs stored in the master data for the boxes and formulas for the price calculation.
The cost surcharge is generated as GR surcharge and is taken over completely only in the 1st partial document (e.g. partial delivery note). The remaining data for the surcharge (name, product group, cost center, account, tax) is taken over from the article number, which must be stored specially for this purpose (e.g. `atype` = other) and entered in the environment variable `RABATT_VERPACKKOSTEN`. Only if this environment variable is active will the discount rate be generated.
The surcharge is always just one-time for an order. If the order is changed and the rack planning done again, the surcharge amount is adjusted.
If a new order is entered as reference, the packaging surcharge is always deleted, regardless of how the question about the takeover of the old discounts was answered.

**Caution:** The surcharge is not written back to the order if the rack planning is called from "Logistics - Rack Management - Rack Planning" or Dispatch and changed.

### 66.7. POs for packaging (boxes)

17.02.2025: Currently the documentation is in the Sharepoint: A+W Clarity R&D - Dokumente\General\Enterprise\BestellKisten.docx
As soon as the module has been tested successfully with pilot customers, the documentation will be taken over into the Enterprise configuration notes.

### 66.8. Log

#### 66.8.1. Standard

**Name:** `kposgpl<MMDD>`

| | |
| :--- | :--- |
| **Source/content** | The log is written by the rack planning in the order entry. |
| **Activation** | The log is always written. There is no expanded log. |
| **Storage location** | The log is in the `$PROTOPFAD`. With internal client separation, this variable is evaluated client-specifically. Normally there is a subdirectory with the appropriate client number. |
| **Notes** | |

#### 66.8.2. Extended

**Name:** `gestplan<pid><mmdd>`

| | |
| :--- | :--- |
| **Source/content** | The log is written by the rack planning in the order entry. |
| **Activation** | The log is written with enabled environment variable `GESTPLAN_PROTO`. |
| **Storage location** | The log is in the `$PROTOPFAD`. With internal client separation, this variable is evaluated client-specifically. Normally there is a subdirectory with the appropriate client number. |
| **Notes** | |

#### 66.8.3. Ftest

| | |
| :--- | :--- |
| **Source/content** | Essentially FTEST messages from the rack planning are possible. However, they are only available to a limited extent. |
| **Activation** | FTEST can be enabled on the dialogs with `<CTRL+F4>`, `<SHIFT+F12>`. |
| **Storage location** | The storage location of the log can be configured as follows: <br> 1. via the variable `FTESTPFAD` <br> 2. If in the path `$DBPATHEXT` there is a subdirectory ftest, logging is done there. <br> 3. If 1 and 2 do not apply, the logging is done in the directory `$PROTOPFAD`. |
| **Notes** | |

### 66.9. Problem handling

**PMPL is canceled with the message "The data is flawed"**
This is the data constellation "Maximum rack weight in the order < weight of a lite." The "maximum rack weight in the order" is drawn from `mp.gmaxgew`.
See also case 166079.
With the document, the plausibility check was changed so that the check only takes place if a "maximum rack weight" > 0 is stored.

**No appropriate box type found**
Although nothing about the master data was changed, no more box was found for identical items.
The problem is that when saving an order, the message appears for the first two items:
"For order xy, item 1, no appropriate box type was found!"
The order can be saved nevertheless, but in production, the rack number is now missing in the work plan.

**The configuration was changed**
The customer uses new cork sheets between the lites. These are now 3 mm thick instead of 2.
That's why the variable `GESTPLAN_DEFAULT_ZWRAUM` was changed from 2 to 3.
e.g. boxes of type A have in the restrictions a maximum depth of 154 mm.
The glass in the order items 1 + 2, for which no appropriate box could be found, is calculated as 9.2 mm in total. The boxes hold 13 lites.
=> 13 * 9,200 mm + 12 * 2mm = 143.6 => that fits
=> 13 * 9,200 mm + 12 * 3mm = 155.6=> no longer fits -> the boxes are no longer found!

### 66.10. Environment variables

- **`GESTPLAN_KUGEST_RESTRIKT` (client reference: no)**
If this variable is switched on, in the packaging material planning, only rack types or rack main groups are used that are assigned to the current market partner.

- **`GESTPLAN_OHNE_VERPACKART` (client reference: no)**
If this variable is active, the packaging type that is stored in the order is ignored in the packaging material planning.

- **`RABATT_VERPACKKOSTEN` (client reference: no)**
The switch activates the logic that the packaging costs (costs of the finished boxes) is shown as cost surcharge and thus flows into the calculation of the DB. (rack planning)
An article number is entered in the switch. The article type should be "999 other article". From this article, the product group, cost center, and name for the discount rate of the type "costs" is used. The costs are taken over from the table `gsergkiste`. The prerequisites are the master data (BOMs) for boxes and formulas for calculation.

## 67. Dispatch control (general)

### 67.1. Switching off the A+W Enterprise dispatch control

The "A+W Clarity Experience Dispatch" module has been available for a few years. In principle, especially in the transition period, parallel operation of the "A+W Enterprise Dispatch Control" and "A+W Clarity Experience Dispatch" is possible. However, to achieve a uniform workflow for the employees, it is possible to deactivated the "A+W Enterprise Dispatch Control" so that only "A+W Clarity Experience Dispatch" can be used. For this, the environment variable `CX_DISPATCH_ONLY` must be activated. On startup of "A+W Enterprise Dispatch Control", the user receives the message 19672 "This module is no longer active."

### 67.2. Environment variables

- **`CX_DISPATCH_ONLY` (client reference: user)**
This environment variable deactivate the acess to the "Dispatch Control" module. This is intended if you want to work only with the "A+W Clarity Experience Dispatch" module.

## 68. Rack-related shipping

### 68.1. Prerequisite

If you want to work with rack-related shipping, the environment variable `LAPOOL_FREIGEST=2` and the environment variable `FREIGEST_SPEZIAL=ON` or 1 have to be active.

- `LS_MIT_GESTELLNUMMER = ON` activates the check for delivery note
- For correct processing of the rack report, `AWC_GESTZU_BUCHEN` has to be set.
- Since the rack assignment only works if the associated quantities in dispatch are not yet packed, the variable `AWC_IGNORE_PACKINGMESSAGE` also has to be activated.

**AWC_IGNORE_PACKINGMESSAGE**
If you work with rack-related shipping and the rack should be permanently assigned from AWP rack reporting, this variable must be used to prevent a packing notification from the AWP from being processed beforehand.
Furthermore, the value can be set to "SUPPRESS-RDY-MSG"; then the completion report from AWP is not processed.

The following variable must absolutely be set in order to combine collective packing racks that were created by assignment to different routes in dispatch automatically and be able to assign them to the route. This action can be performed on the "Rack to order" dialog with `<F3>`.

**LAPOOLMOVE_TOURENPLAN**
The variable activates the additional reason for the shift at route level: route planning. Data is moved according to the customer's request. You can also use `LAPOOL_ROUTE_GRUND` to activate the reason for the default setting.

### 68.2. Free racks

In case #342547, a function for handling free racks in shipping was developed.
With the cases #459400/459099 (among others), the handling of free racks in shipping was expanded.
`AWC_PORT_NR_SERVER` must be set and refer to the number server port. This way, the number range `torservid` is queried. This way, a booking ID for the rack loading is assigned. This excludes double bookings.

### 68.3. Lite allocation

The manual rack-lite allocation can be done via `Logistics -> Rack management -> Lite allocation` or `Dispatch control -> <Shift+F4> -> Rack->Lite allocation`.
Here it must be noted that different program logic underlies the menu elements named although the dialogs look the same. Only when calling from dispatch control is there a comparison with the dispatch data. For the lite allocation via the rack management module, by contrast, there is no check of whether or not the order is already present in dispatch. This distinction is conditions by different workflows. In case of deviating program behavior, the terms rack management variant and dispatch variant are used below.

*Figure 131: Rack allocation*

A lit allocation or change of the rack allocation is essentially possible as long as the rack has not yet been assigned to a dispatch route ("free rack"). In the course of an internal client separation, for the rack variant with the first allocated order, the company of this order is assigned to the rack, so that subsequently only orders from this site can be assigned to the rack. In the dispatch variant, the street address is already determined by the pre-allocation of the site number with the calling of the dispatch module, and there are no orders from other sites available.
As soon as the rack is permanently assigned to a route (rack allocation `<Ctrl G>`), changes to the rack content are no longer possible, no additional order items can be added via the lite allocation. The route allocation is visible in the header of the dialog. Here, route number and driving date are displayed.
If a rack is allocated to a route, then it is not possible to empty it. This is only possible if it is either still free or if it counts as delivered in dispatch (delivery note has been created). Only then can the rack be emptied using the key combination `<Ctrl+F8>` and a new allocation specified.
A manual lite allocation is normally not required if a booking of the rack from production and/or warehouse is configured. In this case, the individual lites are already booked to racks in the PPS and transferred to dispatch with the company-external message (or an outgoing booking in the rack warehouse). If for such a booking all rack items in dispatch are on the same route (delivery date + route), then the rack is also assigned to this route automatically and the units found on it are displayed as "packed."
After entry of the rack number and the type (optional), in the rump portion of the screen it is possible to enter an order number. With the key combination `<Ctrl+F10>`, all data for this order is loaded into the "Item" and "Quantity" fields.
The "Total" field contains the complete item quantity. In the "Available" field, the number of lites is displayed that can still be assigned (because, e.g. a partial quantity of the item was allocated to another rack). If there is appropriate data in the dispatch (see limitation above), then the "Dispatch route" and "Delivery date" fields display the earliest dispatch date.

**Booking racks via PDC**
The rack bookings from PDC readings are reported by A+W ERP Web Services via feedback servers. Reporting is done in two steps.
Lites - rack assignment via `rserv` (status 19)
(data in the table `torserv` + `rserv`)

| Rack recognized (gest) | Rack locked in the foreground | Fixed assignment to route | All delivered | Deadline passed | Is there already an assignment of the lites (gestzu) | What happens/booking |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| X | X | | | | | Booking rejected. Error message |
| X | 0 | X | X | X | - | Delete old data in `gestzu` + book assignment (`gestzu`) Update: `gest.routnr` = 0 `gest.ltdat` = 0 |
| X | 0 | X | X | 0 | | Booking rejected. Error message |
| X | 0 | X | 0 | | - | Booking rejected. Error message |
| X | 0 | 0 | | - | 0 | Book assignment (`gestzu`) Update: `gest.routnr` = 0 `gest.ltdat` = 0 |
| X | 0 | 0 | | - | X | Booking rejected. Error message |
| 0 | 0 | | - | | - | Assignment. Table `gestzu` and entry in `gest` Insert: |

**Rack assignment via `rserv` (status 20)**

| Rack recognized | Rack locked in the foreground | Fixed assignment to route | Appropriate dates in shipping | Enough unpacked quantity | What happens/booking |
| :--- | :--- | :--- | :--- | :--- | :--- |
| | | | | | `gest.routnr` = 0<br>`gest.ltdat` = 0 |
| X | X | - | | | Booking rejected. Error message |
| X | 0 | X | - | | Booking rejected. Error message |
| X | 0 | 0 | X | 0 | Booking rejected. Error message |
| X | 0 | X | X | X | Execute booking<br>(`gest.route` = `lapool.route`, `gest.ltdat` = `lapool.ltplan`)<br>Report packed quantities (`lapool.iststk`) |

Bookings for status 19/20 are always reported in pairs by the A+W ERP Webservices, never separately.

### 68.4. Moving in dispatch

For the moving in dispatch there are differences, depending on the level on which the move takes place. For the moving of a complete route, all data including all permanently allocated racks are moved from the source to the destination route. Free racks remain free on the destination route, already-allocated racks are assigned to the destination route.
On the order level, a moving can only take place if the order contains only free quantities. Such quantities are designated free quantities that either do not yet have a rack allocation or are on free racks.
If you postpone an order that is completely on one or distributed across several racks, you can enter a number directly in the "Rack" field if it is known or use the selo to select a rack: (11/2020: **New, new selo `gestauftrinfolock.sel`**)
As soon as a part of the order is already on one or several permanently-allocated racks, the simple direct moving on the order level is not possible.
If during the order moving it is determined that the selected order is on racks completely assigned to one or several routes, then the user is informed of this and can then perform a rack-by-rack moving using the rack view screen (`<F5>`).

First the data for all racks is loaded on which the items of the order to be moved are located. If items for additional orders are on these racks, these are also displayed. The move is triggered with `<Start>` (`<F3>`). This way only a complete rack can be moved (the one for which you press `<F3>`).

**11/2020: New on the dialog:** the entire quantity from this order for the item is not displayed, but rather the packed quantities that are reported on this route. The postponement can only take place if the quantities reported packed are sufficient. If due to incorrect booking the quantities are not right (if the booked rack has to be postponed, then the packed quantities also have to be postponed), this is reported and data from the rack has to be checked.

*Figure 132: Moving racks in dispatch*

Orders that contain both free and quantities on a permanently-allocated rack are displayed in the status display with a half-yellow traffic light. If you only want to move the free quantities of the order, then this action can be performed either on the item level or using the menu element "c Move several items" / "`<Ctrl+E>`").
If you do not select a particular rack, but instead start the rack overview with `<F5>`, then all booked racks are displayed for the selected order including all third-party order items that are on these racks.

*Figure 133: External order on the rack*

From this overview, you can postpone only the current rack on which you have positioned yourself. To postpone additional racks, you have to repeat the procedure.
If due to rack postponement several orders are postponed, then the view of the order level is not updated immediately for all affected orders. To be certain that the overview is up-to-date, you should update it manually. Please be careful, we're working on this.

#### 68.4.1. Shifting permanently booked racks

If the racks were booked permanently, from PDC or manually, and if they have to be rebooked to another route, then this can now be done via `Shipping control -> <Shift+F4> -> Rack -> the booked Rack (overview)`.
All permanently booked racks for the current route are displayed here. The desired racks can then be marked and shifted with `<F3>`.

*Figure 134: Move dialog*

Here again, the data is assigned with the current route and can then be changed. If a different route is entered, all rack quantities are shifted and the rack is rebooked permanently. Here, the packed quantity is always shifted, even if the shift is done on an earlier date.

### 68.5. Rebooking the rack quantities

Quantities that are already on a rack can be rebooked both via the rack overview dialogs as well as by calling an individual rack on another rack. This applies both for free and for assigned racks.
Using the rebooking function, no rack quantities can be deleted.
If a rack is already permanently allocated to a route, then a rebooking is only possible to a free rack or to a rack that is also allocated to this dispatch route. By rebooking a permanently-allocated rack to another permanently-allocated rack, nothing changes in dispatch since this is only an allocation of the packed quantities.
If quantities are rebooked from a free rack to an already permanently-allocated rack, then these rebooked quantities are reported "packed" in dispatch. In the reverse case, if quantities of a permanently-allocated rack are rebooked to a free rack, then these quantities count as unpacked in dispatch.

Example: two permanently-booked racks on a route:

*Figure 135 Overview of all racks*

Here there are two possibilities for rebooking the rack quantities:
a. Rebooking on a permanently-allocated rack that is on the same dispatch route:

*Figure 136 Quantity rebooking*

The result of this action is that the partial quantities of the item 239598/1 (12 pieces) are rebooked to the rack 00003 and the remaining 8 pieces remain on the original rack 00001.

*Figure 137 Results of the quantity rebooking*

b. Rebooking to a free/empty rack 00008

*Figure 138: Rack rebooking*

With the following result:

*Figure 139 Results of rebooking to a free rack (All/Complete option `<Shift+F8>)*

From the original rack 00003, 20 pieces apiece of the items 2 and 3 are unpacked and un-booked. These quantities are now rebooked to the free rack 00008 (red marking in the overview). Since rack 00008 is a free rack, you can see that the fields Delivery date/Route are not filled.
In dispatch, the situation is as follows:

*Figure 140 Order info (order 239600)*

The packed quantities are reduced and the order has lost its complete marking.
Since the rebooked partial quantities of the order 239600 are now on a free rack, they can either be moved using the "Move several items" (Ctrl+E) function

*Figure 141: Move several items in dispatch*

or from the item level of dispatch.

*Figure 142: Moving in dispatch*

In both cases, the free quantities are calculated the units to be moved are suggested.
After the moving of the rack 00008, the quantities in dispatch look like this:

*Figure 143: Information regarding rack in dispatch*

On the original route 30.10.2015/10, there are only the permanently assigned racks 00001 and 00003. The postponed quantity on rack 00008 is on the route 06.11.2015/10.

### 68.6. Mistaken quantity check

The "Mistaken quantity check" is currently not supported for this type of dispatch configuration.

### 68.7. Correct packed quantity

The menu element "Correct packed quantity" cannot be entered when using the module.
Correction of the packed quantity is only done via rack allocation or rack break-up.

### 68.8. Delivery notes from dispatch

If rack numbers should be printed on the delivery notes, during generation of the delivery notes it can be checked whether all orders have a permanent rack allocation. This check can be configured and is not active by default. With an activated check, there is a query whether the delivery notes should be generated nevertheless. The query is a CU query and can be switched so that it is appropriately restrictive.

### 68.9. Correction of mistaken bookings

#### 68.9.1. Rack bookings reported from PDC

Via `Logistics -> Rack Management -> Lite Assignment`, the correction can be made as follows:
(note: the handling is controlled by access right GESZ)
1. Call up rack

*Figure 144: Rack allocation*

2. With `<Ctrl+F8>`/empty, you can empty racks that have not yet been delivered:
