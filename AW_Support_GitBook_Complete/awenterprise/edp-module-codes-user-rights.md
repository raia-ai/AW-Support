---
title: "EN-CONFIG-AW_Enterprise_EDP_Module_Codes"
source: "EN-CONFIG-AW_Enterprise_EDP_Module_Codes.pdf"
tags: ["A+W Enterprise", "EDP Module Codes", "User Rights", "Access Control", "Software Configuration", "Technical Manual", "Glass Software", "Permissions", "Multi-site"]
version: "1.0"
last_updated: "2025-10-08"
short_description: "A technical guide detailing the module codes used in the A+W Enterprise software. This document explains the general logic for managing user rights and access permissions, including multi-site capabilities, and provides a comprehensive reference for all individual module codes."
long_description: "This document serves as a comprehensive technical manual for the A+W Enterprise – EDP Module Codes. It is designed for both internal and external users, such as system administrators and developers, to understand and manage user access rights and program behavior within the A+W Enterprise system, a specialized software solution for the glass industry. The guide begins with an overview of the general logic behind module codes, explaining how they control user permissions on a per-employee or per-group basis. It covers key concepts like multi-site capability, the hierarchy of user rights evaluation, data access restrictions, and access logging. The core of the document is a detailed, section-by-section breakdown of every module code. Each section corresponds to a specific program area, such as Barcode, Stock Management, Prices, and System Management. Within each section, tables and descriptions provide detailed information for each module code, including its designation, relevant menu items, possible rights allocations (read, write), a description of its function, and any dependencies. This structured reference is essential for correctly configuring user permissions, ensuring data security, and customizing program behavior to meet specific operational needs."
---

# A+W Enterprise – EDP Module Code

**A+W Module Codes**
A+W - Software for Glass
language: english

## 1. Content

1.  **Content**
2.  **Overview**
    *   2.1. History
    *   2.2. General Logic for Module Codes
    *   2.3. Access log
3.  **All Program Modules**
    *   3.1. Multi-site capability
        *   3.1.1. User rights
        *   3.1.2. Copying module rights and rights groups
        *   3.1.3. Evaluation of the rights in the modules
        *   3.1.4. Evaluation hierarchy for user rights
        *   3.1.5. Restriction of data access
        *   3.1.6. Restriction of SQL queries
4.  **Notes**
5.  **Barcode**
6.  **Budgeting Module**
7.  **EDI module**
8.  **Disposition module**
9.  **Rack management**
10. **Internal balancing CONSAFIS**
11. **Terms**
12. **Cost calculation module**
13. **Key management**
14. **Stock management**
15. **Matrix processing**
16. **Marketing Module**
17. **Market partner**
18. **Object management**
19. **PMS**
20. **Prices**
21. **Print management**
22. **Statistics**
23. **Master data management**
24. **System management**
25. **TEKAP programs**
26. **Text management**
27. **Documents**
28. **Receipt of goods**
29. **Contact Address**

## 2. Overview

The documentation of module codes was made for internal and external use. It offers users a description of the module code logic and a detailed description of the individual module codes.

### 2.1. History

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2012-02-01 | Frauke Frantz | Original version | 1.0 |
| 2018-04-15 | Elena Tempelfeld | Update | 1.1 |

### 2.2. General Logic for Module Codes

The module codes in A+W Enterprise serves to manage user rights. The module codes control access rights and program behavior per employee or group.

The definition of user rights is made in user data (Master Data > Employee in section Rights or Right Groups).
If no rights are defined for a user, he has no rights. Use the allocation of rights via module codes to permit access to program sections or to enable functions.

If an employee with module authorization also belongs to an authorization group (Master Data > Employee field Right Groups) with module rights, its employee authorizations takes precedence over the group authorizations. This also means: if an employee has module rights in an authorization group, that are explicitly denied to him, he can not use the corresponding module or function.

If an employee belongs to several authorization groups (Master data > Employee field Rights groups) with module rights, the lower right applies in the case of contradictory assignment of rights (the same right is assigned differently in 2 authorization groups). This means: If in one authorization group a detailed module right has been assigned as write access and in another authorization group as read acces, the employee has read-only access.

The employee rights are divided into module areas and can also be assigned for an entire area (2-digit module authorizations, e.g. KY* for the entire key area). If different rights are assigned to an area and a special module (e.g. KYKA - for calendars), the more specific right applies.
e.g.
KY* - read and KYKA write
This results in write authorization for the calendar, but only read authorization for all other modules in the Key area.

Access right and program behavior can be assigned exclusively for a user. The different display modes in the dialogs show you the kind of access right - read or write. The symbol is in front of the dialog name.

The following pictures show the status:

*   **+** Write and read permissions. A new record will be added.
*   The record is read-only, the data will only be displayed.
*   Status of dialog is not defined.
*   Write and read permission

All module codes have four digits, the first two letters define the section:

| Module sections | Description |
| :--- | :--- |
| **AM** | Notes |
| **BC** | Barcode |
| **BU** | Budgeting |
| **DF** | Data transfer |
| **DI** | Purchasing |
| **GE** | Racks (management and planning) |
| **IVCO** | Internal balancing CONSAFIS |
| **KO** | Terms |
| **KR** | Cost calculation module |
| **KY** | Key management |
| **LA** | Stock management |
| **MA** | Matrix processing |
| **MK** | Marketing |
| **MP** | Market partner |
| **OB** | Object management |
| **PM** | PMS main module |
| **PS** | Price maintenance |
| **RE** | Printer management |
| **SS** | Statistics |
| **ST** | Master data management |
| **SY** | System management |
| **TE** | TEKAP programs |
| **TX** | Text management |
| **VO** | Documents (quotations, orders,...) |
| **WE** | Receipt of goods |

### 2.3. Access log

