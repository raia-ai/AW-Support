---
description: "AUW_HighQuantityBarcoding"
---


# High Quantity Barcoding – A+W Production 5.1

## History of Changes

| Date | Edited by | Notes | Version |
| --- | --- | --- | --- |
| 2012-06-19 | PK | Original version | 1.0 |
| 2012-06-28 | PK | - Chapter 1.3.: Input options amended
- Chapter 2.: Amendment and correction of quantity descriptions
- Chapter 3.4: Extended restriction check for breakage
- Chapter 8.2: Extension of AWInfo | 1.1 |
| 2012-12-17 | PK | - Chapter 5: Change of restriction check configuration | 1.2 |
| 2013-01-14 | PK | - Chapter 5 Extension and amendment of restriction check configuration | 1.3 |
| 2013-05-06 | PK | - Amendments after implementation at Sandomierz | 1.5 |
| 2013-05-22 | PK | - Chapter 1.3: special setting in AWPort
- Chapter 6: Restriction-Check  for Scanners | 1.6 |

## Contents

## Introduction
This document shall describe the necessary properties of Quantity Barcoding. As the concept of quantity barcoding has been implemented to a large extent (and is partly being used already), the actual conditions have to be taken into account. This is therefore not about developing a new concept but rather assessing the existing situation in order to close any gaps in quantity barcoding. This document is thus not to be understood as a "code of law" but shall serve as a working basis for all persons involved. Amendments and comments are therefore most welcome.
### Characteristics / Basics of Quantity Barcoding
In single sheet barcoding, each sheet of a BOM element has a unique barcode. Each barcode represents a quantity of one piece.
In quantity barcoding however, all sheets of a BOM element have the same barcode. Every booking with this barcode must therefore be accompanied by the quantity. The total number of sheets of a BOM element can be distributed at random on the shop floor.
Thanks to quantity barcoding, the amount of data is reduced considerably which increases the booking performance dramatically. The performance of analyses and views is greatly improved too.
Since quantity barcoding cannot provide reliable information on the whereabouts of an element, the table awbar\_teile can be used only in exceptions. Useful analyses are mainly available from the tables awbar\_bearbeit, pool\_bearbeit, awbar\_sollbuchung, and awbar\_istbuchung.
### Limits of Quantity Barcoding
#### Amount of data
The number of records in the database is extremely reduced by quantity barcoding. The biggest tables in the ALCIM database (awbar\_teile, awbar\_sollbuchung, awbar\_istbuchung, awbar\_historie) become a lot smaller.
Since detailed scheduling has to know the individual sheets for optimisation purposes however, the amount of data is still quite high at that point. At least one record has to be created per sheet (depending on the number of lots). Detailed scheduling takes quite long because of that which is why this part still needs to be optimised.
#### Locations
Details of the origin are not required for quantity barcode bookings. The advantage of this is that bookings can be made in the same way as in single sheet barcoding, only with the addition of the quantity.
The disadvantage however is that there is no information on the actual whereabouts of the sheet. This means that it is impossible to say where a sheet is, which is why it cannot be relocated/rebooked from there. Rack loads can be achieved only by booking sheets correctly to a rack. If the rack load is changed, the whole rack must be booked 'empty'; the remaining sheets have to be booked to this rack again.
Quantity barcoding is therefore mainly suitable for evaluations in terms of quantities.
A possible solution for this problem is outlined in chapter "The Future".
#### Overbooking
The quantities will not be checked when a booking is made. This means that the quantity entered by the user will be saved in the database (especially when using scanners). This can only be limited by specific restriction checks in the ToolTVs (see below).
#### Production Progress
The production progress is always shown in "units" because the statement "500 of 1000 holes drilled" does not say for how many of the sheets the next process can be started. If you want to see later - for statistical purposes - how many holes were drilled in one day, it is always easier to multiply a number with a processing quantity. The processing quantity is shown in the fields bearb\_laenge, bearb\_fläche, etc. in pool\_bearbeit. As the individual processing quantities are transferred by Order.XML from the ERP system, not all of the fields will be filled at the same time. Field pool\_bearbeit.me\_einheit determines which field will be filled exactly.
### Input Options
There are various ways of booking sheets in quantity barcoding:
1. XOPTON (standard; no DynOpt!): accumulates identical order items on a sheet and issues a common booking per item.
1. ToolTV-Order: the quantity to be booked is directly entered in the data grid
1. ToolTV-Jobs: not possible at present; release dialogue will have to be extended
→ *** programming required***
1. ToolTV-Processing: not possible at present
→ *** programming required***
1. ToolTV-IG: this is (currently) not feasible because the entire communication and structure in the IG-ToolTVs is based on locations which are not available in connection with quantity barcoding. Also, I do not believe that customers will want to produce large series by means of ToolTV-IG (too much handling required, and little use).
For mixed production (series and non-series), ToolTV IG could be extended so that larger quantities can be reported complete in a separate dialogue. Sub-elements should be automatically booked as "assembled" (as for non-series).
 → *** programming required (but perhaps a separate project)*
