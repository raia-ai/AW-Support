---
description: "EN-INST-AW_Rack_Manager_Starting_Guide"
---


# Rack Manager Start-up
**AWDesk: 347582**

---
## Change history
| Date | Edited by | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2016-02-19 | J. Makowka | Initial version | |
| 2016-03-03 | J. Makowka | Expansion to include 'Tips and Tricks' | |

## 1. Preparation and installation

### 1.1. ERP, databases, and modules
To operate the A+W Rack Manager, you will need:

1.  **A database server (SQL server, version 2008 or higher, or Informix).**
    a. If your A+W ERP system uses another database system, you can install SQL Server Express Edition on the server on which you want to install the CommonBase server. This version is sufficient to operate the CommonBase and Rack Manager database and is available free of charge.

2.  **An A+W ERP system (A+W Business or A+W Enterprise)**
    a. Install the system according to the installation instructions.
    b. Perform the basic configuration according to the start-up instructions.
    c. Make sure that the ERP Webservice is installed correctly and configured for the connection to the Rack Manager (see Figure 1). In the "ERP Web Service feature selection", ensure `AWRack` is selected.

    *Figure 1: ERP Web Service configuration*

3.  **A database for the CommonBase (default name 'CommonBase').**
    a. Create the database before the installation. It will be filled later. Also create a user via which the CommonBase server can access the database. The user must have full read and write rights.
    If you want to use an Informix database, please note that the CommonBase only supports Informix locales with the Western character set (en\_US.CP1252, en\_US.819, en\_US.8859-1 and comparable). In particular, en\_US.UTF8 and such locales are not supported.
    b. If you already have a CommonBase database that is configured for an older version of the Rack Manager, check whether you can continue to use the existing database server. If necessary, make a back-up of the database and load the back-up onto the new database server.

4.  **A database for the Rack Manager (default name 'RackManager')**
    a. Create the database before the installation. It will be filled later. Also create a user via which the Rack Manager can access the database. The user must have full read and write rights.
    If you are using Informix, the same limitations apply with respect for the database locale as for the CommonBase database.
    b. If you are already using an existing AWRack database, check whether you can continue to use the database server. If necessary, make a back-up of the database and import it onto the new database server.

    > **Note:** If the old database server is a SQL Server 2005 or older version, an update to version 2012 or 2014 is not possible in one step. The back-up must be brought up-to-date with the importing and repeated back-up across several SQL Server versions. The sequence is SQL Server 2005 SP 1, SQL Server 2008, SQL Server 2012.

5.  **A Web server (at least Windows Server 2008 R2 with .NET Framework 4.5, recommended is Windows Server 2012 R2)**
    a. For this, activate the Web server role on the server on which you want to install A+W Rack Manager.
    b. Activate the role services depicted in Figure 2 and Figure 3.

    *Figure 2: Web server role services*
    *Figure 3: Web server role services*

    **Required Role Services:**
    - **Common HTTP Features:**
        - Default Document
        - Directory Browsing
        - HTTP Errors
        - Static Content
    - **Health and Diagnostics**
    - **Performance**
    - **Security:**
        - Request Filtering
        - Basic Authentication
    - **Application Development:**
        - .NET Extensibility 3.5 & 4.6
        - ASP.NET 3.5 & 4.6
        - ISAPI Extensions
        - ISAPI Filters

6.  **A CommonBase server**
    a. Install the 'A+W CommonBase Services' role and its dependencies. Tip: if you want to install all modules for the Rack Manager on the same machine, you can do this in a single SetupLauncher session. For the installation of the CommonBase services, the CommonBase update are installed automatically. If the CommonBase database was empty, it is initialized by this installation. If the CommonBase database already contains data, it will be brought up to date.
    b. In the firewall of the server, open the port TCP/1530 so that programs from the network can communicate with the CommonBase server.

7.  **The A+W Rack Manager Web service**
    a. Install the 'A+W Rack Manager Service' and its dependencies.

8.  **The A+W Rack Manager Web application**
    a. Install the 'A+W Rack Manager Web' and its dependencies.

