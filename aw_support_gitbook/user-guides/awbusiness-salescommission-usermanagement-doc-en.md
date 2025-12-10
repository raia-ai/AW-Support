---
title: "EN_AWBusiness_Master_Data_9_4-4"
source: "EN_AWBusiness_Master_Data_9_4-4.pdf"
tags: ["A+W Business", "Sales Commission", "User Management", "Employee Rights", "Software Tutorial", "Master Data", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial segment from the A+W Business Master Data manual, covering the setup and management of sales commissions and the administration of employee data, user groups, and access rights within the system."
long_description: "This document is a detailed tutorial for the A+W Business software, focusing on two key administrative areas: Sales Commission and Management of Employees. The first section on Sales Commission explains how to configure commission rates for salespersons based on various criteria like main product groups (MPG), price lists, turnover, or discount percentages. It details the process of creating standard and graduated commission rates, including examples and step-by-step instructions for entering, modifying, and deleting commission rules in the 'Sales commission' dialog. The section also covers commission splitting between multiple sales representatives and the calculation logic. The second major section, Management of Employees, provides a guide to entering and managing employee data, which is essential for system access and security. It discusses the creation of user profiles, assignment to user groups (e.g., Manager, Supervisor, User), and the detailed allocation of access rights. This includes defining permissions to view, add, edit, or delete data across different modules of the software. The tutorial provides practical examples and instructions for creating new users, setting passwords, locking user accounts, and editing user rights."
---

# Additional Information on the Company

---
## Sales Commission

The dialog "Sales commission" is used to enter the commission rates for individual salespersons. You have to enter a commission rate for every salesman and at least for every main product group (MPG).
Commissions can be distinguished by price list. If `<n.e.>` is selected for the price list and the key, the commission rate is valid for all rates.

*(Fig. B-232 shows the 'Administration - Sales commission' dialog)*

*   **A** Commission is generally applicable
*   **B** Calculation basis
*   **C** Quantity (units) for which the commission rate is calculated
*   **D** Commission rate per graduated quantity

### The commission can be graduated at random.

**Examples: Graduated by discount, graduated by turnover**

| Up to % Discount | % commission | Up to turnover | % Commission |
| :--------------- | :------------- | :------------- | :------------- |
| 10               | 5              | 999,999,999    | 5              |
| 20               | 3              | 5,000          | 3              |
| 40               | 1              | 1,000          | 1              |
| 99               | 0              | 0              | 0              |

The graduated quantity depends on the commission type.

**Example Commission Types**

| Commission type     | Quantity                           |
| :------------------ | :--------------------------------- |
| Discount %          | Discount granted per order/item    |
| Marginal income %   | Marginal income in percent         |
| Turnover            | Total turnover of the salesman     |
| Marginal income     | Marginal income                    |
| Price/PU            | Price per quantity unit            |

### Commission splitting and manual commission rates

Sales representatives are allocated in partner data. If two sales representatives are entered, you can define how the commission is going to be distributed. Calculation of sales commissions is based on orders.

*(Fig. B-233 shows the 'Customer data - tab Sales' dialog for setting sales representatives.)*

The entries in customer data are adopted for the order and can be changed if required.

*(Fig. B-234 shows preset entries for sales representatives in an order.)*
*   **A** Tab Document: Salesman 1
*   **B** Tab Supplement: Salesman 2
*   **C** Share in commission

If no details are entered for the second salesman (in the order), he will get no commission for this order. Commission splitting refers to the commission which is calculated based on the entries in the dialog Sales commission.

The settings made at item entry can be changed in the order.

*(Fig. B-235 shows the 'Item - tab Supplement' for commission rates.)*

You can enter two different commission rates per item. These will be allocated to salesman 1 and salesman 2 respectively.

### Calculation examples

> **Commission 0.75% on the glass price**
> Order = 2000.00 € for glass, commission splitting: **15.00 €**
> - Salesman 1: **10.05 €**
> - Salesman 2: 33.5 %: **4.95 €**

> **Item = 2000.00 €, manual commission rates**
> - Salesman 1: 1.00 %: **20.00 €**
> - Salesman 2: 0.75 %: **15.00 €**

### Calculation of commissions

The sales commission is calculated per item, based on the PGR of the item. If complaints are taken into account for calculation, the commission will be lower. For statistical analysis, the orders can be transferred to commission statistics. In this case, orders will be transferred to commission statistics when they are transferred to archives. These functions have to be enabled in company data.
(⇨ Software Reference, "Company Data > Archives" on page B-962)

By default, the sales commission is calculated when documents are transferred to archives. The following settings must be enabled in company data for this purpose:
*   On tab **Archives**, the checkbox **Transfer to commission statistics**.
*   On tab **Parameters**, the checkbox **Interactive sales commission**.

*(Fig. B-236 shows the 'Interactive sales commission' checkbox in 'Company data - tab Parameters'.)*

If this function is not active, the commission rates defined in master data for calculating the commission will be loaded only when the order is transferred to commission statistics.

Orders can also be transferred manually. This is done by means of the archiving dialog in module Documents.

These settings for commissioning are valid for orders and credit notes.

## Entering the Commission

In this example we are going to enter a graduated commission which shall be valid for all price lists.

### How to enter a sales commission
1.  Go to menu **Master data > Company > Sales commission**. Dialog `Sales commission` appears.
2.  Go to the menu **Start > New** to switch to the input mode.

*(Fig. B-237 shows the fields for a new commission rate are accessible.)*
*   **A** Salesman
*   **B** Rate
*   **C** Commission type
*   **D** Quantity graduation
*   **E** Percentage of the commission

3.  Enter the rate (price list and key) if required (B). If you enter `<n.e.>` in both fields, the commission will be valid for all price lists.
4.  Choose the salesman (A). Only the employees entered in dialog `Sales areas` will be offered for selection as sales representatives. If you choose `<n.e.>`, the commission will be valid for all sales representatives.
5.  Choose the commission type (C), e. g. `turnover`. These are the minimum entries for the header. These details cannot be changed afterwards. If you enter the commission rate now, you can only add the graduation and the percentage of the commission. To differentiate the commission further, please enter data on customers, etc.
6.  Select a customer, the product group and/or the product if required. If no entries are made in these fields, the commission will be valid for all customers, product groups, and products.

> **Changing the details**
> The entries made in steps 3 to 6 **cannot** be changed later. You should therefore check the fields thoroughly before performing the next step. Should you detect later that the commission has been defined incorrectly, you will have to delete all data and enter them again.

7.  Enter the value for the graduated quantity (D) and the commission rate (E). If the commission shall not be graduated, enter `99999999` for the quantity.
8.  Select in the menu **Start > Save** to save the data. The data will be saved.

### How to enter a graduated commission
1.  Enter a commission rate as defined in the previous paragraph. The size of the first graduation step is irrelevant.
2.  Select the commission rate for which another level shall be defined.
3.  Go to the menu **Start > New** to switch to the input mode. Please make sure to adopt the settings in section **Select salesman/product group** as they are.
4.  Enter the value for the graduated quantity (D) and the commission rate (E).
5.  Select in the menu **Start > Save** to save the data. The data will be saved.
6.  Repeat steps 3 to 5 until all levels have been defined.

*(The following table shows an example of graduated commission rates based on turnover for a specific customer.)*

| Salesman ID | Name    | Commission type | Graduated qty. | Commission | Valid from date | Price list | Price key | Customer | Name   |
| :---------- | :------ | :-------------- | :------------- | :--------- | :-------------- | :--------- | :-------- | :------- | :----- |
| T**         | Training| Turnover        | 1,000.00       | 0.250 %    | 01.01.2013      | <K.A.>      | <K.A.>    | 4000     | A+WT   |
| T**         | Training| Turnover        | 10,000.00      | 0.500 %    | 01.01.2013      | <K.A.>      | <K.A.>    | 4000     | A+WT   |
| T**         | Training| Turnover        | 100,000.00     | 0.750 %    | 01.01.2013      | <K.A.>      | <K.A.>    | 4000     | A+WT   |

The sequence in which the commission rates are listed has no effect on the calculation. They can be sorted by double-clicking on a column header.

### How to delete a sales commission
1.  Go to menu **Master data > Company > Sales commission**. Dialog `Management - Sales commission` appears.
2.  Select the commission rate to be deleted.
3.  Go to menu **Start > Delete**.
4.  Confirm the security check by **[Yes]**. The selected commission rate will be deleted.

## Management of Employees

### Objectives
*   Entering employee data and managing them by means of groups.
*   Defining access rights for employees.

### Benefit
*   Only registered employees can use A+W Business. This helps to prevent unauthorised access to the data.
*   Users can have different rights. This way you can define which employees can access certain data.

### Note

*   **Data protection**: Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights.
*   **Employee data**: Using A+W Business requires entering the employees' access data. Only registered users will be able to start the program.
*   **User rights**: Your company's employees can have different access rights for the data in A+W Business. These rights are defined by restrictions.
*   **User group**: The following groups of employees/users are set by default:
    *   Manager
    *   Supervisor
    *   User
    *   Management
    Each of these groups has different access rights which are based on the operational tasks.
*   **Profile**: Allocation of rights is made easy by predefined profiles.
*   **Prerequisite**: You can enter new users only if you have system administrator's rights.

> **Employees (m/f)**
> Female as well as male employees can use A+W Business of course. In this session we are going to use the male form for reasons of legibility. The female sex is included as a matter of fact.

### Staff

All users working with A+W Business have to be entered in the system. The user's real name will be saved for all of his actions. This name will appear in some of the dialogs, e.g. in dialog `Number manager`. You can also define special number ranges for every user. Every user can create his own number manager.

Program login requires a password. The login can be linked with the Windows login in company data.

> **Data protection**
> Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights.

User data cannot be deleted. If a user does no longer work for the company, he has to be blocked in user management.

### Presetting for documents and order areas

Settings for documents and order areas allow to allocate the processing of documents to a client, an order area, and certain document types. These settings can be changed in the actual documents.

*(Fig. B-238 shows the 'Presetting for documents' settings for a user.)*
*   **A** Document types and order areas
*   **B** Standard document for this user

This example shows that for purchase orders, a certain document type has been assigned to the user.

If you enter the order area as well, you define that the documents of this user will be automatically allocated to the order area, using numbers from the corresponding number range.

The entry in column **General (A)** will overrule the entries for the other document types and order areas. This means that you cannot choose at random in this case:
*   **<n.e.> or another selection**: All other columns are `<inactive>`.
*   **<inactive>**: The document type or order areas can be selected in the other columns.

> **Example: Order area - column General**
>
> *   **<n.e.>**: If no settings have been made for the documents, no presetting will be used for the order areas. In this case, the user has to make sure to select the right order area and document type.
> *   **Toughened glass**: No presetting can be made for documents. When the user enters a document, the order area `TG` will be preset by default. The document will get a number from the corresponding number range. The number will be assigned when the document is saved.

### Employee Groups

The following user groups exist by default: manager, supervisor, user, management. Each group has different access rights, depending on their tasks in the company. Predefined user groups and user rights can be edited and completed by new ones.

In case of extensive modifications, it might be better to create a new group with the appropriate rights.

If you allocate a (new) user to a user group, he will automatically get all the rights defined for this group. If he is to get other rights, these can be completed or amended especially for him.

### User Rights

Your company's employees can be granted different access rights to the data in A+W Business so that you can specify which areas shall be open or locked for the individual users.

The following rights can be granted or withdrawn:
*   **Change**: Data can be edited.
*   **Insert**: New records can be entered.
*   **Delete**: Records can be deleted.
*   **Execute/read**: The dialog can be opened.

For these settings you have to bear the logical connections in mind: If a user is entitled to enter data he also has to have the right to open the corresponding dialog.

The allocation of rights refers to all program sections in A+W Business, down to dialog level, and partly the fields as well.

> **Example**
> If a user shall be able to see prices in archived orders in module `Documents`, he has to have the right of executing the program items `0055 Documents-Archives-Search order` and `0002 Price view`.

*(Fig. B-239 shows the 'Management of rights' dialog.)*
*   **A** User group or user
*   **B** Program and sub-right
*   **C** Display of rights for the selected program

This example shows that the selected group is entitled to read the sales prices in an order but cannot change, add, or delete them (C).

> **Rights are defined by restrictions**
> All displayed program items are defined with limited rights. Program items that are not displayed can be used without restrictions.

Rights are granted or withdrawn according to the following system:

| Program item (dialog, field)                   | Right                               |
| :--------------------------------------------- | :---------------------------------- |
| Not listed.                                    | = Full access                       |
| Listed, no checkbox ticked.                    | = Dialog or field is locked.        |
| Listed, but one or more checkboxes have been ticked. | = The corresponding action can be taken. |

### User profiles

Allocation of rights is made easy by predefined profiles. These offer the following settings:
*   **All programs without rights**: Records are created for all programs; the rights to execute, change, add, and delete are disabled, e.g. for employees who have left the company.
*   **All programs executable**: Records will be created for all programs. Only the right to execute is enabled. All others are disabled. Dialogs can only be opened.
*   **All programs with all rights**: In this case, all entries are deleted for the group in question which, like the supervisor, is granted all rights.

### Examples of Group and User Rights

In dialog `Management of rights`, rights are granted or withdrawn by means of checkboxes. When a checkbox is ticked, this is always an exception from the general rule/setting. This is demonstrated in the following examples.

These very basic examples deal only with the main programs as it would be quite confusing to mention all sub-items. It goes without saying that rights can be allocated to sub-items as well.

**Group: Supervisor = System administrator**

| Program           | Sub-right | Execute | Change | Add | Deletion |
| :---------------- | :-------- | :------ | :----- | :-- | :------- |
| Master data       |           | x       | x      | x   | x        |
| Documents         |           | x       | x      | x   | x        |
| Production        |           | x       | x      | x   | x        |
| Statistics        |           | x       | x      | x   | x        |
| Stock             |           | x       | x      | x   | x        |
| Capacity planning |           | x       | x      | x   | x        |
| Utilities         |           | x       | x      | x   | x        |
| References        |           | x       | x      | x   | x        |
*x: all rights (no entry)*

The supervisor is automatically granted all rights. This is why no programs are listed and no checkboxes are ticked.

**Group: User**

| Program           | Sub-right  | Execute | Change | Add | Deletion |
| :---------------- | :--------- | :------ | :----- | :-- | :------- |
| Master data       |            | ☑       | ☐      | ☐   | ☐        |
| Documents         |            | ☑       | ☑      | ☑   | ☑        |
| Production        |            | ☑       | ☐      | ☐   | ☐        |
| Statistics        |            | ☐       | ☐      | ☐   | ☐        |
| Stock             |            | ☑       | ☐      | ☐   | ☐        |
| Capacity planning |            | ☑       | ☐      | ☐   | ☐        |
| Utilities         | Order info | ☐       | ☐      | ☐   | ☐        |
|                   | Debt./Cred. | ☐       | ☐      | ☐   | ☐        |
| References        |            | ☐       | ☐      | ☐   | ☐        |
*x: all rights (no entry)*

The group **Users** can enter, change, delete, and execute documents. In modules **Master data**, **production**, **stock**, and **capacity planning** this group can only open certain dialogs because the checkboxes Change, Add, and Delete have not been ticked. In module **Utilities** this group cannot open the dialogs **Order info** and **Debtors/Creditors to FinAcc** but has full access to all other dialogs of this module. This group has no rights for the modules **Statistics** and **References**.

**Employee: Marc Tender, user**

| Program           | Sub-right  | Execute | Change | Add | Deletion |
| :---------------- | :--------- | :------ | :----- | :-- | :------- |
| Master data       |            | ☑       | ☐      | ☐   | ☐        |
|                   | Partner    | ☑       | ☑      | ☑   | ☑        |
| Documents         |            | ☑       | ☑      | ☑   | ☑        |
| Production        |            | ☑       | ☐      | ☐   | ☐        |
| Statistics        | x          | ☑       | ☐      | ☐   | ☐        |
| Stock             |            | ☑       | ☐      | ☐   | ☐        |
| Capacity planning | x          | ☑       | ☐      | ☐   | ☐        |
| Utilities         | Order info | ☐       | ☐      | ☐   | ☐        |
|                   | Debt./Cred. | ☐       | ☐      | ☐   | ☐        |
| References        | x          | ☑       | ☐      | ☐   | ☐        |
*x: all rights (no entry)*

The user Marc Tender belongs to the group **Users**. He has also full access to the modules **Statistics**, **Capacity planning**, and **References**. He can also enter, edit, and delete partners in master data.

## Input of User Data

When you enter the data for a user you have to define the so-called real name. Once saved, this entry cannot be changed.

You also have to enter a password by means of which the user can log into A+W Business. If the login function in connection with the Windows login is active in company data, the user name and the password for the Windows login must be entered in A+W Business.
(⇨ Software Reference, "Use Windows registration for A+W Business login" on page B-973)

> **Prerequisite**
> You can enter new users only if you have system administrator's rights.

There are the following instructions on this subject:
*   "How to enter a user" on page B-391
*   "How to copy the standard settings for documents" on page B-393

> **Data protection**
> Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights.

In the following steps, a trainee for stock management is defined who belongs to the **Users** group, with limited rights.

### How to enter a user
1.  Go to menu **Master data > Company > Employees**. Dialog `Employees` appears.
2.  Go to the menu **Start > New** to switch to the input mode.

*(Fig. B-240 shows fields for new employee data are accessible.)*
*   **A** Real name
*   **B** Domain
*   **C** Login name

3.  Enter the data in section **Identification**:
    *   **Name (plain)(A)**: Employee's name, preferable the last name. Once saved, cannot be changed. The real name is saved with every action the user performs in A+W Business. The real name appears on selection lists, e.g. at order entry.
    *   **Domain (B)**: Name of the domain if the computer is installed in a network.
    *   **Login name (C)**: Name the employee uses to log into the system.
    The other fields are not mandatory. For external users, communication data may be useful for instance.
4.  Go to tab **Specification**.
5.  Tick the checkbox **Restrict documents to client (B)** if the user may only enter documents for a certain client. The combo box for selecting the client (A) is accessible. If this checkbox is not ticked, the user can enter documents for all clients.
6.  Choose the client if required.
7.  Enter the password (C) the employee has to use for identification. The user can change this password when he logs into A+W Business.
8.  Select the group (E) to which the employee shall belong. When he is allocated to the group, the user will get all rights granted to this group. These can be modified as required.
9.  Select the language (F). This setting only refers to the language of the main menu.
10. Select the printer and the fax.

All necessary data have been entered. If you save your entries now, the real name cannot be changed any more. You can immediately delete the employee's data however. Once he has logged into A+W Business he cannot be deleted.

*(Fig. B-241 shows specific settings for calling A+W Business.)*
*   **A** Client for which the user is working
*   **B** Restricting the document input
*   **C** Password
*   **D** Locking a user
*   **E** User group
*   **F** Language

11. Select in the menu **Start > Save** to save the data. The data will be saved. Tab `Settings` is accessible. You can add further data and amend the user rights now.

### How to copy the standard settings for documents
1.  Go to tab **Settings** and select the user whose settings you want to copy.
2.  Go to tab **Settings**.

*(Fig. B-242 shows the 'Copy user settings' dialog.)*
*   **A** Source
*   **B** Copy the setting button
*   **C** Target user
*   **D** List of employees

3.  Go to combo box **Target (C)** and select the new user.
4.  Click on **[User settings] (B)** to copy the settings. A safety query appears and allows checking the source and the target; these have to be acknowledged. After that, the settings will be transferred. You can amend these settings as required.
5.  Select the new employee from the list (D).

*(Fig. B-243 shows how to amend the user settings after copying.)*
*   **A** Adopted setting
*   **B** Amend the settings

The setting for the document type `P.O.` (A) was adopted. Please note that the settings in the individual columns can be amended only if the column **General** shows the entry `<disabled>`.
6.  Choose the standard settings for the other document types and for the order areas (B). Click on a line to select the required data from the combo box.
7.  Select in the menu **Start > Save** to save the data. The data will be saved.

> **Deletion of data**
> The user's data can be deleted before he logs into the program for the first time. To do this you have to enter your password for the system. If rights had already been allocated they have to be deleted first.

## Change Password

The password for logging into A+W Business can be changed by the corresponding user.

### How to change your password
1.  Click on the icon for starting A+W Business.
2.  Tick the checkbox **Change password**.
3.  Enter your old password and your new password in the appropriate fields.
4.  Enter the new password again in field **Confirmation**.
5.  Click on **[OK]** to save the data.
    The password is changed; A+W Business is started. Next time you start A+W Business you have to untick the checkbox `Change password`.

## Locking of Users

User data cannot be deleted once the user has been working in A+W Business. You can block his access to A+W Business however.

### How to lock a user
1.  Go to menu **Master data > Company > Users**. Dialog `Employees` appears.
2.  Go to tab **Employee** and select the user to be locked.
3.  Go to tab **Specification**.

*(Fig. B-244 shows the 'Locked' checkbox for a user.)*
*   **A** Checkbox

4.  Tick the checkbox **Locked (A)**. The user can no longer work in A+W Business and cannot be selected from the dialog combo boxes either.
5.  Select in the menu **Start > Save** to save the data. The data will be saved.

## Editing of User Rights

A user normally gets the same rights as the user group to which he belongs. These rights can be extended or restricted. If the user is allocated to another group he will automatically get this group's rights. You can complete these rights by copying the rights of another group so that the user is granted the rights of both groups.

> **Prerequisite**
> User rights are defined for a group or for a single employee. Rights can be allocated only if both the group and the user have been entered before.

There are the following instructions on this subject:
*   "How to complete user rights by copying" on page B-397
*   "How to restrict user rights" on page B-401

The following steps describe how rights can be defined quickly and easily by means of the copy function.

### How to complete user rights by copying
1.  Go to menu **Master data > Company > Employee rights**.
2.  Go to menu **Functions > Copy rights**.

*(Fig. B-246 shows the 'Copy employees' rights' dialog.)*
*   **A** Select the source
*   **B** Define the target
*   **C** Delete or keep existing rights

3.  Choose the group in section **Source (A)**. In this example, the rights of a group shall be transferred to an employee.
4.  Choose the employee in section **Target (B)**.
5.  Decide whether the existing rights (C) shall be deleted or kept:
    *   When you tick the checkbox, all rights of the target will be deleted and replaced by the source's rights.
    *   If you do not tick this checkbox, only the rights that had not been granted before will be transferred.
    In this example, the existing rights are completed by the new rights: The checkbox is left unticked.
6.  Click on **[OK]** to start copying. When this process is completed, a message pops up showing the number of rights that have been transferred.
7.  Acknowledge the message and close dialog `Copy rights`.

The rights of the new group or of the new user are listed in dialog `Management of rights` in section `Overview`. You can now edit the rights if required.

### How to edit user rights
1.  Go to menu **Master data > Company > Employee rights**. Dialog `Management of rights` appears.
2.  Select the option **Employee** and choose an employee. The group and the employee appear on the list.
3.  Open the list of existing rights by clicking on `[+]`. The list shows all rights granted to the employee or group of employees. For all program items or dialogs that are not listed, unlimited rights apply.
4.  Select the program item for which the rights shall be changed. The rights are shown in the checkboxes (B).
5.  Go to section **Rights** and tick the checkboxes (B) to restrict the right as required:
    *   **Change**: Data can be edited.
    *   **Insert**: New records can be entered.
    *   **Delete**: Records can be deleted.
    *   **Execute/read**: The dialog can be opened.
    Please note that when a checkbox is left unticked, the corresponding right will be withdrawn. If you tick e.g. the checkbox `Execute`, the user can open the dialog in question but cannot edit it.
6.  Go to the menu **Start > Save** to save the changes. The new rights for the user will be saved and come into force next time he logs into A+W Business.