1. ToolTV-TG: see ToolTV-IG
→ *** programming required (but perhaps a separate project)*
1. ToolTV-LG: see ToolTV-IG
→ *** programming required (but perhaps a separate project)*
1. ToolTV-Edit: has currently access to all labels (original and booked labels). It is therefore not suitable for being used in quantity barcoding. 
→ *** programming required (but perhaps a separate project)*
1. Scanners in the shipping area: is possible with BHT800 but need some special settings in AWPort (A+WBarcodemanager)
- In the **scanner** the option “Quantity input” has to be set to “Quantity mode”. If the input of the quantity is necessary can also be set up:
Yes (recommended): the user has to enter a quantity
No : if the user scan the next barcode the quantity is automatically set to 1. 
- settings in **AWPort**:
**“Force export for…”:** this will force AWPort to send a unit.dat to AWBar-Booking in the specified time. Without this setting, AWPort waits for the next barcode to create that output-file. This is necessary to create also an outputfile when the quantity-input is not mandatory. **IMPORTANT**: if the time is setup to short, so that the user has no chance to enter the quantity, AWPort will create an output-file with the quantity 1.
**“Quantity mode…”:** this is necessary that AWPort will send the quantity coming from the scanner into the output-file.
## Definition of Terms
There are different indications of quantity in both quantity barcoding and single sheet barcoding. Especially the processors work a lot with surplus which results in special behaviour patterns in our software. To achieve a common understanding of the individual indications of quantity, the terms shall be explained at this point.
### Commercial Quantity
The commercial quantity is the quantity ordered by the customer. This means that this is the quantity which is entered in the ERP system, and transferred to ALCIM. There, it is saved in field **pool\_pos.menge**
### Surplus
Surplus is the quantity to be produced in addition to the commercial quantity. It serves to ship the complete order without remakes even if breakage occurs. This means:
- You want to define the shortage or surplus a customer is prepared to accept, and
- Control of remakes
There are currently three ways of defining surplus:
1. Minimum and maximum quantities can be transferred from ALFAK to ALCIM.
(→  see document AUW\_Configuration\_surplus\_quantity.docx)
1. In ALCIB's partner master data, a percentage can be entered in field "Surplus". It serves to transfer a fixed surplus to ALCIM. Unfortunately, this does not work in connection with Order.XML!
1. A surplus editor in ALCIM can be used to define a surplus per item or per element by hand. (→  see document AUW\_Configuration\_surplus\_quantity.docx)
The surplus defines the number of sheets with which production is started. If breakage occurs, remakes will be created only if the minimum quantity is not met.
**Example 1:
**A customer orders 100 sheets
Commercial surplus = 10 sheets
→  110 sheets will be cut.
→  for the first 10 broken sheets, no remakes will be created
**Example 2:
**A customer orders 100 sheets
Commercial surplus = 10 sheets
Commercial shortage = 10 sheets
→  110 sheets will be cut.
→  for the first 20 broken sheets, no remakes will be created
→  the customer wants to get at least 90 sheets
In ALCIM, the surplus is defined by the fields **pool\_teile.menge** and **pool\_teile.mindermenge**. pool\_teile.menge = commercial quantity + surplus. Field pool\_teile.mindermenge defines by how much the target quantity can be reduced before remakes are created.
### Technical Item Quantity / Target Quantity
The technical item quantity refers to the number of sheets to be produced. It consists of the commercial quantity plus the surplus. If a surplus of 7% is transferred, the technical item quantity is 107% of the commercial quantity.
The technical item quantity in ALCIM is saved in the fields **pool\_pos. menge\_auftrag**, **pool\_teile.menge,** and in all barcode tables as the target quantity.

