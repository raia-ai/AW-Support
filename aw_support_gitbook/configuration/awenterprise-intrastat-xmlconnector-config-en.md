---
description: "EN-CONFIG-AW_Enterprise_Intrastat_XML_Connector"
---


# A+W Configuration: A+W Enterprise Intrastat XML Connector

-INTERNAL-

*A+W - Software for Glass*

---

---
## Change history

| Date       | Author | Remarks                            | Version |
| :--------- | :----- | :--------------------------------- | :------ |
| 2022-02-10 | EB     | Original version (separate document) | 1.0     |

## Content

1.  **Intrastat**
    1.1. General Information
    1.2. Requirements
    1.3. env variables
    1.3.1. INTRASTAT_NEU
    1.3.2. INTRASTAT_MIT_RECHADR
    1.4. Process
    1.5. Export of the Intrastat data
    1.6. Master data maintenance
    1.6.1. Country code
    1.6.2. Regions/Federal states
    1.6.3. Type of business
    1.6.4. Dispatch type
    1.6.5. Specifying the product codes
    1.6.6. Article master data
    1.6.7. Market partner adjustments
    1.7. Order entry
    1.8. PO
    1.9. The booking of the intrastat table
    1.9.1. Booking of partial invoices
    1.10. List Printing
    1.11. Notes

---

## 1. Intrastat

### 1.1. General Information
The trade statistics between the member states of the European Union – Intrastat statistics – are kept by the German Federal Statistics Office and serve the purpose of providing current data about the internal trade in Germany in a wide variety of classifications.

This data is required, among other things, to conduct analyses of European competitive ability.

The goal of the statistical examination is exclusively the display of actual goods movements between Germany and other EU member states.

Viewable with the Intrastat module – on the menu branch `System -> Statistical Data -> Intrastat` – it is possible to create standard goods messages about trade with other EU states in AWE.

### 1.2. Requirements
For the messages to the German Federal Statistics Office, various codes are specified, such as:
- Country code
- Type of business
- Modes of transport
- Region/Federal state

The maintenance of the data that is required for Intrastat for A+W Enterprise is done on the respective menus under `Master data => Keys => etc.`

Furthermore, goods catalogs and the product codes arising from these are required, whose maintenance is done under `System => Statistics data => Intrastat`.

Then the assignment should be made in the master data of the market partners and articles.

### 1.3. env variables

#### 1.3.1. INTRASTAT_NEU
The variable was introduced with AWDesk #36918 (in 2002). Here, the prerequisites for the automatic generation of data for Intrastat transfer were reworked.

Due to activation of the variables with "ON" the reworked logic becomes active.

Part of the new logic is that if the shipping address is missing, the invoice address is used as the destination address.

The variable should always be set.

#### 1.3.2. INTRASTAT_MIT_RECHADR
The variable was introduced with AWDesk #27164 (in 2000). If the variable is active with "ON", for the "old" Intrastat message (with not set env variable INTRASTAT_NEU) for a goods shipment, the invoice address of the goods recipient is used as destination address if no delivery address is specified.

> **Caution:** in the "new" Intrastat logic (env variable INTRASTAT_NEU active), the variable is no longer evaluated; the invoice address is automatically considered for missing shipping address.

### 1.4. Process
Bookings in the Intrastat are done in case of an order after the invoicing and in case of a PO after the purchase invoice check. The prerequisite is that an Intrastat country code is stored in the master data for the countries in question and the processes refer to addresses in these countries.

1.  Intrastat booking via order entry is done only after invoicing. The booking is done under the document number in question.
2.  Intrastat booking via a PO proposal is done with the invoice checking and is also booked under the specified document number.

### 1.5. Export of the Intrastat data
With [AW-84955] a module is made available in the AWE FinAc Service for exporting the Intrastat data in xml format.

For detailed information, see the configuration instructions for the AWE FinAc Service.

### 1.6. Master data maintenance
The maintenance of the Intrastat master data is done using menus, which are described in detail below.

#### 1.6.1. Country code
The codes for the country Intrastat statistics are stored on the menu `Master Data -> Keys -> Market Partner -> Countries -> Countries` in the field "Intracode".