It logs which module was entered by whom and when and which rights query for which user was queried. This function is controlled via environment variable ZUTRITT_PROTO. The information is saved in the database table zutrittproto. Please note, that checks for rights and module access within the background processes will not be recorded. (for internal information see AWDesk case #123237)

## 3. All Program Modules

### *

**Designation:** all program modules

**Possible allocation of rights:**
Rights set with * are valid for all module codes of A+W Enterprise. This global setting is valid for all program areas as long as a module code gets its own right. Companies that work with client-specific system settings, must define the rights for „all Program Modules" for each client (see chapter 3.1).

*   **Read (r):** read permission means that the user can only view existing data records. For some access rights, the read permission has no effect. In this case the program requires some entries and then the function will be executed.
*   **Read and write (w):** Full access means that the user can read and write in the mentioned dialog/section/program.

**Description:**
`*` right controls access to A+W Enterprise if necessary client-specific (per site). That means, if an employee gets ‚r‘ right for ‚*‘ module for client 20 he may only start program sections, that allow read access. Changes of any kind are correspondingly excluded.

**Dependencies:** none.

### 3.1. Multi-site capability

In internal site systems where employees of companies with different legal status work simultaneously, it is important to be able to limit both the module rights as well as the data access on the site level. Thus you can prevent any employee from accessing the data for all clients as soon as he has been created in the system.

#### 3.1.1. User rights

A site assignment must be specified for all employees. If he may only operate the program in one site, then it is sufficient to make an assignment in the "client" field. If an employee works in several sites, then there must be a site assignment made using the "Site assignment" button or `<Shift+F5>`. Since only the companies are offered for selection for which the person entering the order has rights, this assignment should be made by one of the master data administrators (MASTER_DATA_ADMIN). (Right STMM)

After the employee is assigned to the different sites, site-specific rights can also be assigned or revoked. To do this, you enter the rights on the lower part of the dialog with entry of the site number. If the site number remains blank, then this right rule applies for all companies to which the employee is assigned.

For rights groups, it is NOT possible to assign a site since these are always defined generally. If for an employee a rights group is selected, then you can limit this only to particular sites. If no site is specified for the rights group assignment, then the rights of the group apply in all sites to which the employee is assigned.

#### 3.1.2. Copying module rights and rights groups

A copy function was added to the sub-dialogs for Rights and Rights groups with which it is possible to transfer existing rights to additional clients.

The function is only available for such records that already have a client assignment. This client applies as source client for the copy action. Trigger the copy function with the key combination `<CTRL+F9>`. A dialog appears on which the target client can be selected. Only such clients are available for selection that were assigned to the employee. If the dialog is triggered with `<F3>` or the `<Start>` button, all data records of the source client are copied to the target client.

If there were already records for the target client, these are deleted before the copy action in order to prevent doubled records and ensure that source rights and target rights are identical after the copy action. With an appropriate query before deletion, the user can prevent the deletion of the rights by canceling and copy action.

In order to copy the configured rights of a source client to all possible target clients for an employee, you can simply leave the field for the target clients blank on the selection dialog.

Additional prerequisites for the copy mechanism are: the employee must have more than one client assignment and the employee type must be 'Employee.'

#### 3.1.3. Evaluation of the rights in the modules

The site that was entered directly in the employee master data applies as main site for the employee and is pre-populated as current site. However, after the start of the program, you can change the site assignment for this session. This is possible using `<CTRL+F4>` > a User Configuration > a Change Site. Naturally this change is only possible if the employee has more than one site assignment. With the start of all menu items (if these are protected with an individual right), user rights are then checked site-specifically. In the process entry, first there is only a general check whether the user has a right to enter orders in at least one site. With a call of an existing process, the site number assignment is then made concrete and then the appropriate rights are checked. For the new entry, the right is checked according to the site number on the process entry dialog. With the `<Start>` button, you can change the site assignment directly in the process during the new entry. Here only the sites are available for selection to which the employee is assigned. After the selection of a site, the appropriate entry rights are checked again for this site.

#### 3.1.4. Evaluation hierarchy for user rights

It is currently possible to store user rights on different levels. Thus even today, you can combine rights into rights groups, in addition there are rights to module groups and directly on the module level. The site level has now been added to these levels. The evaluation of the different hierarchy levels is done as follows here:

| Priority | Site allocation | Module/Module Group | User/Group |
| :--- | :--- | :--- | :--- |
| 1 | H | M | B |
| 2 | H | M | G |
| 3 | H | MG | B |
| 4 | H | MG | G |
| 5 | * | M | B |
| 6 | * | M | G |
| 7 | * | MG | B |
| 8 | * | MG | G |

*   **H**: Rights with site allocation
*   **\***: Rights independent of the site
*   **B**: User rights
*   **G**: Group rights
*   **M**: Module rights (e.g. VOKA)
*   **MG**: Module group rights (e.g. VO*)

Here it is so that rights that are assigned to a site generally have a higher priority than rights that were assigned regardless of the site. Module-specific rights have a higher priority on the next hierarchy level than rights from module groups. In addition, rights that are assigned directly to the user have a higher priority than rights that were assigned via user groups.

#### 3.1.5. Restriction of data access

Since the various sites may be legally independent companies, it is important to ensure that employees who are only assigned to one or more clients can only view the data of the assigned sites as early as the selection dialogs (transaction search, product and market partner search and other SELOS). This restricted data view is relevant to all client-specific master and transaction data. For example, an employee who is assigned only to site 11 can only view orders that are allocated to site 11 in the order search window. All other orders remain hidden.

Such restricted data views are only possible at those points in the program at which the associated data has been assigned to a site. As a result, no site allocations will exist for the Salutation keys, since they are maintained globally across all sites. Therefore it is not possible to implement a restricted data view or site-specific rights check at this location.

#### 3.1.6. Restriction of SQL queries

Since data access for SQL queries is controlled via the saved SQL, it is unfortunately not possible to make general program adjustments that would automatically allow for restricted views in accordance with the user's rights. To nevertheless achieve such restricted access, a temporary nxhaus table is created when the program starts. It contains all of the fields of the xhaus table; but it is reduced to the sites to which the employee registered with A+W Enterprise has been assigned. Hence all tables with a site allocation would be joined with this table, so that only the data from the table for which the employee has access rights (via the site allocation) is displayed. All SQL queries of Group 1 (SQL queries delivered by A+W) were already converted. They will be supplied with the version update.

## 4. Notes

Below you will find the individual rights for section Notes.

**Multi-site capability:** Module codes AM* are global user rights. This means, it is not possible to maintain and evaluate this right client-specific.

### AM*

**Designation:** notes module

**Menu items:**
*   Master Data > Market Partner > Notes `<F5>`
*   Master Data > Market Partner > MP Product Notes `<Shift+F5>`
*   Master Data > Employee > Notes `<F5>`
*   Master Data > Departments > Notes `<F5>`
*   Master Data > Article > `<F5>`
*   Master Data > Article > `<Shift+F5>`

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.

Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:** this module code controls the notes module. It is valid for all notes except the document notes.

**Explanation of the notes:**
Notes on market partners, articles, employee, etc. are managed in a central table. This enables you to save e.g. notes for customer-articles, object-articles and employees.

The function is called in the different sections via `<F5>`.

In order entry: the notes are automatically be displayed if at least one line has the priority 'high'. If not, you can view the notes via `<Shift+F5>`.

A function can be called from different sections, that determines whether a note of the certain priority exists for the selected key.

Important! Only old functions are implemented: notes for MPs, objects and articles.

Document notes remain as before, since they are not only connected to the order number but also to the document. Order texts can only be edited in order entry and not from other sections.

*   Master Data > Market Partner, Notes `<F5>`
*   Master Data > Market Partner, MP Product Notes `<Shift+F5>`
*   Master Data > Employee, Employee Notes `<F5>`
*   Master Data > Departments, Department Notes `<F5>`
*   Master Data > Article, Article Notes `<F5>`
*   Master Data > Article, Customer Article Notes `<Shift+F5>`

**Dependencies:** users must have corresponding rights for master data to change notes. The processing mode in the 'notes' dialogs depends on whether you have got write or read permissions for the corresponding master data record.

**Multi-site capability:** module code AM* involves global user rights. This means, it is not possible to maintain and evaluate this right client-specific. This means, it is not possible to maintain and evaluate this right client-specific.

### AMAL

**Designation:** general notes

**Menu:** access right to menus:
*   Master Data > Market Partner, `<F5>` or `<Shift+F5>`
*   Master Data > Article, `<F5>` or `<Shift+F5>`
*   Master Data > Employee, `<F5>`
*   Master Data > Departments, `<F5>`

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** module code controls access and type of access to Notes dialog.

**Dependencies:** none.

**Multi-site capability:** module code AMAL is a global user right. This means, it is not possible to maintain and evaluate this right client-specific.

### AMAR

**Designation:** article notes module

**Menu items:**
*   in order body: Sales > Order Entry > `<Shift+F4>` > Article Notes
*   Master Data > Article > Notes `<F5>`
*   Master Data > Article > Customer Article Notes `<Shift+F5>`

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** this module code controls the article notes.

**Dependencies:** users must have corresponding rights for master data to change notes. The processing mode in the 'notes' dialogs depends on whether you have got write or read permissions for the corresponding master data record.

**Multi-site capability:** module code AMAR is a global user right. This means, it is not possible to maintain and evaluate this right client-specific.

### AMMP

**Designation:** MP Notes module

**Menu items:**
*   in order header Sales > Order Entry > Shift+F4 > MP Notes
*   Master Data > Market Partner > `<F5>`
*   Master Data > Market Partner > `<Shift>` + `<F5>`

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** this module code controls the market partner notes module.

**Dependencies:** users must have corresponding rights for master data to change notes. The edit mode in the 'notes' dialogs depends on whether you have got write or read permissions for the corresponding master data record.

**Multi-site capability:** module code AMMP is a global user right. This means, it is not possible to maintain and evaluate this right client-specific.

## 5. Barcode

Below you will find the individual rights for section Barcode.
**Barcode module is not supported anymore. The description here is of February 1st, 2012.**

### BC*

**Designation:** Barcoding Module

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this own rights definition is valid.

The following rights can be set for a module section: read (r) and read and write access (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of the barcoding.

**Dependencies:** none

### BCIN

**Designation:** Barcode INSERT

**Menu:**
Barcoding > Simulation

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog shows the edit mode.

**Description:** The module code controls whether barcoding data can be entered manually. Use this function to disable scanning of barcodes and to enable manual input.

**Dependencies:** none

### BCMA

**Designation:** Barcoding employee statistics evaluation

**Menu:**
*   Production > Barcoding > Evaluation > Employees Evaluation
*   Production > Barcoding > Evaluation > Time Registration
*   Production > Barcoding > Evaluation > Machinery Working Times
*   Production > Barcoding > Evaluation > TE Daily Statistics
*   Production > Barcoding > Evaluation > TE Monthly Statistics
*   Production > Barcoding > Evaluation > Furnace Statistics
*   Production > Barcoding > Evaluation > Production Progress
*   Production > Barcoding > Evaluation > Lite - Rack
*   Production > Barcoding > Evaluation > Rejects Statistics
*   Production > Barcoding > Evaluation > Documentation
*   Production > Barcoding > Evaluation > Test Documentation

**Possible allocation of rights:**
Read access is sufficient for this module to enable statistics. Otherwise: both rights can be assigned for this module code: read (r) and read and write (w). Display mode of a dialog shows the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none

### BCPR

**Designation:** Barcode: start and stop process

**Menu:**
*   Production > Barcoding > Start/Stop > Start Barcode
*   Production > Barcoding > Start/Stop > Stop Barcode

**Possible allocation of rights:**
A write access must be defined for code "BCPR" to start and stop the BARCODE process. Otherwise a corresponding message appears and the process can neither be started nor stopped.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none

### BCRKBCRK

**Designation:** Allocation of barcodes to AWRackStatus

**Menu:**
Production > Barcoding > Management > Barcode AWRack Allocation

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog shows the read access and the read and write access (w) shows the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none

### BCST

**Designation:** Barcoding status

**Menu:**
Production > Barcoding > Management > Status Management

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above, in which both the status designation and the reject reason is maintained.

**Dependencies:** none

### BCVW

**Designation:** Barcode Label Management

**Menu:**
Production > Barcoding > Management > Status Labels

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above, in which the print formats for barcode labels are defined.

**Dependencies:** none

## 6. Budgeting Module

Below you will find the individual rights for section Budgeting module.
**The Budgeting module in A+W Enterprise is not supported anymore. The description here is of February 1st, 2012.**

### BU*

**Designation:** budgets module

**Menu items:**
Sales > Distribution > Company Budget

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.

**Description:**
This module section controls the user rights of budgeting.

**Dependencies:** none

### BUBU

**Designation:** budgeting

**Menu:**
Sales > Company Budget > Budgeting

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set, the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none

### BUMA

**Designation:** distribution matrix

**Menu:**
Sales > Distribution > Company Budget > Distribution Matrices

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set, the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none

### BUSI

**Designation:** compare target / actual

**Menu:**
Sales > Distribution > Company Budget > Compare Target/Actual

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set, the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none

### BUVE

**Designation:** vectors

**Menu:**
Sales > Distribution > Company Budget > Distribution Vectors

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set, the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none

## 7. EDI module

Below you will find the individual rights for section EDI module.
EDI modules are global authorizations, mainly used of system in background. Thus, they can not be controlled individually per employee/client.

### DF*

**Designation:** EDI modules

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.

Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
It is possible to configure control of EDI and other sections for customers and suppliers in dialog System > Data Transfer > Transfer Document > Configuration.
This module section controls the user rights of EDI.

**Dependencies:** none.

**Multi-site capability:** module codes DF* involve global user rights.

### DFAB

**Designation:** deferred transmission
**Description:** access authorization DFAB is not supported anymore.

### DFAU

**Designation:** order transfer

**Menu:** access right for menu System > Data Transfer > Transfer Document > Start Transfer.

**Possible allocation of rights:**
*   Read (r): read access has no effect for this access right.
*   Read and write (w): full access.

**Description:** this access authorization allows the employee to start order transfer from site X to site Y.

**Dependencies:** none.

**Multi-site capability:** module code DFAU is a global user right.

### DFFB

**Designation:** FINAC transaction data transfer

**Menu:** access right for menu System > Data Transfer > FINAC Transfer Data

**Possible allocation of rights:**
*   Read (r): read access has no effect for this access right.
*   Read and write (w): full access.

**Description:** this access authorization allows the employee to start transfer of FinAc transaction data from site X to site Y.

**Dependencies:** none.

**Multi-site capability:** module code DFFB is a global user right.

### DFIR

**Designation:** internal balancing

**Menu:** access right for menu System > Data Transfer > Glass Balancing.

**Possible allocation of rights:**
*   Read (r): read access has no effect for this access right.
*   Read and write (w): full access.

**Description:** this access authorization allows the employee to start the internal glass balancing between production site and the corresponding distributor.

**Dependencies:** none.

**Multi-site capability:** module code DFFB is a global user right.

### DFKO

**Designation:** EDI configuration

**Menu:**
*   System > Data Transfer > Transfer Document > Configuration
*   Market Partner Master > `<F4>` > EDI Configuration in field Type of EDI `<F5>`

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** use this module code to control access to EDI.

**Dependencies:** none.

**Multi-site capability:** module code DFKO is a global user right.

### DFRT

**Designation:** key reference table
**Description:** access authorization DFRT is not supported anymore.

### DFSA

**Designation:** article selection for transfer

**Menu:** access right for menu System > Data Transfer > Article Replication

**Possible allocation of rights:**
*   Read (r): read access has no effect for this access right.
*   Read and write (w): full access.

**Description:** this access authorization allows the employee to start synchronization of article data to site X.

**Dependencies:** article replication shall be configured.

**Multi-site capability:** module code DFSA is a global user right.

### DFST

**Designation:** sending table for table transfer
**Description:** access authorization DFST is not supported anymore.

### DFUE

**Designation:** EDI of key tables
**Description:** access authorization DFUE is not supported anymore.

## 8. Disposition module

Below you will find the individual authorizations for section Disposition Modules (Purchase).

### DI*

**Designation:** disposition modules (purchase)

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Purchase.

**Dependencies:** none.

**Multi-site capability:** all module authorizations in section DI* can be maintained and evaluated client-specific.

### DIAB

**Designation:** close purchase orders

**Menu:** Purchase > Goods Receipt > Close Purchase Orders

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set or read-only the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIAB right can be set client-specific.

### DIAN

**Designation:** inquiries

**Menu:** Purchase > Inquiries

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above. In this dialog you can enter and display supplier inquiries.

**Dependencies:** none.

**Multi-site capability:** DIAN right can be set client-specific.

### DIBE

**Designation:** purchase orders

**Menu:** Purchase > P.O. Management

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above. In this dialog you can enter and modify purchase orders.

**Dependencies:** none.

**Multi-site capability:** DIBE right can be set client-specific.

### DIBP

**Designation:** purchase order pool processing

**Menu:** Purchase > Create Purch. Orders
Purchase > Create Purchase Orders > on item level key combination `<Ctrl + N>`

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above and load of supplier assessment.

**Dependencies:** none.

**Multi-site capability:** DIBP right can be set client-specific.

### DIDR

**Description:** form printing Sales

**Menu:** access right for menu Purchase > Form.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module controls access to the dialog mentioned above and thus, print release for all purchase documents.

**Dependencies:** none.

**Multi-site capability:** module authorizations DIDR can be maintained and evaluated client-specific. If the user does not have the right for a client, he can still enter the dialog. In the selection selo, only the purchase documents for other clients where he has the right are made available. If you enter a number manually, the documents from this site are rejected.

### DIFK

**Designation:** missing quantities check pool

**Menu:** Purchase > Goods Receipt > Missing Qty. Check Pool

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:**
When you open the menu Missing quantity pool the system shows a list of items the quantity of which has been corrected. You can either order the missing quantities, or simply remove them from the check pool. The processed records are saved in a log table. If an order has been created, the new P.O. number is shown in the log table.
The module key controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIFK right can be set client-specific.

### DIFR

**Designation:** P.O. release

**Menu:** Purchase > P.O. Release

**Possible allocation of rights:**
Read(r) and read and write permission can be assigned for this module code. There is no difference in program behavior between the two rights. In both cases, you can change the data.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIFR right can be set client-specific.

### DIGB

**Designation:** book purchase credit notes

**Menu:** Purchase > Credit Notes > Book Credit Notes

**Possible allocation of rights:**
Read(r) and read and write permission can be assigned for this module code. There is no difference in program behavior between the two rights. In both cases, you can change the data.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIGB right can be set client-specific.

### DIGS

**Designation:** purchase credit notes

**Menu:** Purchase > Credit Notes > Enter Credit Notes

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIGS right can be set client-specific.

### DILK

**Designation:** rights for local corrections in purchase

**Possible allocation of rights:**
Read(r) and read and write permission can be assigned for this module code. There is no difference in program behavior between the two rights. In both cases, you can change the data.

**Description:** this module code controls the following program function: if the user has no read or read and write permission, purchase and sales documents with status Local Correction can not be loaded.

**Dependencies:** none.

**Multi-site capability:** DILK right can be set client-specific.

### DILS

**Designation:** Cancel receipt of goods

**Possible allocation of rights:**
Cancel receipt of goods is made in manual entry of goods by pressing the `<F7>` key in the invoice header or alternatively by selecting the "Cancel" menu item from the `<F4>` menu. After confirming a security check ("Do you really want to cancel? Yes/No") you can indicate a cancellation reason.

**Description:** This module code controls the functionality to cancel goods receipts: Only if the user has no DILS right, he cannot cancel goods receipts. Read (r): has the same effect as w right.

**Dependencies:** none.

**Multi-site capability:** DILS right can be set client-specific.

### DIRB

**Designation:** book purchase invoices

**Menu:**
*   Purchasing > Invoices > Automatic invoices
*   Purchase > Invoices > Manual Invoices
*   Purchase > Invoices > Transferred Invoices
*   Purchase > Invoices > Booking of Invoices

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above. Module codes DIRB and DIRE control the rights for entering and booking. This function is also influenced by environment variables.

**Dependencies:** variable NO_BUCHENFRAGE in sales and purchase ensures that invoices and credit notes were automatically be booked. Variable EK_DIREKTBUCHEN controls booking in purchase without prior question to the user. For sales, there is also the variable VK_DIREKTBUCHEN.
In addition, the right "DIRB" protects booking of P.O. invoices and right "DIGB" protects booking of P.O. credit notes. If users create invoices or credit notes and do not have this right, booking is skipped. These documents must be booked later.

**Multi-site capability:** DIRB right can be set client-specific.

### DIRE

**Designation:** purchase invoices

**Menu:**
*   Purchasing > Invoices > Automatic invoices
*   Purchase > Invoices > Manual Invoices
*   Purchase > Invoices > Transferred Invoices
*   Purchase > Invoices > Booking of Invoices

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** see module code DIRB

**Multi-site capability:** DIRE right can be set client-specific.

### DIRK

**Designation:** invoice check purchasing

**Menu:** Purchase > Invoices > Check Invoices

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** MODUL_EKRECH_KONTROLLE: use this environment variable to activate module Check P.O. Invoices. (case: 125942)

**Multi-site capability:** DIRK right can be set client-specific.

### DIRS

**Designation:** cancel purchasing invoices

**Menu:** Purchase > Invoices > Manual Invoices
Cancellation is made in manual entry of invoices by pressing the `<F7>` key in the invoice header or alternatively by selecting the "Cancel" menu item from the `<F4>` menu. After confirming a security check ("Do you really want to cancel? Yes/No") you can indicate a cancellation reason.

**Possible allocation of rights:**
Read and write permission must be set to cancel the invoice. In case of read permission the message "Action does not make sense" appears.

**Description:** the module code controls cancellation of invoices.

**Dependencies:** environment variable EK_RECHNUNGS_STORNO must be set.

**Multi-site capability:** DIRS right can be set client-specific.

### DISG

**Designation:** cancel purchasing credit notes

**Menu:** Purchase > Credit Notes > Enter Credit Notes

**Possible allocation of rights:**
Cancellation is done in the manual invoice/credit note entry by pressing `<F7>` in the invoice/credit note header, or switching to the menu via `<F4>` and selecting "Cancel". After confirming a security check ("Do you really want to cancel? Yes/No") you can indicate a cancellation reason.

**Description:** read and write permission is necessary to cancel the invoice. In case of read permission the message "Action does not make sense" appears.

**Dependencies:** environment variable EK_GUTSCHRIFTS_STORNO must be set.

**Multi-site capability:** DISG right can be set client-specific.

### DIUR

**Designation:** transferred invoices

**Menu:** Purchase > Invoices > Transferred Invoices

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:**
When you open the menu Invoices transferred, the menu that appears now shows the purchase invoices to be created in the interface tables. When you open the menu, all invoices received will be checked for consistency. You can decide whether inconsistent invoices shall be checked again next time you open the module, or shall be removed from the interface tables. One reason for inconsistent data may be that no goods have been received in this case or the receipt of goods has been cancelled. You will proceed to a table now in which you can compare the net amounts of the goods received with the invoice amounts. The two checkboxes can be used to tag the corresponding document to be created or deleted from the interface tables. More information is available from a detailed menu. The top part of the menu compares the item prices and discounts from receipt of goods with those on the invoice. The bottom part shows an invoice block similar to document entry. If the system data differ from the data received, they can be located by means of this menu. The module key controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIUR right can be set client-specific.

### DIWA

**Designation:** goods received

**Menu:** Purchase > Goods Receipt > Delivery Schedule, automatic, manual, and rack-related receipt of goods

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. In case of read permission, the goods receipts present in the system are shown in display mode only. No further actions are possible.

**Description:** the module code controls access to the mentioned dialog. The user needs read and write permission to use the dialog and function.

**Dependencies:** none.

**Multi-site capability:** DIWA right can be set client-specific.

### DIWK

**Designation:** check goods received

**Menu:** Purchase > Goods Receipt > Control of Receipt of Goods

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** When you open the menu Check goods received a menu appears showing the goods received to be created from the interface tables. You can change the input date and select the documents to be created. The detailed view shows the individual items and permits to check - and correct if necessary - the quantity received. If you have ticked several goods received, these will be created as separate documents, using the correct quantities. For every item where the corrected quantity differs from the quantity received, an entry will be made in the Missing quantity pool. The documents will be saved in the log directory, in file „eingangek*".
The module key controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** DIWK right can be set client-specific.

### DIWR

**Designation:** antedating the receipt of goods

**Menu:**
*   Purchase > Goods Receipt > Manual Receipt of Goods
*   Purchasing > Receipt of Goods > Automatic Receipt of Goods

**Possible allocation of rights:**
Write (w) permission is necessary to change data. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** Users who do not have this right cannot enter a date in the past as the goods receipt date in goods receipt entry. The right will only be evaluated, if WAEIN_LAPFWLAGER_DATUM=ON is set (AWDesk case #200054)

**Dependencies:** None

**Multi-site capability:** DIWR right can be set client-specific.

## 9. Rack management

Below you will find the individual rights for section Rack management/Packaging planning.
**All modules of group GE* are global authorizations. That means, the access rights cannot be evaluated for each individual client.**

### GE*

**Designation:** rack management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.

Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Rack Management.

**Dependencies:** module Rack Management is configured.

**Multi-site capability:** module code GE* involves global user rights.

### GEAG

**Designation:** rack balancing

**Menu:** Logistics > Rack Management > Central Management > Rack Balancing

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set or read-only the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above and thus, execution of rack balancing.

**Dependencies:** none.

**Multi-site capability:** module code GEAG is a global user right.

### GEBU

**Designation:** rack bookings

**Menu:** Logistics > Rack Management > Rack Bookings

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode. If the right is not set or read-only the user has no access to the dialog.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GEBU is a global user right.

### GEHG

**Designation:** main rack types

**Menu:**
*   Logistics > Rack Management > Master Data (Racks) > Rack Main Groups > Groups
*   Logistics > Rack Management > Master Data (Racks) > Rack Main Groups > Individual Descriptions
*   Logistics > Rack Management > Master Data (Racks) > Rack Main Groups > All Descriptions
*   Master Data > Keys > System > PMO > Rack Groups > Individual Description
*   Master Data > Keys > System > PMO > Rack Groups > All Descriptions

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GEHG is a global user right.

### GEKU

**Designation:** racks at customers

**Menu:** Logistics > Rack Management > Information > Racks at Customers

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GEKU is a global user right.

### GELA

**Designation:** racks on stock

**Menu:** Logistics > Rack Management > Information > Racks on Stock

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GELA is a global user right.

### GELI

**Designation:** rack lists
**Description:** access authorization GELI is not supported anymore.

### GEMA

**Designation:** reminded racks

**Menu:** Logistics > Rack Management > Reminders

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GEMA is a global user right.

### GEMP

**Designation:** manual rack management
**Description:** access authorization GEMP is not supported anymore.

### GEPL

**Designation:** rack planning

**Menu:** Logistics > Rack Management > Rack Scheduling

**Possible allocation of rights:**
*   Reading (r): ineffective at this point, i.e. the 'r' right allows access to the rack planning dialog, but any activity in the dialog is prevented.
*   Read and write (w): full access

**Description:** this module code controls access right to the dialog mentioned above.

**Dependencies:** module „Rack Planning" has to be purchased and must be configured.

**Multi-site capability:** module code GEPL is a global user right.

### GERE

**Designation:** rack restrictions

**Menu:** access right for menu Rack restrictions within rack scheduling in order (F5 in "Specs. Packaging Planning")

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read/write (w): full access.

**Description:** this module code controls access to rack restrictions in order

**Dependencies:** module „Rack Planning" has to be purchased and must be configured.

**Multi-site capability:** module code GERE can be maintained and evaluated client-specific.

### GESL

**Designation:** rack BOM

**Menu:** Logistics > Rack Management > Master Data (Racks) > Rack Types

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** the rack BOM can only be opened, if the environment variables GESTPLAN_PRIO or GESTPLAN_PYRO are set ("ON").

**Multi-site capability:** module code GESL is a global user right.

### GEST

**Designation:** rack master data

**Menu:** Logistics > Rack Management > Master Data (Racks) > Individual Entry

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GEST is a global user right.

### GESZ

**Designation:** lite rack allocation

**Menu:** Logistics > Rack Management > Lite Allocation

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above. Via the Lite Rack Allocation dialog it is also possible to make the rack corrections (PDC readings). For these corrections, the write GESZ access (#459400) is necessary.

**Dependencies:** none.

**Multi-site capability:** module code GESZ is a global user right.

### GETY

**Designation:** rack types

**Menu:** Logistics > Rack Management > Master Data (Racks) > Rack Types

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GETY is a global user right.

### GEVE

**Designation:** rack distribution

**Menu:** Logistics > Rack Management > Central Management > Distribution

**Possible allocation of rights and description:** this module code controls in central rack management, whether an employee may start a rack distribution in connected sites. If a user has no, or only read permission, a message appears after starting the rack distribution: "You have no authorization for rack distribution!" and the program is being terminated.

**Dependencies:** none.

**Multi-site capability:** module code GEVE is a global user right.

### GEZB

**Designation:** central booking racks

**Menu:** Logistics > Rack Management > Central Management > Central Bookings

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code GEZB is a global user right.

## 10. Internal balancing CONSAFIS

Below you will find the individual rights for section Internal balancing CONSAFIS.
**Internal balancing module Consafis is not supported anymore. The description here is of February 1st, 2012.**

### IVCO

**Designation:** internal balancing CONSAFIS

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Internal Balancing CONSAFIS.

**Dependencies:** none.

## 11. Terms

Below you will find the individual rights for section Conditions.
**All modules of group KO* are global authorizations That means, the access rights cannot be evaluated for each individual client.**

### KO*

**Designation:** conditions

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:** this module section controls the user rights of Conditions. Master Data > Conditions

**Dependencies:** none.

**Multi-site capability:** module code KO* involves global user rights.

### KOAF

**Designation:** special exchange list factors

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Exchange List Factors

**Possible allocation of rights:**
*   Read (r): only read access to existing exchange list factors.
*   Read and write (w): full access to exchange list factors.

**Description:** the module code controls the control of special exchange list factors per market partner.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_SPEZATLFAKT.

**Multi-site capability:** module code KOAF is a global user right.

### KOAK

**Designation:** special conditions article conditions

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Article Conditions

**Possible allocation of rights:**
*   Read (r): only read access to existing conditions for article categories.
*   Read and write (w): full access to article conditions.

**Description:** the module code controls access to maintenance module of article conditions.

**Dependencies:** use of this function is controlled via environment variable MODUL_ARTIKELKOND.

**Multi-site capability:** module code KOAK is a global user right.

### KOAR

**Designation:** special conditions article prices

**Menu:** access right for menu Master Data > Conditions > Special Prices > Article Prices

**Possible allocation of rights:**
*   Read (r): only read access to existing "Special Article Prices".
*   Read and write (w): full access to "Special Product Prices".

**Description:** the module code controls access to maintenance module for "Special Product Prices".

**Dependencies:** use of this function is controlled via environment variable SPEZIELLE_ARTIKELPREISE.

**Multi-site capability:** module code KOAR is a global user right.

### KOAUKOAU

**Designation:** special conditions IG exchange

**Menu:** access right for menu Master Data > Conditions > Special Prices > IG Exchange Prices

**Possible allocation of rights:**
*   Read (r): only read access to existing "IG Exchange Prices".
*   Read and write (w): full access to "IG Exchange Prices".

**Description:** the module code controls access to the dialogs mentioned above, in which both the status designation and the reject reason is maintained.

**Dependencies:** use of this function is controlled via environment variable MODUL_ISOAUSTPREISE.

**Multi-site capability:** module code KOAU is a global user right.

### КОВС

**Designation:** conditions: bonus CONSAFIS

**Menu:** Master Data > Prices > Price Control > Bonus Rules

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** this is a customer-specific set of rules.

**Multi-site capability:** module code KOBC is a global user right.

### KOBE

**Designation:** special conditions processings

**Menu:** access right for menu Master Data > Conditions > Special Prices > Processing Prices

**Possible allocation of rights:**
*   Read (r): only read access to existing "Special Processing Prices"
*   Read and write (w): full access to "Special Processing Prices":

**Description:** the module code controls access to maintenance module for "Special Processing Prices".

**Dependencies:** use of this function is controlled via environment variable MODUL_BEARBPREISE.

**Multi-site capability:** module code KOBE is a global user right.

### KOEF

**Designation:** IG-single lites product vectors (condition)

**Menu:** access right for menu Master Data > Conditions > Special Conditions > IG Single Lite Conditions > Article Factors

**Possible allocation of rights:**
*   Read (r): only read access to existing article factors.
*   Read and write (w): full access to article factors.

**Description:** this module code controls the special IG single lite - article factors per client.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_KEZARTFA.

**Multi-site capability:** module code KOEF is a global user right.

### KOEW

**Designation:** IG-single lites product group factors (condition)

**Menu:** access right for menu Master Data > Conditions > Special Conditions > IG Single Lite Conditions > Product Group Factors

**Possible allocation of rights:**
*   Read (r): only read access to existing product group factors for IG single lites.
*   Read and write (w): full access to product group factors for IG single lites.

**Description:** the module code controls access to maintenance module for special product group conditions for IG single lites.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_KEZWGRPFA.

**Multi-site capability:** module code KOEW is a global user right.

### KOFA

**Designation:** special conditions colored articles

**Menu:** access right for menu Master Data > Conditions > Special Prices > Colored Articles

**Possible allocation of rights:**
*   Read (r): only read access to special prices for colored articles.
*   Read and write (w): full access to special prices for colored articles.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOFA is a global user right.

### KOGA

**Designation:** special prices/factors for patterned categories

**Menu:** access right for menu Master Data > Conditions > Special Prices > Exchange Prices Patt. Categ.

**Possible allocation of rights:**
*   Read (r): only read access to special exchange prices for patterned classes.
*   Read and write (w): full access to exchange prices for patterned classes.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_GUSSAUSTAUSCH.

**Multi-site capability:** module code KOGA is a global user right.

### KOKA

**Designation:** general conditions

**Menu:** access right for menu Master Data > Conditions > Special Conditions > General Conditions

**Possible allocation of rights:**
*   Read (r): only read access to special general conditions.
*   Read and write (w): full access to special general conditions.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOKA is a global user right.

### KOKF

**Designation:** special conditions product groups/product factors

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Article Factors

**Possible allocation of rights:**
*   Read (r): only read access to special product group conditions.
*   Read and write (w): full access to special product group conditions.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** Module code KOKF is a global user right.

### KOKM

**Designation:** special conditions shape surcharges

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Shape Surcharges

**Possible allocation of rights:**
*   Read (r): only read access to special shape surcharges.
*   Read and write (w): full access to special shape surcharges.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable MODUL_MODELLZUSCHL.

**Multi-site capability:** module code KOKM is a global user right.

### KOKO

**Designation:** item type conditions

**Menu:** access right for dialog Type Conditions in order entry (`<Ctrl + F9>` in order header)

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOKO is a global user right.

### KOKW

**Designation:** special conditions product groups

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Product Group Conditions

**Possible allocation of rights:**
*   Read (r): only read access to special product group conditions.
*   Read and write (w): full access to special product group conditions.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable MODUL_WARENGRKOND.

**Multi-site capability:** module code KOKW is a global user right.

### KORA

**Designation:** special conditions scale of discount

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Scales of Discount

**Possible allocation of rights:**
*   Read (r): only read access to special scales of discount.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KORA is a global user right.

### KORU

**Designation:** conversion of invoices

**Menu:** Master Data > Prices > Price Control > Redirection of Invoices

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog.

**Dependencies:** none.

**Multi-site capability:** module code KORU is a global user right.

### KOSE

**Designation:** special prices for single lites

**Menu:** access right for menu Master Data > Conditions > Special Prices > IG Single Lites

**Possible allocation of rights:**
*   Read (r): only read access to special prices for IG single lites.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOSE is a global user right.

### KOSF

**Designation:** special conditions muntin factors

**Menu:** access right for menu Master Data > Conditions > Special Conditions > Muntin Factors

**Possible allocation of rights:**
*   Read (r): only read access to special muntin factors.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOSF is a global user right.

### KOSI

**Designation:** special IG prices

**Menu:** access right for menu Master Data > Conditions > Special Prices > IG Basic Prices

**Possible allocation of rights:**
*   Read (r): only read access to special IG basic prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_SPEZISOPREIS.

**Multi-site capability:** module code KOSI is a global user right.

### KOSP

**Designation:** special conditions muntins prices

**Menu:** access right for menu Master Data > Conditions > Special Prices > Muntin Prices

**Possible allocation of rights:**
*   Read (r): only read access to special muntin prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOSP is a global user right.

### KOSV

**Designation:** special variant prices

**Menu:** access right for menu Master Data > Conditions > Special Prices > Variant

**Possible allocation of rights:**
*   Read (r): only read access to special variant prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_SPEZVARPRS.

**Multi-site capability:** module code KOSV is a global user right.

### KOSZ

**Designation:** special conditions: AIR surcharges

**Menu:** access right for menu Master Data > Conditions > Special Conditions > AIR Surcharges

**Possible allocation of rights:**
*   Read (r): only read access to special AIR surcharges.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_SZRZUSCHLAG.

**Multi-site capability:** module code KOSZ is a global user right.

### KOTA

**Designation:** daily conditions general daily conditions

**Menu:** access right for menu Master Data > Conditions > Daily Conditions > General Daily Conditions

**Possible allocation of rights:**
*   Read (r): only read access to general daily conditions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable MODUL_TAGESKOND.

**Multi-site capability:** module code KOTA is a global user right.

### KOTW

**Designation:** daily conditions product groups

**Menu:** access right for menu Master Data > Conditions > Daily Conditions > Product Group Conditions

**Possible allocation of rights:**
*   Read (r): only read access to general product group conditions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable MODUL_TWARENGRKOND.

**Multi-site capability:** module code KOTW is a global user right.

### KOUV

**Designation:** special conditions UV-protection

**Menu:** access right for menu Master Data > Conditions > Special Prices > UV Protection Prices

**Possible allocation of rights:**
*   Read (r): only read access to special UV protection prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable MODUL_UVABDECKUNGEN.

**Multi-site capability:** module code KOUV is a global user right.

### KOVA

**Designation:** special LAMI exchange/additional prices

**Menu:** access right for menu Master Data > Conditions > Special Prices > LAMI Exchange/Addit. Prices

**Possible allocation of rights:**
*   Read (r): only read access to special LAMI exchange/Additional prices.
*   Read and write (w): full access

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable KONDITIONEN_SPEZVSGAUST.

**Multi-site capability:** module code KOVA is a global user right.

### KOVG

**Designation:** special conditions glazing

**Menu:** access right for menu Master Data > Conditions > Special Prices > Glazing Prices

**Possible allocation of rights:**
*   Read (r): only read access to special glazing prices.
*   Read and write (w): full access

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable MODUL_VERGLASUNG.

**Multi-site capability:** module code KOVG is a global user right.

## 12. Cost calculation module

Below you will find the individual rights for section Cost calculation module.

### KR*

**Designation:** cost calculation-modules

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Cost Calculation.

**Dependencies:** none.

**Multi-site capability:** module code KR* involves global user rights. The client-specific possibilities of configuration are described in the corresponding access rights.

### KRER

**Designation:** cost registration

**Menu:** access right for menu Analysis > Statistics > Costs > Cost Protocol

**Possible allocation of rights:**
*   Read (r): entry of costs is not possible.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KOER is a global user right.

### KRSS

**Designation:** cost statistics / cost type

**Menu:** access right for menu Analysis > Statistics > Costs > Cost Statistics > Cost Type

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** -/- .

**Dependencies:** none.

**Multi-site capability:** all module authorizations in section DI* can be maintained and evaluated client-specific.

### KRST

**Designation:** cost calculation-master

**Menu:** access right for menu Master Data > Costs.

**Possible allocation of rights:**
*   Read (r): only read access to costs: cost types, cost units, cost centers.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KRST is a global user right.

## 13. Key management

Below you will find the individual rights for section Key management.

**Multi-site capability:** All modules of section KY* are global user rights. This means, access rights can not be valuated per individual client.

### KY*

**Designation:** key management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Key Management.

**Dependencies:** none.

**Multi-site capability:** module code KY* is a global user right.

### KYAF

**Designation:** identification rules

**Menu:** access right for menu Master Data > Text Management > Text Generation > Text Formulas

**Possible allocation of rights:**
*   Read (r): only read access to existing text formulas.
*   Read and write (w): full access to text formulas.

**Description:** -/- .

**Dependencies:** none.

**Multi-site capability:** module code KYAF is a global user right.

### KYAN

**Designation:** address key

**Menu:** access right for menu Master Data > Keys > Market Partner > Titles

**Possible allocation of rights:**
*   Read (r): only read access to existing titles.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYAN is a global user right.

### KYAT

**Designation:** IG exchange lists

**Menu:** access right for menu Master Data > Keys > Prices > Exchange/Additional Lists

**Possible allocation of rights:**
*   Read (r): only read access to existing exchange/additional lists.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYAT is a global user right.

### KYAY

**Designation:** analysis groups

**Menu:** access right for menu Master Data > Keys > Products > Analysis Groups

**Possible allocation of rights:**
*   Read (r): only read access to existing analysis groups.
*   Read and write (w):

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYAY is a global user right.

### KYAZ

**Designation:** order surcharge

**Menu:** access right and function for order surcharge.

**Description:** module code KYAZ is a special function for surcharges (method 1002=rush orders) to be configured separately.

**Dependencies:** none.

**Multi-site capability:** module code KYAZ is a global user right.

### KYBB

**Designation:** allocate ordered processing

**Menu:** access right for menu Master Data > Keys > Products > Processings Ordered

**Possible allocation of rights:**
*   Read (r): only read access to existing product allocations for purchased processings.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYBB is a global user right.

### KYBO

**Designation:** bonus code

**Menu:** access right for menu Master Data > Keys > Market Partner > Bonus

**Possible allocation of rights:**
*   Read (r): only read access to existing bonus.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYBO is a global user right.

### KYBR

**Designation:** industry code

**Menu:** access right for menu Master Data > Keys > Market Partner > Industries.

**Possible allocation of rights:**
*   Read (r): only read access to existing industries.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYBR is a global user right.

### KYBT

**Designation:** fitting types

**Menu:** access right for menu Master Data > Keys > Products > Fitting Types.

**Possible allocation of rights:**
*   Read (r): only read access to existing fitting types.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYBT is a global user right.

### KYBV

**Designation:** processing vector code

**Menu:** access right for menu Master Data > Keys > Prices > Processing Vectors.

**Possible allocation of rights:**
*   Read (r): only read access to existing processing vectors.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYBV is a global user right.

### KYCO

**Designation:** company master data

**Menu:** access right for menu Master Data > Keys > System > Companies/Corporations > Companies/Corporations

**Possible allocation of rights:**
*   Read (r): only read access to existing company data.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYCO is a local user right. This access authorization can only be used in connection with multi-site system.

### KYDB

**Designation:** db groups

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Groups > Sound Protection (dB).

**Possible allocation of rights:**
*   Read (r): only read access to existing sound protection groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYDB is a global user right.

### KYDI

**Designation:** size variants

**Menu:** access right for menu Master Data > Keys > Products > Variants > Sizes.

**Possible allocation of rights:**
*   Read (r): only read access to existing size variants.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYDI is a global user right.

### KYET

**Designation:** label text code

**Menu:** access right for menu Master Data > Keys > Market Partner > Label Texts.

**Possible allocation of rights:**
*   Read (r): only read access to existing label texts.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYET is a global user right.

### KYFA

**Designation:** color code

**Menu:** access right for menu Master Data > Keys > Products > Variants > Colors.

**Possible allocation of rights:**
*   Read (r): only read access to existing color variants.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYFA is a global user right.

### KYFL

**Designation:** phrases

**Menu:** access right for menu Master Data > Text Management > Phrases. In document entry `<F4>` in order header Texts > Header/Footer > or Product-/Item Texts, button `<Phrases>`

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** module code controls program behavior to use phrases and access to dialog Phrases in Master Data.
If the employee does not have Writer rights, he or she can neither create a new phrase from the document entry nor make any corrections to existing ones. Loading of existing phrases is always allowed.

**Dependencies:** none.

**Multi-site capability:** module code KYFL is a global user right.

### KYFR

**Designation:** generation of texts

**Menu:** access right for menu Master Data > Text Management > Text Generation > Variable Description.

**Possible allocation of rights:**
*   Read (r): only read access to existing variable descriptions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above. These variable names as well as the text formulas are used for generation of customer-specific box signature. This function must be configured separately.

**Dependencies:** use of this function is controlled via environment variable MODUL_KISTENSIGNATUR.

**Multi-site capability:** module code KYFR is a global user right.

### KYFT

**Designation:** film types

**Menu:** access right for menu Master Data > Keys > Products > Film Types.

**Possible allocation of rights:**
*   Read (r): only read access to existing film types.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYFT is a global user right.

### KYGE

**Designation:** g values

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Vectors > Sound Protection (dB), thermal properties.total energy transmission and transmission.

**Possible allocation of rights:**
*   Read (r): only read access to existing sound protection groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYGE is a global user right.

### KYGG

**Designation:** g groups

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Groups > Total Energy Transmission (g).

**Possible allocation of rights:**
*   Read (r): only read access to existing total energy transmission values.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYGG is a global user right.

### KYGR

**Designation:** group codes

**Menu:** access right for menu Master Data > Keys > Market Partner > Groups.

**Possible allocation of rights:**
*   Read (r): only read access to existing market partner groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYGR is a global user right.

### KYGW

**Designation:** restrictions

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Groups > Size Restrictions.

**Possible allocation of rights:**
*   Read (r): only read access to existing size restrictions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYGW is a global user right.

### KYHA

**Designation:** site specific key

**Menu:** access right for menu Master Data > Keys > System > Companies/Corporations > Companies/Corporations.

**Possible allocation of rights:**
*   Read (r): only read access to existing company data.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYHA is a local user right. This access authorization can only be used in connection with multi-site system.

### KYIS

**Designation:** description price matrices

**Menu:** access right for menu Master Data > Keys > Prices > Matrices.

**Possible allocation of rights:**
*   Read (r): only read access to existing company data.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYIS is a global user right.

### KYIW

**Designation:** Intrastat - product groups

**Menu:** access right for menu System > Statistics > Intrastat > Product Index.

**Possible allocation of rights:**
*   Read (r): only read access to the existing product index.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYIW is a global user right.

### KYKA

**Designation:** calendar

**Menu:** access right for menu Master Data > Keys > Market Partner > Calendar or `<Ctrl + F4>` Info Services > Calendar.

**Possible allocation of rights:**
*   Read (r): only read access to existing calendar configuration.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYKA is a global user right.

### KYKF

**Designation:** country code key
**Description:** access authorization KYKF is not supported anymore.

### KYKG

**Designation:** U groups

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Groups > Thermal Properties (U).

**Possible allocation of rights:**
*   Read (r): only read access to existing thermal properties.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYKG is a global user right.

### KYKM

**Designation:** edge calculation of shapes

**Menu:** access right for menu Master Data > Keys > System > Shapes > Edge Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to existing shape edge allocation.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYKM is a global user right.

### ΚΥΚΡ

**Designation:** customer products

**Menu:** access right for menu Master Data > Keys > Products > Customer Products.

**Possible allocation of rights:**
*   Read (r): only read access to existing customer products.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYKP is a global user right.

### KYKS

**Designation:** right for box signature

**Menu:** access right for menu Master Data > Keys > Products > Box Signature.

**Possible allocation of rights:**
*   Read (r): only read access to existing box signature.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYKS is a global user right. The box signature is a customer-specific development and must be configured separately.

### KYLD

**Designation:** country code

**Menu:** access right for menu Master Data > Keys > Market Partner > Countries.

**Possible allocation of rights:**
*   Read (r): only read access to existing countries.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYLD is a global user right.

### ΚΥΜΑ

**Designation:** clients

**Menu:** access right for menu Master Data > Keys > Market Partner > FinAc Clients.

**Possible allocation of rights:**
*   Read (r): only read access to existing FinAc clients.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYMA is a global user right.

### KYME

**Designation:** quantity unit code

**Menu:** access right for menu Master Data > Keys > System > Quantity Units.

**Possible allocation of rights:**
*   Read (r): only read access to existing quantity units.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYME is a global user right.

### KYMW

**Designation:** VAT code

**Menu:** access right for menu Master Data > Keys > System > Taxes > Tax Rates.

**Possible allocation of rights:**
*   Read (r): only read access to existing tax rates.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYMW is a global user right.

### ΚΥΡΑ

**Designation:** parameter description for technical values.

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Parameter Description.

**Possible allocation of rights:**
*   Read (r): only read access to existing parameter description for technical values.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYPA is a global user right.

### KYPB

**Designation:** production sections
**Description:** access authorization KYPB is not supported anymore.

### KYPE

**Designation:** periodic deferring

**Menu:** access right for menu Master Data > Keys > System > End of Period.

**Possible allocation of rights:**
*   Read (r): only read access to existing periods.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYPE is a global user right.

### KYPK

**Designation:** price list code

**Menu:** access right for menu Master Data > Keys > Prices > Price Lists (PLCD).

**Possible allocation of rights:**
*   Read (r): only read access to existing price lists.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYPK is a global user right.

### KYPL

**Designation:** ZIP code

**Menu:** access right for menu Master Data > Keys > System > ZIP Codes.

**Possible allocation of rights:**
*   Read (r): only read access to existing ZIP codes.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYPL is a global user right.

### ΚΥΡΟ

**Designation:** item key

**Menu:** access right for menu Master Data > Keys > System > Item Key.

**Possible allocation of rights:**
*   Read (r): only read access to existing item keys.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYPO is a global user right.

### KYPV

**Designation:** commission code

**Menu:** access right for menu Master Data > Commissions > Commission Code.

**Possible allocation of rights:**
*   Read (r): only read access to existing commission codes.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYPV is a global user right.

### KYPZ

**Description:** PMO rack packing allocation

**Menu:** access right for menu Master Data > Keys > System > PMO > Rack Packing Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to existing rack packing allocations.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above. This function is described in AWDesk case #233929.

**Dependencies:** none.

**Multi-site capability:** module code KYPZ is a global user right.

### KYQU

**Designation:** quality key

**Menu:** access right for menu Master Data > Keys > Market Partner > Quality Scales.

**Possible allocation of rights:**
*   Read (r): only read access to existing quality keys.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYQU is a global user right.

### KYRA

**Designation:** right for complaint method

**Menu:** access right for menu Master Data > Keys > Market Partner > Complaint > Reasons.

**Possible allocation of rights:**
*   Read (r): only read access to existing complaint reasons.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYRA is a global user right.

### KYRE

**Description:** Areas

**Menu:** access right for menu Master Data > Keys > Market Partner > Area/Countries.

**Possible allocation of rights:**
*   Read (r): only read access to existing regions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYRE is a global user right.

### KYRO

**Designation:** right for place of complaint

**Menu:** access right for menu Master Data > Keys > Market Partner > Complaint > Places.

**Possible allocation of rights:**
*   Read (r): only read access to existing complaint places.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYRO is a global user right.

### KYRS

**Designation:** right for complaint type

**Menu:** access right for menu Master Data > Keys > Market Partner > Complaint > Types.

**Possible allocation of rights:**
*   Read (r): only read access to existing complaint types.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYRS is a global user right.

### KYRT

**Description:** routes

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Routes > Routes.

**Possible allocation of rights:**
*   Read (r): only read access to existing routes.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYRT is a global user right.

### KYSD

**Description:** stack - master data

**Menu:** access right for menu Master Data > Keys > Products > Stack.

**Possible allocation of rights:**
*   Read (r): only read access to existing data in section stacks.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYSD is a global user right.

### KYSK

**Description:** discount - keys

**Menu:** access right for menu Master Data > Keys > System > Cash Discount Groups.

**Possible allocation of rights:**
*   Read (r): only read access to existing discount groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYSK is a global user right.

### KYSN

**Description:** Shaping / Nesting key allocation

**Menu:** access right for menu Master Data > Keys > Products > Shaping/Nesting Product.

**Possible allocation of rights:**
*   Read (r): only read access to existing SN article allocation.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYSN is a global user right.

### KYSP

**Description:** language key

**Menu:** access right for menu Master Data > Keys > System > Languages.

**Possible allocation of rights:**
*   Read (r): only read access to existing language data records.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYSP is a global user right.

### KYST

**Description:** tax type keys

**Menu:** access right for menu Master Data > Keys > System > Taxes > Tax Types.

**Possible allocation of rights:**
*   Read (r): only read access to existing tax types.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYST is a global user right.

### KYTG

**Description:** t-groups

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Groups > Transmission.

**Possible allocation of rights:**
*   Read (r): only read access to existing transmission groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYTG is a global user right.

### KYTR

**Description:** routes

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Routes > Route Plan.

**Possible allocation of rights:**
*   Read (r): only read access to existing route plans.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYTR is a global user right.

### KYTW

**Description:** technical values

**Menu:** access right for menu Master Data > Keys > Products > Technical Data > Groups > Thickness.

**Possible allocation of rights:**
*   Read (r): only read access to existing thicknesses in order to calculate technical values.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYTW is a global user right.

### KYTX

**Description:** allocation of master texts
**Description:** access authorization KYTX is not supported anymore.

### KYVA

**Description:** allocation of variants

**Menu:** access right for menu Master Data > Keys > Products > Variants > Sizes.

**Possible allocation of rights:**
*   Read (r): only read access to existing size variants.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYVA is a global user right.

### KYVE

**Description:** price vector code

**Menu:** access right for menu Master Data > Keys > Prices > Article Vectors.

**Possible allocation of rights:**
*   Read (r): only read access to existing article price vectors.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYVE is a global user right.

### KYVG

**Description:** dispatch groups

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Dispatch Groups.

**Possible allocation of rights:**
*   Read (r): only read access to existing dispatch groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYVG is a global user right.

### KYVL

**Description:** rack status

**Menu:** access right for menu Master Data > Keys > System > Rack Status.

**Possible allocation of rights:**
*   Read (r): only read access to existing rack status.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYVL is a global user right.

### KYVM

**Description:** PMO packing methods

**Menu:** access right for menu Master Data > Keys > System > PMO > Packing Methods.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above. See also AWDesk case #233929

**Dependencies:** none.

**Multi-site capability:** module code KYVM is a global user right.

### KYVP

**Description:** packing type code

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Packing Type.

**Possible allocation of rights:**
*   Read (r): only read access to existing packing types.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYVR is a global user right.

### KYVS

**Description:** dispatch type code

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Dispatch Type.

**Possible allocation of rights:**
*   Read (r): only read access to existing dispatch types.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYVS is a global user right.

### KYWR

**Description:** currency code

**Menu:** access right for menu Master Data > Keys > System > Currency.

**Possible allocation of rights:**
*   Read (r): only read access to existing currencies.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** the number of currencies in the system must be configured.

**Multi-site capability:** module code KYWR is a global user right.

### KYWT

**Description:** economic area code

**Menu:** access right for menu Master Data > Keys > Market Partner > Economic Areas.

**Possible allocation of rights:**
*   Read (r): only read access to existing economic areas.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code KYWT is a global user right.

### KYZM

**Description:** payment type code

**Menu:** access right for menu Master Data > Keys > System > Payment Type.

**Possible allocation of rights:**
*   Read (r): only read access to existing payment terms.
*   Read and write (w): full access.

**Description:** the module code controls access to the mentioned dialogs.

**Dependencies:** none.

**Multi-site capability:** module code KYZM is a global user right.

### KYZP

**Designation:** right for customs documents

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Customs Exit and Destin. Customs.

**Possible allocation of rights:**
*   Read (r): only read access to existing customs data.
*   Read and write (w): full access.

**Description:** the module code controls access to the mentioned dialogs.

**Dependencies:** none.

**Multi-site capability:** module code KYZP is a global user right.

### KYZT

**Description:** text additions

**Menu:** access right for menu Master Data > Keys > System > Technical Data > Text Additions.

**Possible allocation of rights:**
*   Read (r): only read access to existing text additions.
*   Read and write (w): full access.

**Description:** the module code controls access to the mentioned dialogs.

**Dependencies:** none.

**Multi-site capability:** module code KYZT is a global user right.

## 14. Stock management

Below you will find the individual rights for section Stock management.
**All modules of section LA* are client-specific user rights. That means, access rights can be valuated per individual client.**

### LA*

**Description:** stock management programs

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Stock Management.

**Dependencies:** none.

**Multi-site capability:** all module authorizations in section LA* can be maintained and evaluated client-specific.

### LAAA

**Description:** outgoing stocks (order-related)

**Menu:** access right for menu Stock > Booking > Outg. Stock (Order-Rel.).

**Possible allocation of rights:**
*   Read (r): has no effect at this point (booking not possible)
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAAA can be maintained and evaluated client-specific.

### LAAG

**Description:** stock out

**Menu:** access right for menu Stock > Booking > Warehouse Out.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (booking not possible)
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAAG can be maintained and evaluated client-specific.

### LAAS

**Description:** cancel order in dispatch

**Menu:** access right for menu Dispatch Control > Order Level > >Shift + F4> Cancel Order.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (cancel not possible)
*   Read and write (w): full access

**Description:** the module code controls the possibility to use the function mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAAS can be maintained and evaluated client-specific.

### LABK

**Description:** correction of erroneous bookings

**Menu:** access right for menu Stock > Info System > Booking Status.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (booking not possible)
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LABK can be maintained and evaluated client-specific.

### LABW

**Description:** stock valuation

**Menu:** access right for menu Stock > Evaluation.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LABW can be maintained and evaluated client-specific.

### LAEG

**Description:** stock receipt

**Menu:** access right for menu Stock > Booking > Warehouse In.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (booking not possible)
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAEG can be maintained and evaluated client-specific.

### LAFI

**Description:** stock inventory of finished goods

**Menu:** access right for menu Logistics > Dispatch Control > `<Shift + F4>` > Stock Inventory of Finished Goods.

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode.

**Description:** the module code controls access to the dialog. The function must be configured separately.

**Dependencies:** none.

**Multi-site capability:** module authorization LAFI can be maintained and evaluated client-specific.

### LAHB

**Description:** stock background booking unit

**Menu:** system authorization for stock booker.

**Possible allocation of rights:**
User-dependent allocation of rights has no effect, here. The authorization LAHB will only be checked internally.

**Description:** the authorization is used internally.

**Dependencies:** none.

**Multi-site capability:** module authorization LAHB shall not be maintained client-specific.

### LAIA

**Description:** stock info system articles

**Menu:** access right for menu Stock > Info System > Article.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAIA can be maintained and evaluated client-specific.

### LAIB

**Description:** stock info system sheet

**Menu:** access right for menu Stock > Info System > Lites.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAIB can be maintained and evaluated client-specific.

### LAID

**Description:** stock info system orders/purchase order

**Menu:** access right for menu Stock > Info System > Orders/Purchase Orders.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAID can be maintained and evaluated client-specific.

### LAIF

**Description:** stock info system

**Menu:** access right for menu Stock > Info System > Slot.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAIF can be maintained and evaluated client-specific.

### LAIP

**Description:** stock info system log

**Menu:** access right for menu Stock > Info System > History.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAIP can be maintained and evaluated client-specific.

### LAIS

**Description:** stock info system stack

**Menu:** access right for menu Stock > Info System > Stack.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAIS can be maintained and evaluated client-specific.

### LAIV

**Description:** stock inventory

**Menu:** access right for menu Stock > Inventory.

**Possible allocation of rights:**
*   Read (r): only read access to existing inventory data.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAIV can be maintained and evaluated client-specific.

### LAES

**Description:** Create backup of stock

**Menu:** access right for menu Stock > System > Stock backup.

**Possible allocation of rights:**
*   Read (r): only read access to view the existing backup times.
*   Read and write (w): full access. You can execute backup of stock tables wlx, wlxv, wlxifo, wlfach, wlgest

**Description:** the module code controls access to the dialog mentioned above. With writing access you can execute the backup manually

**Dependencies:** WL_ARCHIV_DAUER, WL_ARCHIV_TAG.

**Multi-site capability:** module authorization LAES can be maintained and evaluated client-specific.

### LAKD

**Description:** print box labels

**Menu:** access right for menu Stock > Print > Labels.

**Possible allocation of rights:**
*   Read (r): only read access to existing print records.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAKD can be maintained and evaluated client-specific.

### LAKO

**Description:** stock correction.

**Menu:** access right for menu Stock > Booking > Correction.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (booking not possible)
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAKO can be maintained and evaluated client-specific.

### LALS

**Description:** delivery note cancellation in dispatch

**Menu:** access right for menu Dispatch > `<Shift + F4>` > Cancel > Cancel Delivery Note.

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode.

**Description:** the module code controls access to cancel delivery notes system-wide.

**Dependencies:** none.

**Multi-site capability:** module authorization LALS can be maintained and evaluated client-specific.

### LAMG

**Description:** manual rack management in dispatch

**Menu:** none.

**Possible allocation of rights:**
*   Read (r): only read access to existing racks.
*   Read and write (w): full access.

**Description:** the module code controls use of rack management in dispatch.

**Dependencies:** rack management must be configured separately.

**Multi-site capability:** module authorization LAMG can be maintained and evaluated client-specific.

### LANA

**Description:** stock new creation

**Menu:** access right for menu Stock > Master Data > Storeroom.

**Possible allocation of rights:**
*   Read (r): only read access to existing warehouses.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LANA can be maintained and evaluated client-specific.

### LAPG

**Description:** stock info system forecast

**Menu:** access right for menu Stock > Info System > Forecast.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAPG can be maintained and evaluated client-specific.

### LAPL

**Description:** delete stock history

**Menu:** access right for menu Stock > System > Delete Stock History.

**Possible allocation of rights:**
*   Read (r): has the same effect as full access at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAPL can be maintained and evaluated client-specific.

### LAPV

**Description:** stock info system available stock for variants

**Menu:** access right for menu Stock > Info System > Available Stock.

**Possible allocation of rights:**
*   Read (r): has the same effect as full access at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAPV can be maintained and evaluated client-specific.

### LASB

**Description:** stack booking

**Menu:** access right for menu Stock > Booking > Stack Booking (Doc.-Related).

**Possible allocation of rights:**
*   Read (r): has the same effect as ` ,- , ` right (booking is not possible).
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** this function is customer-specific.

**Multi-site capability:** module authorization LASB can be maintained and evaluated client-specific.

### LASD

**Description:** stock master data

**Menu:** access right for menu Stock > Master Data > Article.

**Possible allocation of rights:**
*   Read (r): only read access to existing article master.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LASD can be maintained and evaluated client-specific.

### LASU

**Description:** dispatch control overview dialog

**Menu:** Menu Dispatch Control – Overview contains the search logic of a Sulo (see explanation of terms). The menu can be opened on route level and also on item level via `<Shift + F4>` > Overview. If the dispatch control is configured in the stack logic, the Dispatch Control - Overview is also called via `<Shift +F 4>` > Overview.

**Possible allocation of rights:**
With this module code, it only makes sense to assign read access, since the dialog is only an overview
The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to menu Overview in module Dispatch Control.

**Dependencies:** none.

**Multi-site capability:** module authorization LASU can be maintained and evaluated client-specific.

### LASV

**Description:** stack management

**Menu:** access right for menu Stock > Booking > Stack Management.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** this function is customer-specific.

**Multi-site capability:** module authorization LASV can be maintained and evaluated client-specific.

### LATD

**Description:** Dispatch: Permit transport bookings in past and future

**Menu:** access right for menu Dispatch Control > Route Level / Order Level > `<F4>` > Book to Transport.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above. Booking to transport is only possible, if the item was booked as completely finished.

**Dependencies:** none.

**Multi-site capability:** module authorization LATD can be maintained and evaluated client-specific.

### LAVA

**Description:** stock info system variant

**Menu:** access right for menu Stock > Info System > Variant.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization LAVA can be maintained and evaluated client-specific.

### LAVD

**Description:** dispatch: permit past 'packed' bookings

**Menu:** none.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to function.

**Dependencies:** none.

**Multi-site capability:** module authorization LAVD can be maintained and evaluated client-specific.

### LAVS

**Description:** dispatch control (loading list pool)

**Menu:** access right for menu Dispatch Control > Order Level > `<F4>`.

**Possible allocation of rights:**
*   Read (r): only conditionally usable at this point.
*   Read and write (w): full access.

**Description:** -/- .

**Dependencies:** working with loading pool is controlled via environment variable LAPOOL_LADEFOLGE.

**Multi-site capability:** module authorization LAVS can be maintained and evaluated client-specific.

## 15. Matrix processing

Below you will find the right for Matrix processing.
**All modules of group MA* are global authorizations That means, the access rights cannot be evaluated for each individual client.**

### MA*

**Description:** matrix processing

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:** this module section controls the user rights of Matrix Processing.

**Dependencies:** none.

**Multi-site capability:** module code MA* is a global user right.

### MABE

**Description:** matrix calculation

**Menu:** access right for menu Master Data > Prices > IG Prices > Matrix Calculation

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code MABE is a global user right.

## 16. Marketing Module

Below you will find the individual rights for section Marketing module.
**Marketing module is not supported anymore. The description here is of February 1st, 2012.**

### MK*

**Description:** matrix modules

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Marketing Module.

**Dependencies:** none.

### MKKI

**Description:** customer information system

**Menu:** access right for menu or menu section

**Possible allocation of rights:**
*   Read (r):
*   Read and write (w):

**Description:** -/- .

**Dependencies:** use of this function is controlled via environment variable.

## 17. Market partner

Below you will find the individual rights for section Market partner.
**All modules of group MP* are global authorizations That means, the access rights cannot be evaluated for each individual client. The individual deviations are listed in the following table.**

### MP*

**Description:** market partner

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Market Partners.

**Dependencies:** none.

**Multi-site capability:** all modules of group MP* are global authorizations. That means, the access rights cannot be evaluated for each individual client.

### MPAD

**Description:** address allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Contact Data > Addresses

**Possible allocation of rights:**
*   Read (r): only read access to existing addresses.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPAD is a global user right.

### MPAP

**Description:** contact person

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Contact Data > Contact

**Possible allocation of rights:**
*   Read (r): only read access to existing addresses.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPAP is a global user right.

### MPAR

**Description:** market partner - product allocation.

**Menu:** access right for menu Market Partner > `<F4>` > Product Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to existing addresses.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPAR is a global user right.

### MPAV

**Description:** address logic: dispatch and purchase

**Menu:**
*   access right for menu Dispatch Control > Order Level > `<F4>` > Delivery Address > New Delivery Address
*   Purchase > Create Purchase Orders > Field Supplier > `<F5>` Addresses.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access (allows entry of a new delivery address)

**Description:** the module code controls access to the dialogs and functions mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code MPAV is a global user right.

### MPAZ

**Designation:** right for E/A rules

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Exchange/Additional Rules

**Possible allocation of rights:**
*   Read (r): only read access to existing market-specific exchange/additional rules.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPAZ is a global user right.

### MPBA

**Description:** Base

**Menu:** access right for menu Master Data > Field Configuration > MP-Field Configuration.

**Possible allocation of rights:**
*   Read (r): only read access to existing MP field configuration records.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code MPBA is a global user right.

### MPBV

**Description:** bank account

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Contact Data > Bank Accounts.

**Possible allocation of rights:**
*   Read (r): only read access to existing bank accounts.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPBV is a global user right.

### MPDE

**Description:** delete - delete market partner

**Menu:** function right for menu Master Data > Market Partner > `<F6>`.

**Possible allocation of rights:**
Write permission can be assigned. The user has the right to delete and reactivate market partners that have been created or closed down.

**Description:** the module codes gives employees who have write authorization ('w') for this module permission to delete and reactivate market partners. If an employee does not have this authorization, he or she receives the message "Attention: no authorization to delete/reactivate MP." and is rejected.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPDE is a global user right.

### MPEZ

**Description:** author allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Staff Allocations > User Allocation

**Possible allocation of rights:**
*   Read (r): only read access to allocated user.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPEZ is a global user right.

### MPFD

**Description:** forms

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Text/Print > Forms.

**Possible allocation of rights:**
*   Read (r): only read access to existing
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPFD is a global user right.

### MPGE

**Description:** customer - rack allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Rack Types.

**Possible allocation of rights:**
*   Read (r): only read access to allocated racks.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPGE is a global user right.

### MPGZ

**Description:** market partner: group allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Group Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to allocated groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPGZ is a global user right.

### MPKA

**Description:** customer article texts

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Text/Print > MP Texts.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPKA is a global user right.

### MPLV

**Description:** market partner: limit distribution

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Replication Data.

**Possible allocation of rights:**
*   Read (r): only read access to existing replication data.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPLV is a global user right.

### MPOZ

**Description:** object allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Contract Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to allocated projects.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPOZ is a global user right.

### MPPR

**Description:** MP project

**Menu:** access right for menu Master Data > Market Partner > Customized.

**Possible allocation of rights:**
*   Read (r): only display access to special tabs in market partner master.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** this is a customer-specific function, that must be configured separately.

**Multi-site capability:** module code MPPR is a global user right.

### MPST

**Designation:** master dat

**Menu:** access right for menu Master Data > Market Partner.

**Possible allocation of rights:**
*   Read (r): see description.
*   Read and write (w): see description.

**Description:** access authorization for market partner module MPST is always valid in connection with the permission for the corresponding market partner type:
*   STKU for customers and others and
*   STLI for suppliers.

**Example:** if an employee shall not have read and change rights in the customer master, the rights MPST and STKU must be withdrawn.

**Note:** there is no way to control employee authorization separately for market partner type=object.

**Dependencies:**
MPST authorization depends also on the STKU/STLI authorizations.

**Multi-site capability:** module codes MPST/STKU/STLI involve global user rights.

### MPSV

**Designation:** contact person sales

**Menu:** access right for menu Sales > Order Entry, Order header -> tab Properties, field Ordered from `<F5>` Contacts.

**Possible allocation of rights:**
*   Read (r): only read access to contact persons of customers, allocated in the market partner master.
*   Read and write (w): full access.

**Description:** the module code serves to define a new contact person of the customer directly in the order. `<F5>` starts a dialog to enter the data of the contact person. With read and write permission you can enter a new contact person with `<F6>`. This will be saved in the customer master.

**Dependencies:** dialog access also depends on the access rights of order entry.

**Multi-site capability:** module code MPSV is a global user right.

### MPVZ

**Designation:** representative allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Staff Allocations > Representative Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to allocated representatives.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** dialog access also depends on the MPST authorizations, among other things.

**Multi-site capability:** module code MPVZ is a global user right.

### MPWA

**Designation:** A+W Enterprise Web: address entry
**Description:** MPWA authorization is no longer queried by the program.

## 18. Object management

Below you will find the individual rights for section Project management.
**All modules of group RE* are global authorizations That means, the access rights cannot be evaluated for each individual client.**
*(Note: OCR incorrectly states RE*, but context implies OB*)*

### OB*

**Designation:** object management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Project Management.

**Dependencies:** none.

**Multi-site capability:** all modules of group OB* are global authorizations. That means, the access rights cannot be evaluated for each individual client.

### OBAD

**Designation:** object addresses
**Description:** access authorization OBAD is not supported anymore.

### ОВАР

**Designation:** object - article prices
**Description:** access authorization OBAP is not supported anymore.

### OBAR

**Designation:** object - article conditions
**Description:** access authorization OBAR is not supported anymore.

### OBAZ

**Designation:** object - exchange rules
**Description:** access authorization OBAZ is not supported anymore.

### OBBD

**Designation:** object - transaction data

**Menu:** access right for menu Sales > Distribution > Contract Budgeting > Manual Booking.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code OBBD is a global user right.

### OBEK

**Designation:** object - purchasing conditions
**Description:** access authorization OBEK is not supported anymore.

### OBIV

**Designation:** object-specific glazing prices Prices

**Menu:** access right for menu Master Data > Prices > Price Control > Glass Bal. Object Prices

**Possible allocation of rights:**
*   Read (r): only read access to existing project-specific glass balancing prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** this function is customer-specific.

**Multi-site capability:** module code OBIV is a global user right.

### ОВКО

**Designation:** object account

**Menu:** access right for menu Sales > Distribution > Project Budgeting > Project Accounts.

**Possible allocation of rights:**
*   Read (r): only read access to existing project accounts.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable OBJEKTVERWALTUNG.

**Multi-site capability:** module code OBKO is a global user right.

### OBLO

**Designation:** maintenance of labor type factors

**Menu:** access right for menu Sales > Distribution > Project Budgeting > Payroll Accounting > Labor Type Factors.

**Possible allocation of rights:**
*   Read (r): only read access to existing wage type factors.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is customer-specific and controlled via environment variables MP_PROJECT and MMS_SPECIAL.

**Multi-site capability:** module code OBLO is a global user right.

### OBOT

**Designation:** semi-finished objects

**Menu:** access right for menu Sales > Distribution > Project Budgeting > Invoiced Projects.

**Possible allocation of rights:**
*   Read (r): only read access to the list that contains all invoiced projects.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is customer-specific and controlled via environment variables MP_PROJECT and MMS_SPECIAL.

**Multi-site capability:** module code OBOT is a global user right.

### OBSC

**Designation:** internal invoicing
**Description:** access authorization OBSC is not supported anymore.

### OBSP

**Designation:** object-specific process./muntins/access. prices
**Description:** access authorization OBSP is not supported anymore.

### OBVK

**Designation:** object-customers SA conditions
**Description:** access authorization OBVK is not supported anymore.

### OBWG

**Designation:** object - product group conditions
**Description:** access authorization OBWG is not supported anymore.

### OBZU

**Designation:** market partner allocation

**Menu:** Master Data > Text Management > Contract Texts

**Possible allocation of rights:** for this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code OBZU is a global user right.

## 19. PMS

Below you will find the individual rights for section PMS.
**Barcode module is not supported anymore. The description here is of February 1st, 2012.**

### PM*

**Designation:** PMS main module

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of PMS.

**Dependencies:** none.

### PMAH

**Designation:** general main menu
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMAL

**Designation:** general lock mechanisms
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMAM

**Designation:** general message supervision
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMAN

**Designation:** general number ranges
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMAW

**Designation:** general value entry
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMDB

**Designation:** print calls in stack
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMED

**Designation:** accumulated daily capacities
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMEG

**Designation:** loading: global re-scheduling
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMEK

**Designation:** accumulated weekly capacities
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMEU

**Designation:** loading: re-schedule order
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFA

**Designation:** set of jobs
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFB

**Designation:** detailed scheduling: breakage report
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFE

**Designation:** detailed scheduling: edit data
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFF

**Designation:** detailed scheduling: release job
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFG

**Designation:** dispatch rack planning
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFJ

**Designation:** detailed scheduling: create job
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFL

**Designation:** detailed scheduling: view job
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFM

**Designation:** ready report
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFP

**Designation:** detailed scheduling: print documents
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFR

**Designation:** detailed scheduling: reset job
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMFU

**Designation:** detailed scheduling: sub-selection logical PF
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMGB

**Designation:** rough scheduling: breakage overview
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIA

**Designation:** information system: order result
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIB

**Designation:** PMS information system: rack display
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIE

**Designation:** information system: entered orders
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIF

**Designation:** information system: detailed scheduling
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIK

**Designation:** PMS information system: orders with critical sheets
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIM

**Designation:** information system: screens
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIP

**Designation:** PMS information system: planning results
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMIQ

**Designation:** information system: direct import of data
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMPA

**Designation:** archive work plan
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMPD

**Designation:** delete work plan
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMPE

**Designation:** edit work plan
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMPK

**Designation:** PMS fond editor (manipulate capacities)
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMPL

**Designation:** read work plan
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMPM

**Designation:** create work plan
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSA

**Designation:** master data - working-process-classes
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSB

**Designation:** master data - production facilities
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSC

**Designation:** master data - processing sequence
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSD

**Designation:** master data - print calls
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSF

**Designation:** master data - detailed scheduling
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSK

**Designation:** master data - critical sheets
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSO

**Designation:** master data - optimization
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSP

**Designation:** master data - personnel planning
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSR

**Designation:** master data - restrictions
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMST

**Designation:** master data - text generation
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMSZ

**Designation:** master data - time management
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMTB

**Designation:** master data (internal) production facilities
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMXA

**Designation:** quotation optimization
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMXV

**Designation:** XOPTS - forward interface
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMYB

**Designation:** statistics: breakage statistics
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMYC

**Designation:** statistics: charge tracking
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

### PMYO

**Designation:** PMS statistics: optimization, waste
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** none.

## 20. Prices

Below you will find the individual rights for section Prices.
**All modules of group PS* are global authorizations That means, the access rights cannot be evaluated for each individual client.**

### PS*

**Designation:** price maintenance programs

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:** this module section controls the user rights of Price Maintenance.

**Dependencies:** none.

**Multi-site capability:** all modules of section PS* are client-specific user rights.

### PSAG

**Designation:** patterned exchange prices

**Menu:** access right for menu Master Data > Prices > IG Prices > Pattern Exchange.

**Possible allocation of rights:**
*   Read (r): only read access to existing pattern glass exchange prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSAG is a global user right.

### PSAP

**Designation:** exchange prices for IGU and LAMI

**Menu:** access right for menu Master Data > Prices > IG Prices > Exchange TGH/LAMI/SPECIAL.

**Possible allocation of rights:**
*   Read (r): only read access to existing IG exchange prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSAP is a global user right.

### PSAV

**Designation:** LAMI exchange prices

**Menu:** access right for menu Master Data > Prices > IG Prices > Exchange TGH/LAMI/SPECIAL.

**Possible allocation of rights:**
*   Read (r): only read access to existing IG exchange prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSAV is a global user right.

### PSBM

**Designation:** processing matrix

**Menu:** access right for menu Master Data > Prices > PCD Prices > Matrix Assignment.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSBM is a global user right.

### PSBR

**Designation:** breakage clearing

**Menu:** access right for menu Master Data > Prices > Price Control > Rejects Factors.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization PSBR can be maintained and evaluated client-specific.

### PSBU

**Designation:** global PCD processing price maintenance

**Menu:** access right for menu Master Data > Prices > PCD Prices > Processing Vectors and Master Data > Prices > PCD Prices > Colored Articles > `<F4>`.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSBU is a global user right.

### PSBV

**Designation:** processing vectors

**Menu:** access right for menu Master Data > Prices > PCD Prices > Processing Vectors and Spec. Processing Vectors.

**Possible allocation of rights:**
*   Read (r): only read access to existing processing vectors.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSBV is a global user right.

### PSBW

**Designation:** minimum processing prices

**Menu:** access right for menu Master Data > Prices > PCD Prices > Minimum Processing Prices.

**Possible allocation of rights:**
*   Read (r): only read access to existing minimum processing prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSBW is a global user right.

### PSBZ

**Designation:** processing surcharge vectors

**Menu:** access right for menu Master Data > Prices > Surcharges > Thickness Surcharge Vectors or Master Data > Prices > PCD Prices > Vector Assignment.

**Possible allocation of rights:**
*   Read (r): only read access to existing data records of dialog mentioned above.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSBZ is a global user right.

### PSFF

**Designation:** save prices in file formats

**Menu:** access right for menu Master Data > Prices > Price Import > External Formats.

**Possible allocation of rights:**
*   Read (r): has no effect at this point, i.e. you can open the dialog but each entry is impossible.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSFF is a global user right.

### PSGA

**Designation:** patterned glass categories

**Menu:** access right for menu Master Data > Prices > IG Prices > Pattern Classes.

**Possible allocation of rights:**
*   Read (r): only read access to existing patterned glass categories.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSGA is a global user right.

### PSGZ

**Designation:** size surcharges.

**Menu:** access right for menu Master Data > Prices > Surcharges > Size Surcharges.

**Possible allocation of rights:**
*   Read (r): only read access to existing size surcharges.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSGZ is a global user right.

### PSIE

**Designation:** IG single sheet prices.

**Menu:** access right for menu Master Data > Prices > IG Prices > Single Lites.

**Possible allocation of rights:**
*   Read (r): only read access to existing IG single lite prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSIE is a global user right.

### PSIF

**Designation:** factor conversion SA-PU

**Menu:** access right for menu Master Data > Prices > Price Control > Rules: SA-PU Factor.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSIF is a global user right.

### PSIS

**Designation:** price calculation IG

**Menu:** access right for menu Master Data > Prices > IG Prices > Basic Prices and Master Data > Conditions > Special Prices > IG Basic Prices.

**Possible allocation of rights:**
*   Read (r): only read access to existing IG basic prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSIS is a global user right.

### PSKZ

**Designation:** PCD prices

**Menu:** access right for menu Master Data > Prices > PCD Prices > All Vector Assignments and Master Data > Prices > PCD Prices > Spec. Vector Assignments.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSKZ is a global user right.

### PSLI

**Designation:** price list restrictions

**Menu:** access right for menu Master Data > Prices > Price Control > Price List Control.

**Possible allocation of rights:**
*   Read (r): only read access to existing data records of price list restrictions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSLI is a global user right.

### PSLS

**Designation:** price list control.

**Menu:** access right for menu Master Data > Prices > Price Control > Price Control.

**Possible allocation of rights:**
*   Read (r): only read access to existing data records of price list control.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSLS is a global user right.

### PSMA

**Designation:** take over matrix

**Menu:** access right for function „Import Matrix" in matrix editor.

**Possible allocation of rights:**
*   Read (r): has no effect at this point, i.e. you can open the dialog but each activity is impossible.
*   Read and write (w): full access.

**Description:** the module code controls access to use function (`<F5>`).

**Dependencies:** access PSMA also depends on right „PSME“.

**Multi-site capability:** module code PSMA is a global user right.

### PSMB

**Designation:** manual booking
**Description:** access authorization PSMB is not supported anymore.

### PSME

**Designation:** matrix editor

**Menu:** access right for menu Master Data > Prices > IG Prices > Matrix Editor.

**Possible allocation of rights:**
*   Read (r): only read access to existing price matrices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSME is a global user right.

### PSMG

**Designation:** lines-, columns limit values for matrices

**Menu:** access right for function „Matrix Limits" in matrix editor.

**Possible allocation of rights:**
*   Read (r): has no effect at this point, i.e. full access.
*   Read and write (w): full access.

**Description:** the module code controls access to use function (`<Shift + F11>`).

**Dependencies:** access PSMG also depends on right „PSME“.

**Multi-site capability:** module code PSMG is a global user right.

### PSMP

**Designation:** PCD shape surcharges

**Menu:** access right for menu Master Data > Prices > Surcharges > Shape Surcharges and Spec. Shape Surcharges.

**Possible allocation of rights:**
*   Read (r): only read access to existing shape surcharges.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSMP is a global user right.

### PSMU

**Designation:** global PCD shape surcharge maintenance

**Menu:** access right for function „Global Price Maintenance" in shape surcharges.

**Possible allocation of rights:**
*   Read (r): has no effect at this point, i.e. you can open the dialog but each activity is impossible.
*   Read and write (w): full access.

**Description:** the module code controls access to use function (`<F4>`).

**Dependencies:** access PSMU also depends on right „PSMP“.

**Multi-site capability:** module code PSMU is a global user right.

### PSPF

**Designation:** PCD color depending prices

**Menu:** access right for menu Master Data > Prices > PCD Prices > Colored Articles.

**Possible allocation of rights:**
*   Read (r): only read access to existing prices of colored articles.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSPF is a global user right.

### PSPR

**Designation:** PCD reference table

**Menu:** access right for menu Master Data > Keys > Prices > Price Lists.

**Possible allocation of rights:**
*   Read (r): only read access to existing price list references.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSPR is a global user right.

### PSPS

**Designation:** general price control

**Menu:** access right for menu Master Data > Prices > Price Control > Price Control.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSPS is a global user right.

### PSPU

**Designation:** global PCD price maintenance

**Menu:** access right for menu Master Data > Prices > Price Keys > Price Code.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none

**Multi-site capability:** module code PSPU is a global user right.

### PSPV

**Designation:** price vectors

**Menu:** access right for menu Master Data > Prices > PCD Prices > All and Spec. Article Price Vectors, All and Spec. Processing Vectors.

**Possible allocation of rights:**
*   Read (r): only read access to existing price vectors.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSPV is a global user right.

### PSSE

**Designation:** price maintenance muntin factors PU
**Description:** access authorization PSSE is not supported anymore.

### PSSF

**Designation:** muntin price maintenance

**Menu:** access right for menu Master Data > Prices > Muntin Prices > Muntin Price Classes.

**Possible allocation of rights:**
*   Read (r): only read access to existing muntin price categories.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSSF is a global user right.

### PSSL

**Designation:** muntins price code

**Menu:** access right for menu Master Data > Keys > Prices > Muntin Price Code.

**Possible allocation of rights:**
*   Read (r): only read access to existing muntin price codes.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSSL is a global user right.

### PSSP

**Designation:** allocation muntin price category - muntins PCD
**Description:** access authorization PSSP is not supported anymore.

### PSSZ

**Designation:** AIR surcharges

**Menu:** access right for menu Master Data > Prices > IG Prices > AIR Surcharges.

**Possible allocation of rights:**
*   Read (r): only read access to existing AIR surcharges.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSSZ is a global user right.

### PSTZ

**Designation:** steps - surcharges

**Menu:** access right for menu Master Data > Prices > Surcharges > Offset Surcharge Vectors.

**Possible allocation of rights:**
*   Read (r): only read access to existing offset surcharges.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** maintenance and use of steps may only be configured in consultation with the development department.

**Multi-site capability:** module code PSTZ is a global user right.

### PSUV

**Designation:** prices UV protections

**Menu:** access right for menu Master Data > Prices > IG Prices > UV Protection.

**Possible allocation of rights:**
*   Read (r): only read access to existing UV protection prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSUV is a global user right.

### PSVA

**Designation:** price maintenance for variant prices

**Menu:** access right for menu Master Data > Prices > PCD Prices > Variant Prices and Special Variant Prices.

**Possible allocation of rights:**
*   Read (r): only read access to existing variant prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSVA is a global user right.

### PSVL

**Designation:** PCD glazing

**Menu:** access right for menu Master Data > Prices > PCD Prices > Glazing.

**Possible allocation of rights:**
*   Read (r): only read access to existing PCD glazing prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSVL is a global user right.

### PSVS

**Designation:** PCD LAMI basic prices

**Menu:** access right for menu Master Data > Prices > PCD Prices > LAMI Articles > LAMI Basic Prices and Special LAMI Basic Prices.

**Possible allocation of rights:**
*   Read (r): only read access to existing LAMI basic prices.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSVS is a global user right.

### PSZM

**Designation:** surcharge matrix

**Menu:** access right for menu Master Data > Prices > Surcharges > Surcharge Matrices.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSZM is a global user right.

### PSZS

**Designation:** price-class classification muntins

**Menu:** access right for menu Master Data > Prices > Muntin Prices > Muntin Assignment.

**Possible allocation of rights:**
*   Read (r): only read access to existing muntin allocations.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code PSZS is a global user right.

## 21. Print management

Below you will find the individual rights for section Print management.
**All modules of group RE* are global authorizations That means, the access rights cannot be evaluated for each individual client.**

### RE*

**Designation:** system management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Print Management.

**Dependencies:** none.

**Multi-site capability:** module code RE* is a global user right.

### REDR

**Designation:** printout (printer) allocation

**Menu:** access right for menu System > Print Management > Printer Setup.

**Possible allocation of rights:**
*   Read (r): only read access to existing printer configuration.
*   Read and write (w): full access to printer configuration.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code REDR is a global user right.

### REFP

**Designation:** fax protocols, fax repetition

**Menu:** access right for menu System > Print Management > Fax Protocols (Repeat).

**Possible allocation of rights:**
*   Read (r): only read access to fax protocols.
*   Read and write (w): full access to fax protocols.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code REFP is a global user right.

### REFX

**Designation:** faxing out of form print

**Menu:** access right for function „Faxing" to be called in Sales > Purchase > Forms > Print.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access/possibility to fax.

**Description:** the module code controls the permission to fax.

**Dependencies:** the possibility to fax must be configured separately.

**Multi-site capability:** module code REFX is a global user right.

### RELI

**Designation:** list printing (master data)

**Menu:** access right for function „Print Lists“ in Master Data > List Printing.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls the use to print lists.

**Dependencies:** none.

**Multi-site capability:** module code RELI is a global user right.

### REMP

**Designation:** printout of dialogs/tables

**Menu:** Sorting (`<Ctrl+F5>`) > Generate Print Layout

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code REMP is a global user right.

### REPG

**Designation:** report generator

**Menu:** access right for function „Report Generator".

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls the use of function "Report Generator", that will be called in A+W Enterprise in background.

**Dependencies:** report generation must be configured separately.

**Multi-site capability:** module code REPG is a global user right.

### REPO

**Designation:** define report

**Menu:** access right for menu System > Print Management > Forms > Manage.

**Possible allocation of rights:**
*   Read (r): only read access to existing forms.
*   Read and write (w): full access to forms management.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code REPO is a global user right.

## 22. Statistics

Below you will find the individual rights for section Statistics.
**All modules of section SS* are client-specific user rights. That means, access rights can be valuated per individual client.**

### SS*

**Designation:** statistics module

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Statistics.

**Dependencies:** none.

**Multi-site capability:** module authorization SS* can be maintained and evaluated client-specific.

### SSAP

**Designation:** statistic settled commissions

**Menu:** access right for menu Sales > Distribution > Commissions > Commission Calculation and Accounting Sums.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSAP can be maintained and evaluated client-specific.

### SSAU

**Designation:** order

**Menu:** access right for menu Statistics > Sales > Customer / Invoice.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSAU can be maintained and evaluated client-specific.

### SSDR

**Designation:** print statistics

**Menu:** access right for menu Statistics > Print.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSDR can be maintained and evaluated client-specific.

### SSEK

**Designation:** statistics: purchase

**Menu:** access right for menu Statistics > Purchase > Purchase Statistics.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** -/- .

**Dependencies:** none.

**Multi-site capability:** module authorization SSEK can be maintained and evaluated client-specific.

### SSHB

**Designation:** statistics: background booker

**Menu:** system right to start the statistics background booker.

**Possible allocation of rights:**
User-dependent allocation of rights has no effect, here. The authorization SSHB will only be checked internally.

**Description:** the authorization is used internally.

**Dependencies:** none.

**Multi-site capability:** module authorization SSHB can be maintained client-specific.

### SSIV

**Designation:** statistics: glass balancing

**Menu:** access right for menu Statistics > Sales > Glass Balancing.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSIV can be maintained and evaluated client-specific.

### SSKU

**Designation:** statistics: customer

**Menu:** access right for menu Statistics > Sales > Customer.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSKU can be maintained and evaluated client-specific.

### SSKW

**Designation:** statistics: customer/PrGr

**Menu:** access right for menu Sales > Distribution > Acquisition > Visiting Report or Statistics > Sales > Customer/Sales Repres./PSG and SPG.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSKW can be maintained and evaluated client-specific.

### SSKZ

**Designation:** corporation statistics

**Menu:** access right for menu Sales > Distribution.

**Description:** the corporation-wide statistics within the menu item Sales is no longer supported by A+W Enterprise.

### SSPM

**Designation:** monthly production

**Menu:** access right for menu Statistics > Production > Monthly Sums.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSPM can be maintained and evaluated client-specific.

### SSPR

**Designation:** commissions overview

**Menu:** access right for menu Sales > Distribution > Commissions > Order Overview.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSPR can be maintained and evaluated client-specific.

### SSPT

**Designation:** daily production

**Menu:** access right for menu Statistics > Production > Daily Sums.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSPT can be maintained and evaluated client-specific.

### SSVW

**Designation:** representative/product group

**Menu:** access right for menu Statistics > Sales > Representative / SPG or PSG.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSVW can be maintained and evaluated client-specific.

### SSWG

**Designation:** product groups

**Menu:** access right for menu Statistics > Sales > Sub Product Group or Super Product Group.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SSWG can be maintained and evaluated client-specific.

## 23. Master data management

Below you will find the individual rights for section Master data management.
**All modules of group ST* are mainly global authorizations That means, the access rights cannot be evaluated for each individual client. The individual deviations are listed in the following table.**

### ST*

**Designation:** master data management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
This module section controls the user rights of Master Data Management.

**Dependencies:** none.

**Multi-site capability:** all modules of group ST* are mainly global authorizations. That means, the access rights cannot be evaluated for each individual client. The individual deviations are listed in the following table.

### STAB

**Designation:** department - master data

**Menu:** access right for menu Master Data > Departments.

**Possible allocation of rights:**
*   Read (r): only read access to existing departments.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STAB is a global user right.

### STAF

**Designation:** configuration of article field

**Menu:** access right for menu Master Data > Field Configuration > Article Field Configuration.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** article field configuration is evaluated customer-specific. Thus, the access right depends on use of function.

**Multi-site capability:** module code STAF is a global user right.

### STAL

**Designation:** local product - master data

**Menu:** access right to local article master data Master Data > Article

**Possible allocation of rights:**
*   Read (r): only read access to local article master data.
*   Read and write (w): full access.

**Description:** the module code controls program behavior for local article master data. The right STAL also controls the right to change article numbers that are defined as protected/local by system configuration. If the authorization is read-only, the article sub-menus are also available in READONLY mode. For artikel.mfo, ALCIBARTNR or LOKALARTNR the local number ranges can be defined via nr_kreise.

**Dependencies:** this right depends on the environment variables LOKALARTNR_NO_MODIFY and ALCIBARTNR_NO_MODIFY.

**Multi-site capability:** module code STAL is a global user right.

### STAR

**Designation:** global article master data

**Menu:** access right for menu Master Data > Article.
This access right also controls the storage of fixed products in the article master.

**Possible allocation of rights:**
Read (r): only read access to existing article master data, no storage of fixed articles in article master. If the authorization is read-only, the article sub-menus are also available in READONLY mode.
Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Multi-site capability:** module code STAR is a global user right.

### STAV

**Designation:** article dimensioning

**Menu:** access right for menu Master Data > Article > `<F4>` Dimensioning > Article Dimensioning

**Possible allocation of rights:**
*   Read (r): only read access to existing article dimensioning
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Multi-site capability:** module code STAV is a global user right.

### STEM

**Designation:** eMail master data

**Menu:** access right for menu System > Print Management > Email Address and Master Data > Market Partner > `<F4>` > Contact Data > Email -Address.

**Possible allocation of rights:**
*   Read (r): only read access to existing Email addresses.
*   Read and write (w): full access

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STEM is a global user right.

### STFA

**Designation:** vehicle master data

**Menu:** access right for menu Master Data > Keys > System > Dispatch > Vehicles.

**Possible allocation of rights:**
*   Read (r): only read access to existing vehicles.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STFA is a global user right.

### STKB

**Designation:** customer - bonus allocation

**Menu:** access right for menu Master Data > Market Partner > `<F4>` >Bonus Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to existing bonus.
*   Read and write (w): full access.

**Description:** the module code controls the following program behavior (function)

**Dependencies:** use of this function is controlled via environment variable KUNDENBONUS.

**Multi-site capability:** module code STKB is a global user right.

### STKK

**Designation:** account - cost center allocation
**Description:** access authorization STKK is not supported anymore.

### STKU

**Designation:** customer master data
**Description:** see description for access right MPST.

### STLI

**Designation:** supplier master data
**Description:** see description for access right MPST.

### STMA

**Designation:** client-related article master data

**Menu:** access right for menu Master Data > Articles > `<F4>` > Site Specific Details.

**Possible allocation of rights:**
*   Read (r): only read access to existing site-specific article data.
*   Read and write (w): full access.

**Description:** -/- .

**Dependencies:** use of this function has to be configured separately.

**Multi-site capability:** module authorization STMA can be maintained and evaluated client-specific.

### STMI

**Designation:** employee master data

**Menu:** access right for menu Master Data > Employee.

**Possible allocation of rights:**
*   Read (r): only read access to existing employee data.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STMI is a global user right.

### STMM

**Designation:** employee master data

**Menu:** access right for menu Master Data > Employee > Site Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to existing employee data.
*   Read and write (w): full access.

**Description:** the module code controls the possibility to use this function.

**Dependencies:** client-specific allocations can only be used within multi-site system. For details see chapter "3.1. Multi-site capability.

**Multi-site capability:** module code STMM is a global user right.

### STMO

**Designation:** shape master data

**Menu:** access right for menu Master Data > Keys > System > Shapes.

**Possible allocation of rights:**
*   Read (r): only read access to existing shape records.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** use of this function is controlled via environment variable KATALOGART.

**Multi-site capability:** module code STMO is a global user right.

### STMP

**Designation:** employee password

**Menu:** access right for function „Enter Password" in employee master.

**Description:** the option of maintaining employee passwords in Master Data > Employee is only available to a limited extent and must be checked by the system administrator.

### STOB

**Designation:** master data - contract data
**Description:** access authorization STOB is not supported anymore.

### STPZ

**Designation:** commission settlement

**Menu:** access right for menu Master Data > Commissions > Commission Assignment.

**Possible allocation of rights:**
*   Read (r): only read access to existing commission allocations.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STPZ is a global user right.

### STRA

**Designation:** master data for discounts and surcharges

**Menu:** access right for menu Master Data > Keys > Market Partner > Process Discounts > Discounts.

**Possible allocation of rights:**
*   Read (r): only read access to existing discounts.
*   Read and write (w): full access.

**Description:** presently, this access authorization is not evaluated s.a. #421176.

**Dependencies:** none.

**Multi-site capability:** module code STRA is a global user right.

### STRM

**Designation:** handling of discount methods

**Menu:** access right for menu Master Data > Keys > Market Partner > Process Discounts > Discount Methods.

**Possible allocation of rights:**
*   Read (r): only read access to existing discount methods.
*   Read and write (w): full access.

**Description:** presently, this access authorization is not evaluated s.a. #421176.

**Dependencies:** none.

**Multi-site capability:** module code STRM is a global user right.

### STRP

**Designation:** maintenance of market partner dependent discounts

**Menu:** access right for menu Master Data > Market Partner > `<F4>` > Discounts.

**Possible allocation of rights:**
*   Read (r): only read access to existing discounts.
*   Read and write (w): full access.

**Description:** presently, this access authorization is not evaluated s.a. #421176.

**Dependencies:** none.

**Multi-site capability:** module code STRP is a global user right.

### STSL

**Designation:** define BOM

**Menu:** access right for menu Master Data > Article > `<F4>` BOM and Master Data > BOM.

**Possible allocation of rights:**
*   Read (r): only read access to existing article BOM.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STSL is a global user right.

### STSM

**Designation:** maint. menu size master

**Menu:** access right for function „Sash Code“. Access to all menus in Master Data > Keys > Products > Sash Size Master.

**Possible allocation of rights:**
*   Read (r): only read access to existing sash size master.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above. This is a customer-specific development whose functions must be configured separately.

**Dependencies:** use of this function is controlled via environment variable MODUL_SASCH.

**Multi-site capability:** module code STSM is a global user right.

### STTE

**Designation:** general master data module
**Description:** access authorization STTE is not supported anymore.

### STWA

**Designation:** product group management

**Menu:** access right for menu Master Data > Product Groups.

**Possible allocation of rights:**
*   Read (r): only read access to existing product groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code STWA is a global user right.

### STWM

**Designation:** site specific master data for product groups

**Menu:** access right for function „Client-specific Product Groups" in product group management: Master Data > Product Groups.

**Possible allocation of rights:**
*   Read (r): only read access to existing client-specific indications for product groups.
*   Read and write (w): full access.

**Description:** the module code controls access to the function mentioned above.

**Dependencies:** multi-site system must be configured separately.

**Multi-site capability:** module code STWM is a local user right.

## 24. System management

Below you will find the individual rights for section System management.
**Module code SY* is a global user right. The client-specific possibilities of configuration are described in the corresponding access rights.**

### SY*

**Designation:** system management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:** this module section controls the user rights of System Management.

**Dependencies:** none.

**Multi-site capability:** module code SY* is a global user right. The client-specific possibilities of configuration are described in the corresponding access rights.

### SYAR

**Designation:** invoice archiving

**Menu:** access right for menu System > Save Archive.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYAR is a global user right.

### SYBA

**Designation:** Binary Activation

**Menu:** access right for menu System > Activation / Release > Binary Activation.

**Possible allocation of rights:** Read (r), Read and write (w)

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:**
**Multi-site capability:**

### SYBR

**Designation:** Package Release

**Menu:** access right for menu System > Activation / Release > Package Release.

**Possible allocation of rights:** Read (r), Read and write (w)

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:**
**Multi-site capability:**

### SYCU

**Designation:** configuration of customized routines

**Menu:** access right for menu `<Ctrl + F4>` (Menu System) > System Configuration > Customizing.

**Possible allocation of rights:**
*   Read (r): only read access to existing customizing actions.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** use of this function is controlled via environment variable CUSTOMIZING.

**Multi-site capability:** module code SYCU is a global user right.

### SYDB

**Description:** delete all records from dialog

**Menu:** access right for functions in System > Client PC Administration > Database Access Management.

**Possible allocation of rights:**
*   Read (r): only read access to existing records for database access management.
*   Read and write (w): full access.

**Description:** the module code controls whether someone can open the dialog Delete all Records or not. The command "Delete all Records" can be used to delete all records of a dialog at the same time.

**Dependencies:** none.

**Multi-site capability:** module code SYDB is a global user right.

### SYDM

**Description:** delete all records from dialog

**Menu:** access right for function Sorting menu `<Ctrl + F5>` Delete all Records.

**Possible allocation of rights:**
Write permission is necessary to delete records.

**Description:** the module code controls whether someone can open the dialog Delete all Records or not. The command "Delete all Records" can be used to delete all records of a dialog at the same time.

**Dependencies:** none.

**Multi-site capability:** module code SYDM is a global user right.

### SYEG

**Designation:** group selection environment variables

**Menu:** access right for menu `<Ctrl + F4>` (Menu System) > Environment Variables.

**Possible allocation of rights:**
*   Read (r): only read access to existing environment variables.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYEG is a global user right.

### SYEI

**Designation:** define system environment-variables

**Menu:** `<Ctrl + F4>` > Environment variable

**Possible allocation of rights:**
Description: the module code controls the possibility to define environment variables in dialog ENV variables.
If the SYEI right is revoked from a user it is not possible to use the ENV variables dialog to define or delete environment variables. If the SYEI right to read is set for a user, then entering and reading the environment variables is still allowed. If the SYEI right is allowed for the user, then all functionalities of the environment variable dialog are allowed. As for SYEV authorization, it should be ensured that only appropriately authorized employees have the SYEI authorization.

**Dependencies:** only users with administrator rights should be granted this right.

**Multi-site capability:** module code SYEI is a global user right.

### SYEK

**Designation:** purchase invoice recording

**Menu:** access right for menu Statistics > Purchase > Booking Protocol.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYEK is a global user right.

### SYEV

**Designation:** system environment-variables

**Menu:** `<Ctrl + F4>` > Environment variable

**Possible allocation of rights:**
Description: the module code controls data selection in dialog ENV variables. The user receives a list of the manipulable environment variables in dialog. Two groups of variables are distinguished: on the one hand, variables that are available to all employees for adaptation and on the other hand, environment variables that can only be manipulated by employees to whom the SYEV authorization is assigned in addition to the above-mentioned variables. Therefore, it should be ensured that only appropriately authorized employees have the SYEV authorization.

**Dependencies:** only users with administrator rights should be granted this right.

**Multi-site capability:** module code SYEV is a global user right.

### SYFA

**Designation:** field shielding

**Menu:**
*   System menu `<Ctrl+F4>` > System configuration > Set end of jump
*   System menu `<Ctrl+F4>` > System configuration > Set field invisible

**Possible allocation of rights:**
Only read and write (w) permission controls the program behavior for this module.

**Description:** the module controls the functions to show or hide field contents and to assign markers to fields. It is now possible to hide individual fields individually or for special user groups or to set markers. To do this, go to the corresponding field whose content is not to be displayed or is to be marked with a marker and open the system menu `<Ctrl+F4>`.
The following keys can be used in the opened system menu:
*   `<Ctrl+F9>` - hide field content (or show)
*   `<Ctrl+F9>` - set marker for field (or remove)
Alternatively, these functions can also be accessed in the submenu System menu > System Configuration > Define end of jump. After selecting the relevant function, an input window opens to configure the desired setting for individual users or user groups. If no employee or authorization group number is entered here, the setting is active system-wide (i.e. for all users).

**Dependencies:** none.

**Multi-site capability:** module code SYFA is a global user right.

### SYFP

**Designation:** path for FIXWIN-PCs
**Description:** access authorization SYFB is not supported anymore.

### SYH1-9, SYHA, SYHR

**Designation:** background order 1-9,

**Menu:** system access authorization for background process „intauf"

**Possible allocation of rights:**
Only the write permission can be evaluated within the program.

**Description:** module code SYH* may only be set for system service/-s.

**Multi-site capability:** module code SYH* is a global user right.

### SYI1/SYIB

**Designation:** already transferred purchase orders / internal purchase orders.

**Menu:** access right for function System > Data Transfer > Transfer Document > Check Transfer.

**Possible allocation of rights:**
The assignment of rights for both module abbreviations is not evaluated.

### SYIP

**Designation:** individual programs

**Menu:** System > Indiv. Programs

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none

**Multi-site capability:** module code SYIP is a global user right.

### SYIS

**Designation:** intra-trade statistics (Intrastat)

**Menu:** access right for menu System > Statistics > Intrastat > Bookings.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYIS is a global user right.

### SYKB

**Designation:** reference configuration

**Menu:** access right for menu Master Data > Field Configuration > Reference Configuration.

**Possible allocation of rights:**
*   Read (r): only read access to existing configuration records.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYKB is a global user right.

### SYKP

**Designation:** configuration of private fields in document entry

**Menu:** access right for menu Master Data > Field Configuration > Document Field Configuration.

**Possible allocation of rights:**
*   Read (r): only read access to existing configuration records.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYKB is a global user right.

### SYLV

**Designation:** limit distributions
**Description:** access authorization SYLV is not supported anymore.

### SYMS

**Designation:** reporting system

**Menu:** access right for menu section `<Ctrl + F4>` System > Mail System > System Messages.

**Possible allocation of rights:**
*   Read (r): only read access to the existing configuration for system messages.
*   Read and write (w): full access.

**Description:** the module code controls access to the mentioned dialogs.

**Dependencies:** none.

**Multi-site capability:** module code SYMS is a global user right.

### SYNR

**Designation:** number range management

**Menu:** access right for menu System > Number Ranges.

**Possible allocation of rights:**
*   Read (r): only read access to existing number ranges.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYNR is a global user right.

### SYNS

**Designation:** Number status

**Menu:** access right for menu System > Number Status.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYNS is a global user right.

### SYPR

**Designation:** System Monitor

**Menu:** access right for menus `<Ctrl + F5>` System Menu, System Configuration > Field Protocol, Protocol Field/Record.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): only if the write permission exists, the user can switch field logging on and off.

**Description:** the module code controls use of function „Field Logging".

**Dependencies:** none.

**Multi-site capability:** module code SYPR is a global user right.

### SYSM

**Designation:** System Monitor

**Menu:** access right for menu System > System Monitor.

**Possible allocation of rights:**
*   Read (r): works like „w" access.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above. System monitor must be configured separately.

**Dependencies:** none.

**Multi-site capability:** module code SYSM is a global user right.

### SYSO

**Designation:** default sorting for tables

**Menu:** access right for menu Sorting (Ctrl + F5) > Default Sorting.

**Possible allocation of rights:**
This module code requires read and write permission (r).

**Description:** To sort displayed data with the sort menu, you need a write permission, since temporary tables are created for this.

**Dependencies:** none.

**Multi-site capability:** module code SYSO is a global user right.

### SYSQ

**Designation:** adhocsql functions

**Menu:** access right for menu `<Ctrl + F4>` SQL Queries..

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): the user needs "w" access to use the Adhocsql function.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization SYSQ can be maintained and evaluated client-specific.

### SYSV

**Designation:** message texts

**Menu:** access right to the development internal module to maintain message texts.

**Possible allocation of rights:**
*   Read (r): only read access to existing message texts.
*   Read and write (w): full access.

**Description:** module „alerrmsg" can only be configured for environment-internal purposes.

**Dependencies:** none.

**Multi-site capability:** none.

### SYTD

**Designation:** table documentation
**Description:** access authorization SYTD is not supported anymore. The table documentation is independent from the set right and always available.

### SYTY

**Designation:** terminal allocation

**Menu:** access right for menu System > Client PC Administration > Client PC Allocation.

**Possible allocation of rights:**
*   Read (r): only read access to existing terminal allocations.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above. After message "Logical Terminal unknown"! Code: nnn <ttyxxx>" this terminal can be released for use with given access authorization to the SYTY module (terminal allocation).

**Dependencies:** none.

**Multi-site capability:** module code SYTY is a global user right.

### SYVL

**Designation:** transfer statistics
**Description:** access authorization SYVL is not supported anymore.

### SYVT

**Designation:** virtual terminal code

**Menu:** access right for menu System > Client PC Administration > Logical PC Grouping.

**Possible allocation of rights:**
*   Read (r): only read access to existing PC groupings.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYVT is a global user right.

### SYWV

**Designation:** Representation Definition

**Menu:** access right for menu System > Document Management > Representation Mode.

**Possible allocation of rights:**
*   Read (r): only read access to existing resubmission configuration.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code SYWV is a global user right.

## 25. TEKAP programs

Below you will find the individual rights for single TEKAP programs.
**Module TEKAP is not supported anymore. The description here is of February 1st, 2012.**

### TE*

**Designation:** all TEKAP programs

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
The module section controls the user rights of all TEKAP programs.

**Dependencies:** none

### TEIT

**Designation:** Comp. of planned status/actual state for loading
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** use of this function is controlled via environment variable.

### TEKU

**Designation:** maintenance in test environment
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** use of this function is controlled via environment variable.

### TEST

**Designation:** tmp_leser
**Menu:** access right for menu or menu section
**Possible allocation of rights:** Read (r), Read and write (w)
**Description:** -/- .
**Dependencies:** use of this function is controlled via environment variable.

## 26. Text management

Below you will find the individual rights for section Text management.

**Multi-site capability:**
Module code TX* is a global user right.

### TX*

**Designation:** text management

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
The module section controls the user rights of the text management.

**Dependencies:** none.

**Multi-site capability:** module code TX* is a global user right.

### TXAK

**Designation:** current group texts

**Menu:** access right for menus Master Data > Text Management > Current Texts and Master Data > Text Management > Group Texts

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code TXAK is a global user right.

### TXIF

**Designation:** info texts (customer/supplier. etc)
**Description:** access authorization TXIF is not supported anymore.

### TXKA

**Designation:** customer article texts

**Menu:** Master Data > Market Partner > `<F4>` Menu > Texts/Print > MP Article Texts

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code TXKA is a global user right.

### TXWG

**Designation:** product group texts

**Menu:** Master Data > Text Management > Product Group Texts

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write (w) access represents the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code TXWG is a global user right.

### TXZU

**Designation:** configurable texts

**Menu:** Master Data > Text Management > Configurable Texts

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents read access and the read and write access (w) the edit mode.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module code TXZU is a global user right.

## 27. Documents

The individual authorizations for the Documents are listed below.
**Multi-site capability: all module authorizations in section VO* can be maintained and evaluated client-specific.**

### VO*

**Designation:** documents (quotation, order.)

**Possible allocation of rights:**
Rights, that are set for a section code apply to all module codes of this section. This information is valid for all module codes until a module code of this section gets its own rights definition. Then, this special rights definition is valid.
Both rights can be assigned for a module: read (r) and read and write (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
The module section controls the user rights of all documents.

**Dependencies:** none.

**Multi-site capability:**
The module authorizations in section VO* can be maintained and evaluated client-specific.

### VOAA

**Designation:** order modification

**Menu:** access right for menu Sales > Order Entry.

**Possible allocation of rights:**
*   Read (r): only read access to existing orders.
*   Read and write (w): full access.

**Description:** the module code controls the right to change existing orders. The module code is evaluated when loading existing orders. If a user has writing rights, he can change existing orders unless they have been locked otherwise. If the authorization is read-only, existing orders are only displayed. If a user has got no rights at all, he cannot load existing orders. This allows to grant users the right to enter orders but prevent them from changing existing orders.

**Dependencies:** right VOKA contains the right VOAA.

**Multi-site capability:** module authorization VOAA can be maintained and evaluated client-specific.

### VOAB

**Designation:** finish documents

**Menu:** access right for function "Finish Documents".

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description)
*   Read and write (w): full access.

**Description:** the module code controls the function "Finish Documents", which can be used within invoice generation. The read permission allows the loading of data records (value import), but does not allow the user to close any invoices.

**Dependencies:** none.

**Multi-site capability:** the module authorization VOAB can be maintained and evaluated client-specific.

### VOAE

**Designation:** change other user's orders

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): the read permission allows the user to view orders from other creators. However, any changes are excluded. Own orders may also be changed with the read permission.
*   Read and write (w): full access allows the user to change own and external orders.

**Description:** the module code controls program behavior to change orders for own and foreign orders.

**Dependencies:** module code VOKA controls access to the order entry. The VOKA right overrides all other rights that apply to order entry.

**Multi-site capability:** the module authorization VOAE can be maintained and evaluated client-specific.

### VOAN

**Designation:** quotation processing

**Menu:** access right for menu Sales > Quotation Entry.

**Possible allocation of rights:**
*   Read (r): only read access to existing quotations.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** the module authorization VOAN can be maintained and evaluated client-specific.

### VOAP

**Designation:** order-individual prices

**Menu:** access right for menu `<F4>` > Price Info > Order Prices > Article Prices within the order entry.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description).
*   Read and write (w): full access.