The barcode view "Target/Actual" can therefore show how many sheets have to be delivered (100 pcs. packed plan=commercial quantity), and how  many sheets shall be produced at the individual terminals (107 pcs. cut = technical item quantity = target quantity)
### Excess Quantity
For certain items, excess quantities shall be produced, e.g. in order to use them for testing or for quality assurance purposes. This means that more sheets than necessary shall be produced; these shall be remade in case of breakage (in contrary to surplus). These excess quantities can be entered in the surplus editor as well.
Field **pool\_teile.menge** is amended for this purpose while **pool\_teile.mindermenge** remains unchanged.
### Overbooked Quantity
Processors who handle large quantities often fill up the stock sizes by additional sheets for cutting. It may therefore happen that more sheets are cut than the number defined by the technical item quantity, i.e. the target quantity is overbooked. The overbooked quantity is therefore the number of sheets which are produced in addition to the technical production quantity.

In this example, the customer has ordered 20 sheets. Because of the surplus, 21 sheets shall be cut. Actually, 24 sheets are cut and booked in the cutting area. This means that the overbooked quantity consists of three sheets.
### Available Quantity
The available quantity describes the number of sheets that can be produced at a terminal. This means that these sheets have passed all previous processes except the actual process. This quantity is saved in field **pool\_bearbeit.menge\_verfuegbar** and is updated by AlcimBooking with every booking.
Note: If no restriction checks are used, it may happen that the available quantity becomes negative. This happens if more sheets are booked at a terminal than the number of sheets available from the previous process. This will be balanced however when the quantities for the previous process are booked later.
### Breakage
Breakage is the number of sheets booked as broken. This quantity will be analysed in waste statistics. (**pool\_bearbeit.menge\_bruch**)
### Quantity Produced
The quantity produced is the total number of sheets produced. If a sheet is produced several times because of breakage bookings, the quantity produced will be raised accordingly. This quantity is saved in field **pool\_bearbeit.menge\_gefertigt**.
### Quantity "Accepted"
The quantity "accepted" refers to the "surviving" sheets. This quantity therefore consists of: quantity produced minus the breakage, and is saved in field **pool\_bearbeit.menge\_gut**.

### List of Quantity Descriptions

|   | **Name** | **Description** | **Database Field** |
| --- | --- | --- | --- |
| **A** | Commercial Quantity | Ordered by customer | pool\_pos.menge |
| **B** | Surplus | Planned to be produced additionally | pool\_teile.menge,
pool\_teile.mindermenge |
| **C** | Technical production quantity or target quantity | =A+B | pool\_bearbeit.menge\_prod,
awbar\_sollbuchung.bxxmenge |
| **D** | Excess Quantity | Sheets to be produced additionally | pool\_teile.menge increased,
pool\_teile.mindermenge unchanged |
| **E** | Overbooked Quantity | Quantity booked in excess of C | no separate field |
| **F** | Available Quantity | All previous processes completed | pool\_bearbeit.menge\_verfuegbar |
| **G** | Breakage | Breakage | pool\_bearbeit.menge\_bruch |
| **H** | Quantity Produced | Sheets produced | pool\_bearbeit.menge\_gefertigt |
| **I** | Quantity "Accepted" | "surviving" sheets | pool\_bearbeit.menge\_gut |

