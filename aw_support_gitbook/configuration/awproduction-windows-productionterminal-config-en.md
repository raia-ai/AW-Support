---
description: "AW_Production_Terminal_-_Allow_Multiple_Instances_Version_1.00"
---


**A+W PRODUCTION TERMINAL**
**ALLOW ****MULTIPLE INSTANCES**
**A+W AUSTRALIA**

| **Date** | **Author** | **Modification/Remarks** | **Version** |
| --- | --- | --- | --- |
| 26/09/2023 | Todd Leiseman | First release of document | 1.00 |
|  |  |  |  |

## INTRODUCTION
ProjectFacts Ticket Number - [AW-161312]
In the documentation below we are going to configure a system to allow it to run multiple A+W Production Terminals at the same time on the same system.
**Note** - This change needs to be completed on each system that will run multiple copies of A+W Production Terminal at the same time - Workstations or Terminal Servers.
Why is this a wanted ability - this will allow a A+W Production Terminal Operator to open an A+W Order Station and a custom terminal that shows it’s incomplete processings so the operator can complete the processings as required using the known Barcode, Rack Number Size etc.

## LICENSING REQUIREMENTS
Please contact your local A+W Support personnel for any licensing requirements that need to be accounted for before proceeding with the configuration.
As at the time of this documentation it is licensed as each location in production. In this instance two production terminals running on the same location is counted as a single license.

## BEST USAGE REQUIREMENTS
Because of the minimum space needed by two A+W Production Terminals we have two monitor configurations that can be investigated in this instance.
- Two monitors of at least 1920 x 1080 resolution so that each Production Terminal can be docked to a separate monitor.
- Single Ultrawide Monitor of 3440 x 1440 so that enough screen space can be provided to both A+W Production Terminal screens at the same time.

## SYSTEM CONFIGURATION
Documented below are the required steps to allow multiple instances of a A+W Production Terminal to run at the same time.

### OPTION 1 - SYSTEM SETTINGS INTERFACE
Right Click on My PC (Windows 10 and Windows Server 2022)
Choose Properties
Select Advanced system settings
![Image 1](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_51_1.png)

Click the option Environment Variables… at the bottom right of the screen as shown below.
![Image 2](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_55_2.png)

Under System variables click the New… button and complete it with the following information shown below.
![Image 3](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_59_3.png)
Variable name = AllowMultipleToolTVs
Variable value = True
![Image 4](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_62_4.png)

After the update the System variables will have the new Variable entry as shown below.
![Image 5](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_65_5.png)

### OPTION 2 - COMMAND PROMPT UPDATE
Open a new command prompt in Administrator Mode
Type the following command - **setx /m AllowMultipleToolTVs "True"**
![Image 6](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_70_6.png)
This will update the Environment Variables > System variables the same as completing the steps through the Environment Variables screens.

## EXAMPLE RESULT OF CHANGE
Open A+W Production Terminal and choose the first A+W Production Terminal and Station (**Example** - AUW_ORDER).
![Image 7](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_76_7.png)
Repeat the step again for the second Station (**Example** - AUW_TG_IN).
![Image 8](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_78_8.png)
In the image below we can see that both screens - Order Production Terminal is docked on the left side of the screen while a TG (Furnace) In screen is docked on the right side of the screen.
![Image 9](sandbox:/mnt/data/aw_allow_multiple_instances_images/image_80_9.png)