**Description:** the module code controls program behavior "order-individual prices". Within order entry, it is possible to store the article prices that only apply to this order. If the user does not have the right VOAP (this also applies to the specification 'r'), he or she may not define individual order prices.

**Dependencies:** none.

**Multi-site capability:** the module authorization VOAP can be maintained and evaluated client-specific.

### VOAR

**Designation:** Quotations Creation of reference price lists

**Menu:** access right for reference quotations in the order entry.

**Possible allocation of rights:**
*   Read (r): only read access to existing reference quotations.
*   Read and write (w): full access.

**Description:**
Price list quotes (kauf.auftragsart=13) can be viewed or amended only by users who have been allocated the new user right VOAR (quote reference price list creation), type „r“ or „w“. If a user has got this right, type „w“, this order type can also be entered manually for a quote. Reference quotations are customer-specific developments.

**Dependencies:** none.

**Multi-site capability:** module authorization VOAR can be maintained and evaluated client-specific.

### VOAS

**Designation:** Documents Muntin Prices

**Menu:** access right for menu `<F4>` > Price Info > Order Prices > Article Prices

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description).
*   Read and write (w): full access.

**Description:** the module code controls program behavior "order-individual muntin prices". In the order entry, it is possible to store muntin prices that only apply to this order. If the user does not have the right VOAS (this also applies to the specification 'r'), he or she may not define order-individual muntin prices.

