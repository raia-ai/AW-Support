---
title: "A+W Enterprise iQuote Configuration Instructions"
source: "EN-CONFIG-AW_Enterprise_iQuote_1.pdf"
tags: ["A+W Enterprise", "iQuote", "Configuration", "Workflow", "Master Data", "ICE Environment", "Multi-language", "Software for Glass", "Technical Manual", "System Setup"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed configuration instructions for A+W Enterprise iQuote, a webshop solution for configuring glass product orders. It covers prerequisites, installation, version updates, master data consolidation, and environment variable setup. The guide is intended for technical personnel responsible for deploying and maintaining the A+W iQuote system."
long_description: "This is a comprehensive internal configuration manual for the A+W Enterprise iQuote software. It outlines the necessary steps to set up and customize the iQuote environment, which functions as a webshop for glass product configuration and ordering. The document details the required infrastructure, including A+W Windows services and the ICE (Internet Communications Engine) environment. It provides a full change history, version update instructions, and a complete list of relevant A+W Enterprise environment variables with their descriptions. A significant portion of the manual is dedicated to Master Data Consolidation, explaining how to configure product groups, exchange groups, geometry, employee logins (including Okta integration), and various article master data settings like BOMs, processings, and procurement times. The guide also covers advanced topics such as LAMI inheritance logic, multi-language support setup across database tables and workflows, and the configuration of A+W iQuote Services and Web front end, including multi-client capabilities. It serves as an essential reference for system administrators and implementation specialists."
---

# A+W Configuration Instructions: A+W Enterprise iQuote

**-INTERNAL-**

*A+W - Software for Glass*

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2022-03-15 | Alexander Weil | Creation/transfer from Enterprise config | 1.0 |
| 2022-03-24 | Alexander Weil | 2. Configuration of the ICE environment shifted | 1.1 |
| 2022-05-31 | Alexander Weil | Projects and project prices | 1.2 |
| 2022-05-31 | Alexander Weil | Document structure rearranged | 2.0 |
| 2023-02-02 | Ina Seifert | Master data maintenance reworked; Countersunk drillings added | 2.1 |
| 2023-02-21 | Alexander Weil | Expansion of the workflow configuration: Workflow Core | 2.2 |
| 2023-03-07 | Elena Tempelfeld | Format adjustments!!! | |
| 2023-03-15 | Alexander Weil | Environment variables chapter added | 2.3 |
| 2023-04-19 | Alexander Weil | Status reports | 2.4 |
| 2023-05-09 | Alexander Weil | Multi-Language Support | 2.5 |
| 2023-05-26 | Alexander Weil | Restriction violations | 2.6 |
| 2023-08-10 | Alexander Weil | Sketches Memrel export | 2.7 |
| 2023-08-29 | Alexander Weil | Workflow core upgrade | 2.8 |
| 2023-09-18 | Alexander Weil | Pick-up as procedure note | 2.9 |
| 2023-10-10 | Alexander Weil | Country code/Country selection in delivery information | 2.10 |
| 2023-11-22 | Alexander Weil | Restructuring points from chapter 9 - Configuration | 3.0 |
| 2024-02-14 | Alexander Weil | Okta Login Page | 3.1 |
| 2024-11-25 | Alexander Weil | Dispatch type | |
| 2024-11-25 | Alexander Weil | Restructuring of some section points in delivery information | 4.0 |
| 2025-05-22 | Alexander Weil | Geometrie / Modelle: Shape sketches are urgently required | 4.1 |

## 1. Introduction

Set-up files such as the infrastructure workflow templates and images can be found under `\\jupiter\ALCIB_Install\A+W iQuote Enterprise\`.

For additional A+W iQuote configuration instructions with regard to front end or A+W Infrastructure, check the EN-CONFIG-A+W iQuote.

### 1.1. Infrastructure

Use of A+W iQuote includes three components in an A+W Enterprise environment:

*   A+W iQuote as webshop for configuration of orders
*   The Web.Configurator.Service as interface to A+W iQuote
*   The documentservice as interface to A+W Enterprise and the A+W Enterprise database

The functionality is available starting with Build 13.04.xxx of the documentservice.

The basic development refers to case #297410 A+W iQuote.

With case #452497, an enhancement was made.

### 1.2. Prerequisite

*   ICE environment is configured
*   The documentservice application under Unix is required (binary)
*   Required A+W Windows services installed via the A+W SetupLauncher:
    *   A+W Enterprise 6 Frontend
    *   A+W Infrastructure 6
    *   A+W CAD Services (not to be confused with the A+W Enterprise CAD Service)
    *   A+W CAD Designer (Shapes)
    *   A+W CAD Designer (Bars)
    *   A+W Commercial 6 Converter Services
    *   A+W iQuote 6 Services
    *   A+W iQuote 6 Web

### 1.3. Installation

For installation, the document EN-INST-A+W Enterprise iQuote should be used.

### 1.4. Version update

Critical update for version closing via quality release

#### 1.4.1. 2022/11 - Quality Release 11 from 2022

In Quality Release 11 from 2022, there are two important changes in A+W iQuote, which must be heeded during an update.

The database script **00000211.awdb** is required for the AWSOA database. For this, the infrastructure should be updated. If the customer doesn't want an infrastructure update, then you can store the database script **00000211.awdb** in the directory `(C:\SANDPIPER1\InfrastructureServices\Database\AWDB)` intended for this. The script supplies you from a current test system, e.g. AWEAWP60. After starting A+W iQuote, the script is executed automatically.

Thanks to the new load distribution in A+W iQuote, it is now necessary that the property **AW.MultiSite.Worker** is set in the A+W iQuote Web.Configurator and the document service.

For information and configuration of the load distribution, see chapter "Load distribution"

**Brief info about the Worker property:**
The property `AW.MultiSite.Worker` must be set on the Document Service instance (e.g., `AWEDEV-RHEL7-Commercial-130-Document-130-001`). For example:

*   **Name**: `AW.MultiSite.Worker`
*   **Value**: `001`

For the configuration of the property in the A+W iQuote Web.Configurator, after setup via the SetupLauncher, you will be led through with the subsequent Config tool.

For the documentservice, you should execute the Unix scripts **iceconfig_setup** and **iceconfig_execute** again.

**Very important is that the number of workers on the Windows services and the Unix services of a client is the same.**

For more information, please see chapter "Lastenverteilung Frontend und Dienste".

#### 1.4.2. 2023/02 - Quality Release 02 from 2023

In this Quality Release, some changes were made with respect to multilingual function [AW-81485]. The first part of the development was completed and gives the customer the opportunity to change the language via drop-down list.

The list is generated from the languages of the Infrastructure.Web (Infrastructure.Web > Master Data > Languages). This development is not yet complete and has influenced a few central selects on the database. When importing at the customer's, please pay attention to which languages are released in the Infrastructure.Web. Because there could otherwise be missing data if translations are missing at the customer's. And during the installation of the Windows components, please make sure that the documentservice is also provided.

In addition to these serious changes with regard to language, details for the article selection were undertaken, which also influence the workflow setup. This is why the chapter **Workflow Core** and its subchapters **Art. Type** and **Article group** were written. We hope that this chapter will bring a bit of clarity about article selection in A+W iQuote and the document service.

#### 1.4.3. 2024/10 – Quality Release 10 from 2024

With BugItem 129598, the PDF copy target path was adjusted. When printing for the A+W iQuote and the associated PDFCopy logic, now the files are stored in the path under the `DATEI_REF_PFAD` with document number and subfolder 0, e.g.
`\\aweawpvnext.tse.intra\Trans\AWE\dokuserver\140\500563\0`

This modification was necessary since the old path is not suitable for the document attachment. With this modification, all document files are now stored centrally.

The old printouts are nevertheless found for the PDF download since this path is determined from the `kaufdruck` data.

> **Note:**
> It is urgent that you pay attention that in the stored procedure `rppdfcopyfilename`, which handles the naming of the PDF copy of the printout, all form types used are included in the SP and get unique names. Precisely for the form types that process documents that can contain subnumbers (e.g. delivery note), the subnumber in the name is important so that the uniqueness of the file names can be guaranteed.

## 2. Configuration of the ICE environment

The description of the installation and configuration of the ICE environment is in the system configuration instructions (DE-CONFIG A+W Enterprise System.pdf or EN-CONFIG A+W Enterprise System.pdf).

## 3. A+W Enterprise environment variables

This chapter lists the A+W Enterprise environment variables used for A+W iQuote in short form. For more precise information about configuration relating to the individual environment variables, please read the existing configuration descriptions.

| Environment variable | Value (default/example) | Description |
| :--- | :--- | :--- |
| **AWSOA_ICEHOST** | - | Name of the host on which the A+W Service Locator is running. |
| **AWSOA_ICEPORT** | 12000 (default) | Port on which the A+W Service Locator can be reached. |
| **AWSOAFTEST** | 1 – 9 (Ftest Level) | Activation of FTests for A+W SOA services. |
| **AWSOA_LOGLEVEL_DOCUMENTSERVICE** | 0 – 4 (Loglevel) | Log for the documentservice (A+W iQuote). 0-Fatal 1-Error 2-Warning 3-Info 4-Debug. File: PROTOPFAD\awsoa_documentservice_xxxx |
| **AWSOA_EXPLAIN** | ON or OFF | Enables measurement of the database queries of the AWSOA Backend services. |
| **IQUOTE_IGU_TESTLEVEL** | 1 | For IG, the restriction check can be expanded to the 1st level (glass). |
| **IQUOTE_LAGER_HANDLING** | | Here, the handling time for stock articles in iQuote is stored in days. |
| **IQUOTE_LEERE_BEARB_MELDEN** | ON or OFF | A restriction error message is sent if at least 1 parameter is missing completely and so display is not possible. If a minimum of parameters is there, then additional restrictions can also be checked for the individual parameters from the AWE master data. |
| **IQUOTE_VSG_VERERBUNG** | ON / OFF | Client reference: yes. The special inheritance logic for LAMI in A+W iQuote is activated, which does not map any of the std. LAMI inheritance (AWE, ITOE), but only provides an entry aid where, depending on the BOM structure of the LAMI BOM (1st level atyp183 BA=Lager or Prod/Best the processing entered in A+W iQuote is transferred to the individual lites or to the header article. |
| **IQUOTE_PASS_PROCESS_DOWN_1** <br> **IQUOTE_PASS_PROCESS_DOWN_2** <br> **IQUOTE_PASS_PROCESS_DOWN_3** | A+W processing types | Client reference: no. Here and in the 2 additional ENVs, AWtypes are listed that are inherited via iQuote LAMI inheritance to the subelements. Only applies for iQuote inheritance that is activated with IQUOTE_VSG_VERERBUNG. List separated with `|`. |
| **IQUOTE_WITH_PPARAM_TEST** | ON or OFF | Enables restriction check of the processing parameters in A+W iQuote. |
| **ARTIKELBILD_PFAD** | | This variable describes the root directory for the article images. The article images themselves are maintained in the article master data and are then below this path. |
| **ATTACH_PRINTOUTS_TO_DOCUMENT** | | The environment variable controls whether a PDF copy of a printout should be attached to the document. If the environment variable is set to 1, only printouts from A+W iQuote (kauf.eingang = 14) are processed. If the environment variable is set to 2, copies are created for all documents. In addition to the environment variable, the Stored Procedure `rppdfcopyfilename` must be created. (#439086) |
| **DATEI_REF_PFAD** | | The path for files that are assigned to an order or an order item is stored in this variable. The maximum length of this path is 199 characters. (AWDesk #83527). If created site-specifically, always create a global site with site=0!!! |
| **IQUOTE_ALL_CUSTOM_STATUS** | ON or OFF | A+W iQuote Status is written for all A+W Enterprise procedures. |
| **IQUOTE_DISPLAY_ORDER_DAYS_BACK** | | Number of days that the A+W iQuote history should look back. |
| **IQUOTE_SHOW_DEFAULT_DELIVERY_TIME** | ON or OFF | Switches on the default delivery display for articles. |
| **IQUOTE_WITH_PRODEARULES** | ON or OFF | Client reference: no. Activates the evaluation of general product E/A rule in iQuote. Additional rules and exchange rules for the edgework are loaded. Please make sure that the elements that can come into the BOM via this Z-rule are not changed in iQuote. A special logic also for A-rules for edges. This is described in the documentation. |
| **IQUOTE_LOGIN_PRIVATEKEY** | | The A+W iQuote login key is stored in this environment variable. The private key is required for comparison with the connected login provider. |
| **IQUOTE_LOGIN_REMOTE_ADDRESSES** | | In the environment variable, the permitted IP addresses for the A+W iQuote Login Provider are stored separated by semicolons. The IP address sent by the A+W iQuote Login Page is compared to the addresses stored in the environment variable and login is rejected if they are not the same. Local host is "::1". |

## 4. Master data Consolidation

For the master data maintenance, it has to be noted that this is only the basis for correct data acquisition. For large parts of the configuration, adjustments to the workflows (see A+W Infrastructure 6 Workflow Studio) must be made. As basis for the workflows, standard workflows are provided and there are additional templates from development (see `\\jupiter\ALCIB_Install\A+W iQuote Enterprise\`).

For the creation of master data, the documentservice must be restarted. Articles are, for example, stored temporarily and loaded from this storage if they were read out of the database once.

### 4.1. Key

The prerequisite for the adjustment of the master data are a few new key data.

#### 4.1.1. Product groups

In A+W iQuote, it can be defined via workflows whether the grouping is done via the A+W article types or individual article groupings. (see A+W Infrastructure 6 Workflow Studio).

If you want to work via individual article groups, appropriate language-specific article groups must be created in A+W Enterprise (Master Data > Keys > Products > A+W iQuote-specific details > Article group). The numbering and name can be defined at will. Only the article group 1 is permanently reserved for processings.

If you want to distinguish between articles with fixed, unchangeable BOMs and articles with changeable BOMs, you must create separate article groups for this.

Finally, the article groups must be referenced in A+W iQuote via workflows. If you would like to work with unchangeable BOMs, it must be set for the corresponding article groups in the workflow that processings and exchange are not possible.

In A+W Enterprise, the defined and referenced article groups can then be in Article master data assigned to the articles.

##### 4.1.1.1. IGU technical values grouping

If you want to set up the IGU grouping for technical values, then you must maintain the following master data information.

In the technical values (Master Data > Keys > Products > Technical Values > Groups), at least one group must be created for the value in question (sound, heat, energy).

In the article master data (Master Data > Articles > Techn. Values), these groups must be assigned to the desired insulating glass.

#### 4.1.2. Exchange groups

For the exchange in A+W iQuote, not all variables possible in A+W Enterprise are allowed. Under Master Data > Keys > Products > A+W iQuote-specific details > Exchange Groups > All Descriptions first you specify the required groups for article and spacers. Attention has to be paid that the groups are maintained in all languages used, otherwise the documentservice may later not find a data record if the required language was not maintained.

After that, under Master Data > Keys > Products > A+W iQuote-specific details > Exchange Groups > Group Allocation (article or spacer) you assign the exchange groups the required articles that should be offered for exchange.

If you have created an exchange group, it is initially empty and can be used in two ways in the group allocation. The first possibility would be glass or other products, such as gas. The second possibility affects spacer articles. If then an article is taken into the exchange group, then this group can only be selected under the respective dialog (article or spacer).

If the exchange groups were defined, these groups have to be assigned to the possible articles for exchange of the insulated glass BOM in the article master data (Master data > Article > [F4] > BOM > Groups). The exchange groups can be assigned separated with '|'. (max. 10 groups).

> **Attention:** Currently (02/2023), only the exchange within insulated glass (IGUs) is supported. Glass or foil exchange in LAMI is not possible.

#### 4.1.3. Geometry / Shapes

The geometry data is loaded into the internal cache at the start of the documentservice from the table "modelle". The shapes that should be available in A+W iQuote must be set in the A+W Enterprise master data to online "yes", belong to the catalog type = 0. The names must be maintained in all languages used.

Please make sure that the approved shapes have a sketch in iQuote. The sketches are loaded from the folder `C:\SANDPIPER1\CADServices\Geometry\Shapes`. Shape number is the same as the sketch's .svg file name. If in iQuote a shape is present without sketch image, there is otherwise incorrect behavior in the display data field.

### 4.2. Employee/login

The login of the iQuote is maintained in A+W Enterprise via the employee master data dialog (Master Data > Employee). For the A+W iQuote user, an employee profile must be created and a login + web password assigned in this profile. The decision whether the user should use an e-mail address or another user name as login is left to the company. For the A+W iQuote, the Web login name must be entered in the login data field.

Starting with QR 2310, for the A+W iQuote of A+W Enterprise, there is now a login check implemented via the password stored in the Linux (Unix) system analogous to the A+W Enterprise login. If the Linux logins are synchronized via an Active Directory service, the password is thus checked in the Active Directory. If an employee would like to log in using this login process, then there may be no entry in `mitarb.winpasswort`.

> **Rights do not have to be assigned to the employee created!**

The employee created can now be assigned to a market partner on the market partner master data dialog (Master Data > Market Partner). In order to be able to enter with A+W iQuote, an employee may only be assigned to one market partner. Otherwise, this user is refused access to A+W iQuote. The assignment of an employee to a market partner is managed under the user allocation (Master Data > Partners > [F4] > Staff allocation > User allocation). If an employee should be assigned to several market partners, then a warning message is displayed in the user allocation that A+W iQuote operation is omitted.

#### 4.2.1. Okta Login Page

The Okta login page configuration is done in two steps. The users need an account with www.okta.com and an employee in A+W Enterprise to whom a market partner is assigned.

You can first create the users in A+W Enterprise, as described under 4.2 Employee/Login. To be noted is that you must enter the customer e-mail address on login. It is not possible to work with user names. You don't have to store a password since the passwords are maintained via Okta.

For additional information about configuration of the Okta login page, see chapter 19. Okta Login Page.

### 4.3. Article master data

For articles from A+W Enterprise, on the article master data dialog (Master Data > Articles) settings must be made so that they can be used correctly in A+W iQuote.

#### 4.3.1. Sale items

So that articles (element) from the A+W Enterprise can be used in A+W iQuote, the online flag (article.verkart=2) must be set on the article master data dialog (Master Data > Articles > Phys. Properties > Sales Type).

#### 4.3.2. Customer-specific article name via stored procedure [AW-193055]

In A+W iQuote, it is now possible to expand the article name of the A+W iQuote article. To activate the logic, the stored procedure: `cu_getcustomproductdesc` must be set up. There is a template in the back end under `/develop/sql_scripts/cust/st/cu_getcustomproductdesc.sql`. Please note that if the SP is activated, only the SP for article name determination is used!

#### 4.3.3. Article group

As already mentioned in Product groups, there is a distinction in A+W iQuote whether or not you are working with the A+W Enterprise article groups. If you have decided on the A+W Enterprise article groups, then all articles used in A+W iQuote should be assigned the appropriate article group.

For all articles of article type "part" (artikel.teilflag=1), a product group can be maintained if this product has the online flag. For articles of article type "Part", the assignment of an A+W iQuote product group is only necessary for intended grouping by product group. A product breakdown per product type can also be set up; then a product group set-up is not necessary (see Article group).

For articles of the article type "processing" (teilflag=0), it serves to mark the representative A+W iQuote processings (prototypes). For representative processings, an assignment is always necessary if this processing should be supported in A+W iQuote. The product group of the processing must absolutely be 1.

#### 4.3.4. Replacement product

Exchange articles can now be set in the article master data to "Yes+Online" via sub-element toggle (Article > Phys. Properties > Sub-Element). Therefore, the article does not have to be released as a sales article.

#### 4.3.5. BOM/exchange

So that an exchange of glass can be made for insulating glass, in the article master data (Master Data > Articles > Phys. Properties), the toggle data field "BOM" must be set to "yes/changeable", otherwise the exchange dialog will not be displayed in A+W iQuote.

> **Attention:** Currently (02/2023), only the exchange within insulated glass (IGUs) is supported. Glass or foil exchange in LAMI is not possible.

So that the inner spacer is displayed correctly in the BOM, a standard AIR has to be maintained for the market partner used (Master Data > Market Partner > Order) or for the insulated glass selected (Master Data > Articles > Menu > Dimensioning > Mandatory Dimensions).

If the Exchange groups were defined, these groups have to be assigned to the possible articles for exchange of the insulated glass BOM in the article master data (Master data > Article > [F4] > BOM > Groups). The exchange groups can be assigned separated with '|'. (max. 10 groups).

#### 4.3.6. Processings

**Overview**

In A+W iQuote, the following types of processings are intended:
- Arrissing (awtyp = 1000)
- Grinding (awtyp = 1005)
- Polishing (awtyp = 1010)
- Mitering (awtyp = 1015)
- Beveling (awtyp = 1020)
- Drilling (seamed, ground, polished) (awtyp = 1100)
- Countersunk drilling (seamed, ground, polished) (awtyp = 1100)(starting with QR 2302)
- See additional details about master data creation
- Corner cut-off (seamed, ground, polished) (awtyp = 1305)
- Corner cutout (seamed, ground, polished) (awtyp = 1300)
- Round corner (seamed, ground, polished) (awtyp = 1310)
- Edge cutout (seamed, ground, polished) (awtyp = 1400)
- Inside cutout (seamed, ground, polished) (awtyp = 1415)
- Macro (seamed, ground, polished) (awtyp = 1900)
- Surface macro (seamed, ground, polished) (awtyp = 1910)

In A+W iQuote, only 1 edge processing per edge is allowed. If a product already has a processing in the master BoM and you apply another in A+W iQuote, then the existing edge processing on the edge is removed automatically and the new one is applied. If the new edge processing is applied to all edges, then the old edge processing is removed via an A/Z delete rule generated by the system. That's why it is important that the environment variable `AZ_DELETE_TYP` be active. Since in the normal A+W Enterprise we always warn against DELETE E/A rules, we will consider another logic for A+W iQuote. But in the existing versions, this dependency is there. (Status as of 07/04/2023)

[AW-157665] / October 2023
In A+W Enterprise iQuote, generally only one edge processing of the A+W processing types arissing/grinding/polishing is allowed per edge. IF the product itself has an edge processing of this A+W processing type in the master BOM, then it is deleted from the BOM and the newly entered one inserted. If the new processing is not selected on all edges, then the new processing is inserted only for these edges and the processing from the master for the complementary edges. This also applies if different processings are applied to the individual edges. Attention must always be paid that each edge has only one edge processing of these A+W processing types. If several are applied, then the entry encounters an error and the processings must be adjusted accordingly in A+W Enterprise iQuote.

**Display of standard processings**

By default, processings that in the master BOM are on "Print no" are not displayed as text in A+W iQuote. However, they are marked in the SN Live sketch. This can cause irritation for the user.
QR2308 [AW-149355]: In the master BOM, for the elements that should be visible in A+W iQuote for textual display but should not appear on papers set a separate print identifier "Q". Only processings of a BOM can be made visible with this identifier.
As an aid, a tool tip was stored for the "Print" field.
(see also "EN-CONFIG-A+W Enterprise" - section "Article master data - BOM")

**Processing assignment**

The master data processings for the A+W iQuote entry should be entered in 2 stages.

**Prototype/representative processing**

For each A+W processing type that should be used in A+W iQuote, a representative article must be created (prototype). For all non-edge processings, one article per edge quality must be created. For these articles, you store a previously created A+W iQuote article group for processings in the "Article group" field. The product group (Master Data > Keys > Products > A+W iQuote-specific details > Article Groups) for the processing must be assigned 1 since the documentservice with the product group (artikel.bearbkat) equal to 1 looks to see which processings may be applied.

For the article dimensioning, a record should be present for each dimensioning type (mtyp: Absolute (=0), by 2 edges (=1), by corner and edge (=2)) with a fixed edge quality (1100 = seamed, 1005 = ground, 1010 = polished).

All other intended parameters should be on "variable" and have no default values. These processing articles require no price data in the master, because they are exchanged depending on the glass product.

QR2302/ [AW-124712]
For the prototype processing, default values can be entered in the article dimensioning. IF a processing is selected in A+W iQuote, then the parameters that are stored as defaults in the master data apply for the display. If the default parameters are missing, the processing cannot be displayed on the sketch. Even if a crucial parameter is set to 0, the display is not possible.

If the display is not possible in A+W CAD Designer (Shape), this processing will also not be included in the BOM of the order item. In this case, it is now possible to configure that an error message (restriction error) is sent that the parameters are missing. The user must either enter the parameters or remove this processing in A+W iQuote. (Environment variable: `IQUOTE_LEERE_BEARB_MELDEN`)

**Processing assignment/exchange rules (general)**

Under online processings (Master Data > Keys > Products > A+W iQuote-specific details > Processing assignment) you can define which to specific A+W Enterprise processing article the prototype is assigned.

This will be explained in general in this section. For Special processing types, however, specific extensions apply, which are documented at the end.

Access to this dialog can be restricted with the glass type. If no type is specified, then all exchange rules are loaded.

On the left side, you enter the representative processing article that presents it to A+W iQuote and is used for display. On the right side, you enter a valid processing that with the glass product type is installed in the BOM if this processing is selected in A+W iQuote. (This data is saved in the table `kuaz` with `kunr=-2`.)

It is also possible to store more than one 1:1 assignment, which is irrelevant for seaming, grinding, and polishing. You can also define the exchange through processing parameters. In the detail view, you can store the restrictions for max. 2 processing parameters. You should make sure that a rule without restrictions is always present so that a processing will always be found. The checking of the restrictions is done one after another "starting with dimension". Thus, for a representative "drilling seamed" an article "drilling seamed" starting at 10 mm, another starting at 50 mm, etc. can be stored.

If the master data for e.g. FLOAT glass is stored completely, then the additional glass types can follow. If at the start of menu element the glass type 110 (cast glass) is selected and there is no master data for it, then the user is asked whether the data should be copied from another glass type. The data is then taken over completely and can be adjusted or retained.

**Special processing types: Countersunk drillings (1110)**

QR2302 [AW-131283]: Entry in A+W iQuote of the A+W Enterprise has been expanded to include the A+W processing type countersunk drilling.

**Master data maintenance:**
A prototype article for countersunk drilling (awtyp=1110) per edge quality must be created. For this article, ALL parameters should be permitted ("variable"). Alternatively, the parameters can be pre-populated with values. If default values are already defined, these processings will be pre-populated in A+W iQuote immediately with these values and the processing is visible on the sketch. Furthermore, the edge quality should be set to "fix" + a value entered.

If the prototypes have been entered, now the exchange rules for the A+W iQuote processings must be entered (Master Data - Keys - A+W iQuote-specific Details - Processing Allocation). Each of the prototype articles should be redirected to an A+W Enterprise processing. For the countersunk drilling, 3 parameters are activated for the restrictions: "Diameter", "Diameter bottom", and "Diameter top". However, only the main diameter is checked directly as a dimension. The two other parameters are only for the case that "Countersunk drilling bottom" and "Countersunk drilling top" are redirected to another A+W Enterprise article and priced differently.

*Example for prototype article 10199010 "countersunk drilling arrissed" for float glass*

1.  **Case - general rule**
    This would be a "general" rule for the arrissed countersunk drilling that is always taken if no other E/A rule is stored, if "countersunk drilling arrissed" is attached to a float in iQuote. (e.g., redirecting prototype `10199010` to processing article `199003`).

2.  **Case with special diameter**
    If a record is created in addition (e.g., for prototype `10199010`), where a minimum diameter is specified (e.g., `50.00`), then a different processing article (e.g., `99199003`) is used if the diameter is >=50 mm; otherwise, the general article `199003` from the first rule is used.

3.  **Case – additional countersunk hole**
    If you also need a separate processing article for "countersunk drilling top," then you must create another record. The processing article (e.g., `1199003`) is then used if from A+W iQuote only the main diameter and "diameter top" or main diameter and "depth top" are reported, however "diameter bottom" and "depth bottom" are both = 0.
    *   **3.1.** If you also need a separation with regard to the diameter of the main diameter, then you need another set of rules (e.g., for diameters >= 50mm, use article `91199003`).
    *   **3.2.** Accordingly, you would then need rules for "countersunk drilling bottom" (e.g., using article `2199003`).

What's important if you create a "general" exchange rule for countersunk drilling for different main diameters is that you should also create this for "countersunk drilling bottom" and "countersunk drilling top".

The entry of the main diameter is possible and will also be evaluated during the determination. The entries for "diameter bottom" or "diameter top" are not required since with this setting, the entry of the single-sided countersunk drillings is mapped via depths.

It is very important that the A+W Enterprise processings that will be built into the A+W iQuote process in the BOM do not have their own permanently pre-defined processing parameters (only variable is allowed), so that they do not override the parameters reported from A+W iQuote.

#### 4.3.7. Processings for shape edges

The assignment of edge processings for shape edges (Master Data > Keys > Products > A+W iQuote-specific details > Processings for shape edges) has to be maintained separately. If for particular shapes the individual edges (round arc, e.g.) should be mapped with a deviating article (due to deviating price calculation or deviating machine scheduling), then for each processing that was released for A+W iQuote, an exchange processing for shape edges must be stored.

The special edges are maintained under Master Data > Keys > System > Shapes > Edge Processing.

The processings that should be specified on the left side of the dialog must have an A+W type assignment and belong to the edge processings (seaming = 1000, grinding = 1005, polishing = 1010, mitering = 1015, faceting 1020). Furthermore, this processing should be known via an online assignment (artikel.verkart = 2). On the right side, there must be a processing of the same AWType.

**Extension QR2302 [AW-94463]: Separate edge processings for the individual shapes in A+W iQuote**

The dialog for A+W iQuote edge processings for shape edges is expanded by the fields **shape number** and **special edge**.

The already existing old data for the exchange is adjusted automatically when you first enter the expanded dialog (special edges are active). General exchange, which applies for all shapes that are not listed separately, is then entered with shape=0 and special edge.

In addition, it is now possible to store deviating edge processings for each shape.

If a shape in the shape master data (Master Data > Keys > System > Shapes > Edge Allocation) has special edges and "normal" edges, then for this shape, you can maintain the data separately for "normal" edges and special edges. If according to the master data a shape has no special edge, then it is not possible to create an exchange for the special edge.

In the example, for the processing "edges polished" via the general A+W iQuote exchange rule, the A+W Enterprise article `399101` is determined. If the item as shape X (not No.78 and not No.1) is entered with the special edge (e.g. edge 2), then for the normal edges (all edges except edge 2) the processing `399101` is attached to the BOM and for the special edge (edge 2) also the processing `399103`.

If the item with shape 78 (2 edges according to shape catalog) is entered, which has a special edge (edge 2), then for edge 1 the processing `399102` and for the edge 2 (special edge) the processing `399103` is attached.

If the item is entered with shape 1 (no special edges), then the processing `399104` is taken over into the BOM.

#### 4.3.8. Procurement time for calendar

In A+W iQuote, the delivery dates on the calendar are now pre-populated with consideration that the routine days starting on which the earliest possible date is pre-populated [AW-109411].

The determination of the procurement time is done on the item level via the A+W Document Service for the product in question. This is a preliminary date that can be kept under optimal conditions. Final delivery date only follows after acceptance of the data in AWP.

The determination is based on the data stored in the article master data. The procurement time is determined depending on the procurement type:

*   For products with 1. Procurement type "production" the production time
*   For products with 1. Procurement type "PO" the delivery time of the default supplier
*   For stock articles, the processing time is defined via an ENV switch: `IQUOTE_LAGER_HANDLING`.

#### 4.3.9. Default delivery time for articles

With the AWE environment variable `IQUOTE_SHOW_DEFAULT_DELIVERY_TIME` the default delivery time for the articles can be switched on. If the variable is active, then procurement type is distinguished via article; its default delivery time is displayed.

A purchased article is filled with `artikel.stdlz`.
A production article is filled with `artikel.prodzeit`.
A stock article is filled with the value from the AWE environment variable `IQUOTE_LAGER_HANDLING`.

### 4.4. General exchange/addition rules

Generally A+W iQuote works only with standard BOMs.
However, through configuration you can permit a few exceptions and activate the activation of particular general or customer-specific exchange or addition rules.
Only:
*   the additional rules for product/product type or
*   exchange rules for edgework are evaluated.

Environment variable: `IQUOTE_WITH_PRODEARULES = ON`

## 5. Price calculation/exchange

### 5.1. AIR replacement/frame exchange

If in A+W iQuote for an IG only the AIR in the frame was changed, then previously in the BOM an exchange identifier was set for the frame automatically. This caused another price calculation and eventually also errors in the price calculation.

The logic at this point was changed. If it is now detected that the frame is an identical frame with differing thickness (AIR), the original exchange identifier is retained in the BOM. This means, if the frame was previously price-relevant, it also is after changing of the AIR; if it was not previously, no price will be calculated after the change of the AIR.

## 6. Input stop

*July 2025 / documentservice build 13.04.8089*

Within the A+W Enterprise market partner master data, it is possible to define a "Entry stop for orders". This setting can be considered within A+W iQuote for the entry of orders. This happens in the course of the price calculation for the first item.
If for a customer "Entry stop for orders" is defined, the price calculation encounters an error, and the A+W iQuote user receives the message stored for this. The message for this case must be configured individually in A+W Enterprise. This is done under Keys->System keys->Text blocks via the blocks 170-173. The texts must be stored in all active languages. However, not all 4 blocks must be used.

> **IMPORTANT!** If all 4 text blocks are not maintained, there is no check for entry stop.

Entry stop for quotations is not evaluated in iQuote!

## 7. Limit check

*July 2025 / documentservice build 13.04.8089*

Within the A+W Enterprise, it is possible to define a limit and a limit check. If the limit check is active for a customer, it can also be evaluated in A+W iQuote. This happens in the course of the price calculation for the first item.
If the defined limit check fails for the customer, the price calculation encounters an error and the A+W iQuote user receives the message stored for this. The message for this case must be configured individually in A+W Enterprise. This is done under Keys->System keys->Text blocks via the blocks 174-177. The texts must be stored in all active languages. However, not all 4 blocks must be used.

> **IMPORTANT** If all 4 text blocks are not maintained, there is no limit check during entry.

The limit check for iQuote orders is generally executed, regardless of the user's rights.
If the limit is exceeded by the order entered, the order can only be saved by the user. Further along, the order is placed in the release pool with "limit block".

## 8. LAMI inheritance

*QR 2406 // [AW-179138]*

It is possible in A+W iQuote to use a global setting (ENV switch) to activate an inheritance of the processings to the individual lites. This logic cannot be mapped in the LAMI inheritance via iTOE already implemented in A+W Enterprise or via the background process "intauf". Processings added in A+W iQuote are added as individual processings to the individual lites below the LAMIs and not on the header level, as for all other products. This also assumes that the LAMI has a level with the list of the glass and film elements with corresponding assembly positions, in which it is possible to add the processing. The price of the processing is also calculated per lite. The dependency of these processings on one another is only present during entry in A+W iQuote. If the processing in A+W iQuote is deleted again, then it is removed from all subelements. The LAMI processing entered is visible in the list view on the right of the dialog, once on the associated button. Below the picture, in case of inheritance, this is output multiple times (depending on the number of lites in the LAMI). If the document is stored and then later loaded into A+W Enterprise, there is no dependency of the processings on one another. If something should be corrected, then the correction must be done manually on all corresponding processings on the other lites.

Whether the processing on the LAMI is inherited by the individual lites or added to the header element is determined by the structure of the BOM.

*   If a LAMI (atyp 170) has one LAMI stock dimension (atyp 183) on the first level, which has the procurement type LAGER(=5) or PO(=4), the processing is attached to the header level.
*   If a LAMI (atyp 170) has a LAMI stock dimension (atyp 183) on the first level that is set to production and there is a level with glass and film under this, then the processings are inherited.
*   If a LAMI already has glass and film on the 1st level, the processing is inherited.
*   If a LAMI (atyp 170) has another LAMI article on the first level (atyp 170), the processing is added to the header element.

The case that a LAMI has another LAMI on the glass/film level is not supported in A+W iQuote.

If new edgework was placed on the LAMI and the inheritance must be executed, any existing edgework on the individual lites is deleted and the new one inserted. If the inserted one is not linked to all edges, the existing edgework is reduced by these edges.

If you are working with the evaluation of product-specific exchange rules in A+W iQuote, these are also considered.

The logic applies for all processings with the exception of surface processings. No processing is applied to the LAMI header if the BOM is suitable for inheritance and the procurement type is PRODUCTION.

A separate development must be commissioned for the surface processings, insofar as these processings are included in A+W iQuote.

If the inheritance logic should not apply for all edgework (1000 - 1090), drillings (1100 - 1190), corner processings (1300 - 1390) and geometric processings (1400 - 1490), but only for particular AW processing types, this can be entered in the corresponding list of ENV switches (e.g. ENV = "1000|1005|1010|1015|1100|1300|...").

The special logic applies for the inheritance of countersunk holes; the dimensions are converted explicitly for the individual lites. From the conversion, it can happen that a countersunk hole should not be inherited on all lites, but only a drilling. Therefore, it is very important that the data for the calculation (thickness of the individual lites, films) and also the exchange rules for the inheritance in A+W Enterprise (Keys=>Products=->LAMI) are maintained. If the exchange rules for the inheritance are not present, this will cause incorrect results.

Development is based on the current status of the A+W iQuote LAMI detection without glass exchange. If later an exchange of the individual lites in LAMI is commissioned, then the expansion of the inheritance must be ordered along with this. This also applies for the inheritance for surface processings.

**Relevant environment variables:**
```
IQUOTE_VSG_VERERBUNG = ON
IQUOTE_PASS_PROCESS_DOWN_1 = 'X|Y|Z....'
IQUOTE_PASS_PROCESS_DOWN_2
IQUOTE_PASS_PROCESS_DOWN_3
```

## 9. Multi-Language Support

Under the ticket [AW-81485] and feature #41873, the multi-language support for the A+W iQuote of the A+W Enterprise was implemented completely.

Please work through the following points when setting up the customer system so that there is no incorrect data in various languages at the customer's.

### 9.1. Database tables

#### 9.1.1. Core_CustomTexts

The Core_CustomTexts table is found under the AWSOA database and is not an A+W Enterprise Backend table.
The database table must be filled via Inserts/Updates. Currently, there is a maintenance tool for this database table.

| Column name | Type | Description |
| :--- | :--- | :--- |
| guid | Char(36) | Key (must get a unique GUID) |
| versionid | Integer(4) | Version number |
| lockingtoken | Char(36) | Not in use, must be present as "00000000-0000-0000-0000-000000000000" |
| Code | Nvarchar(255) | Variable name that is used by the A+W iQuote or Workflow Studio |
| languagecode | Nvarchar(5) | Language code (reference: core_languages.code) |
| text | Text(56) | Text that should be displayed |
| Description | Text(56) | Description of the text (help text) |

#### 9.1.2. Core_Languages

The Core_Languages table is found under the AWSOA database and is not an A+W Enterprise Backend table.
The Core_Languages table is maintained via the Master data tab in the Infrastructure.Web. The language codes are specified. Please make sure that each language maintained in the Infrastructure.Web is released for the A+W iQuote. Only create languages that are 100% configured.

| Column name | Type | Description |
| :--- | :--- | :--- |
| Guid | Char(36) | Key (must get a unique GUID) |
| versionid | Integer(4) | Version number |
| lockingtoken | Char(36) | Not in use, must be present as "00000000-0000-0000-0000-000000000000" |
| code | Nvarchar(5) | Language code |
| Description | Nvarchar(16) | Language written out |

#### 9.1.3. xsprzu expansion

The back end table `xsprzu` was expanded to include the database field `xsprzu.sprcode`. This guarantees that the customer language and Alcib language do not differ and we have a starting point for data determination for the A+W iQuote. The reason for this adjustment is that some texts that must be determined from the back end are created in customer language and other texts in the Alcib language.

The language codes can be maintained on the A+W Enterprise dialog (Master Data > Keys > System > Languages).

Please make sure that the language codes from the Core_Languages table are entered correctly in the xsprzu table. The query is case-sensitive, so make sure to take upper and lower-case letters into account!

#### 9.1.4. errmsg

Some texts for the A+W iQuote are determined from the A+W enterprise back end data. The table for this is "errmsg". The table is 0-based.

| Name | Type | Description | References |
| :--- | :--- | :--- | :--- |
| errno | integer | Error number | |
| errtxt | char(80) | Error description | |
| manr | integer | Responsible employee | mitarb.manr |
| moddate | date | Date of the last change | |
| moduser | integer | Employee who last changed this record | |
| prgname | char(15) | Module or section | |
| sprache | smallint | Language detection note: Env var $SPRACHE | |

**List of currently used texts (errno):**
22083, 22084, 22183, 22195, 22196, 22588, 22589, 22591, 22592, 22593, 22598, 22599, 28805, 30685, 35728, 36185, 37593, 37594, 37598, 38201, 38203, 38281, 38297, 38334, 38335, 38341, 38367, 35674, 37951, 37389, 37840, 37841, 38255, 37842, 37843, 37839, 37844, 37838, 37837, 37845, 38260, 38259, 36531, 37345, 37347, 37346, 22197, 22400.

### 9.2. Master data

Due to the complete conversion to multi-lingual capability, master data for all released languages must be maintained in the Infrastructure.Web. The necessary master data that should be maintained is listed below.

| Category | Table | A+W Enterprise Path | Description |
| :--- | :--- | :--- | :--- |
| Articles, processings, muntins, exchange articles | artbezfremd | Master Data > Article > [F4] > Additional Descriptions | All designations where articles are at issue. |
| Shapes | Shapes | Master data > Keys > System > Shapes | Shapes in the geometry. |
| Product groups | xsprbez with xiqartgrp | Master Data > Keys > Products > A+W iQuote-Specific Details > Product Groups | Product groups in the article selection. |
| Exchange groups | Xsprbez with xiqchangegrp | Master Data > Keys > Products > A+W iQuote-Specific Details > Exchange Groups | IGU exchange groups (are not displayed in the A+W iQuote front end). |
| Colors | xsprbez with xxfarbe | Master data > Keys > Products > Variants > Colors | All names for the color selection. |
| Countries | xland with xsprbez | Master data > Keys > Partners > Countries | Country names are required for the delivery address in the delivery information. |

If texts for a language should not be maintained, then the particular e.g. articles for the missing language are not displayed.

### 9.3. Interface texts

A+W iQuote obtains the language-dependent screen texts as a message resource; these cannot be changed. Interface texts can be overwritten via the database table `Core_CustomTexts`. Thus, for example, the name of the application can be adapted in the browser or the buttons in the header area if the customer so wishes.

**Selection of the texts**
```sql
SELECT Guid, Code, LanguageCode, Text, Description FROM Core_CustomTexts;
```

After the program start, the "Core_CustomTexts" table is filled automatically with blank texts for the screen translation. This is done in the first language that is entered in the infrastructure languages.

Texts that should also be localized then have to be entered via database insert/update command for the language in question. The value that is obtained by default from the message resource and displayed is in the comment column. It serves as template for the customer's texts. Among other things, this is very important if there are placeholders {0},{1}... in the text. With these default records, you always have an overview of which messages there are. The list adjusts itself. However, nothing is overwritten.

**Inserting a text for the browser application names:**
```sql
INSERT INTO Core_CustomTexts (Guid, VersionId, LockingToken, Code, LanguageCode, Text, Description) 
VALUES (GUID-Function(), 1, '00000000-0000-0000-0000-000000000000', 'WebConfigurator', 'de-DE', 'A+W Buy', '');
```

After the restart of the Web.Configurator Service, the application presents itself under the name "A+W Buy".

Not all interface texts can be adjusted but many buttons and central texts can be replaced. A trick for seeing all text codes in iQuote is to use a script to fill all blank texts with the content of the codes; then the iQuote is only displayed with the codes and the changes can be made efficiently.

```sql
-- Preset all Text with the textcode
UPDATE [AWSOA].[dbo].[Core_CustomTexts] SET Text=Code where Text= '';

-- undo the preset
UPDATE [AWSOA].[dbo].[Core_CustomTexts] SET Text='' where Text=Code;
```

### 9.4. Workflow

It is possible to change texts that are maintained via the workflow for the customer individually. For example, the Workflow tab or if you do not create back end-related product groups such as the subgrouping in the IG exchange and you need multilingual group names for this.

The multilingual texts are managed in the table `Core_CustomTexts`. Currently there is no management program for this. It would make sense to create an Excel table. This could be translated and then Insert Statements created with the help of the Excel table.

```sql
INSERT INTO Core_CustomTexts (Guid, VersionId, LockingToken, Code, LanguageCode, Text, Description)
VALUES (newid(), 1, '00000000-0000-0000-0000-000000000000', <Code nvarchar(255)>, <LanguageCode nvarchar(5)>, <Text nvarchar(max)>, <Description nvarchar(max)> );
```

These must be executed on the AWSOA database for the A+W iQuote.
The language codes (`Core_CustomTexts.LanguageCode`) correspond to the table `Core_Languages`.

In order to assign the texts to the workflows, a global variable must be assigned. This variable must be created in the desired workflow (see screenshot). The user's current language is made accessible via "Cart.CurrentItem.Culture" in the workflow and must be assigned to the variable.

Open the desired workflow in the Workflow Studio and add a `System.Activities.Statements.Assign` element before the workflow core element and enter the values displayed below.
- **To**: `LanguageCode` (create a new string variable with this name)
- **Value**: `Cart.CurrentItem.Culture`

When assigning the culture, you must pay attention to the workflow in which you're working.
- In the main configurator workflow, the assignment is: `Cart.CurrentItem.Culture`
- In the checkout workflow, the assignment is: `Cart.CheckOut.Culture`

In order to use these texts in the workflow, there are 2 possibilities:

1.  **Via function `Configurator.GetCustomText(code, languageCode)`**
    `Configurator.CustomMessage("Test", LanguageCode)`
    This function can be used for all activities, for the properties Category, Description, and Name. To establish a collection, the function can also be used in an expression.
    Example expression for a collection item:
    `New CommonTile() With {.Tileld = 5, .Description = Configurator.CustomMessage("Test", LanguageCode), .Image = "test.png"}`

2.  **Via language code sequence `@@<code>@@`**
    To simplify this, in an activity (not in an expression) without function call, there can be a text determination. For this a "@@" must be placed in front of the message code and attached. The function is then expanded internally and the `Configurator.CustomMessage("Test", ...)` function is called.
    Example: In the Category property, enter `"@@CategoryProduct@@"`.

## 10. A+W iQuote Services + Web

A+W iQuote Web is the front end of A+W iQuote and includes all information so that the A+W iQuote can be displayed via the Web browser.

The A+W iQuote services include the functionality for communication between browser, the Service Locator, and the backend (documentservice).

- A+W iQuote 6 Services (A+W)
- A+W iQuote 6 Web (A+W)

### 10.1. Change of the start page

The A+W iQuote is accessible without configuration change via `computername/web.web`. Many customers would like their own web address to be used for their online presence. So that you can incorporate this web address, a new start page must be created in the Internet Information Services manager (IIS).

For this, in the IIS, you must right-click on Sites and select "Add website" there.

Now in the next step, you can configure a new start page. Here, you can specify the `Web.WebAppPool` directly via physical path (Ex. `C:\Sandpiper1\WebWeb`) or you use an own directory as the default site uses (Ex. `%SystemDrive%\inetpub\wwwroot`).

With the direct path in the AppPool, the folder structure of the WebWeb folder is taken over.

If you do not want to define a new hostname, a new free port must be selected since otherwise the starting point overlaps with the default page. A+W iQuote can thus also be reached via the `computer name:port`.

If a hostname should be configured, that is, another website name/domain, this hostname must be acquired by the customer. This way, the website will run over the new hostname. If necessary, the multi-client number would be displayed behind this. You could hide the multi-client number in the content area with the `index.htm` named below.

With a superior folder structure, you must add the Web.WebAppPool via application.

There should be an `index.htm` file in this folder that serves as the starting point.

**Content example:**
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="refresh" content="0; URL=https://alw-dev22.tse.intra/Web.Web/140" />
<title>iQuote</title>
<style type="text/css">
</style>
</head>
</html>
```

For more precise setting possibilities, please consult Google or a colleague.

### 10.2. A+W Infrastructure 6 Web

The A+W Infrastructure 6 Web is a browser application and can be found in the A+W folder on the desktop. Here, the settings for the A+W iQuote and the A+W Infrastructure can be set up. Some settings have to be made here, which are relevant since A+W iQuote uses the A+W Enterprise functionality.

#### Configuration

The system switches are managed on the Configuration tab. Here, the business case functions (Configuration > A+W iQuote > Business Case Functions) can be set. Particular functions can be switched on and off for the 5 different representatives. Presently, only the customer order is evaluated.

| Business case | Meaning |
| :--- | :--- |
| **Display overviews** | Shall the history/overview be displayed? |
| **Form printing** | Not in use. Controlled from the back end. |
| **Order export** | May orders be saved? |
| **Request order export** | May quotations be saved? Button active for query. |
| **Quotation to order** | Copy quotations in the history to orders [AW-64004]. |
| **Quotation to quotation** | Copy quotation into history [AW-109408]. |
| **Order to order** | Copy order into history [AW-109408]. |
| **Order to quotation** | Copy order in the history to quotation [AW-109408]. |
| **Save shopping cart** | Do you want to save shopping carts not saved yet? If this switch is active, a list of the not completely entered orders or quotations is displayed before each entry into the article selection. |
| **Direct check-out** | Not in use. |
| **Enter quotations** | Permit quotation entry? If desired, also set order export! |
| **Enter orders** | Permit order entry? If desired, also set order export inquiries! |
| **Show prices** | Show price? AWE always on! |
| **Price manipulation** | Not in use. |
| **All documents of history** | Shall all quotations/orders from A+W Enterprise be displayed in the history? Limited to 60 days or can be changed via ENV variable. |

Under the `Commercial > Backend` field there is a drop-down menu that must be set to Enterprise. With it, the A+W Web Configurator controls the correct back end.

Via `System Configuration > Company Logo file name`, a company logo can be set up. The logo file must be in the content folder of the installation directory of the A+W Web Configurator (`C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content`).

Under `System Configuration > Web settings`, a selection of tabs opens on the right. On the Web tab, settings for the appearance of A+W iQuote can be set. The element "Advertising file name" serves to set up advertising images that run in the browser if you are on the log-in and main menu in A+W iQuote. Here too, the images must be in the content folder. To get a better overview in the content folder, you can create the subfolders and then the data field "Advertising file name" can be filled like this, for example: `auw/ads/ads1.jpg;auw/ads/ads2.jpg;auw/ads/ads3.jpg;auw/ads/ads4.jpg`

Similarly, you can create a background image and select a scheme that changes the color design in A+W iQuote.

Similarly, you can see the configuration instructions EN-CONFIG-A+W iQuote for additional information.

#### Workflow

The Workflow tab serves to manage the workflows of the individual expansion points. For A+W iQuote, the following points are relevant:

- **0000 – A+W iQuote**: Product configuration in A+W iQuote
- **0001 – WebConfiguratorMapper**: Not relevant, leave on default.
- **0002 – WebConfiguratorCheckIn**: Dialog window before you get to the product configuration.
- **0003 – WebConfiguratorCheckout**: Dialog window after leaving the shopping basket and before going to checkout
- **0004 – WebConfiguratorDocumentValidation**: Not relevant, leave on default.
- **0005 – WebConfiguratorAddToCart**: Not relevant, leave on default.
- **0006 – WebConfiguratorBackEndUpdate**: Not relevant, leave on default.

### 10.3. Multi-client capability

With the development of multi-client capability (#52389), the problem that you had to provide and install several process servers for several clients was eliminated.

Please ensure during the update that the DB script: `00000211.awdb` is present on the FTP or in the installation folder (`...\A+W\Sandpiper1\InfrastructureServices\Database\AWDB`).

#### 10.3.1. Communication flow

The communication flow of A+W iQuote is as follows, the user operates the A+W iQuote via the browser with an extended web address (e.g. `aweawpvnext.a-w.intra/Web.Web/140`). At the end, the new web address includes the client number to which the company's customer is assigned. With this client number, we can ensure client-specific communication through the system.

Each action in the browser is directed via the Internet Information Services (IIS) direction of the services. This communication runs to the so-called HomeController, where the assignment to the client-specific services is distributed. With the incoming client number, the HomeController determines a web configurator service and passes the action along.

In the web configurator service, a connection to the document service may be required, e.g. for data procurement in the backend. Now the web configurator service searches for a document service using incoming client number and connects with it and the processing of the action can be completed.

**Browser ↔ IIS (HomeController) ↔ Web Configurator ↔ Documentservice**

#### 10.3.2. Configuration

The description of the installation and configuration of the documentservice under the Unix environment is in the system configuration instructions (DE-CONFIG A+W Enterprise System.pdf or EN-CONFIG A+W Enterprise System.pdf). The section Ice environment > Unix > Configuration there must be run through. The scripts mentioned lead the user through the configuration.

Before you undertake the configuration on Windows, you should maintain the clients required and their client numbers in the A+W Infrastucture 6 Web > Master Data > Clients. For the installation on Windows, the setups A+W iQuote 6 Services and A+W iQuote 6 Web must be updated. These setups have config tools that determine the client maintained via the A+W Infrastructure 6 Web. These clients can now be enabled for multi-client capability.

For the A+W iQuote 6 Service, the settings are made in the Service Locator Administrator. You enable the clients that you need and assign a number of workers to these clients. More about the topic of workers and load distribution in the next chapter. Finally, a start port must be selected. All required services are assigned a port number by this port startend.