## Quantity Barcoding in the Database
Basically, data in the database are displayed differently in quantity barcoding and single sheet barcoding. This is the only way by which the amount of data can be drastically reduced.
### Comparison of Single Sheet Barcoding and Quantity Barcoding
In single sheet barcoding, every sheet (or every BOM element) is identified by a unique barcode (see 1.1). When a booking is made, an existing record only needs to be updated (depending on the type of booking), e.g. if the current location of a barcode is changed or if a processing step is booked as 'completed'. If one wants to book large numbers of those single barcodes at once, the booking effort in the database is quite high (because n records need to be updated).
This means: 100 single sheets with three processing steps each will mean in connection with single sheet barcoding:
100 entries with a quantity of 1 in awbar\_teile
100 entries with a quantity of 1 in awbar\_sollbuchung
100 entries with a quantity of 1 in awbar\_istbuchung
300 entries with a quantity of 1 in awbar\_bearbeit		→  600 entries

In quantity barcoding, identical BOM elements are represented by a single barcode (starting with "1"):
1 entry with a quantity of 100 in awbar\_teile
1 entry with a quantity of 100 in awbar\_sollbuchung
1 entry with a quantity of 100 in awbar\_istbuchung
3 entries with a quantity of 100 in awbar\_bearbeit		→  6 entries!
When a booking is made, a copy of this record is created and the quantities are adjusted. The original record (starting with "1") is kept with the reduced quantities, and the new record (starting with an "S") shows the booked quantity and the appropriate location. The connection between these label numbers is made by the field "gruppenbc" (=label number of the original record).
To determine the quantity for a certain record, the new field "smenge" has been added. Its meaning varies depending on the table:
awbar\_bearbeit.smenge = quantity still to be produced in this work step (for the original record) or the quantity produced in this work step (S record).
awbar\_teile.smenge = is always the total quantity for this BOM element. Only for breakage bookings, it shows the number of broken sheets.
Field awbar\_teile.menge can only be used for S records. In this case, it shows the booking quantity. This field is of no use for the original records because it will be reduced with every booking (no matter if the processing or the location is booked).
As in case of a booking, only a certain part of the original record is deducted, the S records will remain unchanged once they have been created. This also explains why an exact location cannot be defined(yet) in quantity barcoding. When 100 sheets are booked to a registration point or rack, there is currently (almost) no way of removing those sheets from this registration point or rack. At present, this is only possible by a previous "Start" or "Empty" booking (as yet untested).
### Activating Quantity Barcoding
#### Settings in the barcoding system
In Master Data/Barcoding/Barcode Options you can define the quantity from which on an order has to be initialised as a quantity barcoding order:

This means that you can define a value (here: 10 pcs.) **and** scheduling will load an SP (CU\_PRT\_ITEMWRT\_BDE) which can be used to overrule the behaviour. This could e.g. be used for initialising orders from a certain customer as quantity barcoding orders, irrespective of the actual quantity.
The SP has to fill field pool\_teile.bde\_serien in the database:
Pool\_teile.bde\_serie = 0 →  single sheet barcoding
Pool\_teile.bde\_serie = 1 →  quantity barcoding
#### Settings in detailed scheduling
From the document on quantity barcoding issued by RK (2008), the following parameters have to be set in detailed scheduling in Master data/Configuration in ALCIM/Detailed scheduling/Specials:

**ALLOWITEMSPLITTING=2 **
**[FORCEWRITEFEIN\_UNIT = 1]** (entries for the main element and the spacers also have to be made in fein\_unit)
**GRUPPENNUMMER = 1** (grouping will not be determined by the master organisation)
**[SERIENETIKETTHOCHZAEHLEN = 2]**
**SERIENINFEIN\_UNIT = 1** (quantity barcoding orders shall be saved as individual sheets in fein\_unit)

**The entries in square brackets are not accessible from master data. They have to be changed directly in the database.**

The parameters can be checked by the following select:
select entry, text from parameter where section='FEIN\_SPECIALS' and entry in ("SERIENINFEIN\_UNIT", "GRUPPENNUMMER", "FORCEWRITEFEIN\_UNIT", "SERIENETIKETTHOCHZAEHLEN", "ALLOWITEMSPLITTING")order by 1;
#### Settings in XOPTON
In XOPTON.CFG you can set the following flag so that you will get the correct breakage label for sheets without ‘High Quantities’.
; ............. Section for XTV (XPATDIS) ...................................
[XTV]
**UseBarcode=Y**
#### Other settings
????