### 1.2. Initializing and update of the A+W Rack Manager database
After the installation, you must initialize the database of the A+W Rack manager, that is, bring it up to date. To do this, call the 'A+W Database Update' module from the A+W start menu. Enter the database system, the connection information, and access data. Select the 'Update Type' 'AWRack' and the version 'v6' (see Figure 4). Then click 'Connect' and 'OK'.

*Figure 4: A+W database update*

## 2. A+W Rack Manager basic configuration
This chapter describes the basic configuration that you must perform if you install the Rack Manager in an environment where there was previously no AWRack. If you are in an environment that already contains settings for AWRack or the Rack manager, you can use this chapter as a guideline in order to check whether the configuration is complete and plausible. Note, however, that there are different possibilities for creating a correct configuration in CommonBase. Important is only that the user in question has the correct effective rights and settings, regardless of the way in which the rights and settings come about.

### 2.1. Configuration of the company structure
If you start with an 'empty' CommonBase, there is already a company group 'Standardcompanygroup' and a site 'Standardmandant'. For the simplest case where you have no internal settlement of accounts between sites, this configuration is sufficient. You need only an additional site for the external users, that is, users who belong to the company who do not participate in the rack system (typically customers).

Open the 'A+W CommonBase Configuration' module from the A+W Start menu. On the menu, open the 'Company >> Clients' area (see Figure 5) and insert the new site 'External'.

*Figure 5: Creating a site*

> **Note:** In case of a newly-initialized CommonBase, you can log in with the user name 'admin' and the password 'admin'. Please note that for the CommonBase login, capital and lower-case letters must be heeded for the user name. If this is an existing CommonBase, you may have to ask the person responsible for the admin user password.

### 2.2. Creating and configuring the user group
On the menu, in the 'User Groups >> User Group Overview' area, create two new user groups with the names 'RackMgrAdmin' and 'RackMgrUser'. These user groups function as bearers of the rights and settings for RackManager administrators and users.

*Figure 6: Creating user groups*

Open the 'User Groups >> User Group – Client – Relations' area and create a new assignment for the 'RackMgrAdmin' group. In the 'Priority' field, specify the value 100.

*Figure 7: Assignment of user group*

> **Note:** For the meaning of the 'Priority' field, please read the CommonBase manual.

Now from the context menu for the assignment (Figure 8), select the 'Edit Rights' element. Set the following rights to 'Right Set Explicitly'. Leave all other rights uninitialized.

*Figure 8: Context menu of the assignment*

- 'Admintool for Customer >> Administration >> Client' area all rights
- 'Admintool for Customer >> Administration >> Configuration' area all rights with the exception of 'The user has access to the switch group display'.
- 'Admintool for Customer >> Administration >> Group of companies' area all rights.
- 'Admintool for Customer >> Administration >> Rights area all rights with the exception of 'Determines whether the user has access to the right group display'.
- 'Admintool for Customer >> Administration >> User area all rights
- 'Admintool for Customer >> Administration >> User – Client – Relations' area all rights
- 'Admintool for Customer >> Administration >> User Group – Client – Relations' area all rights
- 'Admintool for Customer >> Administration >> User Groups' area all rights
- 'AWRack' area all rights with exception of 'AWRack >> Master Data >> Management >> End Customer Menu'.

Save the rights settings and select the 'Edit Switch' element (Figure 8) from the assignment context menu. In the 'AWRack >> Configuration >> Database' area, activate the switches 'Database User AWRack' and 'Password AWRack'. Enter the user name and password here that Rack Manager should use to access its database when an administrator is logged in. Then save the settings.

*Figure 9: Rack Manager DB access data*

Create an assignment of the user group 'RackMgrUser' for the 'Standardmandant' site. In the 'Priority' field, specify the value 200.

Edit the rights of the new assignment and set the following explicit rights. Leave the other rights uninitialized.
- **Admintool for Customer >> Administration >> Client**
    - Reading Clients
- **Admintool for Customer >> Administration >> Configuration**
    - Reading Switch Dependencies
    - Reading Switch Groups
    - Reading switches of switch groups
- **Admintool for Customer >> Administration >> Group of Companies**
    - Reading Company Groups
- **Admintool for Customer >> Administration >> Rights**
    - Reading Right Dependencies
    - Reading Right Groups
    - Reading Rights of Right Groups
