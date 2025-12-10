---
description: "AW_Production_-_Other_Edgework_Configuration_For_Extra_Cutting_Allowance"
---


# A+W BUSINESS AND A+W PRODUCTION OTHER EDGEWORK CONFIGURATION FOR EXTRA CUTTING ALLOWANCE

## A+W Business – New Product Code

**AWB - NEW PRODUCT CODE**

- Under Master Data Products > Product > Products
- Create a new product with the required number (Example - 49013)
- This can be created by copying an existing edgework processing like Polish and then confirming the details below.

> Note - The information below is the minimum to get this function working – further changes to the new processing could be required to suit the business need.

### Tab 1
- Product Type = 020 - Processing
- Product Class = 0031 - Katen Edges
- PGR = B00 - Edge Processings
- PGR Statistics = B00 – Edge Processings

### Tab 2
- Edge Quality = 113 - Individual Edge Quality

### Tab 3
- Proce Table SP / PP be updated if needed

### Tab 9
- Processing and Surcharge Type = 1090 - Other Edgework

**TAB 1**
**TAB 2**
**TAB 3**
**TAB 9**

## A+W Production – Grinding Allowance

**AWP - GRINDING ALLOWANCE**

- Open Master Data > Grinding Allowances
- Ensure a Processing Group of Other Edgework is available and confirm that a entry for the Standard Group is setup.
- In this example we have configured a 100mm glass allowance to be added onto the glass when the matching processing is transferred from A+W Business to A+W Production.

## A+W Production – Processing Articles

**AWP - PROCESSING ARTICLES**

- Open Master Data > Processings > Processing Articles
- Click on Article Number - 49013 to show the details.

> Note - The information below is the minimum to get this function working – further changes to the new processing could be required to suit the business need.

- Grinding Group = 1090 Other Edgework
- Processing Type and A+W Type = 1090
- Work Process Allocation 10900 - Set the correct Machine for the Processing
- Extra 1 Value = 113 - This needs to match the Individual Edge Quality value under A+W Business and will be used to match with the SN.INI file

## SN.INI – Change to the SN.INI file

**SN.INI - CHANGE TO THE SN.INI FILE**

- Collect the from A+W Business the Edge Quality Number used under Tab 2 or the Extra 1 value from A+W Production.
- Open the P:\\SN\\SN.INI and then -1 (minus one) from the Edge Quality Number. In this instance 113 was used for the Edge Quality making the value needed in the SN.INI of 112.
- Create the four following entries listed below in the SN.INI under the [Decoration] heading under the existing Deco### entries.

> Note - Deco112 = xE Is the marking to be shown on the SN in A+W Business, this value should be no more than 4 values long.

```ini
Deco112 = xE
Deco112Name = Extra-Edge
Deco112Shift = @CALCULATED
Deco112EnableForDrawingViews = 1
```

- After making a change to the SN.INI it is recommended to restart the A+W CAD 6 and A+W ALCIM Items4ALCIM Windows Services under services.msc.

## A+W Business – Order Entry Example and Result

**A+W BUSINESS ORDER ENTRY EXAMPLE AND RESULT**

- In the example below we can see the Processing being added to the glass and the xE Processing Marking on each side of the glass in black lettering.

- This should provide an order size of 1024 x 1024 and a cutting size of 1224 x 1224 after import into A+W Production.

## A+W Production – Order Import Result

**A+W PRODUCTION ORDER IMPORT RESULT**

- CUTTING SIZE - 1224 x 1224
- ORDER SIZE - 1024 x 1024