## Bookings and Restriction Checks
Bookings are made in the same way at all terminals. Only the restriction check, i.e. the definition of how many sheets can be booked at a terminal, is different for the individual terminals.
### Bookings in the Cutting Area
In the cutting area (or at the production terminal) it must be possible to overbook the target quantity (=technical item quantity) because complete stock sizes shall be cut always. This means that the stock size is completed by the order item (=overbooked quantity). To prevent incorrect entries as far as possible, maximally x% of the target quantity can be booked at this point (adjustable).
**Example:**
Overbooking of 50% is permitted
Commercial quantity = 100
Technical item quantity = 107
→  Maximally 161 sheets must be booked (107 sheets \* 150%)
Considering the previous processes is irrelevant for cutting because cutting is always the first process. This is why the field pool\_bearbeit.menge\_verfuegbar shows the technical item quantity right away.
Further overbooking is only permitted in connection with the restriction check. The restriction check refers to the technical production quantity in this case. This always applies to the first processing step for a sheet or depends on a switch in ToolTV (see below).
### Bookings at the Processing Terminals
At the individual processing terminals (except cutting and packing), the number of booked sheets must not exceed the number of sheets provided by the previous process (=available quantity = pool\_bearbeit.menge\_verfuegbar). Overbooking should not be permitted here (the more as it makes no sense).
**Example:
**Commercial quantity= 100
Technical item quantity = 107
120 sheets are booked in the cutting area
Maximally 120 sheets can be booked at the next terminal.
### Bookings at the Packing Terminals
At the packing terminals, it must be possible to overbook the available quantity because one might want to ship additional sheets from stock.
**Example:
**Overbooking of 50% is permitted
Commercial quantity = 100
Technical item quantity = 107
Available quantity = 120 
→  Maximally 180 sheets can be booked at the packing terminal (120 sheets \* 150%)
### Restrictions for Breakage Bookings
For breakage bookings, an 'accepted' report will always be issued first. This is why the restriction check applies to breakage bookings too. This means that if the restriction check is switched off, the available quantity may become negative.

## Breakage Reports
Breakage bookings are mainly made for statistical purposes. A breakage booking should also render the processes at the previous terminals visible and bookable.
Also, it should be possible to transfer the breakage to the breakage pool for automatic remakes. Whether a breakage booking will create a remake, is defined by the status type and the commercial surplus.
Since the individual sheets cannot be clearly identified in quantity barcoding (i.e. location and status of the individual sheet are unknown), the processing steps to be repeated after breakage cannot be defined with certainty.
**Example:
**30 sheets shall be cut, polished, and drilled
30 sheets were cut already
20 sheets of those were polished already
10 sheets of those were drilled already
2 sheets are reported broken now 
→ ** **The question: "how many sheets still remain to be polished?" cannot be answered precisely because one does not know which of the sheets were reported broken.
This problem is solved by defining that all processing steps prior to the terminal at which the breakage was booked, have to be repeated. If in the example above, the breakage booking was made at the polishing terminal, only two sheets would have to be cut again. The polished and drilled sheets are in good shape.
This method works only if there is a fixed processing sequence and if a terminal can book just one processing step. If this is not the case, the following cases have to be distinguished.
### Breakage Reports if the Processing Sequence is Clear
A clear process chain is marked by the fact that a process can be executed only after the previous process has been completed. Cutting for example always comes before edge processing, and holes always have to be drilled prior to toughening.
Breakage reports in a clear process chain always results in the automatic resetting of the previous processes for the quantity booked because the previous processes can be clearly identified.
### Breakage Reports if the Processing Sequence is Flexible
There are processing steps the sequence of which may be scheduled, but which do not have to stick to this sequence. It does not matter for instance whether large holes are drilled first or small holes. In this case, a breakage report cannot automatically reset all previous processes but the user has to add the necessary details to the booking.
|   | In this example, all processing steps are shown which can be executed at this terminal. In the standard case, all processing steps are marked because it is assumed that all of them were executed – i.e. that processing was done according to schedule. If the breakage report is made this way, all processing steps will be reset. If one of the processing steps has not been made however (which should be the exception), the user only has to remove the appropriate tick before issuing the breakage report. |
| --- | --- |