- **Admintool for Customer >> Administration >> User**
    - Reading Languages
    - Reading Users
- **Admintool for Customer >> Administration >> User - Client - Relations**
    - Reading User – Client – Relations
- **Admintool for Customer >> Administration >> User Group – Client – Relations**
    - Reading Allocations (user to client user groups)
    - Reading User Group – Client – Relations
- **Admintool for Customer >> Administration >> User Groups**
    - Reading User Groups
- **AWRack >> Information all rights**
- **AWRack >> Master Data >> Management**
    - Reading (all owner groups)
    - Reading (owner group of user)
- **AWRack >> Rack Invoicing all rights**
- **AWRack >> Rack Movements >> ERP Webservice all rights**
- **AWRack >> Rack Movements >> Racks**
    - Booking
    - Modifying

Save the rights settings. Then edit the switches for the new assignment and adjust the access data for Rack Manager users. The procedure is the same as for the administrator group.

> **Note:** If you prefer that each user should log into the database with his own access, you must leave this switch deactivated and configure the access data for each individual user assignment.

### 2.3. Configuring the global settings
From the A+W CommonBase Configuration, open the area 'User >> User – Client –Relations'. From the context menu of the site 'Standardmandant', select the 'Edit Switch' element (see Figure 10).

*Figure 10: Configuring the global settings*

Activate the switches depicted in Figure 11 and set the values shown in the figure. For the database parameters, instead of 'RackManager', 'localhost', etc., use the values valid for your system. The switch 'Selection for pickup scheduling' has the omission value stored in CommonBase 'SELECT * FROM RATRANSACTION WHERE ACTUAL = 1 AND BOOKINGOWNER = 1 AND BOOKINGSTATE = 4'.

Here, in the 'Enterprise ERP' area, you must make the settings for the ERP system with which the Rack Manager should work. The settings differ. Select only one of the following configurations.

*Figure 11: Rack Manager switch settings*

> **Note:** Some switches may have deviating settings that make complete sense. Consult the AWRack manual if you are of the opinion that the switch settings depicted here do not suit your situation. Make adjustments if necessary.

### 2.3.1. Enterprise ERP settings for A+W Business
In the 'Enterprise ERP >> Webservice area, make the settings depicted in Figure 12. For the database parameters, instead of 'AUW50', 'localhost', 'SYSADM', etc., use the values valid for your system. The database to which reference is made here is the database of the A+W Business, not the database of the Rack Manager.

The 'Alfak Ini File' switch is used by the ERP Webservice in order to specify the language. There is no access to a file. For this switch, it is sufficient to specify the value '<Language>.ini'.

Note: the access data and password used for database access and for A+W Business are normally identical.

If you wish, you can specify individual access data for the users later by setting the appropriate switches for the user in question explicitly.

Save the configuration.

*Figure 12: Settings for A+W Business*

### 2.3.2. Enterprise ERP settings for A+W Enterprise
Make the settings depicted in Figure 13. Replace the database and access parameters, as well as 'localhost' port numbers, etc. with the values valid on your system. Save the configuration.

Note that the database to which reference is made here is the database of the A+W Enterprise, not the database of the Rack Manager.

If you wish, you can specify individual access data for the users later by setting the appropriate switches for the user in question individually.

*Figure 13: Settings for A+W Enterprise*

### 2.4. Creating the configuration for external users
Access for external users is created directly in the Rack Manager. The whole configuration for external users is therefore done through the settings for the 'External' site to which these users are assigned.

> **Note:** External users are people for whom access to the Rack Manager is possible, but who do not belong to the organization of a rack owner. Such users have only the possibility to view rack assignments, to report racks ready for pick-up, and to cancel the report of readiness for pick-up.

### 2.4.1. Rights for external users
In the 'User >> User – Client – Relations' area, select the 'Edit Rights' element from the context menu for the 'External' site. Assign the following rights:

- **Admintool for Customer >> Administration >> Client**
    - Reading Clients
- **Admintool for Customer >> Administration >> Configuration**
    - Reading Switch Dependencies
    - Reading Switch Groups
    - Reading switches of switch groups
- **Admintool for Customer >> Administration >> Group of Companies**
    - Reading Company Groups
