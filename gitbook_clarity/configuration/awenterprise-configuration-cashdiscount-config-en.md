---
description: "EN-CONFIG-AW_Enterprise_11"
---


| | **401** | **301** | **201** | **101** |
| :--- | :--- | :--- | :--- | :--- |
| **Condition** | 401 | 301 | 201 | 101 |
| **Deadline 1** | 15: 07/10/2021<br>(06/25 + 15 days) | 15: 07/30/2021<br>(07/15 + 15 days) | 15: 08/15/2021<br>(07/31 + 15 days) | 15: 08/30/2021<br>(08/15 + 15 days) |
| **Creation date 1** | 15: 07/15/2021<br>next possible Date | 15: | 15: 08/15/2021<br>next possible Date | 15 |
| **Creation date 2** | 30 | 30 (next possible<br>date: last day of the<br>month) | 30 | 30: 08/31 (next<br>possible date: last<br>day of the month) |
| **Following record** | 301 | 201 | 101 | - |
| **Due date** | 2021-07-15 | 2021-07-31 | 2021-08-15 | 2021-08-31 |
| **Amount** | 308.50 | 308.50 | 308.50 | 308.50 |

---
## Additional configuration possibilities: Alternative 1

In the market partner master data, Payment tab, Cash discount 1 field, a payment term (e.g., 2) can be stored. This condition can include a following condition in the key cash discount conditions.

*(The image "Figure 164: 1st alternative for following conditions" shows a user interface for setting up payment conditions. In the main "Marktpartner" window, under the "Zahlung" (Payment) tab, the "Skonto 1" field is set to a value of '2', which corresponds to a payment condition named "Testskonto (nach 2 Monaten...)". A dialog box for this payment condition (ID 2) is open, showing its details. Crucially, it has a "Folgebedingung" (Following condition) field, which is set to a value of '3'. This demonstrates how one payment condition can lead to another.)*

## Additional configuration possibilities: Alternative 2

In the market partner master data, Payment tab, Cash discount 1 field, a payment term (e.g., 2) can be stored; in the Cash discount 2 field, another cash discount condition (e.g., 3) can be stored. In the key cash discount conditions, these cash discount groups have no additional following conditions.

*(The image "Figure 165: 2nd alternative for the cash-discount configuration" displays a user interface where two separate cash discount conditions are configured. In the "Marktpartner" window, "Skonto 1" is set to '2' and "Skonto 2" is set to '3'. The pop-up windows for both condition '2' and '3' are shown. Unlike the first alternative, the "Folgebedingung" (Following condition) field in both of these windows is blank, indicating that they are independent conditions and do not chain into one another.)*

This possibility offers simplified conversion processes due to retention of existing keys, avoids unexplained circumstances with simultaneous use of following conditions in the market partner master data and cash discount master data, thus simplifies the texting on reports.

This configuration possibility has been used at Interpane since 2011.

## 86.3. Database structure

The key cash discount conditions are found in the DB table `xxskonto`. The calculated (or determined) values for the respective invoice are found in the table `rechfuss`.

The table `rechfuss` includes no sensible data for the use of due dates; therefore a FinAc and report adjustment would be required.

Invoices with due dates can be recognized by the flag `kauf.skontoart=1`.

The partial amounts with their respective due dates are saved in the table `zahlplan` (in the invoice under menu `<F4>` > Payment schedule).

## 86.4. Conversion at customers

1.  **1st step:** Since simple and extended logic cannot be operated in parallel in the real-time system, the data is maintained on a test client (if possible, while retaining the existing keys).
    - **Advantage:** In the existing MP master data, no larger adjustments must be made (only for partners with new/changed payment terms).
    - **Advantage:** Simplified conversion of the transaction data since the cash discount conditions are already present in the document (`kaufp.skonto1-3`, `kauf._skonto1-3`, `kauf.sktage1-3`).