**Dependencies:** none.

**Multi-site capability:** module authorization VOAS can be maintained and evaluated client-specific.

### VOAT

**Designation:** authorization for changing generated article texts

**Menu:** access right for menu `<F4>` > Texts > Article Texts (`<F5>`) in order entry.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** the module code controls the right to change generated article texts. Users who do not have this authorization cannot change the generated article text lines.

**Dependencies:** none.

**Multi-site capability:** module authorization VOAT can be maintained and evaluated client-specific.

### VOAU

**Designation:** edit order conditions

**Menu:** access right for menu `<F4>` > Price Info > Document Conditions or Item Conditions in order entry.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description).
*   Read and write (w): full access.

**Description:** the module code controls program behavior "order-individual conditions". Within order entry, it is possible to define the order conditions that only apply to this order. If the user does not have the right VOAU (this also applies to the specification 'r'), he or she may not define order- or item-individual conditions.

**Dependencies:** none.

**Multi-site capability:** module authorization VOAU can be maintained and evaluated client-specific.

### VOAW

**Designation:** document evaluations

**Menu:** access right for function "Market Partner Info".
`<Ctrl + <F4>>` >Information Services > Information System > Customers or Suppliers or Master Data > Market Partner, `<F4>` > Market Partner Info.

**Possible allocation of rights:**
For this module code both rights can be assigned: the read(r) as well as the read and write access (w). the dialog provides only the market partner information, therefore there is no difference in read and write access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOAW can be maintained and evaluated client-specific.