- **Admintool for Customer >> Administration >> Rights**
    - Reading Right Dependencies
    - Reading Right Groups
    - Reading Rights of Right Groups
- **Admintool for Customer >> Administration >> User**
    - Reading Languages
    - Reading Users
- **Admintool for Customer >> Administration >> User - Client - Relations**
    - Reading User – Client – Relations
- **Admintool for Customer >> Administration >> User Group – Client – Relations**
    - Reading Allocations (user to client user groups)
    - Reading User Group – Client – Relations
- **Admintool for Customer >> Administration >> User Groups**
    - Reading User Groups
- **AWRack >> Information all rights**
    - Reading Statistic Data
- **AWRack >> Master Data >> Management**
    - End Customer Menu
    - Reading (all owner groups)
- **AWRack >> Rack Movements >> ERP Webservice**
    - Executing
- **AWRack >> Rack Movements >> Racks**
    - Booking

Save these rights settings.

### 2.4.2. Configuration settings for external users
In the 'User >> User – Client – Relations' area, select the 'Edit Rights' element from the context menu for the 'External' site.

In the AWRack area, set the switch as depicted in Figure 14. Replace 'localhost', 'RackManager', etc. with the values valid for your installation.

Here you must specify a database user because the management of external users within the Rack Manager does not give you the opportunity to enter individual access data.

If necessary, you can assign created external users individual database access rights after the fact by setting the appropriate switches in the assignment of the user to the 'External' site.

You must now just set the configuration in the 'Enterprise ERP' area. For this, proceed as described in chapter 2.3.1 or 2.3.2.

*Figure 14: Rack Manager settings for external users*

> **Note:** Depending on the situation, different individual settings may make sense. Read the AWRack manual.

## 3. Creating users

### 3.1. Creating an administrator
Rack Manager administrators have the necessary rights for creating and changing master data. In addition, they can also make rack bookings and create rack invoices.

In the A+W CommonBase Configuration, open the area 'User >> User Overview'. Use the 'New' button to create a new user with the 'RackAdmin' login. Here, fill out as many input fields as possible (see Figure 15).

You can also create users for individual people if you prefer. This procedure also allows you to use individual database logins.

Now open the area 'User >> User – Client-Relations'.

*Figure 15: Creating an administrator*

Create a new user-site assignment. Use the search tools to select the 'RackAdmin' user and the 'Standardmandant' site. Use the 'Add' button to add the association with the user group 'RackMgrAdmin' (see Figure 16).

*Figure 16: Creating site assignment*

### 3.2. Creating Rack Manager users
Rack Manager users have the rights required for making rack bookings and creating rack invoices. However they do not have the right to enter or change master data or to create or edit external users.

In the A+W CommonBase Configuration, open the area 'User >> User Overview' and create a new user. Fill out as many fields as possible on the input dialog. For the example in this document, the user name 'RackUser' is used. In practice, for each Rack Manager user, you will want to assign an individual user name so that later on you can trace who booked rack transactions and created invoices.

If you want to create several users, it is recommended that you first create all users in the 'User >> User Overview' area and then make the assignments in the 'User >> User – Client – Relations' area.

To create the assignments, open the area 'User >> User – Client -Relations'. Create a new assignment. Use the search tools to select the user ('RackUser') and the site 'Standard-mandant'. Use the 'Add' button to add the association with the user group 'RackMgrUser' (see Figure 17).

*Figure 17: Assigning standard users*

## 4. Creating Rack Manager master data
Start the Rack Manager and log in as a Rack Manager administrator. You have a link on the A+W Start menu to the server on which you have installed the Rack Manager. If you want to connect from another computer, the URL is `http://hostname/RackManager.Web`. Here you must replace 'hostname' with the registry entry for the server in the DNS or its IP address.

The figures in this document were created with the Microsoft Edge browser. However you can also use Internet Explorer, Google Chrome or Mozilla Firefox.

### 4.1. Creating owner group
You do not absolutely have to create a new owner group since the Rack Manager database already includes an owner group with the name 'Default' after the initialization; you can use this. However if you want to have the settings completely under your control, it is recommended that you create a new owner group. For this, switch to the 'Master Data >> Owner Groups' area and click the 'New' button. Then fill out the fields in the header area of the page. As 'Accounting Type' select the value 'Owner'. Save the new owner group with the 'Save' button.