## Configuring the Restriction Check
The examples above (chapter 3) show that the settings for the restriction checks are directly connected with the registration points, not to the ToolTV station (for a ToolTV Order which can book cutting and a processing terminal, just one restriction could be set = conflict!).
This is why the following settings are directly made in ALCIM master data and at the registration points (Master data /Barcoding/Registration points).
**ATTENTION**: this settings are in Alcim-Masterdata for registrationpoints, but they will not affect bookings done by a scanner! Quantities coming from a scanner are always booked independent of the settings for the restriction-check!
The following switches are used for enabling and setting the restriction check:

1. Restriction check = awbar\_stellen.restriction (default = 0)
1. Quantity transgression in % = awbar\_stellen.overbook (default = 0)
1. Show produced elements = awbar\_stellen.show\_produced\_parts (default = false)
### Restriction Check
This setting enables or disables the restriction check and defines the quantity to which the restriction check refers.
The following settings are possible:
| **Restriction Check** | **Behaviour** |
| --- | --- |
| = 0 (No Restriction) | The restriction check is switched off. Any quantity can be booked in quantity barcoding. |
| = 1 (To Technical Production Quantity) | The restriction check refers to the technical production quantity. |
| = 2 (To Available Quantity (Previous Process Step)) | The restriction check refers to the quantity available. All sheets which have completed **the** previous process, are available. |
| = 3 (To Available Quantity (All Process Steps)) | The restriction check refers to the quantity available. All sheets which have completed **all** previous processes, are available. |

### Quantity Transgression in %
This entry will be analysed only if the restriction check is switched on (awbar\_stellen.restriction >0). It defines the percentage by which the initial quantity can be overbooked. The initial quantity is defined by the switch "Restriction" (see 5.1). In practice, the initial quantity for the glass producing processing step (cutting) is always the technical production quantity (i.e. restriction = 1). For all following terminals, it is always the available quantity (i.e. restriction = 2 or 3).
### Show Produced Elements
This switch defines whether ToolTV can show sheets even if they have been completely produced. This switch already exists in ToolTV-Order but it has been moved to barcoding master data for the above reasons. The behaviour of the existing switch in case of an update will be described below.
### Example Settings
To achieve the behaviour describe in chapter 3, the restriction check would have to be set as follows:
| **Terminal** | **Restriction check** | **Quantity transgression in %** | **Show Produced Elements** | **Behaviour** |
| --- | --- | --- | --- | --- |
| Cutting | 1 | 50 | True | Maximally 150% of the technical order quantity can be booked |
| Processing terminal | 2 | 0 | False | Only the sheets for which **the** previous process has been completed, can be booked |
| Packing | 1 | 50 | True | Maximally 150% of the technical order quantity can be booked |

### Behaviour of the Switch in Case of an Update
Since the above switches ("Restriction check", "Quantity transgression allowed", "Show produced elements") are already part of ToolTV (with limited functions) and shall be used in ALCIM master data later, the following scenarios have to be considered in case of an update:
1. When ToolTV is started after an update, it reports that the database version is outdated. When this is acknowledged, ToolTV closes. This means that ToolTV cannot be run without a database update.
1. The database must be updated to the version required (to ensure that the necessary columns for the new switches are available in awbar\_stellen).
1. The old parameters in ToolTV are still visible, but "read-only". This allows transferring the existing settings to master data.
1. The descriptions of the switches in ToolTV will be extended. A note is therefore required saying that these switches are only displayed but that the settings for the registration points are now loaded from barcoding master data. (still to be implemented).

## Analysis in Quantity Barcoding
### Views in ToolTV
ToolTV must be able to show the following quantities:
| A | Commercial Quantity | Ordered by customer |
| --- | --- | --- |
| C | Technical production quantity or target quantity | =commercial quantity + surplus |
| H | Available Quantity | All previous processes completed |
| I | Breakage | Breakage |