### VOBK

**Designation:** Release documents with status Purchased - local Correction

**Menu:** access right for function (see description).

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. Only if the user has a write access, when saving an order with status Ordered-Local-Correction, he or she is asked whether the order should be released again despite the P.O. Employees without this permission get a message that the order change remains local.

**Description:** the module code controls whether a user can transfer a document with status Ordered Local Correction to the system again for further processing.

**Dependencies:** none.

**Multi-site capability:** Module authorization VOBK can be maintained and evaluated client-specific.

### VOBU

**Designation:** activate booking unit
**Description:** access authorization VOBU is not supported anymore.

### VOCA

**Designation:** management orders

**Menu:** access right to define management orders.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (i.e. has the same meaning as the write permission).
*   Read and write (w): full access.

**Description:** the module code can be used to control the rights for selecting the order type "Management Order" and the reference to management orders in the order entry. If an employee does not have the right to create a management order, a message appears on the screen informing the employee of the missing right. The order type is reset to the original type. However, the missing authorization does not prevent the management order or the management quotation from being subsequently changed at will.

**Dependencies:** none.

**Multi-site capability:** module authorization VOCA can be maintained and evaluated client-specific.

### VODH

**Designation:** evaluate printing history
**Description:** access authorization VODH is not supported anymore.

### VODR