*Figure 18: Creating owner group*

> **Note:** For the possible values in the input fields, please read the explanations in the AWRack manual. You can display the manual by clicking the 'Documentation' link in the navigation area. Please note that you will need a PDF reader to read the manual.

### 4.2. Creating an owner
Open the page 'Master Data >> Owner'. Click the 'New' button to create a new owner. Assign a new number. The fields 'Group' and 'Company' are the company group and the site from CommonBase to which this user is assigned.

As 'Owner Group', specify the owner group created in chapter 4.1. Under 'Path webservice', specify the URL of the ERP Webservice. Here, leave off the final '/ErpData.asmx'.

Then place a check next to 'Rack Invoicing'. Thus you have the possibility to calculate rack rents.

Save the rack owner with the 'Save' button.

Note: You can use the 'Table' button to display the existing data records.

*Figure 19: Creating users*

### 4.3. Creating rack types
Open the page 'Master Data >> Rack Types'. Normally you will create several rack types for the rack in use. If racks that are used differ in their shape or technical data, you must create a rack type for each individual variant. You can display the already-existing rack types by clicking the 'Table' button.

*Figure 20: Creating rack types*

In the table, click on the 'Select' link in the line for the newly-created rack type. Thus the 'Assignment' tab can be selected. On this tab, you must assign the rack type to an owner. Use the 'New' button for this. On the 'Owner' combo box, select the 'Standardowner' entry. Specify a product code. Please note that the product code that you specify here is the product code that is used if orders are transmitted to the ERP system for invoicing. The product code must be known to the ERP system and it must be the item that is used to account for one day's rack rental.

Specify how many rent-free days the rack may stand in a delivery point and whether rent is even calculated for racks of this type.

*Figure 21: Owner assignment rack type*

Save the assignment with the 'Save' button. Create appropriate assignments for all rack types that you create.

> **Note:** To use the 'Table' and 'Selection' buttons, please read the AWRack manual.
> **Note:** For additional information, see the attachments about the configuration of the ERP systems for work with the Rack Manager.

### 4.4. Creating racks
Open the page 'Master Data >> Racks'. Display the existing racks with a click on the 'Table' button. If you have just installed the Rack Manager, the list is empty.

Create new racks with a click on the 'New' button. Fill out the input fields on the header part of the page. Make sure that you set the correct rack owner under 'Owner'. If you are creating a test installation, please note the information in the footnote.

*Figure 22: Creating racks*

You can create several racks in one step here. To do this, enter a value greater than the value in the first field in the second field. One rack is then created for each number in the range. The rack bar code is also incremented for each newly-created rack.

For the assignment of the rack bar codes, make sure that the values assigned fit the ones that are used for rack reporting from A+W Production.

> **Note for test installations:** If racks are entered for an existing operation, the creation data is automatically in the past, in any case if it is input correctly. If, by contrast, you are creating a test installation for the Rack manager, it is important to take over current data. However you should not do this. Instead, select a procurement time that is approximately one month in the past. This gives you the opportunity to make outgoing bookings in the past immediately after entering the rack. After such backdated bookings, you can also create messages about pick-up readiness that create retention periods for which rack rentals are actually due. Only if you proceed this way can you actually test the rack invoicing.
> **Note:** For additional information, see the attachments about the configuration of A+W Production in combination with the A+W Rack Manager.

### 4.5. Specifying accessories (optional)
The A+W Rack Manager allows you to maintain an overview of how many accessory parts are currently at a customer's. If you do not want to use this possibility, you do not have to create any accessories. You can then skip this chapter.

If you want to work with accessories, create the accessories that you are using according to the following instructions.

Open the page 'Master Data >> Accessories'. Use the 'Table' button to display the existing accessory items. If you are starting up the Rack Manager with a new database, this table will be empty at first.

Use the 'New' button to create a new accessory item. Give the item a unique number ('Number' field, see Figure 23). Specify the remaining information about the accessory item. The 'Inventory' field specifies the stock (number of units of the item that are on hand in the warehouse).

Save the accessory item with the 'Save' button.

*Figure 23: Creating accessories*