**Figure 1: Intracode in country key table**
| KFZ | ISO | Landesbezeichnung        | FIBU | Intracode |
| :-- | :-- | :----------------------- | :--- | :-------- |
| A   | AT  | Österreich               | A    | AT        |
| AL  | AL  | Albanien                 | AL   |           |
| AUS | AU  | Australien               | AUS  |           |
| AZ  | AZ  | Aserbaidschan            | AZ   |           |
| B   | BE  | Belgien                  | B    | BE        |
| BG  | BG  | Bulgarien                | BG   | BG        |
| BH  | BH  | Bahrain                  | BRN  |           |
| BIH | BA  | Bosnien und Herzegowina  | BIH  |           |
| BN  | BN  | Brunei                   | BRU  |           |
| BR  | BR  | Brasilien                | BR   |           |
| BY  | BY  | Weißrussland             | BY   |           |
| CA  | CA  | Kanada                   |      |           |
| CH  | CH  | Schweiz                  | CH   |           |
| CHN | CN  | China                    | CN   |           |
| CY  | CY  | Zypern                   | CY   | CY        |
| CZ  | CZ  | Tschechische Republik    | CZ   | CZ        |
| D   | DE  | Bundesrepublik Deutschland | D    |           |
| DJ  | DJ  | Djibouti                 | DJI  |           |

In the `Intracode` field the appropriate Intrastat keys have to be assigned to the country names.

> **Warning:**
> All countries for which an Intrastat country code is entered here are identified as EU member states.
> For your own country, no key may be entered here; otherwise deliveries within your own country will be booked in the Intra-trade statistics.
> In multisite systems, however, it is possible that the main site is assigned to another country than the subsite(s) and that a different, non country-specific Intrastat booking is configured with the Config tool of the AWE FinAc service.
> In this case, the Intrastat key of your own country (main site) must be stored. Bookings (intrastat table) within your own country will be detected by the FinAc service in this case and sorted out after the fact before the Intrastat file is generated.
> See also PF [AW-158197].

**Notes**
Since 1/1/1999, the new country codes are no longer numeric according to the specifications of the German Federal Statistics Office.

#### 1.6.2. Regions/Federal states
This data is maintained under `Master Data > Keys > Market Partner > Region/Federal states`.

**Figure 2: Regions/Federal states**
| Nr | Spr | Region/Bundesland      |
| :- | :-- | :--------------------- |
| 1  | 1   | Schleswig-Holstein     |
| 2  | 1   | Hamburg                |
| 3  | 1   | Niedersachsen          |
| 4  | 1   | Bremen                 |
| 5  | 1   | Nordrhein-Westfahlen   |
| 6  | 1   | Hessen                 |
| 7  | 1   | Rheinland-Pfalz        |
| 8  | 1   | Baden-Württenberg      |
| 9  | 1   | Bayern                 |
| 10 | 1   | Saarland               |
| 11 | 1   | Berlin                 |
| 12 | 1   | Brandenburg            |
| 13 | 1   | Mecklenburg-Vorpommern |
| 14 | 1   | Sachsen                |
| 15 | 1   | Sachsen-Anhalt         |
| 16 | 1   | Thüringen              |

The numeric keys are specified by the German Federal Statistics Office and specify precisely the number of the (German) federal state.

In the market partner master data, in the **Region** field (References tab), the company's code is stored so that the region can be entered in the Intrastat booking.

**Figure 3: Assignment of the appropriate region in the market partner master data**
This figure shows the market partner master data screen where a user can select the appropriate `Region` (e.g., 'Schleswig-Holstein', 'Hamburg') for a specific partner.

#### 1.6.3. Type of business
On the menu `Master Data -> Keys -> Market Partner -> Complaint -> Reasons -> Reasons for Complaint`, the type of business is assigned for the complaint reason.

**Figure 4: Reasons for complaint dialog**
| Nr | Reklamationsgrund       | Intrastat |
| :- | :---------------------- | :-------- |
| 1  | Verpackung kaputt       | 1         |
| 2  | Scheibe kaputt          | 1         |
| 3  | Falsche Lieferung       | 1         |
| 4  | Lieferung unvollständig | 1         |
| 5  | Sonstiges               | 1         |
| 6  | Glasbruch               | 1         |
| 11 | Endgültiger Kauf         | 11        |
| 12 | Ansicht/ Probesendung   | 12        |
| 21 | Rücksendungen           | 21        |

This dialog contains the `Keys` field with the number for the internal statistics. The assignment of the business type is stored in the `Intrastat` field. In this case, the complaint type makes the assignment of the business type in the Intrastat booking (see example 11, 12, 21). Here, assignments for complaints in internal trade could also be set up.