2.  **2nd step:** Transfer of the key data to the real-time system (via unload/load).
3.  **3rd step:** Activation of the new logic in the real-time system.
4.  **4th step:** Conversion of the transaction data (open documents at the time of the conversion).

### Reference to non-converted documents

In individual cases, it can happen that reference should be made to documents that were already completed before activation of the logic and therefore were not converted:
- Credits (invoices will not be converted)
- Complaint orders

For these, the following is recommended:
1.  Alternative 1: Suppressing of the reference
2.  Alternative 2: Obtaining of the cash discount conditions from the MP master data with reference to old documents:
    - via `vorgangs_sql` after saving the document
    - In the foreground for invoices, PU invoices, credit notes, and PU credit notes

## 86.5. Cash discount before VAT

**Active environment variable:** `SKONTO_VOR_MWST` (client reference: no)

The cash discount determination is based on the following cash discountable amount:

> Skontierbarer Betrag = (Summe aller skontierbaren Positionspreise / Summe aller Positionspreise) * Netto-Total

The VAT is calculated (environment variable `MWST_SPECIAL` deactivated):

> (Nettototal - Skonto) / 100 * MwSt [%]

If the environment variable `MWST_SPECIAL` is active, the VAT is calculated:

> Nettototal / 100 * MwSt [%]

## 86.6. Cash discount after VAT

**Deactivated environment variable:** `SKONTO_VOR_MWST` (client reference: no)

The cash discount determination is based on the following cash discountable amount:

> Skontierbarer Betrag = (Summe aller skontierbaren Positionspreise / Summe aller Positionspreise) * Gesamt-Brutto

The VAT is calculated:

> Nettototal / 100 * MwSt [%]

## 86.7. Configuration

### MWST_SPECIAL (client reference: no)

Only applies if the variable 'SKONTO_VOR_MWST' is active and must be understood as complement to it. However, it is overridden by `SKONTO_MWST_LOGIK`.
The cash discount is calculated before the VAT, but the VAT is not deducted from the net amount less cash discount, but instead from the original net amount.

### SKONTO_SPECIAL (client reference: no)

With the variables, the alternative procedure for cash discount records in the customer master and in the order is activated. Table `xxskonto`.

### SKONTO_MWST_LOGIK (client reference: no)

This variable overrides `SKONTO_VOR_MWST` and `MWST_SPECIAL`.

**Variants:**

1.  `discount = net total * discount%`
    `VAT = (net total - discount) * vat%`
    `Gross = net total - discount + vat`
2.  `discount = net total * discount%`
    `VAT = net total * vat%`
    `Gross = net total + vat`
3.  `discount = gross * discount%`
    `vat = net total * vat%`
    `Gross = net total + vat`
4.  `discount = net total * discount%`
    `vat = net total * vat%`
    `Gross = net total + vat`

**Note:** 2 and 4 only differ due to the display in the order (footer).

### SKONTO_VOR_MWST (client reference: no)

In some countries (e.g. France or England) it is usual to calculate the cash discount before value added tax (i.e. from the net amount). This can be achieved with this switch. `SKONTO_MWST_LOGIK` overrides the variable.

## 87. Selection of Windows files via the "File open" dialog

In interplay with the A+W CAD Designer (Shapes), in A+W Enterprise, files are assigned to an article or an order item that are stored on a Windows system. This affects:

- SN files (also for synchronization with the item)
- DXF files
- SN macro files
- Motif files

Since for these files, depending on the configuration in the EDI a FTP transfer under Unix is executed, restrictions apply here with regard to the characters that can be used in file names.

**Permitted characters in file names are:**
- Letters: A-Z and a-z
- Numbers: 0-9
- Special characters: "_" (underscore), "." (dot), "-" (minus), "+" (plus), "," (comma)

**Other characters, especially umlauts, are not permitted.** After selection of a file via the "File open" dialog, the check of the file name for illegal characters is done. Impermissible file names are then rejected.