### Views in ALCIM
As the whereabouts of the sheets is unknown in quantity barcoding, ALCIM should mainly present a simple production overview.

(is created from awbar\_sollbuchung and awbar\_istbuchung)
### Effects on Capacity Planning
Capacity planning and the production monitor get their contents from the fields pool\_teile.menge and pool\_bearbeit.dauer. This means that even surplus is shown correctly. If surplus sheets are broken, the entry in field pool\_teile.menge will not be reduced however (but the entry in field pool\_bnearbeit.menge\_prod), i.e. backlogs may occur even if these sheets do not have to be remade.
### Reports
- **Production statistics** (what - and which quantity - has been produced where, and by whom)
→  There are two options:
1. Analysing all records from awbar\_bearbeit which show complete=1 (totals have been created for the individual bookings)
1. Analysing pool\_bearbeit as it shows the sums anyway (bearb\_fläche, bearb\_gewicht, etc. and menge\_bruch, menge\_gefertigt, menge\_gut)
- **Breakage statistics** (what - and how much - has been reported broken, when and by whom)
1. awbar\_teile.bruch\_flag=1 or 3 can be used to determine the number of sheets
1. in pool\_bearbeit.menge\_bruch (shows only the quantities without saying where the breakage occurred)
- **Machine utilisation** (what shall be produced when, and on which machine - scheduling data)
→  in awbar\_bearbeit or pool\_bearbeit (more performance)
- **Production labels** (what - and how much - is included in a stack of glass, which processing steps were performed, which have to be performed yet, which are the next steps)
→  printed with the new report technique in ToolTV. The necessary entries (mainly from pool\_bearbeit) can be directly transferred to the label.
- **Production status** (which status does an order have)
→  display of target/actual values in the barcoding view, analysis in pool\_bearbeit)
- **Packing lists** (contents of a rack/registration point) – only possible after an "empty" booking or definition of the source (see chapter "The Future")
### Reports
Reports in quantity barcoding are also made by ERP Web service.
### Borderlines
There are database fields which only make sense for single sheet barcoding and are analysed only there.
**Examples (incomplete):**
**awbar\_teile.bearboffen\_anz** (=processing steps still open for this sheet); always shows the total number of processing steps in quantity barcoding (which is wrong for the booked records), or
**awbar\_teile.next\_es** (next scheduled registration point for a sheet); shows the correct entries only for the initial record and for breakage in quantity barcoding.
These fields cannot be analysed in quantity barcoding.

## Example Cases
Since data structures have already been defined and the structures of quantity barcoding have to be compatible with single sheet barcoding, general case studies are of little use. This is why the individual booking cases are assessed in the Excel sheet "".
The individual sheets describe example bookings; the database fields involved and the changes are highlighted. A link to the current database description shall help to understand the individual fields and revise the description if necessary.

## The Future
### Reliable Locations
A big impediment of the current quantity barcoding version is the loss of the exact whereabouts of the individual sheets or packages. This is important however at least in the shipping area and can be remedied only by adding the source when issuing a booking. It needs to be discussed how this can be handled for the individual modules to make things easier for the users.
In ToolTV for instance, the users could be guided by an additional dialogue. This means that the users enters the quantity to be booked and the dialogue shows all locations (stacks) where those sheets can be found. The user chooses the appropriate stack and AlcimBooking corrects or removes the S records in awbar\_teile so that the locations always match. By means of practical rules, the stacks can be limited accordingly (e.g. shipped sheets are no longer displayed).
To achieve the same when using a scanner, bi-directional communication with the scanners is required. At present, the scanners only communicate towards ALCIM; there are no reports from ALCIM to the scanner at present.
→ *** requires programming***
### AWInfo
AWInfo has been used without quantity barcoding so far. The available analyses in AWInfo were based on statistics reports like those our customers have been using. These reports were also made without the use of quantity barcoding. To determine quantities, label numbers would often be counted which does not work for quantity barcoding. As a result, AWInfo is currently not suitable for being used in connection with quantity barcoding.
→ *** requires programming***