#### 1.6.4. Dispatch type
In the menu `Master Data -> System Keys -> Shipping -> Shipping type`, the type of transport - according to the means of transport with which the goods will leave/reach the company location - is stored.

**Figure 5: Type of transport - assignment in shipping type key table**
This view allows assigning a transport type (`Verk`) and a transport surcharge (`Transportzuschlag`) to a shipping type (`Bezeichnung`). For example:
- **LKW:** `Verk` = 3 (Landstraße), `Transportzuschlag` = 2.00
- **Luftfracht:** `Verk` = 4 (Luftverkehr), `Transportzuschlag` = 5.00
- **per Express:** `Verk` = 3 (Landstraße), `Transportzuschlag` = 4.50

In the `Transport surcharge` field, the surcharges to be considered for the statistical value can be entered in percent.

#### 1.6.5. Specifying the product codes
Under the menu `System -> Statistics Data -> Intrastat -> Product Index`, the product index can be kept.

**Figure 6: Product index**
This screen allows defining Intrastat product codes. Key fields include:
- **Warennummer:** e.g., 70071910
- **Maßeinheit:** e.g., Stück
- **Warenbezeichnung:** e.g., Isolierglaseinheit

The product index with its numbers and titles is created here according to the requirements of the German Federal Statistics Office.
If a quantity unit is also stored here, in the Intrastat to which this goods number was assigned in the article master data, a physical quantity is also booked. The quantity unit stored here must match the quantity unit of the article to which the goods number is assigned.

The specifications of the German Federal Statistics Office have to be heeded for the structure, organization, and content of product indices. Furthermore, the people who are entrusted with the creation and maintenance of the product index have to ensure that the registration of the goods for foreign trade statistics is always done according to the valid product index for foreign trade statistics.

#### 1.6.6. Article master data
In the article master data, on the **Statistics** tab, the product codes for the goods to be registered in the intra-trade statistics are assigned.

**Figure 7: Intrastat code in article master**
This figure shows the article master data screen. On the 'Statistik' tab, a user can enter the `Intrastat` code (e.g., 70071910) for a specific article.

#### 1.6.7. Market partner adjustments
The branching to the country code is done via the CAR identifier in the market partner master data.

For a customer whose location/company headquarters is in an EU member state, the delivery address should be stored as main address.

In the menu `Master Data -> Market Partner -> Menu -> Addresses`, the main address is switched on with `<Detail>` (`<A5>`).

**Please note:**
- If for the customer no main address is entered in the master data and INTRASTAT_NEU is enabled, a delivery address must first be entered in the document entry since otherwise no Intrastat booking will be generated.
- If for the customer record for the site the region is not entered, this field will not be filled in the Intrastat booking.

### 1.7. Order entry
The following points have to be noted in the order entry:

1.  For a customer whose delivery address lies in an EU member state, it is possible to select the delivery address with the additional menu `<MENU>` (`<F4>`). The delivery address overrides the main address stored in the master data. It is absolutely necessary that the delivery address refer to an EU member state since otherwise no Intrastat booking will be generated.
2.  By default, the business type "11" final purchase/sale is entered in the Intrastat booking. In case of deviations, it is possible to reach the second detail dialog in the order header by pressing `<F2>` twice
    - and to select the complaint type for the type of business.
    - possibly to assign the correct shipping type if this has not already been assigned to the route.

Then the order can be entered as usual and completed.

The Intrastat booking is then made after the invoicing.

**Examples:**
1.  An order is entered for an internal partner. The main address is entered in the master data. It refers to an Intrastat country code. When the order is completed, an Intrastat booking is generated automatically during invoicing.
2.  A delivery should be made to an internal partner within Germany – e.g. in Spain. Due to the override of the main address - here the CAR identifier refers to an Intrastat country code - with an address within Germany, no Intrastat booking will be generated.

### 1.8. PO
The PO entry is done analogously to the order entry.

Here, however, there is no absolute requirement that the delivery be defined as the main address. The reference to the Intrastat is achieved via the CAR identifier - Intrastat country code - in the supplier master data. Here, the Intrastat booking is done during invoice checking.

**Notes:**
The following constellations also have to be included for the processing:
- No main address is entered for the market partner: store delivery address in the order entry!
- The type of business is not final purchase/sale: enter the new type for the document entry in the complaint type!

