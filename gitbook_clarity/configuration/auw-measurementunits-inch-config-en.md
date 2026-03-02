---
description: "AUW_Configuration_measurement"
---


## History
| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 12.02.2013 | GG | Issue | 1.0 |
| 12.02.2013 | DLA | Erweiterung | 1.1 |

## Content




## A+W Production
The ALCIM settings are configured in [Parameter / General / Formats].
### Settings for inch/pound
**mm  inch:**
```sql
UPDATE parameter SET text = '20' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATAREA';
UPDATE parameter SET text = '128' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATLENGTH';
UPDATE parameter SET text = '64' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATAIRSPACE';
UPDATE parameter SET text = '128' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATTHICKNESS';
UPDATE parameter SET text = '985' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATTIMESTAMP';
UPDATE parameter SET text = '995' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATDATE';
UPDATE parameter SET text = '945' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATWEIGHT';
```
**inch  mm:**
```sql
UPDATE parameter SET text = '231' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATAREA';
UPDATE parameter SET text = '100' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATLENGTH';
UPDATE parameter SET text = '101' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATAIRSPACE';
UPDATE parameter SET text = '102' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATTHICKNESS';
UPDATE parameter SET text = '986' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATTIMESTAMP';
UPDATE parameter SET text = '996' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATDATE';
UPDATE parameter SET text = '940' WHERE bereich = 'ALCIM_SETTINGS' AND eintrag = 'FORMATWEIGHT';
```
### POOL display
UPDATE the fields in tables POOL_SORT and DBFIELDS with the following SQL. The selects are for language USA, for other language change the parameter.
**Date: 24.12.2012 to 12/31/2012**

```sql
UPDATE pool_sort SET displayformat = 985 WHERE displayformat = 986 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 987 WHERE displayformat = 988 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 995 WHERE displayformat = 996 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 997 WHERE displayformat = 998 AND sprache = 'USA';
UPDATE dbfields SET format = 985 WHERE format = 986 AND language = 'USA';
UPDATE dbfields SET format = 987 WHERE format = 988 AND language = 'USA';
UPDATE dbfields SET format = 995 WHERE format = 996 AND language = 'USA';
UPDATE dbfields SET format = 997 WHERE format = 998 AND language = 'USA';
```
**Length: mm to inch**

```sql
UPDATE pool_sort SET displayformat = 64 WHERE displayformat = 100 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 128 WHERE displayformat = 101 AND sprache = 'USA';
UPDATE dbfields SET format = 64 WHERE format = 100 AND language = 'USA';
UPDATE dbfields SET format = 128 WHERE format = 101 AND language = 'USA';
```
**Area: m² to sqft**

```sql
UPDATE pool_sort SET displayformat = 20 WHERE displayformat IN (230,231,232,30) AND sprache = 'USA';
UPDATE dbfields SET format = 20 WHERE format IN (230,231,232,30) AND language = 'USA';
```
**Date: 12/31/2012 to 24.12.2012**

```sql
UPDATE pool_sort SET displayformat = 986 WHERE displayformat = 985 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 988 WHERE displayformat = 987 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 996 WHERE displayformat = 995 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 998 WHERE displayformat = 997 AND sprache = 'USA';
UPDATE dbfields SET format = 986 WHERE format = 985 AND language = 'USA';
UPDATE dbfields SET format = 988 WHERE format = 987 AND language = 'USA';
UPDATE dbfields SET format = 996 WHERE format = 995 AND language = 'USA';
UPDATE dbfields SET format = 998 WHERE format = 997 AND language = 'USA';
```
**Length: inch to mm**

```sql
UPDATE pool_sort SET displayformat = 100 WHERE displayformat = 64 AND sprache = 'USA';
UPDATE pool_sort SET displayformat = 101 WHERE displayformat = 128 AND sprache = 'USA';
UPDATE dbfields SET format = 100 WHERE format = 64 AND language = 'USA';
UPDATE dbfields SET format = 101 WHERE format = 128 AND language = 'USA';
```
**Area: sqft to m²**
```sql
UPDATE pool_sort SET displayformat = 232 WHERE displayformat IN (20,30) AND sprache = 'USA';
UPDATE dbfields SET format = 232 WHERE format in (20,30) AND language = 'USA';
```
#### List of possible formats