For files that are assigned to an article or item in the context of the declaration of performance, the same rules apply.

See PF [AW-119029] and [AW-128380].

## 88. ViaPlant/via Plant

A+W Enterprise dispatch control offers this function that allows a company (site A) to organize shipment via a second site ("via plant"), i.e. the goods will be shipped from site A to the "via plant" site and from there on to the customer. That is, the goods are first transported from site A to the "via plant" site and from there to the customer. Which prerequisites are required to use the function and which consequences this produces in the overall system is described in detail in "EN-CONFIG-A+W Enterprise Internal client separation".

## 89. Intrastat

All information about the configuration of the Intrastat message and the operation of the booking dialog is in the configuration document "A+W Enterprise Intrastat XML Connector" on the Sharepoint.

## 90. Subscriber

The subscriber is an A+W-internal help program for correcting FinAc and statistics bookings. The application is documented in a separate internal document: `SharePoint A+W Clarity R&D - Dokumente\Interfaces\Enterprise\FinAc Interfaces\General\ AWE FinAc Info Intern.docx`

## 91. Data warehouse

### 91.1. Configuration

> **ATTENTION:** This module is not currently released for multisite or call center.

Since 2001 the A+W Enterprise (Alcib) has the data warehouse system for order inventory (AWD 26904, 43201, 43765). This is a for-fee module. It must be provided by the module environment variable `MODUL_DATAWAREHOUSE` and activated with the value "ON".

In the early versions, there were various scripts that create the necessary data structures on the ALCIB side. If necessary, these scripts must be checked and executed. All scripts are in the TOOLS area in the `sql/bosql` directory. The scripts with the ".sql" extension must be executed with the command: `cat scriptname.sql | isql $DBNAME`.

In order to create the data warehouse tables in the A+W Enterprise database if necessary, the following scripts must be executed:
- `dwTabellen.sql`: creates the tables.
- `dwIndex.sql`: creates the indices for these tables.
- `dwsend.sql`: creates a table in which the orders to be booked are kept.

In order to transfer the master data from A+W Enterprise to the DataWare master tables, the following scripts must be executed:
- `fillBran.sql`: Industries.
- `fillClaim.sql`: Complaint master data (Art, Ort and Spec).
- `fillCoce.sql`: Cost centers.
- `fillCoe.sql`: Manufacturing cost elements.
- `fillCont.sql`: Projects.
- `fillCountry.sql`: Countries.
- `fillPartn.sql`: Customers and suppliers.
- `fillProduct.sql`: Articles.
- `fillRegion.sql`: Regions.
- `fillSite.sql`: Sites.
- `fillStaff.sql`: Employees.
- `fillWaregroup.sql`: Product groups.
- `dwmd_coe`: specifies a manufacturer cost group. (Must be executed with "fslo dwmd_coe").
- `dwmd_sae`: specifies the revenue elements. (Must be executed with "fslo dwmd_sae").
- The actual transmission of the master data is triggered with the script `fillDWMD_all`. This action must be performed once during initial installation and periodically in ongoing operation (e.g. weekly). In ALCIB there are particular master data that is provided with the change date. This data can be booked daily with the script `fillDWMD_daily`.

For the booking of the transaction data, a few stored procedures are required, which are created with the following scripts:
- `dwSendProcess.sql`: Main booking SP (calls up the following SPs).
- `dwSendProcessHead.sql`: SP for booking the document header information.
- `dwSendProcessItem.sql`: SP for booking the item information.
- `dwSendProcessItCo.sql`: SP for booking the production costs.
- `dwSendProcessDisc.sql`: SP for booking the footer discount.
- `pkBetragInEW.sql`: SP for recalculating amounts from foreign currency to own currency.