### 1.9. The booking of the intrastat table
The automatic booking of the table `intrastat` is done with the SA/PU invoice booking.

In the "buch.prot" log it is possible to trace whether or not and why a statistics booking was made.

Here again, is an overview of the prerequisites for the automatic booking with activated env variable `INTRASTAT_NEU`:

**SA invoices**
- Delivery and invoice address are abroad
- Booking to the country of the delivery address
- Special case drop shipments: only the items are booked that are ordered by a supplier in a foreign country.

**PU invoices**
- Pick-up and delivery address in a foreign country
- Booking to the country of the pick-up address
- In case of non-existent pick-up address, booking to the country of the supplier's address

For the booking the configurable fields of the SETID 5 are considered for the invoice header. These are 3 long values (longval2 to longval4), which are taken over from the invoice in the intrastat fields private2 to private4. Caution: with automatic invoice generation, the configurable fields from SETID 5 are not taken over by the order into the invoice and in this case, also cannot be transferred to the table intrastat.

A special logic applies for the field `intrastat.private1`. The value from `kauf.company` is written in this field.

The booking can then be checked immediately in the menu `System -> Statistics Data -> Intrastat -> Bookings`. On this menu, it is also possible to make new bookings, correct or delete existing ones.

**Figure 8: Intrastat, Overview 1**
This overview shows booked Intrastat records.

**Field description:**

- **Invoice:** The Intrastat invoice number.
    - for the order: SA invoice number
    - for the PO: PA invoice number
- **Date:** Date of the booking
- **Country of origin:** Here the supplier's country is entered for an incoming message. This field should not be populated for a shipping message.
- **Country:** Country code
    - For shipping, the member country has to be specified in which the goods should be used or consumed, machined or processed.
    - For import, the EU member state has to be specified from which the goods are sent.
- **Product code:** Intrastat product code for the article
- **Stat.Verf.:** Statistical process is generally pre-populated:
    - for a dispatch message with 10000 (dispatch)
    - for an incoming message with 43000 (receipt)
    - For the other messages, the process must be changed manually
- **Amount:** Invoice amount

**Figure 9: Intrastat, Overview 2**
This is the second tab of the Intrastat booking screen.

**Field description:**

- **Status:** Status of the record
- **Status description:** A brief description of the status. For more precise information, see the configuration instructions for the FinAc service (Chapter "14.5 Status values in the table intrastat").
- **Type:** Type of business according to the specifications of the German Federal Statistics Office (reference to complaint type from the order).
- **Va:** Mode of transport (Master data -> Dispatch type).
- **Bes. Maßeinheit:** Special dimension unit from the assignment of the product code.
- **Stat. Wert:** Statistical value (revenue + transport surcharge), in percent. Generally the statistical value is derived from the invoice amount. It is identical to the statistical value for deliveries to the border, fob (free on board) or to delivery/post office at destination. For delivery ex works, the invoice amount has to be increased by the transport costs to the border; for delivery fob, by contrast, reduced by the transport costs from the border. These surcharges and deductions can be estimated.
- **Weight:** Weight of the goods sent.
- **Region:** So that this field is filled, the region has to be entered in the customer record for the site.
    - For shipping, the federal state has to be specified in which the goods were manufactured, installed, assembled or processed.
    - For import, the country code of the federal state has to be specified in which the incoming goods should likely remain.

**Figure 10: Intrastat, Overview 3 - Private fields**
In the last overview, there are also 4 private fields that are still available in the intrastat table (`Privat 1`, `Privat 2`, `Privat 3`, `Privat 4`).

#### 1.9.1. Booking of partial invoices
There is also a booking to the table `intrastat` for partial invoices (of collective invoices). To distinguish them, the Intrastat data records of the partial invoices contain the "subnr". It is also displayed on the booking dialog. Partial invoices can be edited after the fact just like individual invoices.
(AWDesk #34825)

### 1.10. List Printing
The call for list printing is done for the shipping message in `Analysis -> Print List -> Intrastat Shipment`; for the incoming message in `Analysis -> Print List -> Intrastat receipt`.

Under some circumstances, these lists first have to be configured separately.

### 1.11. Notes
1.  Corrections to the German Federal Statistics Office, e.g. credits, essentially have to be created manually since the correction messages have to be marked as a clear copy of the original message. Furthermore, the various exception rules cannot be mapped by the system.
2.  The basis for the documentation are the descriptions of the Intrastat statistics of the German Federal Statistics Office.