| Code | Description |
| --- | --- |
| 0 | Text |
| 1 | Number |
| 911 | Number "-" if 0 |
| 2 | Imperial inch (1/2) |
| 4 | Imperial inch (1/4) |
| 8 | Imperial inch (1/8) |
| 16 | Imperial inch (1/16) |
| 32 | Imperial inch (1/32) |
| 64 | Imperial inch (1/64) |
| 128 | Imperial inch (1/128) |
| 256 | Imperial inch (1/256) |
| 180 | Imperial inch (7) |
| 181 | Imperial inch (7.2) |
| 182 | Imperial inch (7.25) |
| -2 | Thai inch (1/2) |
| -4 | Thai inch (1/4) |
| -8 | Thai inch (1/8) |
| -16 | Thai inch (1/16) |
| -32 | Thai inch (1/32) |
| -64 | Thai inch (1/64) |
| -128 | Thai inch (1/128) |
| -256 | Thai inch (1/256) |
| 20 | q feet, Imperial (8.1) |
| 30 | q feet, Thai (8.1) |
| 230 | qm (8) |
| 231 | qm (8.1) |
| 232 | qm (8.10) |
| 100 | mm (1234) |
| 101 | mm (1234.1) |
| 110 | cm (123) |
| 111 | cm (123.1) |
| 130 | m (12) |
| 131 | m (12.1) |
| 132 | m (12.10) |
| 970 | Time 00:00:00 |
| 985 | Timestamp US 4-digit year |
| 986 | Timestamp 4-digit year |
| 987 | Timestamp US 2-digit year |
| 988 | Timestamp 2-digit year |
| 995 | Date US 4-digit year |
| 996 | Date 4-digit year |
| 997 | Date US 2-digit year |
| 998 | Date 2-digit year |
| 1500 | 1 = + / 0 = '' |
| 1501 | 1 = + / 0 = - |
| 1502 | 1 = * / 0 = '' |
| 1510 | 1 = '' / 0 = + |
| 1511 | 1 = - / 0 = + |
| 1512 | 1 = '' / 0 = * |
| 1600 | Georgian bars |
| 1601 | Shapes |
| 1602 | IG |
| 1604 | Coating |
| 1605 | Structure |
| 1606 | Gas |
| 1607 | TG |
| 1608 | LG |
| 1609 | GH |
| 1610 | Processing |
| 1611 | Complex Processing |
| 1612 | Release part |
| 1703 | Part type |
| 1704 | Subpart type |
| 1804 | Component types for batch (Glass articles [1], Interlayers [10], Spacer [12]) |
### A+W Production Lists
Since A+W Production 5.1 all standard-Lists (starting with AUW_xxx) are changing their format automatically depending on the global settings of A+W Production. SO there is nothing special to do.
## A+W Production Terminal
In ToolTV there are local and global settings for the dimensions. In the standard-ToolTV’s it is only necessary to change the global-settings if you like to use inches or other non-metric dimensions.

### Local settings
Those settings are directly made during the definition of fields in an A+W Production Terminal-Mask:

![AUW_Configuration_measurement_image2](sandbox:/mnt/data/AUW_Configuration_measurement_image2.png)

This setting is only valid for the specified field.

If you chose one of the following formats:
- ALXF_TOOLTV_AREA
- ALXF_ToolTV_DIMENSION
- ALXF_ToolTV_THICKNESS

the field will be displayed as defined in the global settings.
### Global Settings
The global settings are mad directly in the parameter of ToolTV (Global Formats):
![AUW_Configuration_measurement_image3](sandbox:/mnt/data/AUW_Configuration_measurement_image3.png)

For Us the settings can be changed like this:

![AUW_Configuration_measurement_image4](sandbox:/mnt/data/AUW_Configuration_measurement_image4.png)

Now all fields in ToolTV which are designed in the formats ALXF_TOOLTV_AREA, ALXF_ToolTV_DIMENSION, ALXF_ToolTV_THICKNESS are replaced by those values.

**mm  inch:**
```sql
UPDATE parameter SET text = 'ALXF_AREASQFTX1' WHERE bereich = '@PROPERTY_SYSTEM' AND eintrag = 'FORMATTOOLTVAREA';
UPDATE parameter SET text = 'ALXF_MASSUSINCH64' WHERE bereich = '@PROPERTY_SYSTEM' AND eintrag = 'FORMATTOOLTVDIMENSION';
UPDATE parameter SET text = 'ALXF_MASSUSINCH64' WHERE bereich = '@PROPERTY_SYSTEM' AND eintrag = 'FORMATTOOLTVTHICKNESS';
```
**inch  mm:**
```sql
UPDATE parameter SET text = 'ALXF_AREAQMX1' WHERE bereich = '@PROPERTY_SYSTEM' AND eintrag = 'FORMATTOOLTVAREA';
UPDATE parameter SET text = 'ALXF_NUMMMX0' WHERE bereich = '@PROPERTY_SYSTEM' AND eintrag = 'FORMATTOOLTVDIMENSION';
UPDATE parameter SET text = 'ALXF_NUMMMX0' WHERE bereich = '@PROPERTY_SYSTEM' AND eintrag = 'FORMATTOOLTVTHICKNESS';
```
## A+W Business
For new projects uses the INCH database of MarketSolution team!

For A+W Business there normally exist a database for metric and one for inch. The following parameters are set in an inch database.

**[Basic data / Company / Company Data / System]**
![AUW_Configuration_measurement_image5](sandbox:/mnt/data/AUW_Configuration_measurement_image5.png)

In ALFAK you enter the weight in kg or pounds, standard is kg. If you enter the weight in pounds you have to activate the checkbox . If you do this the system knows that all weight values in ALFAK are in pound. This is necessary for the ORDERXML interface, because the weight in the interface is always in kg and if the value is in pound ALFAK convert it for the interface.
![AUW_Configuration_measurement_image6](sandbox:/mnt/data/AUW_Configuration_measurement_image6.png)

Until AWDesk #273964 is solved you have to convert (multiplied by 2.2) the weight on ALCIM reports if you want see the value in pounds.

[Basic data / Partner / Customer / Customers]
![AUW_Configuration_measurement_image7](sandbox:/mnt/data/AUW_Configuration_measurement_image7.png)

```sql
UPDATE SYSADM.KU_KUNDEN SET KZ_MASSEINH = 1 WHERE KZ_MASSEINH = 0;
```
[Basic data / Partner / Supplier / Suppliers]
![AUW_Configuration_measurement_image8](sandbox:/mnt/data/AUW_Configuration_measurement_image8.png)

All master data has to be updated to the right inch value, because A+W Business writes the values into database in the defined measurement. If the system is set to metric, all measurements are in mm, if it set to inch than it depends on the inch factor (32,64,128,…). The same happens with all order data, they have to enter new.

```sql
UPDATE SYSADM.LI_LIEFERANTEN SET KZ_MASSEINH = 1 WHERE KZ_MASSEINH = 0;
```