**Description:** form printing Sales

**Menu:** access right for menu Sales > Forms > Print.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** the module code controls access to the above dialog and thus the print release for all sales documents.

**Dependencies:** none.

**Multi-site capability:** module authorization VODR can be maintained and evaluated client-specific. If the user does not have the right for a client, he can still enter the dialog. In the selection selo, only the sales documents for other clients where he or she has the permission are made available. If you enter a number manually, the documents from this site are rejected.

### VOEM

**Designation:** Email dispatch sales

**Menu:** access right for menu Sales > Forms > E-mail/Fax

**Possible allocation of rights:**
For this module code, both rights can be assigned: the read(r) as well as the read and write access (w). The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** using this function, documents can be selected and sent by e-mail similar to form printing. This accesses the xemail table. An e-mail address that can still be changed is displayed in the hit list for each document. After the e-mails have been sent, these documents are regarded as printed and are therefore no longer displayed in normal form printing. The module code controls access to the dialogs mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOEM can be maintained and evaluated client-specific. Similar to permission VODR, dialog access is treated differently: if the user does not have the right for a client, he can still enter the dialog. In the selection selo, only the sales documents for other clients where he or she has the permission are made available. If you enter a number manually, the documents from this site are rejected.

### VOFE

**Designation:** activate order ready-report