If the booking of the DW tables should be done with ctrl_server control, then the following steps must be performed:
- The environment variable `DW_CTRLSERV` must be activated with the value "ON".
- The booking program `statserv` must be delivered.
- Change to the directory where the configuration file of the ctrl_server is with the `ga` command. The file `ctrl_serv.par` must be expanded by one entry to start the `statserv`:

**Example:**
`Statistics booker ^SOB^SOS^SOW^SOE^SOX^statserv^romulus^statserv^60^900^116^ 31571^^stat.log^`

- `romulus` - Customer computer
- `116` - Employee number of the person who should get the message about the booker.

### 91.2. Writing the anchor record

Only the table "dwsend" is written by A+W Enterprise, by intauf or the booker. All other tables are booked by individual SPs.

### 91.3. Processing of the anchor set

The statistic booker reads all records from `dwsend` with state = -2 (in processing) or 0 (new) and processes these. It writes a log according to `statMMDD` in `$PROTOPFAD`. If `TEST_STATSERV` is set, an expanded log will be written.

In case of error, the record will be re-presented to the booker.

Starting the statserv process is done via the CTRL server via `sctrl SOB` (if necessary, + `$HAUS`).

## 91.4. Booking of the data warehouse tables for order data

The table `dwo_head` includes the header data for the order and is filled by the SP `SendProcessHead`.

| Order header (dwo_head) | Data Type | A+W Enterprise DB field | Remark |
| :--- | :--- | :--- | :--- |
| **ext_ordno** | num 10,0 | kauf.auftrnr | Order number |
| **int_ordno** | num 10,0 | kauf.aufnr | internal order number |
| **type** | num 10,0 | kauf.vorgang | 5 = Order |
| **ordkind** | char(2) | kaufp.kaufart | Type of order |
| **siteno** | num 10,0 | kauf.hausnr | Site number |
| **e_date** | date | kauf.edat | Date the order was received |
| **d_date** | date | kauf.ltplan | Deliv. date |
| **cuno** | num 10,0 | kauf.kunr | Customer number |
| **contno** | num 10,0 | kauf.objnr | Project number |
| **country** | char(3) | kauf.orgkfzcode | Country from customer address |
| **reno** | num 10,0 | mp.region selected with cuno. | Territory (region) of the customer |
| **brno** | num 10,0 | mp. kbranche selected with cuno. | Condition branch of the customer |
| **salesrep_1** | num 10,0 | kauf.vertrerlbe | The employee number of the customer's sales representative |
| **salesrep_2** | num 10,0 | kauf.vertrerlbe | The employee number of the customer's sales representative |
| **salesval** | num 18,6 | kauf.nettototal calculated in own currency | Net total sales value |
| **costval** | num 18,6 | kauf.ektotal | Total purchasing value |
| **cashdisc** | num 18,6 | kauf.skvh1 | Amount of the cash discount |
| **claim_reas** | num 10,0 | kaufp.reklamart | Reason for the complaint |
| **claim_place** | num 10,0 | kaufp.reklamort | Location of the complaint |
| **claim_type** | num 10,0 | kaufp.reklamspec | Complaint type |
| **cancel** | num 10,0 | | 1 = cancelled |
| **spec_no1** | num 10,0 | kaufp.private_long1 | User-defined numeric field |
| **spec_no2** | num 10,0 | kaufp.private_long2 | User-defined numeric field |
| **spec_char1** | char(15) | kaufp.private_char1 | User-defined text field |
| **spec_char2** | char(15) | kaufp.private_char2 | User-defined text field |
| **dept_no** | num 10,0 | | |
| **inv_no** | num 10,0 | | |
| **inv_flag** | num 10,0 | | |
| **deliv_flag** | num 10,0 | | |

**Key of the table `dwo_head` is:** `int_ordno` and `siteno` or `ext_ordno` and `siteno`.

---
There is another (older) document under
`\\hausi\BUG\A+W_Allgemein\Entwicklung\Uebergreifende Projekte\Data-Warehouse\20010206_Controlling_ERP.doc`