### 4.6. Creating external users (optional)
If you want to give users who do not belong to your organization access to the Rack Manager so that they can view rack assignments and report rack readiness for pick-up, you must use the logins for these external users. If your organization does not make such a possibility available to external users, you can ignore this chapter.

Open the page 'Master Data >> Logins'. Create a new external user with the 'New' button and enter the data for the external user into the header area of the page. Then save the data with the 'Save' button.

With this procedure, you can create a new user in CommonBase who is assigned to the 'External' site.

*Figure 24: Creating external users*

However, you must still assign the external user to an owner. To do this, click the 'Select' link in the cell for the external user in the table. Then click the 'Assignment' tab and use the 'New' button to create a new assignment. In the 'Owner' field, select the 'Standardowner' entry. In the Customer Number field, specify the customer's customer number from the ERP system to which the external user belongs. Save the assignment with the 'Save' button.

*Figure 25: Customer assignment of external users*

## 5. Completing the start-up
If you have followed the instructions in the previous chapters, the start-up of the Rack Manager is essentially complete. Now you should conduct a few tests in order to check the functionality of the Rack Manager and the connection to the ERP system. Use a standard user to log in and perform a rack delivery, report a rack ready for pick-up, and create a rack invoice.

You can see whether the connection to the ERP Webservice is working using the information page ('Information >> System Info'). The connection can be established if you see a version number in the 'Version of ERP Webservice' field. If there is a text in this field, then there is a problem with the connection to the ERP Webservice.

To complete the start-up work, you should make sure that there is an appropriate data back-up procedure for the Rack Manager database and the CommonBase database.

*Figure 26: Displaying system information*

## Anhang A: Configuring A+W Enterprise for working with the Rack Manager

### A.1 Settings in the A+W Enterprise back end
To create the rack invoicing, `intauf4` must be configured. This is done as follows:

- The following line must be added to the file `$ALDATPFAD/ctrl_serv.par`:
    - `„Intauf4 ^I4B^I4S^I4W^I4E^I4X^intauf_E^vmauwx^alcib intaufrech^360^900^99999^22018^^intauf4.log^0^1^”`
    - `99999` refers to the employee's employee number; this is the person who receives a message if the service could not be started.
    - The '1' at the end means that the service is started automatically when starting the CTRL server. - Starting with Version 6, this is triggered via the ERP WebService.

- The following entry must be completed in the file `/etc/services`:
    - `intauf_E1 65001/tcp`
    - The '1' in 'intauf_E1' corresponds to the content of the variable SOCKETMD for this site.
    - Please check that the port number is unique!

- After that, the CTRL server must be stopped and restarted with `ctrlservstop; ctrlserstart`.

### A.2 Requirements for the item for rack invoicing
To generate the rack invoicing, an item with the item type 'Other item' must be created. This is a piece item (quantity unit 9) that refers to a piece price in the prices that corresponds to the rack rental for one day.

## Anhang B: Configuring A+W Business for working with the Rack Manager

### B.1 Configuration settings

#### B.1.1 Settings in A+W Business
By default, A+W Business is not configured for working with the Rack Manager, but rather for the integrated rack management. The configuration must be changed for working with the Rack Manager.

The settings are made in the master data under **Company/Company data** on the **Dispatch** tab.
- Under **Rack Management**, you must select **AWRack** instead of ALFAK.
- The URL of the RackManager Webservice must be entered for **AWRack Webservice**. Here the actual service name (AWRackService.asmx) must be omitted.
- Under **Default Range for Invoices**, you must select **Standardaufträge / Standard order**.
- Furthermore, the **Current site is default site for invoices** must be checked.

*Figure 27: A+W Business settings for the Rack Manager*

### B.2 Master data requirements

#### B.2.1 Item numbers of the rack
In the Rack Manager, a rack type has a separate item number for each owner who uses this rack type. These item numbers are set under **Master data/Rack types** on the **Assignment** tab.

If a rack of this type is invoiced by an owner, its item number for the rack type is transmitted to the ERP. Therefore, the item number must exist in the owner's ERP and belong to an item that is compatible with the rent costs for a rack.

There is no automatic comparison of the item number for the rack rental in the ERP and the Rack Manager. The user must ensure that the item numbers are present on both sides and used for the same racks.