**Menu:** access right for menu Sales > Complet. Report

**Possible allocation of rights:**
*   Read (r): no effect at this point, i.e. it is possible to enter the dialog, but the booking option is disabled.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOFE can be maintained and evaluated client-specific.

### VOFH

**Designation:** authorization for changing processes of external plants

**Menu:** access right for menu Sales > Order Entry

**Possible allocation of rights:**
*   Read(r): This right allows to view documents from other site.
*   Read and write (w): with the read and write permission, the dialog is shown in editing mode.

**Description:** the module code controls whether a user has the authorization to load and correct orders from any client, including employees of other clients.

**Dependencies:** the environment variable MODIFY_KAUFHAUSNR="ON" controls whether you can enter orders for different clients within the same database.

**Multi-site capability:** module authorization VOFH can be maintained and evaluated client-specific. In the multi-site system, order handling is controlled differently using several clients. Please note the corresponding function description.

### VOFR

**Designation:** temporary release for document alteration

**Menu:** access right for menu Sales > Order Release > Authorization.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access: write access is required to release documents.

**Description:** the module code controls whether a user is authorized to release orders. The "Authorization to release orders" function is customer-specific and must be configured separately.

**Dependencies:** none.

**Multi-site capability:** module authorization VOFR can be maintained and evaluated client-specific.

### VOGS

**Designation:** creation of credit notes

**Menu:** access right for menu Sales > Credit Notes > Enter Credit Notes.

**Possible allocation of rights:**
*   Read (r): only read access to existing credit notes.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOGS can be maintained and evaluated client-specific.

### VOKA

**Designation:** order entry

