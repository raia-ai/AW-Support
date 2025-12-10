---
title: "AUW_Configuration_surplus_quantity"
source: "AUW_Configuration_surplus_quantity.docx"
tags: ["Produced", "pool_teile", "Technical", "Maximum", "Entered", "Order", "Alcim", "Editor", "Information", "Alfak"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides structured configuration guidance and reference material. It covers: Configuration of Surplus Function, What is Surplus?, **Commercial****surplus**, **Technical****surplus**, **Additional****quantities**, Requirements. Content has been normalized into markdown with preserved headings, lists, and tables for reliable indexing in a vector store."
long_description: "This markdown version restructures the original DOCX into semantically clear sections to support accurate retrieval, chunking, and embedding in vector-based search systems. All headings, bullet lists, and tables have been preserved and converted to GitHub-Flavored Markdown. Encoding artifacts were cleaned, duplicate spacing removed, and table content normalized so that column headers and cell values remain machine-readable.\nOrganization and coverage:\n- Configuration of Surplus Function: History Includes tabular data. Content\n- What is Surplus?: There are two types of surplus: commercial surplus and technical surplus. The basis includes the commercial surplus. Technical surplus isproduction- and customer-specific.\n- **Commercial****surplus**: Commercial surplus and shortfall refers to a complete item. There is a minimum and a maximum quantity. Producing the maximum quantity is the target. If breakage occurs, remakes will not be produced unless the quantity falls below the defined minimum.\n- **Technical****surplus**: Technical surplus refers to element chains in the bill of material and can even refer to processing steps. It is not controlled by order entry but is entered in ALCIM, either automatically by SPs or by hand in a special surplus editor.\n- **Additional****quantities**: Additional quantities are also defined in production only and can also be set by means of the surplus editor. They are required if a couple of units more shall be produced in general, e.g. for test sheets.\n- Requirements: OrderXML – Interface, ERP Feedback Interface, ALCIM2011, ALFAK2011\n- Surplus in theDatabase: The tables POOL_POS, POOL_TEILE and POOL_BEARBEIT offer information on surplus. The table POOL_POS will be filled only if the surplus was transferred from order entry. If the surplus is entered only in ALCIM, the fields of POOL_POS remain unchanged.\n- Surplus inOrderXML file: Surplus information is transfer inOrderXML in the following tag: <CommercialQuantitiessurplusQuantity=\"**10**\"requestedQuantity=\"**100**\"shortageQuantity=\"**10**\" />\n- Feedback toOrderEntry: Surplus can only be reported via file-lessfeedback; this is made byALCIMBooking. No further configuration is required; the reports will be created automatically like all barcode bookings. Prerequisite is that barcoding is implemented. The reports transfer the quantity and information BDEFERTIG.\n- **A+W Business**: A+W Business adapts the quantity as from BDEFERTIG = 1. A change of order status has no effect; the order status can reactto status (in ALFAK registration point) 700 and 800 as usual. If surplus has been entered in ALCIM, the reported quantity is processed only if surplus has been configured for this product in ALFAK master data.\n- **A+W Enterprise**: A global switch in ALCIB dispatch control permits the reporting of surplus.\n- SurplusEditor inA+W Production: There are two surplus editors in ALCIM: one for entering surplus and additional quantities perlineitem and another for entering technical surplus. You have to choose one of them in an installation; the function will search for a dialogue called**MEDIT**.\nThis file is intended for upload to OpenAI’s vector store. The metadata block..."
---

## Configuration of Surplus Function
History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 21.05.2012 | Dirk Langwald | First Release | 1.0 |
| 27.06.2013 | Dirk Langwald | process chart / format | 1.1 |
|  |  |  |  |

Content

## What is Surplus?
There are two types of surplus: commercial surplus and technical surplus. The basis includes the commercial surplus. Technical surplus isproduction- and customer-specific.
## **Commercial****surplus**
Commercial surplus and shortfall refers to a complete item. There is a minimum and a maximum quantity. Producing the maximum quantity is the target. If breakage occurs, remakes will not be produced unless the quantity falls below the defined minimum.
Surplus can be entered at order entry or directly in ALCIM by means of a surplus editor. ALCIM reports the produced quantity to the commercial system.

## **Technical****surplus**
Technical surplus refers to element chains in the bill of material and can even refer to processing steps. It is not controlled by order entry but is entered in ALCIM, either automatically by SPs or by hand in a special surplus editor.
## **Additional****quantities**
Additional quantities are also defined in production only and can also be set by means of the surplus editor. They are required if a couple of units more shall be produced in general, e.g. for test sheets.
## Requirements
OrderXML – Interface, ERP Feedback Interface, ALCIM2011, ALFAK2011
## Surplus in theDatabase
The tables POOL_POS, POOL_TEILE and POOL_BEARBEIT offer information on surplus. The table POOL_POS will be filled only if the surplus was transferred from order entry. If the surplus is entered only in ALCIM, the fields of POOL_POS remain unchanged.
**POOL_POS. MENGE / POOL_TEILE.MENGE****
**Maximum quantity, quantity entered + surplus
**POOL_POS. MINDERMENGE / POOL_TEILE.MINDERMENGE****
**Quantity by which the maximum quantity can be reduced before remakes are produced. This field will not be set for additional quantities.
The next fields are set by barcoding and are adapted based on the booking.
**POOL_TEILE.BDESTUECKOFFEN_ANZ****
**Number of the units that have to be produced for aline item = maximum quantity – produced quantity – breakage (for which no remakes had to be produced)
**POOL_TEILE.BDEFERTIG****
**0 = item has not been completely produced
1 = minimum quantity (MENGE – MINDERMENGE) reached
2 = maximum quantity (MENGE– breakage) reached
**POOL_BEARBEIT.FINAL_KZ****
**The field controls the completion reports for units. A unit is complete when the last processing step prior to packing and shipping was booked. This field is filled by barcode initialisation.
0 – any processing step
1 – last processing on the shop floor
2 - packing (BEARBEITSTAMM.AW_BEARBTYP = 1800)
3 - shipping (BEARBEITSTAMM.AW_BEARBTYP = 1810)
*For packing and shipping, AW_BEARBTYP must be set; the field cannot be initialised otherwise!*
There are additional fields for technical surplus.
POOL_TEILE.MENGE_NACH
POOL_TEILE.MINDERMENGE_NACH
POOL_BEARBEIT.MENGE_PROD
POOL_BEARBEIT.MINDERMENGE_PROD
## Surplus inOrderXML file
Surplus information is transfer inOrderXML in the following tag:
<CommercialQuantitiessurplusQuantity="**10**"requestedQuantity="**100**"shortageQuantity="**10**" />
## Feedback toOrderEntry
Surplus can only be reported via file-lessfeedback; this is made byALCIMBooking. No further configuration is required; the reports will be created automatically like all barcode bookings. Prerequisite is that barcoding is implemented.
The reports transfer the quantity and information BDEFERTIG. This is done when the processing step is reported complete by FINAL_KZ = 1,feedback status being 700. This information is also transferred in case of 'off site'feedback, status = 800
## **A+W Business**
A+W Business adapts the quantity as from BDEFERTIG = 1. A change of order status has no effect; the order status can reactto status (in ALFAK registration point) 700 and 800 as usual.
If surplus has been entered in ALCIM, the reported quantity is processed only if surplus has been configured for this product in ALFAK master data. If this is not the case, the quantity will not be changed in ALFAK.
If the final quantity of produced units reported to ALFAK, the quantity ofthe line itemin ALFAK will be adjusted accordingly and invoiced.
## **A+W Enterprise**
A global switch in ALCIB dispatch control permits the reporting of surplus.
## SurplusEditor inA+W Production
There are two surplus editors in ALCIM: one for entering surplus and additional quantities perlineitem and another for entering technical surplus. You have to choose one of them in an installation; the function will search for a dialogue called**MEDIT**.
To be able to load the editor in the POOL views by*[**Reentry**** Surplus** quantities**]*, it has to be activated by means of the parameter*[POOL_SETTINGS / MENGEX] = 1*.
**SELECT** text,***FROM****parameter****WHERE**bereich='POOL_SETTINGS'**AND**eintrag='MENGEX';
**INSERT****INTO****parameter**(bereich,eintrag, text,typ)**VALUES**('POOL_SETTINGS','MENGEX','1',0);
The editor is used for items in the basic database; it is also included in the basic package. To change this or to get more information on the editor, please refer to the documentation
.
The used dialog can be set for eachStationID:
## Input ofSurplus inA+W Business
Surplus can be entered in master data right for the product or for a combination of product and customer. If both have been defined, the customer will be used.
*[Master data / Partner / Customer /**Exceeds amount**]*

*[Master data / Products /**Product / Products /**2.** Production]*

The values for every item can be changed at order entry.

The information is stored in the following ALFAK - database fields:
- BW_Auftr_POS.PP_MENGE
- BW_Auftr_POS.PP_UEBERMENGE
- BW_Auftr_POS.PP_UNTER-MENGE