*Figure 28: Item numbers of the rack types in the RackManager*

## Anhang C: Configuring A+W Production for working with the Rack Manager

### C.1 Configuration settings

#### C.1.1 Settings in A+W Production
Settings must be made in A+W Production so that work with the Rack Manager is possible:

On the **Master data/Configuration** menu element, the parameters under **ALCIM/General**, the **AWRack Connection** area must be filled out.
- Under **AWRack Web address** the URL of the Rack Manager service must be entered (including the service name [AWRackService.asmx]).
- For **Userlogin** and **Userpassword**, the user's CommonBase(CB) access data must be entered.
- If in the CB more than one site is used, you must make sure that the values **Company group CB** and **Site** are set correctly for the CB user. If only one company group and site are used, then the values are normally 1/1.

*Figure 29: Configuration settings in A+W Production*

### C.2 Requirements for the rack bar codes
The rack bar codes are specified by A+W Production using the currently-used rack. You must make sure that the appropriate bar codes are present in the Rack Manager. With the standard database, bar codes like the one marked in green are generated.

The bar codes are in the Rack Manager in the master data under **Racks**. If no rack with the bar code specified by A+W Production exists, then there is an error booking for which the rack must be created after the fact (**Rack transactions/Rack transactions, Error bookings** tab).

There is no automatic master data comparison for rack bar codes between A+W Production and the Rack Manager. The user must enter the bar codes correctly in the Rack manager or create racks after the fact using the error bookings.

*Figure 30: Rack bar codes in the Rack Manager master data*

## Anhang D: Tips and Tricks

### D.1 Incorrect display in Internet Explorer
If you start the Rack Manager with Internet Explorer, it can happen that the display is not correct. This happens if the Web server on which the Rack Manager is running and the PC on which Internet Explorer is started are on the same intranet.

*Figure 31: Incorrect display in Internet Explorer*

The reason for the incorrect display is a setting in Internet Explorer that exists in some intranet configurations. This is an unsuitable setting for the compatibility view of Internet Explorer. The Rack Manager uses modern formatting possibilities that are also provided by current browsers. In some intranet environments, however Internet Explorer is set so that for pages from the local intranet, it has the behavior of much older versions in which the new formatting possibilities are not available.

To change this, call up the 'Settings for the compatibility view' element from Internet Explorer's Settings menu (see Figure 32).

*Figure 32: Calling up settings for the compatibility view*

Remove the checkmark next to **'Display intranet pages in the compatibility view'** (see Figure 33). If you are using intranet pages for which the compatibility view is required, add these pages to the list. The pages in the list will continue to be displayed in the compatibility view.

As soon as you make settings for the compatibility view, the Rack Manager is displayed correctly.

*Figure 33: Settings for the compatibility view*

### D.2 Creating external users in Firefox
If you are trying to create external users with the Firefox browser, the browser asks with each step whether you want to save the password for the user in the Password Manager. Here, Firefox does not offer you the opportunity to omit saving the password only for the created users as other browsers do. You must either save the password or suppress the saving of passwords for the Rack Manager completely. For security reasons, A+W recommends selecting the 'Never save passwords for this page' option when using Firefox. As soon as you have done this, you can create external users without any additional hurdles.

*Figure 34: Password inquiry for Firefox*

### D.3 Informix local information for the Rack Manager database
The setting possibilities for the access data for the Rack Manager database in the CommonBase area 'AWRack >> Configuration >> Database' do not include any fields for the additional local information that is required for Informix databases. You must therefore use a workaround in order to provide this information to Rack Manager. The most secure way to do this is to attach the information to the database password. To do this, open an editor and enter the following text on a line:

```
passwort;Client Locale=en_US.CP1252;Database Locale=en_US.819
```

Instead of 'password', use the actual password for the database login, and instead of 'en\_US.CP1252' and 'en\_US.819' use the values valid in your system. Note that the keywords 'Client locale' and 'Database locale' can include precisely one blank space in the middle. Note also that you use only the semicolon (';') as separator, no other character.

Copy the line to the clipboard and insert it into the input fields for the password and password repetition. Save the password modified this way.

With this modification, the local information is transmitted correctly to Informix.