**Menu:** access right for menu Sales > Order Entry

**Possible allocation of rights:**
*   Read (r): only read access to orders, already entered.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above. The missing VOKA right overrides other function rights that are queried during order entry.

**Dependencies:** none.

**Multi-site capability:** module authorization VOKA can be maintained and evaluated client-specific.

### VOKE

**Designation:** authorization for entry of orders free of charge

**Menu:** access right to enter orders free of charge.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (i.e. has the same meaning as the write permission).
*   Read and write (w): full access.

**Description:** the module code can be used to control the rights for selecting the order type "Order free of charge" and the reference to such orders in order entry. If an employee does not have the right to create an order free of charge, a dialog message appears informing the employee of the missing right. The order type is reset to the original type.

**Dependencies:** none.

**Multi-site capability:** module authorization VOKE can be maintained and evaluated client-specific.

### VOKK

**Designation:** information systems: customer conditions
**Description:** access authorization VOKK is not supported anymore.

### VOKO

**Designation:** production cost calculation

**Menu:** access right for menu Sales > Order Entry, field Price > `<Ctrl + F10>`.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** the module code controls access to the dialogs for material and production cost calculation.

**Dependencies:** none.

**Multi-site capability:** module authorization VOKO can be maintained and evaluated client-specific.

### VOKU

**Designation:** Customer/site allocation must not be ignored

**Menu:** access right for function in dialog Sales > Order Entry.

**Possible allocation of rights:**
With the right VOKU, you can specify for users company-specifically or globally whether they can select all customers in the sales transactions (manually or via market partner search) or only the customers who are assigned to the company of the transaction (table mpmdzu). By revoking the right ("-"), the person making the entry now has a limited overview of the customers (customers who are assigned to this company). By activating the right ('r' or 'w'), all customers' companies are available for selection.

**Description:** the module code controls the selection of customers in the order entry.

**Dependencies:** none.

**Multi-site capability:** module authorization VOKU can be maintained and evaluated client-specific.

### VOKZ

**Designation:** minor shipment surcharges

**Menu:** access right for menu Sales > Invoices > Automatic Release > `>Ctrl + K>`.

**Possible allocation of rights:**
For this module code, both rights can be assigned: the read(r) as well as the read and write access (w). The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** with the help of `<Ctrl + K>` in the first field of the dialog for the automatic release of sales invoices, you reach the dialog for handling the minor shipment surcharges. When you open this, all records from table 'kleinlief' are loaded.

**Dependencies:** the function for handling minor shipment surcharges is controlled by the environment variable DELIVERY_SURCHARGE.

**Multi-site capability:** module authorization VOKZ can be maintained and evaluated client-specific.

### VOLI

**Designation:** creation of delivery notes

**Menu:** access right for menu Sales > Delivery Notes > Automatic Release.
In the Delivery Notes dialog, the Release field has several specifications. The right VOLI applies here only to the delivery note release. The right VORE is responsible for invoice generation.

**Possible allocation of rights:**
*   Read (r): no effect at this point, i.e. the user may enter the dialog, but may not edit any data records for delivery note creation.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above. Users who have this writing right will be able to access the dialog. This allows the user to create delivery notes automatically.

**Dependencies:** the option of generating delivery notes in sales instead of in shipping control must be explicitly enabled and is regarded as not recommended working method.

**Multi-site capability:** module authorization VOLI can be maintained and evaluated client-specific.

### VOLK

**Designation:** local correction authorization

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** the module code controls whether a user has the right to edit an order in local correction. Users who do not have this authorization can no longer change orders that are already in the local correction state.

**Dependencies:** use of this function is controlled via environment variable LOKAL_KORREKTUR_DISPLAY.

**Multi-site capability:** module authorization VOLK can be maintained and evaluated client-specific.

### VOMA

**Designation:** authorization for changing clients in the order

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode.

**Description:** the module code controls whether a user has the right to change the client allocation in the order. This gives the user the right to enter orders for any client.

**Dependencies:** the environment variable MODIFY_KAUFHAUSNR="ON" controls whether you can enter orders for different clients within the same database. Furthermore, this right also applies to the extended client separation with company and market partner assignment. Additional configuration required.

**Multi-site capability:** module authorization VOMA can be maintained and evaluated client-specific.

### VOMN

**Designation:** release orders with a net amount above the MAX value

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): no effect at this point (see description)
*   Read and write (w): full access.

**Description:** the module code controls the following functions within order entry: The system configuration allows to store the maximum net value for an order (in your own currency). If the order exceeds this value, it is automatically placed in the release pool. Only an employee with the write permission VOMN may subsequently activate these orders.

**Dependencies:** use of this function is controlled via environment variable MAX_NETTOWERT. The authorizations for order release depend on the other rights (VOOF, VOOD, VOKE; VOSE, VOMN, VOSM).

**Multi-site capability:** module authorization VOMN can be maintained and evaluated client-specific.

### VOOD

**Designation:** margin check can be ignored

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): no effect at this point (i.e. seems like full access). s. description)
*   Read and write (w): full access.

**Description:** the module code controls the following function within order entry: The margin is checked during order entry. If the user does not have the right, he or she may not save an order with the restriction violation for the range.
If environment variable FREE_NO_SPANNE_TEST is active and the user has no VOOD right but VOKE write permission, the range will be ignored for the order free of charge, because for free orders the range is always -100% and so an order with VOOD='-' would never be enterable.

**Dependencies:** accesses to release orders also depend on other rights (VOOF, VOOD, VOKE, VOSE, VOMN, VOSM).

**Multi-site capability:** module authorization VOOD can be maintained and evaluated client-specific.

### VOOF

**Designation:** authorization for order release during saving

**Menu:** access right for menu Sales > Order Release.

**Possible allocation of rights:**
The module code VOOF can now be assigned in the employee master. Employees with read permission (display mode) cannot release orders directly during order entry. Order changes are also no longer directly activated with this setting.

**Description:** these module codes are used to control who can release an order for further processing.

**Dependencies:** accesses to release orders also depend on other rights (VOOF, VOOD, VOKE, VOSE, VOMN, VOSM).

**Multi-site capability:** module authorization VOOF can be maintained and evaluated client-specific.

### VOOL

**Designation:** limit check can be ignored

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): see description
*   Read and write (w): full access.

**Description:** without the VOOL right, the user may not enter any orders for the customer whose limit check is negative. If the limit check is violated during a new entry, the user cannot save the order. Read permission has the same effect in both cases.
Only users with write permission are allowed to continue entering the order if the limit check is violated.
Depending on the system configuration and the VOOL permission, different program behavior is possible:
*   'r' and LIMITPOOL=ON mean that the user may enter the order despite the missing write permission, but this is automatically placed in the release pool.
*   If the user has the permission VOOL ='r' and LIMITFREI_AUS_POOL=ON, the user can neither enter the orders nor release them to the release pool when the limit is violated.
*   VOOL= '-' always means: if the limit is exceeded, no entry is possible, independent of environment variables.

**Dependencies:** none.

**Multi-site capability:** module authorization VOOL can be maintained and evaluated client-specific.

### VOOR

**Designation:** restriction check can be ignored

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): no effect at this point (i.e. seems like "no right").. s. description)
*   Read and write (w): full access.

**Description:** without the granted VOOR right, the user may not enter an order item whose dimensions violate the restriction check. The user cannot complete such items and must either reject the entry or correct the values. Read permission is the same at this point.
The creator can only continue order entry with a restriction violation in the item if he or she has write permission.

**Dependencies:** none.

**Multi-site capability:** module authorization VOOR can be maintained and evaluated client-specific.

### VOOV

**Designation:** insurance limit check can be ignored

**Menu:** access right for function in the order entry (similar to VOOL).

**Possible allocation of rights:**
*   Read (r): no effect at this point (i.e. seems like "no right").. s. description)
*   Read and write (w): full access.

**Description:** without the granted VOOV right, the user may not enter any orders for the customer whose AKV limit check is negative. If the AKV limit check is violated during a new entry, the user cannot save the order. Read permission has the same effect in both cases. The creator is only allowed to continue order entry in the event of an AKV limit check violation if he or she has write permission

**Dependencies:** none.

**Multi-site capability:** module authorization VOOV can be maintained and evaluated client-specific.

### VOPA

**Designation:** activate commission calculation

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description).
*   Read and write (w): full access.

**Description:** the function for commission settlement must be configured separately. The VOPA right controls the possibility of influencing the configured commission settlement within order entry by changing the value of the commission fields. If the user does not have write permission, he or she cannot make any changes.

**Dependencies:** use of this function is controlled via environment variable PROV_VERFAHREN Further configuration is also possible.

**Multi-site capability:** module authorization VOPA can be maintained and evaluated client-specific.

### VOPC

**Designation:** profit center clearing
**Description:** access authorization VOPC is not supported anymore.

### VOPK

**Designation:** make price calculation

**Menu:** access right for menu Sales > Price Calculation.

**Possible allocation of rights:**
*   Read (r): has no effect at this point, that is, the read permission has the same value as the write permission.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOPK can be maintained and evaluated client-specific.

### VOPL

**Designation:** limit release from POOL with authorized limit logic

**Menu:** access right for menu Sales > Order Release > Release.

**Possible allocation of rights:**
*   Read (r): no effect at this point. i.e. read access is not enough to release such orders.
*   Read and write (w): full access.

**Description:** the module code overrides the VOOL right within the release pool. Only if the right has been set to w, the LSp field in the release pool can be changed to the value N and the associated order released.

**Dependencies:** the right will only be evaluated, if the environment variable LIMIT_FREI was enabled.

**Multi-site capability:** module authorization VOPL can be maintained and evaluated client-specific.

### VOPR

**Designation:** edit price recorder

**Menu:** access right for menu Info System > Prices.

**Possible allocation of rights:**
*   Read (r): has no effect at this point, that is, the read permission has the same value as the write permission.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOPR can be maintained and evaluated client-specific.

### VOPW

**Designation:** price view in quick entry

**Menu:** access right for functions in the quick entry.

**Possible allocation of rights:**
*   Read (r): only read access to the item price.
*   Read and write (w): full access.

**Description:** the module code controls access to the price condition dialog `<Shift + F9>` in the item (Sales > Quick Entry).

**Dependencies:** none.

**Multi-site capability:** module authorization VOPW can be maintained and evaluated client-specific.

### VORE

**Designation:** invoice creation

**Menu:** access right for menu Sales > Invoices > Partial Invoice or Sales > Invoices > Final Invoice > Automatic Release.
In the Invoices dialog, the first field Release has multiple values. The VORE right only applies to invoice generation. The right VOLI is responsible for the release of the delivery note.

**Possible allocation of rights:**
*   Read (r): no effect at this point, i.e. the user may enter the dialog, but may not edit any data records for invoice creation.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialogs mentioned above. Users who have this writing right will be able to access the dialog. This allows the user to create invoices automatically.

**Dependencies:** none.

**Multi-site capability:** module authorization VORE can be maintained and evaluated client-specific.

### VORO

**Designation:** Input of return consignments

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
*   Read (r): see description.
*   Read and write (w): full access.

**Description:** entry and release of return consignments is protected by the right VORO. With the VORO right to write, a user can enter and release return consignments. If he has read-only right, he will be able to enter these consignments but not release them. If he does not have this right at all, he will not be able to enter this type of orders at all.

**Dependencies:** none.

**Multi-site capability:** module authorization VORO can be maintained and evaluated client-specific.

### VORS

**Designation:** cancel sales invoices

**Menu:** access right for functions in the credit note entry Sales > Invoices > Manual Invoice.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description).
*   Read and write (w): full access.

**Description:**
The user can only cancel the invoice that has not yet been booked if read and write authorization has been set. In case of read permission the message "Action does not make sense" appears.

**Dependencies:** the environment variable VK_RECHNUNGS_STORNO allows you to cancel entered but not yet canceled invoices

**Multi-site capability:** module authorization VORS can be maintained and evaluated client-specific.

### VOSA

**Designation:** display of purchasing prices

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. Only the write permission controls whether the Margin field is displayed. Otherwise, it is hidden.

**Description:** the module code controls whether the margin fields are displayed or not in the footer of orders and quotations.

**Dependencies:** none.

**Multi-site capability:** module authorization VOSA can be maintained and evaluated client-specific.

### VOSE

**Designation:** corridor-overstepping price manipulation

**Menu:** access right for functions in the order entry.

**Possible allocation of rights:**
For this module code both rights can be assigned: read (r) and read and write (w) access. The display mode of a dialog represents the read access and the read and write access (w) the edit mode.

**Description:** the module code controls whether the employee who does not have VOSE authorization can change the price determined by the system within the price area. If the price is manipulated beyond the value stored here, the order is placed in the release pool and must be activated there by an authorized user.
The range allowed for a price change is stored in currency units (1 = one currency unit). For orders free of charge, the system can be configured so that this check can be ignored (environment variable FREE_WITHOUT_SPANNE_TEST).

**Dependencies:** the price area is defined in the system using the environment variable PRS_MAN_KORRIDOR.

**Multi-site capability:** module authorization VOSE can be maintained and evaluated client-specific.

### VOSG

**Designation:** cancel sales credit notes

**Menu:** access right for functions in the credit note entry Sales > Credit Notes > Entry of Credit Notes.

**Possible allocation of rights:**
*   Read (r): has no effect at this point (see description).
*   Read and write (w): full access.

**Description:**
The user can only cancel the credit note that has not yet been booked if read and write authorization has been set. In case of read permission the message "Action does not make sense" appears.

**Dependencies:** the environment variable VK_GUTSCHRIFTS_STORNO allows you to cancel credit notes that have been entered but not yet cancelled.

**Multi-site capability:** module authorization VOSG can be maintained and evaluated client-specific.

### VOSL

**Designation:** authorization to cancel orders in local correction

**Menu:** access right for functions in the order entry (`<F4>` > Cancel, `<F7>`) or Dispatch > `<Shift + F4>` > Cancel > Cancel order.

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode.

**Description:** the module code controls the authorization to cancel orders in local correction system-wide (in sales and dispatch control).

**Dependencies:** only evaluated if CANCEL_RIGHT_EXTENSION is enabled.

**Multi-site capability:** module authorization SS* can be maintained and evaluated client-specific.
With regard to the cancellation rights, there are further configuration options. See also „EN-CONFIG-A+W Enterprise" section „Cancellation rights"

### VOSM

**Designation:** release for closed customers

**Menu:** access right for menu Sales > Order Release.

**Possible allocation of rights:**
*   Read (r): has no effect at this point.
*   Read and write (w): full access.

**Description:**
An order for a closed customer can only be released if read and write authorization has been set.
#445963

### VOSR

**Designation:** creation of collective invoices

**Menu:** access right for functions in the invoicing (Sales > Invoices > Automatic Release > `<Shift + F8>`).

**Possible allocation of rights:**
*   Read (r): no effect at this point (collective invoice creation is not possible).
*   Read and write (w): full access.

**Description:** the module code controls the possibility of generating collective invoices.

**Dependencies:** none.

**Multi-site capability:** module authorization VOSR can be maintained and evaluated client-specific.

### VOST

**Designation:** authorization to cancel orders that are not in local correction

**Menu:** access right for functions in the order entry (`<F4>` > Cancel) or Dispatch > `<Shift + F4>` > Cancel > Cancel order.

**Possible allocation of rights:**
For this module only read and write (w) permission have effect on the program behavior. With the read and write permission, the dialog is shown in editing mode.

**Description:** the module code controls the authorization to cancel orders system-wide (in sales and dispatch control).

**Dependencies:** none.

**Multi-site capability:** module authorization VOST can be maintained and evaluated client-specific.
With regard to the cancellation authorizations, there are further configuration options. See also „EN-CONFIG-A+W Enterprise“ section „Cancellation rights"

### VOTF

**Designation:** order release

**Menu:** access right for menu Sales > Order Release.

**Possible allocation of rights:**
*   Read (r): no effect at this point, i.e. the user may enter the dialog, but the release is not enabled.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization VOTF can be maintained and evaluated client-specific.

### VOTR

**Designation:** cash invoice

**Menu:** access right for menu Sales > Invoices > Cash Transaction

**Possible allocation of rights:**
*   Read (r): has the same effect as full access at this point.
*   Read and write (w): full access.

**Description:** the module code controls the authorization to generate cash invoices. Thus, it is possible to withdraw the authorization to create cash invoices issued with the authorization "VOKA" or "VO*" from individual sales employees.

**Dependencies:** none.

**Multi-site capability:** module authorization DI* can be maintained and evaluated client-specific.

## 28. Receipt of goods

Below you will find the individual rights for section Goods receipt.

**Multi-site capability:**
all module authorizations in section WE* can be maintained and evaluated client-specific.

### WE*

**Designation:** Goods receipt - modules

**Possible allocation of rights:**
The rights that are set for an area code apply to all module codes of this area. This statement applies to all module codes in this area until a module code from this area has its own rights definition. The special rights definition is then the valid one.
For a module area, both rights can be assigned: read (r) and read and write access (w). The display mode of a dialog shows the corresponding edit mode.

**Description:**
The module section controls the user rights of all receipt of goods.

**Dependencies:** none.

**Multi-site capability:** all module authorizations in section WE* can be maintained and evaluated client-specific.

### WEER

**Designation:** Goods receipt - entry

**Menu:** access right for menu Purchase > Goods Receipt.

**Possible allocation of rights:**
*   Read (r): only read access for existing receipt of goods.
*   Read and write (w): full access.

**Description:** -/- .

**Dependencies:** use of this function depends on configuration of Purchase module.

**Multi-site capability:** module authorization WEER can be maintained and evaluated client-specific.

### WERE

**Designation:** Notification

**Menu:** access right for menu Purchase > Notification.

**Possible allocation of rights:**
*   Read (r): no effect at this point.
*   Read and write (w): full access.

**Description:** the module code controls access to the dialog mentioned above.

**Dependencies:** none.

**Multi-site capability:** module authorization WERE can be maintained and evaluated client-specific.

## 29. Contact Address

**A+W Software GmbH**
Am Pfahlgraben 4 - 10
35415 Pohlheim
Germany

Tel. +49 6404 2051 0
Fax. +49 6404 2051877

E-Mail: zentrale@a-w.com
Internet: http://www.a-w.com/
