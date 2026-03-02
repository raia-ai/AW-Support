---
description: "EN CONFIG A+W Enterprise iQuote"
---



# EN CONFIG A+W Enterprise iQuote

         Configuration Instructions


A+W Enterprise iQuote




                                                                      english




   A+W Software GmbH   EN-CONFIG-A+W Enterprise iQuote.docx   - -INTERNAL-
                                                                      1
Change history

Date         Author                Remarks                                 Version
                                   Creation/transfer from Enterprise
2022-03-15   Alexander Weil                                                1.0
                                   config
                                   2. Configuration of the ICE
2022-03-24   Alexander Weil                                                1.1
                                   environment shifted
2022-05-31   Alexander Weil        Projects and project prices             1.2
2022-05-31   Alexander Weil        Document structure rearranged           2.0
                                   Master data maintenance reworked
2023-02-02   Ina Seifert                                                   2.1
                                   Countersunk drillings added
                                   Expansion of the workflow
2023-02-21   Alexander Weil                                                2.2
                                   configuration: Workflow Core
2023-03-07   Elena Tempelfeld      Format adjustments!!!
2023-03-15   Alexander Weil        Environment variables chapter added     2.3
2023-04-19   Alexander Weil        Status reports                          2.4
2023-05-09   Alexander Weil        Multi-Language Support                  2.5
2023-05-26   Alexander Weil        Restriction violations                  2.6
2023-08-10   Alexander Weil        Sketches Memrel export                  2.7
2023-08-29   Alexander Weil        Workflow core upgrade                   2.8
2023-09-18   Alexander Weil        Pick-up as procedure note               2.9
                                   Country code/Country selection in
2023-10-10   Alexander Weil                                                2.10
                                   delivery information
                                   Restructuring points from chapter 9 -
2023-11-22   Alexander Weil                                                3.0
                                   Configuration
2024-02-14   Alexander Weil        Okta Login Page                         3.1
2024-11-25   Alexander Weil        Dispatch type
                                   Restructuring of some section points in
2024-11-25   Alexander Weil                                                4.0
                                   delivery information
                                   Geometrie / Modelle: Shape sketches
2025-05-22   Alexander Weil                                                4.1
                                   are urgently required




A+W Software GmbH             EN-CONFIG-A+W Enterprise iQuote.docx                   2
Content

1.   Introduction                                                                   6
     1.1. Infrastructure                                                            6
     1.2. Prerequisite                                                              6
     1.3. Installation                                                              6
     1.4. Version update                                                            7
          1.4.1. 2022/11 - Quality Release 11 from 2022                             7
          1.4.2. 2023/02 - Quality Release 02 from 2023                             8
          1.4.3. 2024/10 – Quality Release 10 from 2024                             9
2.   Configuration of the ICE environment                                          10
3.   A+W Enterprise environment variables                                          11
4.   Master data Consolidation                                                     14
     4.1. Key                                                                      14
          4.1.1. Product groups                                                    14
          4.1.2. Exchange groups                                                   15
          4.1.3. Geometry / Shapes                                                 16
     4.2. Employee/login                                                           17
          4.2.1. Okta Login Page                                                   18
     4.3. Article master data                                                      19
          4.3.1. Sale items                                                        19
          4.3.2. Customer-specific article name via stored procedure [AW-193055]   19
          4.3.3. Article group                                                     19
          4.3.4. Replacement product                                               21
          4.3.5. BOM/exchange                                                      21
          4.3.6. Processings                                                       23
          4.3.7. Processings for shape edges                                       29
          4.3.8. Procurement time for calendar                                     31
          4.3.9. Default delivery time for articles                                31
     4.4. General exchange/addition rules                                          32
5.   Price calculation/exchange                                                    33
     5.1. AIR replacement/frame exchange                                           33
6.   Input stop                                                                    34
7.   Limit check                                                                   35
8.   LAMI inheritance                                                              36
9.   Multi-Language Support                                                        38
     9.1. Database tables                                                          38
          9.1.1. Core_CustomTexts                                                  38
          9.1.2. Core_Languages                                                    38
          9.1.3. xsprzu expansion                                                  39
          9.1.4. errmsg                                                            39
     9.2. Master data                                                              40
     9.3. Interface texts                                                          40
     9.4. Workflow                                                                 42
10. A+W iQuote Services + Web                                                      46


A+W Software GmbH             EN-CONFIG-A+W Enterprise iQuote.docx                      3
     10.1. Change of the start page                                    46
     10.2. A+W Infrastructure 6 Web                                    48
     10.3. Multi-client capability                                     50
           10.3.1. Communication flow                                  50
           10.3.2. Configuration                                       50
     10.4. Load distribution front end and services                    52
           10.4.1. Configuration                                       53
     10.5. Maximum number of users                                     53
           10.5.1. Configuration                                       53
11. Studio Workflow                                                    55
    11.1. A+W Infrastructure 6 Workflow Studio                         55
    11.2. Workflow entry                                               55
    11.3. Installation of a workflow via XAML file                     57
    11.4. Workflow                                                     57
          11.4.1. Database tables                                      57
    11.5. Workflow Core                                                58
          11.5.1. Art. Type                                            59
          11.5.2. Article group                                        63
          11.5.3. Article                                              67
          11.5.4. Geometry                                             70
          11.5.5. Subgroups/collections                                71
    11.6. Workflow shopping cart information                           72
    11.7. CheckOut Workflow                                            73
12. Overview of orders and inquiries                                    75
    12.1. Reporting                                                     75
          12.1.1. Display of files name                                 77
    12.2. File attachments                                              78
    12.3. Copying or transforming from order or quotation               78
13. Exchange dialogs                                                   80
    13.1. Muntins                                                      80
    13.2. Gas for IG exchange                                          81
    13.3. Spacer exchange filters                                      82
    13.4. Article designation filter for IGU exchange                  84
    13.5. Structure and coating                                        85
14. Delivery information                                               88
    14.1. Self collection as note                                      88
    14.2. Country selection                                            90
    14.3. Minimum delivery time in calendar (procurement time)         91
    14.4. Pick-up times/dispatch times                                 92
    14.5. Disp. Type                                                   93
15. Operation                                                           96
    15.1. Article designation filter                                    96
          15.1.1. Set-up filter for article selection                   96
          15.1.2. Set-up of filter for processing                       97
    15.2. Filtering processings for individual processing articles      99
    15.3. Projects and project prices                                  100
    15.4. Stock inventory display of an article from several clients   102
    15.5. Item reference text in shopping cart                         104

A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx         4
     15.6. Images for A+W iQuote                                                106
           15.6.1. Product images                                               106
           15.6.2. Images for product groups                                    107
     15.7. Colors and variants                                                  107
           15.7.1. Master Data                                                  108
           15.7.2. Appearance of the selection possibilities in A+W iQuote      109
           15.7.3. Workflow                                                     110
16. Order release                                                               114
17. Orders in the call center                                                   115
18. Status                                                                      116
19. Okta Login Page                                                             117
    19.1. Installation                                                          117
    19.2. Configuration                                                         118
          19.2.1. Okta platform                                                 118
          19.2.2. A+W iQuote Login Okta                                         120
          19.2.3. Preparation of iQuote for the Okta login                      122
          19.2.4. Customization                                                 123
    19.3. Okta data maintenance                                                 123
          19.3.1. Group                                                         124
          19.3.2. User                                                          125
20. Restrictions                                                                127
    20.1. Input                                                                 127
    20.2. Processings                                                           127
    20.3. Glass                                                                 127
    20.4. Incorrect or locked quotations/PO requests                            128
21. Troubleshooting                                                             130
    21.1. License server                                                        130
          21.1.1. No connection to the license server                           130
          21.1.2. License expired                                               131
    21.2. Problems with zero workflows and predefined workflows                 132
    21.3. No images in the IG exchange BOM                                      132
    21.4. Problems during loading/opening of workflows in Workflow Studio       133
    21.5. No database connection on the host server of the A+W infrastructure   135
    21.6. No dispatch of the OC possible                                        135
    21.7. Web Configurator does not start or timed out                          135
    21.8. Duplicate key when saving a workflow                                  136
    21.9. General performance problems                                          137
22. Search/service                                                              138
    22.1. Logs                                                                  138
          22.1.1. Price report                                                  138
    22.2. General                                                               138
    22.3. Which services are affected for A+W iQuote?                           140
    22.4. Export of the Memrels sketches                                        141




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                  5
1. Introduction
Set-up files such as the infrastructure workflow templates and images can be found under
\\jupiter\ALCIB_Install\A+W iQuote Enterprise\.
For additional A+W iQuote configuration instructions with regard to front end or A+W
Infrastructure, check the EN-CONFIG-A+W iQuote.


1.1. Infrastructure
Use of A+W iQuote includes three components in an A+W Enterprise environment:
    •   A+W iQuote as webshop for configuration of orders

    •   The Web.Configurator.Service as interface to A+W iQuote

    •   The documentservice as interface to A+W Enterprise and the A+W Enterprise database

The functionality is available starting with Build 13.04.xxx of the documentservice.
The basic development refers to case #297410 A+W iQuote.
With case #452497, an enhancement was made.


1.2. Prerequisite
    •   ICE environment is configured
    •   The documentservice application under Unix is required (binary)
    •   Required A+W Windows services installed via the A+W SetupLauncher:
            o   A+W Enterprise 6 Frontend
            o   A+W Infrastructure 6
            o   A+W CAD Services (not to be confused with the A+W Enterprise CAD Service)
            o   A+W CAD Designer (Shapes)
            o   A+W CAD Designer (Bars)
            o   A+W Commercial 6 Converter Services
            o   A+W iQuote 6 Services
            o   A+W iQuote 6 Web


1.3. Installation
For installation, the document EN-INST-A+W Enterprise iQuote should be used.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                         6
1.4. Version update
Critical update for version closing via quality release


1.4.1. 2022/11 - Quality Release 11 from 2022
In Quality Release 11 from 2022, there are two important changes in A+W iQuote, which must be
heeded during an update.
The database script 00000211.awdb is required for the AWSOA database. For this, the
infrastructure should be updated. If the customer doesn't want an infrastructure update, then
you can store the database script 00000211.awdb in the directory
(C:\SANDPIPER1\InfrastructureServices\Database\AWDB) intended for this. The script supplies
you from a current test system, e.g. AWEAWP60. After starting A+W iQuote, the script is executed
automatically.
Thanks to the new load distribution in A+W iQuote, it is now necessary that the property
AW.MultiSite.Worker is set in the A+W iQuote Web.Configurator and the document service.
For information and configuration of the load distribution, see chapter "Load distribution"
Brief info about the Worker property:




For the configuration of the property in the A+W iQuote Web.Configurator, after setup via the
SetupLauncher, you will be led through with the subsequent Config tool.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                           7
For the documentservice, you should execute the Unix scripts iceconfig_setup and
iceconfig_execute again.
Very important is that the number of workers on the Windows services and the Unix services of
a client is the same.
For more information, please see chapter "Lastenverteilung Frontend und Dienste".


1.4.2. 2023/02 - Quality Release 02 from 2023
In this Quality Release, some changes were made with respect to multilingual function [AW-
81485]. The first part of the development was completed and gives the customer the opportunity
to change the language via drop-down list.




The list is generated from the languages of the Infrastructure.Web (Infrastructure.Web > Master
Data > Languages). This development is not yet complete and has influenced a few central selects
on the database. When importing at the customer's, please pay attention to which languages are

A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                            8
released in the Infrastructure.Web. Because there could otherwise be missing data if translations
are missing at the customer's. And during the installation of the Windows components, please
make sure that the documentservice is also provided.
In addition to these serious changes with regard to language, details for the article selection were
undertaken, which also influence the workflow setup. This is why the chapter Workflow Core and
its subchapters Art. Type and Article group were written. We hope that this chapter will bring a bit
of clarity about article selection in A+W iQuote and the document service.


1.4.3. 2024/10 – Quality Release 10 from 2024
With BugItem 129598, the PDF copy target path was adjusted. When printing for the A+W iQuote
and the associated PDFCopy logic, now the files are stored in the path under the DATEI_REF_PFAD
with document number and subfolder 0, e.g.
\\aweawpvnext.tse.intra\Trans\AWE\dokuserver\140\500563\0
This modification was necessary since the old path is not suitable for the document attachment.
With this modification, all document files are now stored centrally.
The old printouts are nevertheless found for the PDF download since this path is determined from
the kaufdruck data.
Note:
It is urgent that you pay attention that in the stored procedure rppdfcopyfilename, which handles
the naming of the PDF copy of the printout, all form types used are included in the SP and get
unique names. Precisely for the form types that process documents that can contain subnumbers
(e.g. delivery note), the subnumber in the name is important so that the uniqueness of the file
names can be guaranteed.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                9
2. Configuration of the ICE environment
The description of the installation and configuration of the ICE environment is in the system
configuration instructions (DE-CONFIG A+W Enterprise System.pdf or EN-CONFIG A+W Enterprise
System.pdf)




A+W Software GmbH             EN-CONFIG-A+W Enterprise iQuote.docx                          10
3. A+W Enterprise environment variables
This chapter lists the A+W Enterprise environment variables used for A+W iQuote in short form.
For more precise information about configuration relating to the individual environment
variables, please read the existing configuration descriptions.


Environment variable                       Value             Description
                                           (default/example)
AWSOA_ICEHOST                              -                     Name of the host on which the A+W
                                                                 Service Locator is running
AWSOA_ICEPORT                              12000 (default)       Port on which the A+W Service Locator can
                                                                 be reached
AWSOAFTEST                                 1 – 9 (Ftest Level)   Activation of FTests for A+W SOA services
AWSOA_LOGLEVEL_DOCUMENTSERVICE             0 – 4 (Loglevel)      Log for the documentservice (A+W iQuote)
                                                                 0-Fatal 1-Error 2-Warning 3-Info 4-Debug
                                                                 File:
                                                                 PROTOPFAD\awsoa_documentservice_xxxx
AWSOA_EXPLAIN                              ON or OFF             Enables measurement of the database
                                                                 queries of the AWSOA Backend services
IQUOTE_IGU_TESTLEVEL                       1                     For IG, the restriction check can be
                                                                 expanded to the 1st level (glass).
IQUOTE_LAGER_HANDLING                                            Here, the handling time for stock articles in
                                                                 iQuote is stored in days.
IQUOTE_LEERE_BEARB_MELDEN                  ON or OFF             A restriction error message is sent if at
                                                                 least 1 parameter is missing completely
                                                                 and so display is not possible. If a minimum
                                                                 of parameters is there, then additional
                                                                 restrictions can also be checked for the
                                                                 individual parameters from the AWE
                                                                 master data.
IQUOTE_VSG_VERERBUNG                       ON /OFF               Client reference: yes
                                                                 The special inheritance logic for LAMI in
                                                                 A+W iQuote is activated, which does not
                                                                 map
                                                                 any of the std. LAMI inheritance (AWE,
                                                                 iTOE), but only provides an
                                                                 entry aid where, depending on the BOM
                                                                 structure of the LAMI BOM (1st level
                                                                 atyp183
                                                                 BA=Lager or Prod/Best the processing
                                                                 entered in A+W iQuote is
                                                                 transferred to the individual lites or to the
                                                                 header article.



A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                              11
IQUOTE_PASS_PROCESS_DOWN_1           A+W     processing Client reference: no
                                     types              Here and in the 2 additional ENVs,
IQUOTE_PASS_PROCESS_DOWN_2
                                                        AWtypes are listed that are inherited via
IQUOTE_PASS_PROCESS_DOWN_3                              iQuote LAMI inheritance to the
                                                        subelements.
                                                        Only applies for iQuote inheritance that is
                                                        activated with IQUOTE_VSG_VERERBUNG.
                                                        List separated with |


IQUOTE_WITH_PPARAM_TEST              ON or OFF           Enables restriction check of the processing
                                                         parameters in A+W iQuote
ARTIKELBILD_PFAD                                         This variable describes the root directory
                                                         for the article images.
                                                         The article images themselves are
                                                         maintained in the article master data and
                                                         are then below this path.
ATTACH_PRINTOUTS_TO_DOCUMENT                             The environment variable controls whether
                                                         a PDF copy of a printout should be
                                                         attached to the document. If the
                                                         environment variable is set to 1, only
                                                         printouts from A+W iQuote (kauf.eingang =
                                                         14) are processed. If the environment
                                                         variable is set to 2, copies are created for
                                                         all documents.
                                                         In addition to the environment variable,
                                                         the Stored Procedure rppdfcopyfilename
                                                         must be created. (#439086)
DATEI_REF_PFAD                                           The path for files that are assigned to an
                                                         order or an order item is stored in this
                                                         variable. The maximum length of this path
                                                         is 199 characters. (AWDesk #83527). If
                                                         created site-specifically, always create a
                                                         global site with site=0!!!
IQUOTE_ALL_CUSTOM_STATUS             ON or OFF           A+W iQuote Status is written for all A+W
                                                         Enterprise procedures.
IQUOTE_DISPLAY_ORDER_DAYS_BACK                           Number of days that the A+W iQuote
                                                         history should look back.
IQUOTE_SHOW_DEFAULT_DELIVERY_TIME ON or OFF              Switches on the default delivery display for
                                                         articles
IQUOTE_WITH_PRODEARULES              ON or OFF           Client reference: no
                                                         Activates the evaluation of general product
                                                         E/A rule in iQuote. Additional rules and
                                                         exchange rules for the edgework are
                                                         loaded.
                                                         Please make sure that the elements that
                                                         can come into the BOM via this Z-rule are


A+W Software GmbH          EN-CONFIG-A+W Enterprise iQuote.docx                        12
                                                       not changed in iQuote. A special logic also
                                                       for A-rules for edges. This is described in
                                                       the documentation
IQUOTE_LOGIN_PRIVATEKEY                                The A+W iQuote login key is stored in this
                                                       environment variable. The private key is
                                                       required for comparison with the
                                                       connected login provider.
IQUOTE_LOGIN_REMOTE_ADDRESSES                          In the environment variable, the permitted
                                                       IP addresses for the A+W iQuote Login
                                                       Provider are stored separated by
                                                       semicolons. The IP address sent by the
                                                       A+W iQuote Login Page is compared to the
                                                       addresses stored in the environment
                                                       variable and login is rejected if they are not
                                                       the same. Local host is ":::1"




A+W Software GmbH         EN-CONFIG-A+W Enterprise iQuote.docx                         13
4. Master data Consolidation
For the master data maintenance, it has to be noted that this is only the basis for correct data
acquisition. For large parts of the configuration, adjustments to the workflows (see A+W
Infrastructure 6 Workflow Studio) must be made. As basis for the workflows, standard workflows
are provided and there are additional templates from development (see
\\jupiter\ALCIB_Install\A+W iQuote Enterprise\).
For the creation of master data, the documentservice must be restarted. Articles are, for
example, stored temporarily and loaded from this storage if they were read out of the database
once.


4.1. Key
The prerequisite for the adjustment of the master data are a few new key data.


4.1.1. Product groups
In A+W iQuote, it can be defined via workflows whether the grouping is done via the A+W article
types or individual article groupings. (see A+W Infrastructure 6 Workflow Studio).
If you want to work via individual article groups, appropriate language-specific article groups must
be created in A+W Enterprise (Master Data > Keys > Products > A+W iQuote-specific details >
Article group). The numbering and name can be defined at will. Only the article group 1 is
permanently reserved for processings.
If you want to distinguish between articles with fixed, unchangeable BOMs and articles with
changeable BOMs, you must create separate article groups for this.
Finally, the article groups must be referenced in A+W iQuote via workflows. If you would like to
work with unchangeable BOMs, it must be set for the corresponding article groups in the
workflow that processings and exchange are not possible.
In A+W Enterprise, the defined and referenced article groups can then be in Article master data
assigned to the articles.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               14
            4.1.1.1.   IGU technical values grouping
If you want to set up the IGU grouping for technical values, then you must maintain the following
master data information.
In the technical values (Master Data > Keys > Products > Technical Values > Groups), at least one
group must be created for the value in question (sound, heat, energy).
In the article master data (Master Data > Articles > Techn. Values), these groups must be assigned
to the desired insulating glass.




4.1.2. Exchange groups
For the exchange in A+W iQuote, not all variables possible in A+W Enterprise are allowed. Under
Master Data > Keys > Products > A+W iQuote-specific details > Exchange Groups > All Descriptions
first you specify the required groups for article and spacers. Attention has to be paid that the
groups are maintained in all languages used, otherwise the documentservice may later not find a
data record if the required language was not maintained.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             15
After that, under Master Data > Keys > Products > A+W iQuote-specific details > Exchange Groups
> Group Allocation (article or spacer) you assign the exchange groups the required articles that
should be offered for exchange.
If you have created an exchange group, it is initially empty and can be used in two ways in the
group allocation. The first possibility would be glass or other products, such as gas. The second
possibility affects spacer articles. If then an article is taken into the exchange group, then this
group can only be selected under the respective dialog (article or spacer).
If the exchange groups were defined, these groups have to be assigned to the possible articles for
exchange of the insulated glass BOM in the article master data (Master data > Article > [F4] >
BOM > Groups). The exchange groups can be assigned separated with '|'. (max. 10 groups).


Attention: Currently (02/2023), only the exchange within insulated glass (IGUs) is supported.
Glass or foil exchange in LAMI is not possible.




4.1.3. Geometry / Shapes
The geometry data is loaded into the internal cache at the start of the documentservice from the
table "modelle". The shapes that should be available in A+W iQuote must be set in the A+W
Enterprise master data to online "yes", belong to the catalog type = 0. The names must be
maintained in all languages used.


A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                 16
Please make sure that the approved shapes have a sketch in iQuote. The sketches are loaded from
the folder C:\SANDPIPER1\CADServices\Geometry\Shapes. Shape number is the same as the
sketch's .svg file name. If in iQuote a shape is present without sketch image, there is otherwise
incorrect behavior in the display data field.


4.2. Employee/login
The login of the iQuote is maintained in A+W Enterprise via the employee master data dialog
(Master Data > Employee). For the A+W iQuote user, an employee profile must be created and a
login + web password assigned in this profile. The decision whether the user should use an e-mail
address or another user name as login is left to the company. For the A+W iQuote, the Web login
name must be entered in the login data field.
Starting with QR 2310, for the A+W iQuote of A+W Enterprise, there is now a login check
implemented via the password stored in the Linux (Unix) system analogous to the A+W Enterprise
login. If the Linux logins are synchronized via an Active Directory service, the password is thus
checked in the Active Directory. If an employee would like to log in using this login process, then
there may be no entry in mitarb.winpasswort.


Rights do not have to be assigned to the employee created!




The employee created can now be assigned to a market partner on the market partner master
data dialog (Master Data > Market Partner). In order to be able to enter with A+W iQuote, an
employee may only be assigned to one market partner. Otherwise, this user is refused access to
A+W iQuote. The assignment of an employee to a market partner is managed under the user
allocation (Master Data > Partners > [F4] > Staff allocation > User allocation). If an employee
should be assigned to several market partners, then a warning message is displayed in the user
allocation that A+W iQuote operation is omitted.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            17
4.2.1. Okta Login Page
The Okta login page configuration is done in two steps. The users need an account with
www.okta.com and an employee in A+W Enterprise to whom a market partner is assigned.
You can first create the users in A+W Enterprise, as described under 4.2 Mitarbeiter/Login. To be
noted is that you must enter the customer e-mail address on login. It is not possible to work with
user names. You don't have to store a password since the passwords are maintained via Okta.




For additional information about configuration of the Okta login page, see chapter 17. Okta Login
Page.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            18
4.3. Article master data
For from A+W Enterprise, on the article master data dialog (Master Data > Articles) settings must
be made so that they can be used correctly in A+W iQuote.


4.3.1. Sale items
So that articles (element) from the A+W Enterprise can be used in A+W iQuote, the online flag
(article.verkart=2) must be set on the article master data dialog (Master Data > Articles > Phys.
Properties > Sales Type).




4.3.2. Customer-specific article name via stored procedure [AW-
    193055]
In A+W iQuote, it is now possible to expand the article name of the A+W iQuote article. To activate
the logic, the stored procedure: cu_getcustomproductdesc must be set up. There is a template in
the back end under /develop/sql_scripts/cust/st/cu_getcustomproductdesc.sql.Please note that if
the SP is activated, only the SP for article name determination is used!


4.3.3. Article group
As already mentioned in Product groups, there is a distinction in A+W iQuote whether or not you
are working with the A+W Enterprise article groups. If you have decided on the A+W Enterprise
article groups, then all articles used in A+W iQuote should be assigned the appropriate article
group.


A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             19
For all articles of article type "part" (artikel.teilflag=1), a product group can be maintained if this
product has the online flag. For articles of article type "Part", the assignment of an A+W iQuote
product group is only necessary for intended grouping by product group. A product breakdown per
product type can also be set up; then a product group set-up is not necessary (see Article group).

For articles of the article type "processing" (teilflag=0), it serves to mark the representative A+W
iQuote processings (prototypes). For representative processings, an assignment is always necessary
if this processing should be supported in A+W iQuote. The product group of the processing must
absolutely be 1.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                               20
4.3.4. Replacement product
Exchange articles can now be set in the article master data to "Yes+Online" via sub-element
toggle (Article > Phys. Properties > Sub-Element). Therefore, the article does not have to be
released as sales article.




4.3.5. BOM/exchange
So that an exchange of glass can be made for insulating glass, in the article master data (Master
Data > Articles > Phys. Properties), the toggle data field "BOM" must be set to "yes/changeable",
otherwise the exchange dialog will not be displayed in A+W iQuote.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            21
Attention: Currently (02/2023), only the exchange within insulated glass (IGUs) is supported.
Glass or foil exchange in LAMI is not possible.
So that the inner spacer is displayed correctly in the BOM, a standard AIR has to be maintained for
the market partner used (Master Data > Market Partner > Order) or for the insulated glass
selected (Master Data > Articles > Menu > Dimensioning > Mandatory Dimensions).
If the Exchange groups were defined, these groups have to be assigned to the possible articles for
exchange of the insulated glass BOM in the article master data (Master data > Article > [F4] >
BOM > Groups). The exchange groups can be assigned separated with '|'. (max. 10 groups).




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             22
4.3.6. Processings
Overview
In A+W iQuote, the following types of processings are intended:
-       Arrissing (awtyp = 1000)
-       Grinding (awtyp = 1005)
-       Polishing (awtyp = 1010)
-       Mitering (awtyp = 1015)
-       Beveling (awtyp = 1020)
-       Drilling (seamed, ground, polished) (awtyp = 1100)
-       Countersunk drilling (seamed, ground, polished) (awtyp = 1100)(starting with QR 2302)
        See additional details about master data creation
-       Corner cut-off (seamed, ground, polished) (awtyp = 1305)
-       Corner cutout (seamed, ground, polished) (awtyp = 1300)
-       Round corner (seamed, ground, polished) (awtyp = 1310)
-       Edge cutout (seamed, ground, polished) (awtyp = 1400)
-       Inside cutout (seamed, ground, polished) (awtyp = 1415)
-       Macro (seamed, ground, polished) (awtyp = 1900)
-       Surface macro (seamed, ground, polished) (awtyp = 1910)


Note:


A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             23
In A+W iQuote, only 1 edge processing per edge is allowed. If a product already has a processing
in the master BoM and you apply another in A+W iQuote, then the existing edge processing on
the edge is removed automatically and the new one is applied. If the new edge processing is
applied to all edges, then the old edge processing is removed via an A/Z delete rule generated by
the system. That's why it is important that the environment variable AZ_DELETE_TYP be active.
Since in the normal A+W Enterprise we always warn against DELETE E/A rules, we will consider
another logic for A+W iQuote. But in the existing versions, this dependency is there. (Status as of
07/04/2023)

[AW-157665] / October 2023

In A+W Enterprise iQuote, generally only one edge processing of the A+W processing types
arissing/grinding/polishing is allowed per edge. IF the product itself has an edge processing of this
A+W processing type in the master BOM, then it is deleted from the BOM and the newly entered
one inserted. If the new processing is not selected on all edges, then the new processing is
inserted only for these edges and the processing from the master for the complementary edges.
This also applies if different processings are applied to the individual edges. Attention must
always be paid that each edge has only one edge processing of these A+W processing types. If
several are applied, then the entry encounters an error and the processings must be adjusted
accordingly in A+W Enterprise iQuote.

Display of standard processings
By default, processings that in the master BOM are on "Print no" are not displayed as text in A+W
iQuote. However, they are marked in the SN Live sketch. This can cause irritation for the user.
QR2308 [AW-149355]: In the master BOM, for the elements that should be visible in A+W iQuote
for textual display but should not appear on papers set a separate print identifier "Q". Only
processings of a BOM can be made visible with this identifier.
As an aid, a tool tip was stored for the "Print" field.
(see also “EN-CONFIG-A+W Enterprise” – section “Article master data - BOM“)
Processing assignment
The master data processings for the A+W iQuote entry should be entered in 2 stages.

Prototype/representative processing
For each A+W processing type that should be used in A+W iQuote, a representative article must
be created (prototype). For all non-edge processings, one article per edge quality must be
created. For these articles, you store a previously created A+W iQuote article group for
processings in the "Article group" field. The product group (Master Data > Keys > Products > A+W
iQuote-specific details > Article Groups) for the processing must be assigned 1 since the
documentservice with the product group (artikel.bearbkat) equal to 1 looks to see which
processings may be applied.

For the article dimensioning, a record should be present for each dimensioning type (mtyp:
Absolute (=0), by 2 edges (=1), by corner and edge (=2)) with a fixed edge quality (1100 = seamed,
1005 = ground, 1010 = polished).


A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                            24
All other intended parameters should be on "variable" and have no default values. These
processing articles require no price data in the master, because they are exchanged depending on
the glass product.

QR2302 / [AW-124712]

For the prototype processing, default values can be entered in the article dimensioning. IF a
processing is selected in A+W iQuote, then the parameters that are stored as defaults in the
master data apply for the display. If the default parameters are missing, the processing cannot be
displayed on the sketch. Even if a crucial parameter is set to 0, the display is not possible.

If the display is not possible in A+W CAD Designer (Shape), this processing will also not be
included in the BOM of the order item. In this case, it is now possible to configure that an error
message (restriction error) is sent that the parameters are missing. The user must either enter the
parameters or remove this processing in A+W iQuote. (Environment variable:
IQUOTE_LEERE_BEARB_MELDEN)



Processing assignment/exchange rules (general)
Under online processings (Master Data > Keys > Products > A+W iQuote-specific details >
Processing assignment) you can define which to specific A+W Enterprise processing article the
prototype is assigned.

This will be explained in general in this section. For Special processing types, however, specific
extensions apply, which are documented at the end.

Access to this dialog can be restricted with the glass type. If no type is specified, then all exchange
rules are loaded.

On the left side, you enter the representative processing article that presents it to A+W iQuote
and is used for display. On the right side, you enter a valid processing that with the glass product
type is installed in the BOM if this processing is selected in A+W iQuote. (This data is saved in the
table kuaz with kunr=-2.)




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                25
It is also possible to store more than one 1:1 assignment, which is irrelevant for seaming, grinding,
and polishing. You can also define the exchange through processing parameters. In the detail
view, you can store the restrictions for max. 2 processing parameters. You should make sure that
a rule without restrictions is always present so that a processing will always be found. The
checking of the restrictions is done one after another "starting with dimension". Thus, for a
representative "drilling seamed" an article "drilling seamed" starting at 10 mm, another starting
at 50 mm, etc. can be stored.

If the master data for e.g. FLOAT glass is stored completely, then the additional glass types can
follow. If at the start of menu element the glass type 110 (cast glass) is selected and there is no
master data for it, then the user is asked whether the data should be copied from another glass
type. The data is then taken over completely and can be adjusted or retained.

Special processing types :Countersunk drillings (1110)
QR2302 [AW-131283]: Entry in A+W iQuote of the A+W Enterprise has been expanded to include
the A+W processing type countersunk drilling.


Master data maintenance:
A prototype article for countersunk drilling (awtyp=1110) per edge quality must be created. For
this article, ALL parameters should be permitted ("variable"). Alternatively, the parameters can be
pre-populated with values. If default values are already defined, these processings will be pre-


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                  26
populated in A+W iQuote immediately with these values and the processing is visible on the
sketch. Furthermore, the edge quality should be set to "fix" + a value entered.
If the prototypes have been entered, now the exchange rules for the A+W iQuote processings
must be entered (Master Data - Keys - A+W iQuote-specific Details - Processing Allocation). Each
of the prototype articles should be redirected to an A+W Enterprise processing. For the
countersunk drilling, 3 parameters are activated for the restrictions: "Diameter", "Diameter
bottom", and "Diameter top". However, only the main diameter is checked directly as a
dimension. The two other parameters are only for the case that "Countersunk drilling bottom"
and "Countersunk drilling top" are redirected to another A+W Enterprise article and priced
differently.


Example for prototype article 10199010 "countersunk drilling arrissed" for float glass
1. Case – general rule




This would be a "general" rule for the arrissed countersunk drilling that is always taken if no other
E/A rule is stored, if "countersunk drilling arrissed" is attached to a float in iQuote.
2.   Case with special diameter




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                            27
If this record is created in addition, then article 99199003 is used if the diameter is >=50 mm;
otherwise article 199003 from the 1st rule.


3. Case – additional countersunk hole
If you also need a separate processing article for "countersunk drilling top," then you must create
another record:




The processing article 1199003 is then used if from A+W iQuote only the main diameter and
"diameter top" or main diameter and "depth top" are reported, however "diameter bottom" and
"depth bottom" are both = 0.


2.1. If you also need a separation with regard to the diameter of the main diameter, then you
need another set of rules:




2.2 Accordingly, for "countersunk drilling bottom" you then need




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               28
Processing article 2199003 is used if from A+W iQuote only the main diameter and "diameter
bottom" or main diameter and "depth top" are reported, however "diameter top" and "depth
top" are both = 0.
In addition, a data record for "countersunk drilling bottom" for main diameter >=50mm can be
created analogous to 1.1 and 2.1.


What's important if you create a "general" exchange rule for countersunk drilling for different
main diameters is that you should also create this for "countersunk drilling bottom" and
"countersunk drilling top".
The entry of the main diameter is possible and will also be evaluated during the determination.
The entries for "diameter bottom" or "diameter top" are not required since with this setting, the
entry of the single-sided countersunk drillings is mapped via depths.


It is very important that the A+W Enterprise processings that will be built into the A+W iQuote
process in the BOM do not have their own permanently pre-defined processing parameters
(only variable is allows), so that they do not override the parameters reported from A+W
iQuote.



4.3.7. Processings for shape edges
The assignment of edge processings for shape edges (Master Data > Keys > Products > A+W
iQuote-specific details > Processings for shape edges) has to be maintained separately. If for
particular shapes the individual edges (round arc, e.g.) should be mapped with a deviating article
(due to deviating price calculation or deviating machine scheduling), then for each processing that
was released for A+W iQuote, an exchange processing for shape edges must be stored.

The special edges are maintained under Master Data > Keys > System > Shapes > Edge Processing.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              29
The processings that should be specified on the left side of the dialog must have an A+W type
assignment and belong to the edge processings (seaming = 1000, grinding = 1005, polishing =
1010, mitering = 1015, faceting 1020). Furthermore, this processing should be known via an
online assignment (artikel.verkart = 2). On the right side, there must be a processing of the same
AWType.




Extension QR2302 [AW-94463]: Separate edge processings for the individual shapes in A+W
iQuote
The dialog for A+W iQuote edge processings for shape edges is expanded by the fields shape
number and special edge




The already existing old data for the exchange is adjusted automatically when you first enter the
expanded dialog (special edges ad active). General exchange, which applies for all shapes that are
not listed separately, is then entered with shape=0 and special edge.
In addition, it is now possible to store deviating edge processings for each shape.
If a shape in the shape master data (Master Data > Keys > System > Shapes > Edge Allocation) has
special edges and "normal" edges, then for this shape, you can maintain the data separately for
"normal" edges and special edges. If according to the master data a shape has no special edge,
then it is not possible to create an exchange for the special edge.
In the example above, for the processing "edges polished" via the general A+W iQuote exchange
rule, the A+W Enterprise article 399101 is determined. If the item as shape X (not No.78 and not
No.1) is entered with the special edge (e.g. edge 2), then for the normal edges (all edges except
edge 2) the processing 399101 is attached to the BOM and for the special edge (edge 2) also the
processing 399103.


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             30
If the item with shape 78 (2 edges according to shape catalog) is entered, which has a special edge
(edge 2), then for edge 1 the processing 399102 and for the edge 2 (special edge) the processing
399103 is attached.
If the item is entered with shape 1 (no special edges), then the processing 399104 is taken over
into the BOM.


4.3.8. Procurement time for calendar
In A+W iQuote, the delivery dates on the calendar are now pre-populated with consideration that
the routine days starting on which the earliest possible date is pre-populated [AW-109411].
The determination of the procurement time is done on the item level via the A+W Document
Service for the product in question. This is a preliminary date that can be kept under optimal
conditions. Final delivery date only follows after acceptance of the data in AWP.
The determination is based on the data stored in the article master data. The procurement time is
determined depending on the procurement type:
    •   For products with 1. Procurement type "production" the production time
    •   For products with 1. Procurement type "PO" the delivery time of the default supplier
    •   For stock articles, the processing time is defined via an ENV switch:
        IQUOTE_LAGER_HANDLING.


4.3.9. Default delivery time for articles
With the AWE environment variable: IQUOTE_SHOW_DEFAULT_DELIVERY_TIME the default
delivery time for the articles can be switched on. If the variable is active, then procurement type is
distinguished via article; its default delivery time is displayed.
A purchased article is filled with artikel.stdlz.
A production article is filled with artikel.prodzeit.
A stock article is filled with the value from the AWE environment variable
IQUOTE_LAGER_HANDLING.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                             31
4.4. General exchange/addition rules
Generally A+W iQuote works only with standard BOMs.
However, through configuration you can permit a few exceptions and activate the
activation of particular general or customer-specific exchange or addition rules.
Only

   •   the additional rules for product/product type or
   •   exchange rules for edgework are evaluated.

Environment variable: IQUOTE_WITH_PRODEARULES = ON




A+W Software GmbH            EN-CONFIG-A+W Enterprise iQuote.docx                   32
5. Price calculation/exchange
5.1. AIR replacement/frame exchange
If in A+W iQuote for an IG only the AIR in the frame was changed, then previously in the BOM an
exchange identifier was set for the frame automatically. This caused another price calculation and
eventually also errors in the price calculation.
The logic at this point was changed. If it is now detected that the frame is an identical frame with
differing thickness (AIR), the original exchange identifier is retained in the BOM. This means, if the
frame was previously price-relevant, it also is after changing of the AIR; if it was not previously, no
price will be calculated after the change of the AIR.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                               33
6. Input stop
July 2025 / documentservice build 13.04.8089

Within the A+W Enterprise market partner master data, it is possible to define a "Entry stop for
orders". This setting can be considered within A+W iQuote for the entry of orders. This happens in
the course of the price calculation for the first item.
If for a customer "Entry stop for orders" is defined, the price calculation encounters an error, and
the A+W iQuote user receives the message stored for this. The message for this case must be
configured individually in A+W Enterprise. This is done under Keys->System keys->Text blocks via
the blocks 170-173. The texts must be stored in all active languages. However, not all 4 blocks
must be used.
IMPORTANT! If all 4 text blocks are not maintained, there is no check for entry stop.

Entry stop for quotations is not evaluated in iQuote!




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             34
7. Limit check
July 2025 / documentservice build 13.04.8089

Within the A+W Enterprise, it is possible to define a limit and a limit check. If the limit check is
active for a customer, it can also be evaluated in A+W iQuote. This happens in the course of the
price calculation for the first item.
If the defined limit check fails for the customer, the price calculation encounters an error and the
A+W iQuote user receives the message stored for this. The message for this case must be
configured individually in A+W Enterprise. This is done under Keys->System keys->Text blocks via
the blocks 174-177. The texts must be stored in all active languages. However, not all 4 blocks
must be used.
IMPORTANT If all 4 text blocks are not maintained, there is no limit check during entry.

The limit check for iQuote orders is generally executed, regardless of the user's rights.
If the limit is exceeded by the order entered, the order can only be saved by the user. Further
along, the order is placed in the release pool with "limit block".




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              35
8. LAMI inheritance
QR 2406 // [AW-179138]

It is possible in A+W iQuote to use a global setting (ENV switch) to activate an inheritance of the
processings to the individual lites. This logic cannot be mapped in the LAMI inheritance via iTOE
already implemented in A+W Enterprise or via the background process "intauf". Processings
added in A+W iQuote are added as individual processings to the individual lites below the LAMIs
and not on the header level, as for all other products. This also assumes that the LAMI has a level
with the list of the glass and film elements with corresponding assembly positions, in which it is
possible to add the processing. The price of the processing is also calculated per lite. The
dependency of these processings on one another is only present during entry in A+W iQuote. If
the processing in A+W iQuote is deleted again, then it is removed from all subelements. The LAMI
processing entered is visible in the list view on the right of the dialog, once on the associated
button. Below the picture, in case of inheritance, this is output multiple times (depending on the
number of lites in the LAMI). If the document is stored and then later loaded into A+W Enterprise,
there is no dependency of the processings on one another. If something should be corrected, then
the correction must be done manually on all corresponding processings on the other lites.
Whether the processing on the LAMI is inherited by the individual lites or added to the header
element is determined by the structure of the BOM.

    •   If a LAMI (atyp 170) has one LAMI stock dimension (atyp 183) on the first level, which has
        the procurement type LAGER(=5) or PO(=4), the processing is attached to the header
        level.
    •   If a LAMI (atyp 170) has a LAMI stock dimension (atyp 183) on the first level that is set to
        production and there is a level with glass and film under this, then the processings are
        inherited.
    •   If a LAMI already has glass and film on the 1st level, the processing is inherited.
    •   If a LAMI (atyp 170) has another LAMI article on the first level (atyp 170), the processing is
        added to the header element.

The case that a LAMI has another LAMI on the glass/film level is not supported in A+W iQuote.
If new edgework was placed on the LAMI and the inheritance must be executed, any existing
edgework on the individual lites is deleted and the new one inserted. If the inserted one is not
linked to all edges, the existing edgework is reduced by these edges.
If you are working with the evaluation of product-specific exchange rules in A+W iQuote, these
are also considered.
The logic applies for all processings with the exception of surface processings. No processing is
applied to the LAMI header if the BOM is suitable for inheritance and the procurement type is
PRODUCTION.
A separate development must be commissioned for the surface processings, insofar as these
processings are included in A+W iQuote.
If the inheritance logic should not apply for all edgework (1000 - 1090), drillings (1100 - 1190),
corner processings (1300 - 1390) and geometric processings (1400 - 1490), but only for particular
AW processing types, this can be entered in the corresponding list of ENV switches (e.g. ENV =
"1000|1005|1010|1015|1100|1300|...").


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                36
The special logic applies for the inheritance of countersunk holes; the dimensions are converted
explicitly for the individual lites. From the conversion, it can happen that a countersunk hole
should not be inherited on all lites, but only a drilling. Therefore, it is very important that the data
for the calculation (thickness of the individual lites, films) and also the exchange rules for the
inheritance in A+W Enterprise (Keys=>Products=->LAMI) are maintained. If the exchange rules for
the inheritance are not present, this will cause incorrect results.
Development is based on the current status of the A+@ iQuote LAMI detection without glass
exchange. If later an exchange of the individual lites in LAMI is commissioned, then the expansion
of the inheritance must be ordered along with this. This also applies for the inheritance for
surface processings.


Relevant environment variables:
IQUOTE_VSG_VERERBUNG = ON
IQUOTE_PASS_PROCESS_DOWN_1 = 'X|Y|Z....'
IQUOTE_PASS_PROCESS_DOWN_2
IQUOTE_PASS_PROCESS_DOWN_3




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                 37
9. Multi-Language Support
Under the ticket [AW-81485] and feature #41873, the multi-language support for the A+W iQuote
of the A+W Enterprise was implemented completely.
Please work through the following points when setting up the customer system so that there is no
incorrect data in various languages at the customer's.


9.1. Database tables
9.1.1. Core_CustomTexts
The Core_CustomTexts table is found under the AWSOA database and is not an A+W Enterprise
Backend table.
The database table must be filled via Inserts/Updates. Currently, there is a maintenance tool for
this database table.
 Column name         Type              Description
 guid                Char(36)          Key (must get a unique GUID)
 versionid           Integer(4)        Version number
 lockingtoken        Char(36)          Not in use, must be present as "00000000-0000-0000-
                                       0000-000000000000"
 Code                Nvarchar(255) Variable name that is used by the A+W iQuote or
                                   Workflow Studio
 languagecode        Nvarchar(5)       Language code (reference: core_languages.code)
 text                Text(56)          Text that should be displayed
 Description         Text(56)          Description of the text (help text)



9.1.2. Core_Languages
The Core_Languages table is found under the AWSOA database and is not an A+W Enterprise
Backend table.
The Core_Languages table is maintained via the Master data tab in the Infrastructure.Web. The
language codes are specified. Please make sure that each language maintained in the
Infrastructure.Web is released for the A+W iQuote. Only create languages that are 100%
configured.
 Column name          Type             Description
 Guid                 Char(36)         Key (must get a unique GUID)
 versionid            Integer(4)       Version number




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                          38
 lockingtoken          Char(36)         Not in use, must be present as "00000000-0000-0000-
                                        0000-000000000000"
 code                  Nvarchar(5)      Language code
 Description           Nvarchar(16)     Language written out



9.1.3. xsprzu expansion
The back end table xsprzu was expanded to include the database field xsprzu.sprcode. This
guarantees that the customer language and Alcib language do not differ and we have a starting
point for data determination for the A+W iQuote. The reason for this adjustment is that some
texts that must be determined from the back end are created in customer language and other
texts in the Alcib language.
The language codes can be maintained on the A+W Enterprise dialog (Master Data > Keys >
System > Languages).
Please make sure that the language codes from the Core_Languages table are entered correctly
in the xsprzu table. The query is case-sensitive, so make sure to take upper and lower-case
letters into account!


9.1.4. errmsg
Some texts for the A+W iQuote are determined from the A+W Enterprise back end data. The table
for this is "errmsg". The table is 0-based and
 Name                Type            Description                                References
 errno               integer         Error number
 errtxt              char(80)        Error description
 manr                integer         Responsible employee                       mitarb.manr
 moddate             date            Date of the last change
 moduser             integer         Employee who last changed this record
 prgname             char(15)        Module or section
 sprache             smallint        Language detection note: Env var
                                     $SPRACHE


List of currently used texts (errno):
22083, 22084, 22183, 22195, 22196, 22588, 22589, 22591, 22592, 22593, 22598, 22599, 28805,
30685, 35728, 36185, 37593, 37594, 37598, 38201, 38203, 38281, 38297, 38334, 38335, 38341,
38367, 35674, 37951, 37389, 37840, 37841, 38255, 37842, 37843, 37839, 37844, 37838, 37837,
37845, 38260, 38259, 36531, 37345, 37347, 37346, 22197, 22400.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                          39
9.2. Master data
Due to the complete conversion to multi-lingual capability, master data for all released languages
must be maintained in the Infrastructure.Web. The necessary master data that should be
maintained is listed below.
                      Table           A+W Enterprise                   Description
 Articles,            artbezfremd     Master Data > Article > [F4] >   All designations where
 processings,                         Additional Descriptions          articles are at issue
 muntins,
 exchange articles
 Shapes               Shapes          Master data > Keys > System      Shapes in the geometry
                                      > Shapes
 Product groups       xsprbez with    Master Data > Keys >             Product groups in the
                      xiqartgrp       Products > A+W iQuote-           article selection
                                      Specific Details > Product
                                      Groups
 Exchange groups      Xsprbez with Master Data > Keys >                IGU exchange groups (are
                      xiqchangegrp Products > A+W iQuote-              not displayed in the A+W
                                   Specific Details > Exchange         iQuote front end)
                                   Groups
 Colors               xsprbez with    Master data > Keys >             All names for the color
                      xxfarbe         Products > Variants > Colors     selection.
 Countries            xland with      Master data > Keys >             Country names are
                      xsprbez         Partners > Countries             required for the delivery
                                                                       address in the delivery
                                                                       information
If texts for a language should not be maintained, then the particular e.g. articles for the missing
language are not displayed.


9.3. Interface texts
A+W iQuote obtains the language-dependent screen texts as a message resource; these cannot
be changed. Interface texts can be overwritten via the database table Core_CustomTexts. Thus,
for example, the name of the application can be adapted in the browser or the buttons in the
header area if the customer so wishes.

 -- Selection of the texts
 SELECT Guid, Code, LanguageCode, Text, Description FROM Core_CustomTexts;

After the program start, the "Core_CustomTexts" table is filled automatically with blank texts for
the screen translation. This is done in the first language that is entered in the infrastructure
languages.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               40
Texts that should also be localized then have to be entered via database insert/update command
for the language in question. The value that is obtained by default from the message resource and
displayed is in the comment column. It serves as template for the customer's texts. Among other
things, this is very important if there are placeholders {0},{1}... in the text. With these default
records, you always have an overview of which messages there are. The list adjusts itself.
However, nothing is overwritten.
Inserting a text for the browser application names:

 INSERT INTO Core_CustomTexts (Guid, VersionId, LockingToken, Code, LanguageCode, Text,
 Description) VALUES (GUID-Function(), 1, '00000000-0000-0000-0000-000000000000',
 'WebConfigurator', 'de-DE' , 'A+W Buy', '')

The test of this is in the AWEAWPVNEXT test system.




After the restart of the Web.Configurator Service, the application presents itself under the name
"A+W Buy".




Not all interface texts can be adjusted but many buttons and central texts can be replaced.
A trick for seeing all text codes in iQuote is to use a script to fill all blank texts with the content of
the codes; then the iQuote is only displayed with the codes and the changes can be made
efficiently.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                                  41
 -- Preset all Text with the textcode
 UPDATE [AWSOA].[dbo].[Core_CustomTexts] SET Text=Code where Text= '';

 -- undo the preset
 UPDATE [AWSOA].[dbo].[Core_CustomTexts] SET Text= '' where Text=Code;




9.4. Workflow
It is possible to change texts that are maintained via the workflow for the customer individually.
For example, the Workflow tab or if you do not create back end-related product groups such as
the subgrouping in the IG exchange and you need multilingual group names for this.




The multilingual texts are managed in the table Core_CustomTexts, currently there is no
management program for this. It would make sense to create an Excel table. This could be
translated and then Insert Statements created with the help of the Excel table.
 INSERT INTO Core_CustomTexts (Guid, VersionId, LockingToken, Code, LanguageCode, Text, Description)
 VALUES (newid(), 1,'00000000-0000-0000-0000-000000000000', <Code nvarchar(255)>, <LanguageCode
 nvarchar(5)> ,<Text nvarchar(max)>,<Description nvarchar(max)> )



These must be executed on the Informix database for the A+W iQuote.
The language codes (Core_CustomTexts.LanguageCode) correspond to the table Core_Languages.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                 42
In order to assign the texts to the workflows, a global variable must be assigned. This variable
must be created in the desired workflow (see screenshot). The user's current language is made
accessible via "Cart.CurrentItem.Culture" in the workflow and must be assigned to the variable.
Open the desired workflow in the Workflow Studio and add a
"System.Activities.Statements.Assign" element before the workflow core element and enter the
values displayed below.




When assigning the culture, you must pay attention to the workflow in which you're working.
In the big configurator workflow, the assignment is: Cart.CurrentItem.Culture
In the checkout workflow, the assignment is: Cart.CheckOut.Culture
A good hint about where the right place is to assign to the culture is the ItemIn, which is
assigned via the culture in the following screenshot.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               43
In order to use these texts in the workflow, there are 2 possibilities:
    1. Via function Configurator.GetCustomText(code, languageCode)
        Configurator.CustomMessage("Test", LanguageCode)




This function can be used for all activities, for the properties Category, Description, and Name.
To establish a collection, the function can also be used in an expression.




    2. Via language code sequence „@@<code>@@“
To simplify this, in an activity (not in an expression) without function call, there can be a text
determination. For this a "@@" must be placed in front of the message code and attached. The



A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                44
function is then expanded internally and the Configurator.CustomMessage("Test", ...) function is
called.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                            45
10. A+W iQuote Services + Web
A+W iQuote Web is the front end of A+W iQuote and includes all information so that the A+W
iQuote can be displayed via the Web browser.
The A+W iQuote services include the functionality for communication between browser, the
Service Locator, and the backend (documentservice).




10.1.           Change of the start page
The A+W iQuote is accessible without configuration change via computername/web.web. Many
customers would like their own web address to be used for their online presence. So that you can
incorporate this web address, a new start page must be created in the Internet Information
Services manager (IIS).
For this, in the IIS, you must right-click on Sites and select "Add website" there.




Now in the next step, you can configure a new start page. Here, you can specify the
Web.WebAppPool directly via physical path (Ex. C:\Sandpiper1\WebWeb) or you use an own
directly as the default site uses (Ex. %SystemDrive%\inetpub\wwwroot).
With the direct path in the AppPool (see picture below), the folder structure of the WebWeb
folder is taken over.
If you do not want to define a new hostname, a new free port must be selected since otherwise
the starting point overlaps with the default page. A+W iQuote can thus also be reached via the
computer name:port.
If a hostname should be configured, that is, another website name/domain, this hostname must
be acquired by the customer. This way, the website will run over the new hostname. If necessary,
the multi-client number would be displayed behind this. You could hide the multi-client number in
the content area with the index.htm named below.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                            46
With a superior folder structure, you must add the Web.WebAppPool via application.




There should be an index.htm file in this folder that serves as the starting point.
Content example:
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="refresh" content="0; URL=https://alw-dev22.tse.intra/Web.Web/140" />
<title>iQuote</title>
<style type="text/css">


For more precise setting possibilities, please consult Google or a colleague.

A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                    47
10.2.            A+W Infrastructure 6 Web
The A+W Infrastructure 6 Web is a browser application and can be found in the A+W folder on the
desktop. Here, the settings for the A+W iQuote and the A+W Infrastructure can be set up. Some
settings have to be made here, which are relevant since A+W iQuote uses the A+W Enterprise
functionality.
Configuration
The system switches are managed on the Configuration tab. Here, the business case functions
(Configuration > A+W iQuote > Business Case Functions) can be set. Particular functions can be
switched on and off for the 5 different representatives. Presently, only the customer order is
evaluated.




 Business case                       Meaning
 Display overviews                   Shall the history/overview be displayed?
 Form printing                       Not in use. Controlled from the back end.
 Order export                        May orders be saved?
 Request order export                May quotations be saved?
                                     Button active for query
 Quotation to order                  Copy quotations in the history to orders [AW-64004]
 Quotation to quotation              Copy quotation into history [AW-109408]
 Order to order                      Copy order into history [AW-109408]
 Order to quotation                  Copy order in the history to quotation [AW-109408]
                                     Do you want to save shopping carts not saved yet?

 Save shopping cart                  If this switch is active, a list of the not completely entered
                                     orders or quotations is displayed before each entry into
                                     the article selection.
 Direct check-out                    Not in use.
 Enter quotations                    Permit quotation entry? If desired, also set order export!
                                     Permit order entry? If desired, also set order export
 Enter orders
                                     inquiries!



A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                                   48
 Show prices                         Show price? AWE always on!
 Price manipulation                  Not in use.
                                     Shall all quotations/orders from A+W Enterprise be
 All documents of history            displayed in the history? Limited to 60 days or can be
                                     changed via ENV variable:


Under the Commercial > Backend field there is a drop-down menu that must be set to Enterprise.
With it, the A+W Web Configurator controls the correct back end.
Via System Configuration > Company Logo file name, a company logo can be set up. The logo file
must be in the content folder of the installation directory of the A+W Web
Configurator(C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content).
Under System Configuration > Web settings, a selection of tabs opens on the right. On the Web
tab, settings for the appearance of A+W iQuote can be set. The element "Advertising file name"
serves to set up advertising images that run in the browser if you are on the log-in and main menu
in A+W iQuote. Here too, the images must be in the content folder. To get a better overview in
the content folder, you can create the subfolders and then the data field "Advertising file name"
can be filled like this, for example: 
auw/ads/ads1.jpg;auw/ads/ads2.jpg;auw/ads/ads3.jpg;auw/ads/ads4.jpg
Similarly, you can create a background image and select a scheme that changes the color design in
A+W iQuote.
Similarly, you can see the configuration instructions EN-CONFIG-A+W iQuote for additional
information.
Workflow
The Workflow tab serves to manage the workflows of the individual expansion points. For A+W
iQuote, the following points are relevant:




 0000 – A+W iQuote                                 Product configuration in A+W iQuote
 0001 – WebConfiguratorMapper                      Not relevant, leave on default.
 0002 – WebConfiguratorCheckIn                     Dialog window before you get to the product
                                                   configuration.
 0003 – WebConfiguratorCheckout                    Dialog window after leaving the shopping
                                                   basket and before going to checkout



A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                              49
 0004 – WebConfiguratorDocumentValidation          Not relevant, leave on default.
 0005 – WebConfiguratorAddToCart                   Not relevant, leave on default.
 0006 – WebConfiguratorBackEndUpdate               Not relevant, leave on default.



10.3.           Multi-client capability
With the development of multi-client capability (#52389), the problem that you had to provide
and install several process servers for several clients was eliminated.
Please ensure during the update that the DB script: 00000211.awdb is present on the FTP or in
the installation folder (...\A+W\Sandpiper1\InfrastructureServices\Database\AWDB).


10.3.1.         Communication flow
The communication flow of A+W iQuote is as follows, the user operates the A+W iQuote via the
browser with an extended web address (e.g. aweawpvnext.a-w.intra/Web.Web/140). At the end,
the new web address includes the client number to which the company's customer is assigned.
With this client number, we can ensure client-specific communication through the system.
Each action in the browser is directed via the Internet Information Services (IIS) direction of the
services. This communication runs to the so-called HomeController, where the assignment to the
client-specific services is distributed. With the incoming client number, the HomeController
determines a web configurator service and passes the action along.
In the web configurator service, a connection to the document service may be required, e.g. for
data procurement in the backend. Now the web configurator service searches for a document
service using incoming client number and connects with it and the processing of the action can be
completed.
Browser  IIS (HomeController)  Web Configurator  Documentservice



10.3.2.         Configuration
The description of the installation and configuration of the documentservice under the Unix
environment is in the system configuration instructions (DE-CONFIG A+W Enterprise System.pdf or
EN-CONFIG A+W Enterprise System.pdf). The section Ice environment > Unix > Configuration there
must be run through. The scripts mentioned lead the user through the configuration.
Before you undertake the configuration on Windows, you should maintain the clients required
and their client numbers in the A+W Infrastucture 6 Web > Master Data > Clients. For the
installation on Windows, the setups A+W iQuote 6 Services and A+W iQuote 6 Web must be
updated. These setups have config tools that determine the client maintained via the A+W
Infrastructure 6 Web. These clients can now be enabled for multi-client capability.
For the A+W iQuote 6 Service, the settings are made in the Service Locator Administrator. You
enable the clients that you need and assign a number of workers to these clients. More about the
topic of workers and load distribution in the next chapter. Finally, a start port must be selected.
All required services are assigned a port number by this port startend.



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             50
For the A+W iQuote 6 Web, shortcuts are stored in the A+W folder on the process server for the
selected clients that contain the expanded web addresses (e.g. aweawpvnext.a-
w.intra/Web.Web/140).




A+W Software GmbH             EN-CONFIG-A+W Enterprise iQuote.docx                           51
If an AutoUpdate should be set up, then the setup handles the previous settings.
The clients and workers maintained can be found in the Service Locator Administrator under
Properties.




10.4.           Load distribution front end and services
Thanks to the newly installed load distribution (#52389), the service inquiries can be distributed
across several services, which should guarantee the stability of the A+W iQuote in case of heavy
loads.
Please ensure during the update that the DB script: 00000211.awdb is present on the FTP or in
the installation folder (...\A+W\Sandpiper1\InfrastructureServices\Database\AWDB).
The load distribution is currently implemented according to the round robin principle. Example:
we have 4 services and one service after another is controlled. Service 1, then service 2, then
service 3, etc. If all services are controlled at the same time, they start at the beginning.
There is an internal cache for the load distribution, which saves the browser sessions and their
associated services. This cache is cleared out with a 15-minute time period. If an ongoing session
is only called up again after 15 minutes, a new service must be sought.



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                 52
10.4.1.          Configuration
The load distribution is provided with the above-mentioned setups A+W iQuote 6 services and
A+W iQuote 6 web.
The number of workers must be greater than 1 to use the load distribution. As mentioned in the
previous section, you can set up the number of workers for the Windows services in the config
tool. The number of document service workers is set up via the Unix scripts. The help for the
setup of the document service under Unix is in the system configuration instructions (DE-CONFIG-
A+W Enterprise System.pdf or EN-CONFIG-A+W Enterprise System.pdf).
Very important is that the number of workers on the Windows services and the Unix services of
a client is the same.
Explanation:
As in the communication flow explained in the section above, only the services whose client
numbers match communicate with one another. This applies to the load distribution and the
workers.
Example:
A “Web Configurator Service Mandant 140 Worker 1“ speaks only with a “Documentservice
Mandant 140 Worker 1“
A “Web Configurator Service Mandant 140 Worker 3“ speaks only with a “Documentservice
Mandant 140 Worker 3“


10.5.            Maximum number of users
With the development [QR 2302/AW-97000], it became possible to set the maximum number of
users for A+W iQuote. This development was developed for the user-specific Informix license and
must be set for customers who do not have a core license with Informix.
Similarly, you can use this logic for load reduction of the system, whereby we would actually
recommend Load distribution logic.
The default logic works with the browser session ID, which makes it possible to log in on several
browsers or systems with one user login.
These session IDs are saved in a cache centrally on the IIS (Internet Information Services). The
limit "Maximum users" applies for every IIS once. (40 users entered 1 IIS, 40 users can work in
A+W iQuote, regardless of how many document services are running in the background).
Via timeout time interval, the cache is cleaned out regularly, so that individual inactive users
cannot block the system.
Important: For adjustments to the configuration, the IIS and Web.Configurator service must be
restarted.


10.5.1.          Configuration
The configuration of this development is done with the A+W iQuote 6 Web Config Tool.
Setting possibilities:
Limit A+W iQuote users: Activate logic. Default: deactivated.

A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                53
Maximum users: Specify maximum number of users.
Timeout interval: Specify inactive time interval in minutes. This value serves to clean out the user
cache. If a user is inactive for longer than this value, he will be removed from the cache. Another
login is then only possible if there is still a free space on the system.
Username logic: Change the default logic from session ID to user name. More restrictive logic
since you can then no longer log in several times with one user.




After the configuration, the IIS must be restarted, as must the WebConfigurator service.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              54
11. Studio Workflow
The application A+W Infrastructure 6 Workflow Studio is found in the ..\Programs\A+W\Config
Tools folder.


11.1.           A+W Infrastructure 6 Workflow Studio
In the A+W Infrastructure Workflow Studio, the required workflow is added for A+W iQuote. This
workflow can be adjusted customer-specifically. For initial installation, standard workflows are
included. You have to check whether
For detailed explanations of the use of the Workflow Studio, use the configuration documentation
EN-CONFIG-A+W iQuote.
First, it should be checked whether the reference path in the Workflow Studio is correct and
accessible. In the image below, the standard folders are displayed; these are always entered but
they do not have to be used by the customer.
These are found in Workflow Studio under "Configuration > Settings > Reference paths". The
paths point to the installation folders of the applications that use workflows. For our case, the
configurator must be set correctly.




11.2.           Workflow entry
The general widget setting parameters relevant for A+W Enterprise will be explained here. For
detailed explanations of the workflow widgets, see Chapter 4 of the configuration documentation
EN-CONFIG-A+W iQuote.
To be noted is that the predefined workflows cannot be changed. If such a workflow should be
used as the basis, the workflow has to be loaded and saved as a special workflow.
A change to a workflow always has to be associated with a restart of the ICE service. It's easiest to
do this via the Service Locator Administration.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                55
When the workflow is loaded, double-click on the Workflow Core. Then the required workflow
will open. For more information about the workflow core, see section Workflow Core




For information about the other selection possibilities of the Init area workflow, as well as the
activities or widgets that can be used to design the workflow, see Chapter 4 of the configuration
instructions EN-CONFIG-A+W iQuote.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             56
11.3.           Installation of a workflow via XAML file
In the Workflow Studio via File > Open XAML, you can select an existing workflow file and confirm
with Open. Via the new window, select the workflow type that is hidden behind the workflow file.
For a classic A+W iQuote workflow, the type "WebConfiguratorWorkflowTypeDto" is required.
The workflow opens in the Editor window and can be adjusted if necessary. Now the workflow
has to be saved in the Workflow Studio; to do this, click "File > Save" in the menu bar. On the
following dialog, check the workflow type again and save with "Save."
In order to assign the workflow to A+W iQuote, the Workflow Studio must first be restarted. Now
use the menu bar to select "Configuration > Workflow Management." On this dialog, the
individual A+W iQuote sections are managed via workflow. Via expansion points, you can see the
particular sections, such as 0000 - A+W iQuote, which reflects the flow of product configuration
through to adding to the shopping cart. Now click the line on the Workflow tab that you would
like to change. With the drop-down box, you can select the possible workflows. Select and save
the desired workflow.


11.4.           Workflow
For detailed descriptions of the general workflow configuration possibilities, see the A+W iQuote
configuration instructions for A+W Business (DE-CONFIG-A+W iQuote.pdf or EN-CONFIG-A+W
iQuote.pdf)


11.4.1.         Database tables
All workflows are saved and archived in the following database tables.

Core_WFActivities

Each saved workflow is in this table.
 Name               Type                Description                              References
 guid               GUID                Unique number
 versionid          int                 Version number (numeric)
 lockingtoken       GUID                Not in Use („00000000-0000-0000-
                                        0000-000000000000“)
 description        NVARCHAR(255)       Name of workflow
 activity           NVARCHAR(MAX) XML code of the workflow
 workflowtype       int                 Workflow type ( 0 = iQuote main
                                        workflow)
 active             bit                 Active workflow? (1=yes, 0=no)
 systemworkflow     bit                 System workflows cannot be changed.
                                        (1=yes, 0=no)
 version            NVARCHAR(40)        Version number (alphanumeric)



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            57
Core_WFActivityAssignments

Assignment table for the workflows
 Name              Type                 Description                             References
 guid              GUID                 Unique number
 versionid         int                  Version number (numeric)
 lockingtoken      GUID                 Not in Use („00000000-0000-0000-
                                        0000-000000000000“)
 extensionpoint    int                  Expansion point of the workflow
 workflowguid      NVARCHAR(MAX) XML code of the workflow
 workflowtype      int                  Workflow type (0 =
                                        WebConfigurator)
 clientguid        GUID                 Client number from the                  core_clients.guid
                                        Infrastructure Web
 Token             NVARCHAR(255)        AWP logic


Core_WFActivityArchives

Archive table of the workflows
 Name               Type                Description                              References
 guid               GUID                Unique number
 versionid          int                 Version number (numeric)
 lockingtoken       GUID                Not in Use („00000000-0000-0000-
                                        0000-000000000000“)
 archivetime        Datetime            Time stamp of the change
 activity           NVARCHAR(MAX) XML code of the workflow
 wfactivityguid     GUID                Unique number of the wfactivity table    wfactivity.guid




11.5.             Workflow Core
The core of the A+W iQuote is in the Workflow Core Element, which can be found for the A+W
iQuote with the type WebConfigurator and the extension point 0000 - A+W iQuote. As basis, you
should always use an old workflow in order to have the basic structure of the workflow.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                          58
If one of the workflows mentioned above opens, you will find the
structure depicted on the right. In this structure, double-click on the
Workflow Core in order to find the core of the configurator.
In the core, the configurator flow is now configured, which grouping
underlay the article, which dialog options are released for the user
for particular article groups, whether filters should be displayed, etc.




11.5.1.           Art. Type
In the Workflow Studio, you will find the ActionValidatorProductTypes widget, which is
abbreviated in the following examples as ValidatorProductTypes by the display name. In the
Workflow Studio Toolbox (left side), you will find the widget under iQuote Common > Product
Types.
  Product Types
  Selection of the product types by product type number. The images are searched for in the Content directory.
  Parameter             Description                                                        Default
  Category              Display of category (breadcrumb)                                   AWSOA.Core.Messages.Globa
                                                                                           l.WebCategoryProduct
  Configurator          Access to the Configurator service                                 Configurator



A+W Software GmbH                     EN-CONFIG-A+W Enterprise iQuote.docx                                       59
  ContentPath        Relative directory for the content of the widget in the Content   e.g. "auw/producttypes"
                     directory
  Description        Description that appears after the widget header
  Display Name       Name of the activity in the Studio workflow
  ItemIn             Incoming item object of iQuote                                    ItemIn
  ItemOut            Output item object of iQuote                                      ItemOut
  Name               Title of the widget in iQuote
  ProductType        Selected product type as workflow variable
  ProductTypesIn     ERP product type number                                           „100,150,170,200,800,1000"

For the product types logic, the following ERP product type numbers are specified:
100 – Floats
150 – TG
170 – LAMI
200 – IG
800 – Accessories
1000 – Dimensioned articles (A+W iQuote exclusive and not with reference to an A+W article
type.)
In the ProductTypesIn property, you can reduce the number of product types displayed. Just omit
the desired product type in the property.
The variable that is in the ProductType property serves as the basis for forwarding in the workflow
flow. In the existing workflows (supplied workflows or here), the property is assigned the
productType. Variable declarations are found at the lower edge of the Workflow Studio.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                       60
The specified article types are all assigned to a flow, which specifies the further dialog possibilities
in A+W iQuote for the respective type. If an article type was selected in A+W iQuote, the
workflow runs to the next ActionValidatorProduct.
Important for the selection of the article from the back end is precisely this
ActionValidatorProducts, here displayed as ValidatorProducts and its following parameters.




Only after selection of an article does the workflow run via the next elements in the flow chart.
The article determination from the back end looks like this when encountering the
ActionValidatorProducts:
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and a.atyp= $productType and a.prodbemass=0…

$sprache  current iQuote language
$productType  the value from ProductTypesIn


Exceptions:
Fixed products/dimensioned products with the Artikeltyp=1000
If you use the Artikeltyp=1000, then the select where condition looks like this:


A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                61
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and (a.prodbemass=1 or a.prodbemass=2)“ attached.

$sprache  current iQuote language


IGU grouping by technical values
If you would like to use the technical values grouping of the IGU products, you can use the
workflow implementation from an existing workflow. The master data maintenance is in section
Product groups.
The difference from other article types is in the ProductGroupIn property of the
ActionValidatorProducts. The property filled out in the default as "0" will now be changed for the
group in question.
The groups are:
 Value                             Group                            Database reference
 „1“                               Energy/heat insulation           artikel.kgrp
 „2“                               Acoustic/sound damping           artikel.dbgrp
 „3“                               Sun/energy transmission          artikel.ggrp




The select where condition is expanded as follows:
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and a.atyp= $productType and $gruppe;


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            62
$sprache  current iQuote language
$productType  the value from ProductTypesIn
$gruppe  "a.kgrp>0" or "a.dbgrp>0" or "a.ggrp>0"


11.5.2.            Article group
In the Workflow Studio, you will find the ActionValidatorProductGroups widget for the article
groups, which is abbreviated in the following examples as ValidatorProductGroups by the display
name. In the Workflow Studio Toolbox (left side), you will find the widget under iQuote Common
> Product Groups.
As the name indicates, here you are no longer working exclusively with article types, but rather
with article groups. But not just with article groups, but also together with article types. You
should be sure how you want to structure the workflow before you create article groups and
assign these article groups to articles. The various set-up possibilities are described below.


So that you can use the widget, article groups must be created in the master data. For
information about creating article groups in A+W Enterprise, see Product groups in the master
data section.
  Product Groups
  Selection of the product groups by product type number or product groups. The images are searched for in the Image
  directory.
  Parameter             Description                                                       Default
  Category              Display of category (breadcrumb)                                  AWSOA.Core.Messages.Globa
                                                                                          l.WebCategoryProduct
  Configurator          Access to the Configurator service                                Configurator
  ContentPath           Relative directory for the content of the widget in the Content   e.g. "auw/producttypes"
                        directory
  Description           Description that appears after the widget header
  Display Name          Name of the activity in the Studio workflow
  ItemIn                Incoming item object of iQuote                                    ItemIn
  ItemOut               Output item object of iQuote                                      ItemOut
  Name                  Title of the widget in iQuote
  ProductGroup          Selected product group as workflow variable
  ProductGroupsIn       ERP product group number that should be displayed                 „2,3,4,…“
  ProductTypesIn        ERP product type number for display of all groups of the types    "1" or "0"



The variable that is in the ProductGroup property serves as the basis for forwarding in the
workflow flow. In the existing workflows (supplied workflows or here), the property is assigned
the productGroup. Variable declarations are found at the lower edge of the Workflow Studio




A+W Software GmbH                     EN-CONFIG-A+W Enterprise iQuote.docx                                      63
The properties ProductGroupsIn and ProductTypesIn are required in different variants, which will
be described below.
Simplified, the ProductGroupsIn property is the listing of the desired article groups that should be
displayed.
And the ProductTypesIn property is used to display all article groups or just the quantity listed
from ProductGroupsIn.




The article groups used are assigned a flow in the workflow; it specifies the further dialog
possibilities of the respective group in A+W iQuote. The product groups can be defined at will; in
the example above, we set the groups equal to the AWTypes for better legibility.
If you click on an article group in the A+W iQuote selection menu (1. Selection list), the workflow
runs up to the next ActionValidatorProducts.
Important for the selection of the article from the back end is precisely this
ActionValidatorProducts, here displayed as ValidatorProducts and its following parameters.




ProductGroupsIn: The group in the select where that reflects the artikel.bearbkat. (There are
exceptions!)
ProductId: Variable for forwarding the article clicked on. This variable is used in the other widgets
in the workflow.
ProductNumberIn: Not used in AWE

A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                64
ProductTupleId: Not used in AWE
ProductTypesIn: Article type that reflects the artikel.atyp in the select where (there are
exceptions!). With "1" this field is ignored.
Option 1: Display all article groups
If you want to display all article groups from the master data in the first search bar, then you must
set the properties ProductGroupsIn and ProductTypesIn to "0" in the
ActionValidatorProductGroups.
In the ActionValidatorProducts, the PropertyGroupsIn must have a value of the groups that are in
the best case reached with the above-mentioned variable. The ProductTypesIn Property is
assigned "-1".
Option 2: Display a quantity of article groups
If you want to generate more complex workflow flows, you can reduce the number of product
groups displayed in the ProductGroupsIn property. Thus, only the desired product groups will be
listed. To do this, you must set the ProductTypesIn property to "1".
With this construct, you can now work with subgroups in the workflow. All subgroups must be
attached to the workflow flow of a main group via collection (Workflow Studio > Toolbox >
Control Flow > Sequence)(take example for this from an existing workflow).
Important to note is that you must create the main group that must be specified in the
ActionValidatorProductGroups and the last subgroup before you come to the product selection in
the master data article groups. If in the meantime you insert groups into the workflow, these
intermediate groups are only attached via collection (Workflow Studio > Toolbox > Control Flow >
Sequence).
With this variant, there are a lot of possibilities for generating a workflow for a customer.
The selection of the article quantity of an article group is also only triggered with reaching of the
ActionValidatorProduct in the workflow.
Option 2.1: Only select on article group
ProductGroupsIn: Must match the last article group in the flow
ProductTypesIn: "-1"


Where:
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and a.bearbkat = $artikelgruppe and a.prodbemass=0…”


$sprache  current language
$artikelgruppe  article group from ActionValidatorProducts


Option 2.2: Select article group and article type
ProductGroupsIn: Must match the last article group in the flow
ProductTypesIn: Is set to the desired article type. (e.g. "200" for insulated glass)



A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                               65
Where:
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and a.bearbkat = $artikelgruppe and a.atyp = $artikeltyp and
a.prodbemass=0…”


$sprache  current language
$artikelgruppe  article group from ActionValidatorProducts
$artikeltyp  article type from ActionValidatorProducts
Option 2.3: Article groups with fixed articles

ProductGroupsIn: Must match the last article group in the flow
ProductTypesIn: "1000" (iQuote-exclusive type, is not used directly in the select)

Where:
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and a.bearbkat = $artikelgruppe and (a.prodbemass=1 or
a.prodbemass=2)…”


$sprache  current language
$artikelgruppe  article group from ActionValidatorProducts


Option 2.4.1: Article group from the article type insulated glass
There is a particularity for the article type IGU since there we have the variant with the technical
values as basis. See exception under Art. Type.

ProductGroupsIn: Must match the last article group in the flow, this article group must be greater
than 3 since the values "1", "2", and "3" are blocked for the implementation of the technical
values.
ProductTypesIn: "200" for insulated glass


Where:
…from artikel a, artbezfremd b where a.artnr = b.artnr and a.verkart = 2 and a.still = 0
and b.sprkz = $sprache and a.bearbkat = $artikelgruppe and a.atyp = 200 and a.prodbemass=0…”


$sprache  current language
$artikelgruppe  article groups from ActionValidatorProducts (greater than 3)




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               66
11.5.3.            Article
For the article selection, the ActionValidatorProducts widget is required.
  Product
  Selection of the products that are defined via the properties of the activity
  Parameter                     Description                                                   Default
  Category                      Display of category (breadcrumb)
  ContentPath                   Relative directory for the content of the widget in the       „auw/products“
                                Content directory
  Description                   Description that appears after the widget header
  Display Name                  Name of the activity in the Studio workflow
  ItemIn                        Incoming item object of iQuote                                ItemIn
  ItemOut                       Output item object of iQuote                                  ItemOut
  Name                          Title of the widget in iQuote
  ProductGroup                  Returns the product group of the selected product.            ProductGroupOut
  ProductGroupsIn               Enumeration of the product group numbers of the ERP           „100,101,102“
                                that should be displayed (additive to other enumerations)
  ProductId                     Number of the selected product
  ProductNumbersIn              Enumeration of individual ERP product numbers that            „1004,1005,1006“ or 104-
                                should be displayed (additive to other enumerations)          110,118
  ProductType                   Returns the product type of the selected product.             ProductTypeOut
  ProductTypesIn                Enumeration of the product type numbers of the ERP that       „1,2,3“
                                should be displayed (additive to other enumerations)
  AutoSelect                    The first product will be selected automatically and thus     False
                                the workflow is forwarded and the next widget
                                established.
  OptionShowStockOnSite         Stock inventory display of an article from several clients.   False
                                Configuration under 9.12
  OptionShowCoating             NOT IN USE for AWE
  OptionShowPattern             NOT IN USE for AWE
  ProductTupleId                NOT IN USE for AWE




For checking which select condition was generated for your article selection, you can search for
the following line in the documentservice log (backend):
documentserverhelper::fillProductCacheByType artikel_fastselect_count with ' artikel.verkart=2
and artikel.still = 0 and artbezfremd.sprkz = 1 and artikel.bearbkat=150 and artikel.prodbemass=0'
The where clause is output once at the end of the selection function.
                11.5.3.1.   Expansion of return value ProductType and ProductGroup
With the development #101398 ([AW-144589]) an upgrade for the ActionValidatorProducts in the
Workflow Studio was developed. The ActionValidatorProducts now, in addition to the product



A+W Software GmbH                     EN-CONFIG-A+W Enterprise iQuote.docx                                         67
number, also returns the product type and product group of the selected article. This
development enables the construction of more specific workflows for the customer.
During the configuration of the workflow, it is now possible to access the product group and the
product type of the selected article. Important is that you assign variables to the two new return
parameters (ProductGroup and ProductType), which were initialized as integers.
See sample figures:




You can access these variables after running through the ActionValidatorProduct (called
ValidatorProducts in the flow diagram).
Flow explanation of the sample figure:

A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             68
Before the ValidatorProducts, the workflow runs through a product group or a product type.
These are not relevant for us, since for the steps after the article selection, we would like to work
with the return values.
If the workflow now comes to the ValidatorProducts, the product number (ProductId), product
group (ProductGroup), and Producttype (ProductType) of the article selected in A+W iQuote are
returned.
Please make sure that the workflow loops of a product group or a product type are always run
through, even if no article has been selected. In order to have no tab (such as Geometry, for
example) show before the selection, we have inserted the decision query after the
ValidatorProducts ("Filter float products" can be ignored). With the condition: "productId > 0", the
workflow strand will only keep running if an article was actually selected; that is the article
number is greater than 0. As default value if not yet selected, the C# integer MinValue is returned,
which corresponds to -2,147,483,648.
In the subsequent switch, the product type recorded is evaluated from the ValidatorProducts. In
this flow, a group with float glass is formed, which can come with different product types. With
this flow, we have switched off the processing tab (ActionValidatorProcessing) for all articles with
product type: 110 since this strand only runs through the geometry (ValidatorGeometry). Lites
with product type has both tabs active.




Remarks:
Please note that the ActionValidatorGeometry must always be before the
ActionValidatorProcessing; otherwise, there can be problems during transfer to the backend.
            11.5.3.2.   Expansion of the input parameters


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               69
With the development [AW-162515] the input parameters ProductTypeIn, ProductGroupIn, and
ProductNumbersIn were expanded for the article selection to the possibility of a list transfer.
It is now possible to select several product groups or product types via string listing (e.g., "1,2,3,4"
or "100,130,150,200").
The effect of this possibility is to use the select condition to access the table artikel using IN clause
and to no longer be dependent on an article group (artikel.bearbkat) or an article type
(artikel.atyp).
The same applies for article numbers with ProductNumbersIn. If an article listing (e.g., "110044,
110055, 500044") is entered in this property, then the select condition is expanded by an IN
clause to the table artikel to the database field artikel.artnr.

Exceptions:
IGU grouping for technical values
The IG grouping for technical values (4.3.2 Artikelgruppe) are not possible with the string listing
for all 3 parameters. Should you want to use the IG grouping for technical values, then you must
fill this workflow string using individual article group and article type=200.
Fixed articles
If you would like to use the string listing for fixed articles, then you can still transfer the "1000" as
value to the ProductTypeIn. If you should transfer several article types, then you must put 1000 at
the end (e.g., "100, 130, 150, 1000").
With 1000, the select condition is changed from "artikel.prodbemass=0“ to "artikel.prodbemass=1
or artikel.prodbemass=2".


11.5.4.           Geometry
  Geometry
  Entry of the geometry data. All shapes enabled for iQuote appear in this widget. It enables the entry of an additional
  dimension or the width and height of the rectangle
  Parameter                    Description                                                            Default
  Category                     Display of category (breadcrumb)
  ContentPath                  Relative directory for the content of the widget in the Content        unused
                               directory
  Description                  Description that appears after the widget header
  Display Name                 Name of the activity in the Studio workflow
  ItemIn                       Incoming item object of iQuote                                         ItemIn
  ItemOut                      Output item object of iQuote                                           ItemOut
  Name                         Title of the widget in iQuote
  DefaultRectangleWidth        Specified width of the rectangle
  DefaultRectangleHeight       Specified height of the rectangle
  RectangleOnly                Only rectangle entry should be possible. No shapes.                    False
  ShapeFilters                 Filter to restrict the available shapes and products                   CartItemActionFilter
                                                                                                      Object
  ValidGeometry                Entry of a valid geometry


A+W Software GmbH                     EN-CONFIG-A+W Enterprise iQuote.docx                                           70
  SelectedGeometry        Selected geometry (object must be defined as variable)   GlassShape Object
  WidthOnly               Only the width is displayed. No shapes.




11.5.5.         Subgroups/collections
In this example, a product group 830 has been created, which runs into the workflow outside of the
screen.     This    group    will   be    assigned    subgroups      via   collection   "Others."




The content of the "Others" collection is taken up by a ValidatorByFunction widget and processed
further. With the switch widget, the 2 paths of the product group are determined.

In the ValidatorProducts widgets, the product groups are passed along as ProductGroup and the
values from the ValidatorByFunction (830, 100) as ProductType.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            71
The ProductGroup is used for the select on the artikel table as artikel.bearbkat. ProductType is used
as artikel.atyp.


11.6.           Workflow shopping cart information
It is possible to access particular data that is stored in the shopping cart in the workflows. The
following information is accessible:
 Name                               Data type                        Application
 Project no.                        Integer                          Cart.Header.ObjectNo
 Market partner no.                 Integer                          Cart.Header.CustomerNo
 Document type (order or            DocumentTypeViewModel            Cart.Header.DocumentType
 quotation)                         (quotation or order)             (Example:
                                                                     Cart.Header.DocumentType =
                                                                     DocumentType.Quotation)

 Language code                      String                           Cart.CurrentItem.Culture
                                                                     (See Chapter: Multi-
                                                                     language support)


Example:




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                72
11.7.             CheckOut Workflow
The Checkout workflow controls the process of order completion. After the configuration of the
products, delivery addresses and delivery dates as well as order texts and reference numbers
(order number), it allows entry. Essentially each checkout activity can also be used in the Checkin
workflow. Sometimes it makes more sense to determine data such as the delivery information
after entering the products.
  InOut DeliveryDate
  Entry of the delivery date and the delivery time. For determination of the delivery date, the default delivery times of all
  products in the cart are examined and the date with respect to the longest delivery time is the suggested delivery date. If
  a weekday is stored in the customer route in the ERP, delivery is shifted to the next possible route day. This is a non-
  binding delivery request by the customer.
  Parameter                 Description                                                       Default
  Category                  Display of category (breadcrumb)
  ContentPath               Relative directory for the content of the widget in the Content   unused
                            directory
  Description               Description that appears after the widget header
  Display Name              Name of the activity in the Studio workflow
  ItemIn                    Incoming item object of iQuote                                    ItemIn
  ItemOut                   Output item object of iQuote                                      ItemOut
  Name                      Title of the widget in iQuote
  CustomerNoIn              Number of the customer for whom the route days should be          Cart.Header.CustomerNo
                            determined



A+W Software GmbH                     EN-CONFIG-A+W Enterprise iQuote.docx                                           73
 DesiredDeliveryDate       Specification of the delivery date, there is no more calculation   DateTime.MinValue
                           using the delivery time and route day
 DeliveryTimeHide          The delivery time can be switched off with this property           "True" = delivery time will not
                                                                                              be displayed
 DeliveryTimeFrom          Specification of the delivery time from                            new TimeSpan(18,0,0)
 DeliveryTimeUntil         Specification of the delivery time until                           new TimeSpan(8,0,0)
 SelfCollects              Collection with KeyValue objects for self collection               New
 SelfCollectSelected       Selected key value for self collection                             „0“
 BlockDaysBeforeMin        If true, then the days before the first possible delivery date     False
 DeliveryDate              are removed from the calendar.
 ShowDispatchType          Display of the dispatch type selection                             False



 InOut DeliveryAddress
 Entry of the deviating delivery address. The existing delivery addresses are offered for selection. However, any delivery
 address can also be entered. Any change to an existing delivery address causes the customer number of the delivery
 address to be reset. It is then no longer the default delivery address.
 Parameters                      Description                                                  Default
 Category                        Display of category (breadcrumb)
 ContentPath                     Relative directory for the content of the widget in the      unused
                                 Content directory
 Description                     Description that appears after the widget header
 Display Name                    Name of the activity in the Studio workflow
 ItemIn                          Incoming item object of iQuote                               ItemIn
 ItemOut                         Output item object of iQuote                                 ItemOut
 Name                            Title of the widget in iQuote
 SelectionOnly                   Selection of delivery addresses possible, no changes or      False
                                 new entries
 CustomerNoIn                    Number of the customer for whom the delivery                 Cart.Header.CustomerNo
                                 addresses from the ERP are displayed
 ShowCountryDropDownList         Displays the country selection in the address input          False




A+W Software GmbH                    EN-CONFIG-A+W Enterprise iQuote.docx                                            74
12. Overview of orders and inquiries
12.1.           Reporting
Under the AWDesk case #439086 or Feature 20920, the reporting for A+W iQuote was developed.
The required components have to be from the release May 2021 or older.
    •   alcib
    •   documentservice
    •   A+W Printservice 6
    •   A+W Commercial 6 Converter Services
    •   A+W iQuote 6 Services
    •   A+W iQuote 6 Web
    •   Environment update
The print jobs are listed in A+W iQuote on the <My orders> or <My order purchase order
requests> dialog window. For this, the desired PO with the little triangle on the first line has to be
opened and under the <Reports> tab, the print jobs are listed. These reports are always created as
PDF and can be downloaded by the customer.




The reports displayed are PDF copies, which are generated during printing. These PDF copies are
stored under the DATEI_REF_PFAD with document number and subfolder 0, e.g.
\\aweawpvnext.tse.intra\Trans\AWE\dokuserver\140\500563\0
Today, the structure of DATEI_REF_PFAD is not distinguished from document types and/or
subnumbers; accordingly, the following subfolders are specified:
    •   For delivery notes, in the future, a subfolder
        DATEI_REF_PFAD\delnote\<ORDERNR><SUBNR> will be used
    •   For invoices the folder DATEI_REF_PFAD\invoice\<AUFTRNR>
    •   For collective invoices, we write the file in all invoices (all subnr)
    •   For collective invoices of the folder DATEI_REF_PFAD\invoice\<ORDERNO><SUBNR>
This modification was made with ButItem 129598 since the old path is not suitable for the
document attachment. With this modification, all document files are now stored centrally.


A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                              75
The named PDF copies do not absolutely have to be A+W iQuote relevant. This functionality can
also be used for customers who would like to attach PDF copies of desired forms to their
documents.
A+W Enterprise Master Data
On the document types dialog (Master data > Keys > System > Document types), there is a new
document type (3 - print output). A new document type with the new document type <3 - Print
output> has to be created.




This document type can be assigned to the desired forms on the assignment dialog (System >
Print management > Forms > Document type assignment). In the ongoing process, these forms
are attached to the associated document.




A+W Enterprise printing
So that the assigned forms are created and stored as PDF copy in the print area of A+W Enterprise
(Master data > Purchasing/Sales > Forms > Printing/e-mail/fax), the following settings have to be
configured.
The environment variable ATTACH_PRINTOUTS_TO_DOCUMENT is activated, the database script:
130004136_printparam.sql executed, and the stored procedure rppdfcopyfilename set up.
The environment variable ATTACH_PRINTOUTS_TO_DOCUMENT can be assigned 1 for A+W
iQuote processes (kauf.eingang = 14) or 2 for all processes.
The stored procedure rppdfcopyfilename has the following call parameters: integer pid, short
seqnr, short formart, integer auftrnr, short vorgang, short subnr and has the return value


A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                            76
char(128) filename.
It is urgent that you pay attention that all form types used are included in the SP and get unique
names. Precisely for the form types that process documents that can contain subnumbers (e.g.
delivery note), the subnumber in the name is important so that the uniqueness of the file names
can be guaranteed.
A+W Print Service 6
The A+W Print Service 6 generates an additional PDF copy of the current print job for print jobs,
copies this PDF document to the reference path (DATEI_REF_PFAD), and attaches this PDF
document to the associated transaction.
The environment variable DATEI_REF_PFAD has to be maintained for the print service and the
settings for the A+W Enterprise print made so that a file name is generated in the database field
printparam.pdfcopy. The A+W Print Service checks whether the DATEI_REF_PFAD is filled and a
file name is present in printparam.pdfcopy; only then is the PDF copy procedure initiated.
Since the print service has to generate folders in the area of the DATEI_REF_PFAD path, it should
be checked whether the user who is entered for the A+W print service has rights to the
directories used.
documentservice
The documentservice obtains from the table kaufdruck with order no. (kaufdruck.auftrnr),
document (kaufdruck.vorgang), type of printing process = 2 (kaufdruck.druckart) and report type
= 1 (kaufdruck.repart) the stored expressions and provides this information to A+W iQuote
weiter.
A+W Commercial 6 Converter Services
The A+W Converter Service has to be updated and serves to transfer the files from the reference
path to A+W iQuote if a customer would like to download a file.
Restrictions/notes:
    •   Only Crystal Report print jobs can be used
    •   Reports can only be stored as PDF on the transaction
    •   If a form is printed out several times, the last printing is always displayed in A+W iQuote


12.1.1.         Display of files name
With the development [AW-157964] the display of the printouts is restructured to the file names.
The name displayed is now determined from kaufdruck.filename.
As described under 9.1 Reporting , the database field kaufdruck.filename is filled from
printparam.pdfcopy, which gets the name generated from the Stored Procedure
rppdfcopyfilename .




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                77
12.2.           File attachments
The attachment of files for the A+W iQuote was developed under AWDesk case #439086 or
Feature 20920. The required components have to be from the release May 2021 or older.
    •   alcib
    •   documentservice
    •   A+W Commercial 6 Converter Services
    •   A+W iQuote 6 Services
    •   A+W iQuote 6 Web
    •   Environment update
A+W iQuote 6
The file attachments are listed in A+W iQuote on the <My purchase orders> or <My purchase
order requests> dialog window under the respective purchase orders or purchase order requests.
For this, the desired PO with the little triangle on the first line has to be opened and under the
<Attachments> tab, the print jobs are listed. These file attachments can be downloaded by the
customer.




A+W Enterprise
In the A+W Enterprise order entry (Sales > Order entry), now file attachments for the A+W iQuote
can be approved. For this, you have to open the desired order or quotation, attach the desired file
with the document assignment ([CTRL]+[K]), and activate the online checkbox. Or after the fact
for an existing file, activate the online checkbox.


12.3.  Copying or transforming from order or
  quotation
With the tickets [AW-64004] and [AW-109408] the functionalities copy and transformation of
order and quotations were enabled.
In order to activate the functionality, the set-ups named in the ticket (or newer) must be installed
and the following switches in the Infrastructure.Web > Configuration > A+W iQuote > Business
case functions must be set.



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              78
Im A+W iQuote Enterprise, there is currently only the middle business case "customer order." Of
course the individual functions can be activated or deactivated independently of one another.
After the configuration, the buttons are displayed when A+W iQuote is restarted (browser +
Web.Configurator).




If the history display should also display A+W Enterprise Backend orders or quotations, then the
buttons for copying and transforming will be grayed out because we cannot generate these
orders/quotations in A+W iQuote. The copy or transformation will be enabled by the basis of the
AWSOA database (iQuote DB).




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                            79
13. Exchange dialogs
13.1.           Muntins
With the case #452497, a simplified muntin entry was developed for A+W iQuote.

So that you can attach muntins for IGs, exchange groups for the muntins have to be created in A+W
Enterprise. First groups have to be generated in which the individual muntin articles are listed.
These groups are created on the Exchange Groups – All Descriptions – dialog (Master Data > Codes>
Products> A+W iQuote-specific details> Exchange Groups> All Descriptions).

These groups have to be maintained in A+W Enterprise via the Group Assignment (Article) – dialog
(Master Data> Codes> Products> A+W iQuote-specific details> Exchange groups> Group Allocation
(articles)). If the group is complete, the group can be added to the respective BOMs in the spacer
of the IG. It is possible to add muntin groups and spacer groups to the BOM entry for the spacer.

If you would also like to have the muntin colors displayed for the muntins in question, the
parameter ColorHide on the Invalidation must be set to false (see 5.5. Sprossen über den Workflow
einrichten). Here it is important to note that the colors maintained in A+W Enterprise have red,
green, and yellow values to be set in Master data > Codes > Products > Variants > Colors > Colors.
These values are used in order to generate the selected color in A+W iQuote; it is then displayed. If
the colors are not maintained, black is generated as basis.




So that the muntin dialog can be used in A+W iQuote, adjustments have to be made to the "0000
– A+W iQuote" workflow. The ActionValidatorBar is on the left in the toolbox of the Workflow
Studio.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              80
So that the muntin extension is activated, the ActionValidatorBar has to be attached in the
workflow in the IG area.

If you would also like to have the muntin colors displayed for the muntins in question, the
parameter ColorHide on the ActionValidationBar must be set to false.


13.2.           Gas for IG exchange
Master Data
For the gas exchange, the desired gas must be in the BOM of the main article, that is, of the IG,
and not in the spacer BOM. Exchange groups with gases can then be made available to this gas.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                81
If it should be an IGU with more than two types of glass, then for each spacer you must add a gas
and assign the gas the same installation position as the spacer.

Workflow
So that the gas exchange can be used in A+W iQuote, the "0000 – A+W iQuote“ workflow has to
be adjusted in the Workflow Studio.




The ActionValidator exchange (used for the exchange dialog), to be found in the branch of the IG,
now has a parameter GasHide. This parameter must be set to false and after that, it is possible to
use the extension for the gas exchange in A+W iQuote.


13.3.            Spacer exchange filters
The filters for the spacer exchange for IG are set up via workflow (see: Filter Möglichkeit für
Rahmen über den Workflow). The data for the filters is determined from the table xchangegrp.
If the AIR filter is set up, the AIRs maintained on the Group Assignment dialog (Master Data >
Codes > Products > A+W iQuote-specific details > Exchange Groups > Group Allocation (spacers))
are determined and offered as filter possibilities.
If the group filter is set up for the spacer, then it is possible to filter according to the colors of the
spacers. The selection possibilities for the spacer colors are drawn from the description of the
table artikel and the data field artbez1. This description is displayed on the Group Allocation



A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                                  82
dialog. Important is that the article have a "RAL" + four-digit number somewhere in this
description. Examples: Ral 1234 or RAL 1000 or ral 3007




Similarly, in the table xxfarbe, the RAL code used must be maintained so that a color description
can be drawn from the database and the filters in A+W iQuote have a proper description. The RAL
code can be maintained on the Color dialog (Master Data > Codes > Products > Variants > Colors >
Colors).
So that the filters in A+W iQuote become active, a sequence of FilterMethods must be added in
the branch of the IG. This sequence has to be inserted after the ValidatorExchange.




Currently there are two filter possibilities. First the filter of the thickness or of the AIR and second
the filter for descriptions within the article description. RAL codes are used as an example here
since some of our customers display different spacer colors via RAL code in the product
description and the product variants are specified for the price calculation using the thickness.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                 83
The filter possibilities for the AIR are determined from the Exchange Group (spacers) dialog or the
table xchangegrp. The filter possibilities for the second variant are drawn from the article
description of the exchange spacers created. In the current state (04/01/2020), this variant
searches for the RAL codes for different colors.
For more information, please read the master data maintenance documentation:
Rahmenaustausch Filter


13.4.           Article designation filter for IGU exchange
The filter in the main workflow of A+W iQuote is set up with the extension point: 0000 – A+W
iQuote. The workflow to be changed must be opened with the Workflow Studio. Now you enter
the flow chart with a double-click on "Workflow Core".
The filter will be added to any existing collection, as described under Spacer exchange filters.




The collection is on the left in Workflow Studio and found under Control Flow as sequence. Drag
the sequence into the workflow and attached in the IGU product branch after the IGU exchange
widget (ActionValidatorExchange). The collection must only be assigned a name in the properties.
Open the collection with a double-click. Now under iQuote Methods, the
ProductExchangeFiltersByType is dragged in. This filter is required several times if you would like
to filter spacer and different glass types. For each product type (TypeId), you need one of these
filters.



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               84
In the example above, I have three filters active for the spacer (TypeId=60). Thickness and product
group (as explained under Spacer exchange filters) and the new filters for the article description. I
have duplicated and changed the article description filter for floats (TypeId=1). If you have TGH or
LAMI in your exchange groups, you must also add a filter for these TypeIds.
Please make sure that in the first filter in the collection, the ClearFilter property is set to true. Set
the description filter for the ClearFilter property to true if it is not a spacer. Otherwise there will
be doubled filter data fields for the glass.
  ProductExchangeFiltersByType
  Parameters              Description                                                          Default
  ClearFilter             Deletes the filter collection; should be set to true for the first   False
                          assignment and then to false for all others
  Configurator            Access to the Configurator service                                   Configurator
  Description             Description of the filter that is displayed in iQuote; if blank,
                          then the default description is displayed
  Display Name            Name of the activity in the Studio workflow
  ExchangeFilterType      Type of the filter, e.g. by thickness or by product type and         ExchangeFilterType.
                          group
                                                                                               Thickness
                                                                                               ProductGroup
                                                                                               Description
  ItemOut                 Initial item object of iQuote; the filter is inserted here           ItemOut


  TypeId                  The product group to be selected (e.g. 1 = float glass, 2 = TG,
                          3 = LAMI, 60 = spacer)



After all filters have been set up, the workflow must be saved and the WebConfigurator restarted.


13.5.            Structure and coating
With the development #104283 the display of surface processing structure and coating in IGU
exchange was taken up.
Master Data
The coating or structure must be maintained on the article master data dialog (Master data >
Articles > Phys. properties) for the individual types of glass under surfaces. It can be set to
structure one-sided or coating. These values are supported in A+W iQuote.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise iQuote.docx                                              85
Workflow
The small cloud next to the sun serves to rotate the patterned glass. For coatings, the rotation
function is not released.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               86
The rotation mechanics (cloud) can be deactivated if this function is not wanted.
For this, you must open the configurator in Workflow Studio and set the PatternCloudHide
property to true in the ActionValidatorExchange.




The default value for PatternCloudHide is false.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                       87
14. Delivery information
14.1.           Self collection as note
With the development #101611 the self collection information for the A+W Enterprise was
expanded.
For orders entered in A+W iQuote that were marked with self collection, now preliminary notes
are generated in the A+W Enterprise order entry. These preliminary notes receive the priority
high and contain the text of the selection box of the delivery information dialog.
For this change, the SelfCollect - Collection in the CheckOut workflow should be filled with
sensible texts so that more unique texts are displayed in the preliminary notes. It would be best if
the texts could be created due to multi-language support. For this, please read the multi-language
support chapter.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             88
Individual collection KeyValues:
A KeyValue with Key = 0 must always be created!




Example:




The KeyValue.Description generated in the item is displayed in the selection box and later in the
document note.


A+W Software GmbH                  EN-CONFIG-A+W Enterprise iQuote.docx                         89
14.2.          Country selection
With the development #92728, the country selection in the delivery address for A+W iQuote was
added.
The country data field is a selection box that is filled with the database data from xland and
xsprbez. Attention must be paid that a translation of the countries for all languages approved in
A+W iQuote is provided. The country names are maintained on the country dialog (Master data >
Keys > Partners > Countries).
If for a selected language you change the country via the selection box, the marking of the
address in the selection list is removed and a new address generated if the order or the quotation
is sent to A+W Enterprise.




For configuration of the country data field, you must open the CheckOut workflow and set the
Property ShowCountryDropDownList to true in the InOutDeliveryAddress widget. Default value of
the Property ShowCountryDropDownList is false.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             90
14.3.   Minimum delivery                                     time           in       calendar
  (procurement time)
In A+W iQuote, the delivery dates on the calendar are now pre-populated with consideration that
the routine days starting on which the earliest possible date is pre-populated [AW-109411]. See
4.3.6




It is possible to block the days before a calculated date (image: 10/17/2023). For this, the



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                           91
property BlockDaysBeforeMinDeliveryDate in the InOutDeliveryDate widget must be set to true in
the Workflow Studio.




The days before the date will thus be removed from the calendar.




14.4.          Pick-up times/dispatch times
In the "Checkout" workflow activity, it can be configured whether the delivery time can be
entered.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                          92
So that this data is also taken over into the A+W Enterprise order, Set 8 in the "Configurable fields
of the document entry" (Master Data - Field Configuration - Document Field Configuration) for the
order header (table: kaufprvfld) must be created with 2 char fieldnr.




14.5.           Disp. Type
With the development [AW-178430], the selection possibility of the dispath type is included in the
delivery information of the A+W iQuote. There is no pre-population of the dispatch type.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              93
The data for the selection list of the A+W iQuote comes from the A+W Enterprise master data. For
this, the required dispatch types (Master Data > Keys > System > Dispatch > Dispatch Type) must
be set to online.
documentservice - 13.04.7673 (May 2025) - VERSARTHOLEN_BEI_ROUTENAEND
(see also „EN-CONFIG-A+W Enterprise“)
By default, the dispatch type is determined from the master data (see "EN-CONFIG-A+W
Enterprise" - "Dispatch type vs. route")
If the dispatch type is changed in iQuote, there is an attempt to find a route automatically. If there
is a clear assignment, this route is taken over. If there is no clear assignment, the route with the
highest priority (1= highest, 9999 lowest priority) is taken. If no clear assignment is found here,
the first appropriate route that was found for this dispatch type is used and the order includes a
note that no clear route could be determined.




To switch on the dispatch type in the A+W iQuote, you must adjust the CheckOut workflow via
the Workflow Studio. Open the CheckOut workflow and select the
ActionValidatorInOutDeliveryDate widget. There, the "ShowDispatchType" property must be set
to true.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                               94
A+W Software GmbH   EN-CONFIG-A+W Enterprise iQuote.docx   95
15. Operation
On request from our users, the user friendliness was also increased. The following changes in
A+W Enterprise iQuote count toward this:
    •   Next and Back buttons in entry
    •   New entry flow on the processing dialog
    •   Info texts for the selection of dimensioning type for corners and edges.


15.1.           Article designation filter
QR2302: With the development [AW-118384] the filters for article designation were implemented
in A+W iQuote. The filter can be used for articles from the article selection, processings, and the
IGU exchange. To simplify the search for the user, we have made the filter not case-sensitive.




15.1.1.         Set-up filter for article selection
If you want to set up the description filter for the article selection, the filter for each article
group and each article type must be created in the workflow.
The filter in the main workflow of A+W iQuote is set up with the extension point: 0000 – A+W
iQuote. The workflow to be changed must be opened with the Workflow Studio. Now you enter
the flow chart with a double-click on "Workflow Core".
The filter can be inserted for any product branch after the product widget
(ActionValidatorProducts). Each product branch, whether run through with product type or
product group, has its own flow and must be maintained separately.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                                 96
The ProductFilters are on the left side of Workflow Studio under iQuote methods. The
ProductFilters widget takes you to the workflow. It's best to maintain the properties of the widget
once since the parameters can be the same for all product branches. Then duplicate with
Copy+Paste and attach. For better legibility in the workflow, the display name can be changed for
individual product branches.
  ProductFilters
  Parameters             Description                                                          Default
  ClearFilter            Deletes the filter collection; should be set to true for the first   False
                         assignment and then to false for all others.
                         If without collection created set to true; otherwise there is
                         incorrect behavior.
  Configurator           Access to the Configurator service                                   Configurator
  Description            Description of the filter that is displayed in iQuote; if blank,     MUST CURRENTLY REMAIN
                         then the default description is displayed                            EMPTY!!!
  Display Name           Name of the activity in the Studio workflow
  ItemIn                 Incoming item object of iQuote                                       ItemIn
  ItemOut                Initial item object of iQuote; the filter is inserted here           ItemOut
  ProductFilterType      Type of the filter, here only name                                   ProductFilterType.
                                                                                              Description


If the ProductFilter widget is filled, it must still be inserted into the desired product branch. For
this, click the arrow that points down after the ActionValidatorProduct widget and remove it. Now
position the mouse over the same widget and you will see small squares appear. Select one of the
squares and drag it to the new ProductFilter widget using drag and drop. The ProductFilter widget
must then be connected to the additional widget so that the flow of the product branch is closed
again.
After all filters have been set up, the workflow must be saved and the WebConfigurator
restarted.


15.1.2.          Set-up of filter for processing
The filter in the main workflow of A+W iQuote is set up with the extension point: 0000 – A+W
iQuote. The workflow to be changed must be opened with the Workflow Studio. Now you enter
the flow chart with a double-click on "Workflow Core".


A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                                             97
The filter can be inserted for any product branch after the product widget
(ActionValidatorProcessing). Each product branch, whether run through with product type or
product group, has its own flow and must be maintained separately.




The ProcessingFilters are on the left side of Workflow Studio under iQuote methods. Drag the
ProcessingFilters widget to the workflow. It's best to maintain the properties of the widget once
since the parameters can be the same for all product branches. Then duplicate with Copy+Paste
and attach. For better legibility in the workflow, the display name can be changed for individual
product branches.
  ProcessingFilters
  Parameters             Description                                                          Default
  ClearFilter            Deletes the filter collection; should be set to true for the first   False
                         assignment and then to false for all others.
                         If without collection created set to false; otherwise there is
                         incorrect behavior.
  Configurator           Access to the Configurator service                                   Configurator
  Description            Description of the filter that is displayed in iQuote; if blank,
                         then the default description is displayed
  Display Name           Name of the activity in the Studio workflow
  ItemIn                 Incoming item object of iQuote                                       ItemIn
  ItemOut                Initial item object of iQuote; the filter is inserted here           ItemOut
  ProcessingFilterType   Type of the filter: here only possible by name                       ProcessingFilterType.Descri
                                                                                              ption


If the ProcessingFilters widget is filled, it must still be inserted into the desired product branch.
For this, click the arrow that points down after the ActionValidatorProcessing widget and remove
it. Now position the mouse over the same widget and you will see small squares appear. Select
one of the squares and drag it to the new ProcessingFilters widget using drag and drop. The
ProcessingFilters widget must then be connected to the additional widget so that the flow of the
product branch is closed again.
After all filters have been set up, the workflow must be saved and the WebConfigurator
restarted.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                                             98
15.2.    Filtering processings for individual processing
  articles
With the ticket [AW-235465], the possibility was created to filter processings for individual article
groups for fixed processing articles and thus to work around the master data (4.3
Artikelstammdaten – processings) logic.
This functionality must be configured via the Workflow Studio.
First, you must open the main workflow of iQuote, go into the Workflow Core, and create a
variable in the lower area (variables). The name of the variable can be selected at all, the rest
should be maintained as in the following figure.




After that, go into the workflow strand that you want to adjust. In our example, I took a
processing list for the LAMI group (170) and changed the rounded corner processing there.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                99
Now you must drag a sequence (example: Filter processings) onto the workflow (Toolbox >
Control Flow > Sequence) in the sequence the ClearCollection, and then insert the desired
processings, as seen above.
As always, it is easier to work with Copy/Paste if there is already a sequence in the workflow.
The processings in the sequence are numbered (A+W Business processing groups) and can now be
filled with a value. This value contains, comma-separated, the processing article numbers that are
now evaluated and displayed in iQuote. In our example, the rounded corner is reduced to a
processing article.
!!!CAUTION!!!: If a filter sequence is used in the workflow, only the processings are displayed in
iQuote that are present in the filter sequence. Similarly, for processings that have a value entry,
only precisely these processing articles are drawn. If the value entry is empty, all processings
maintained in the master data (4.3.6 Bearbeitungen) are drawn.
Lastly, in the ActionValidatorProcessing (this ensures that the processing view is displayed),
properties of the variable added above (in the example: ProcessingTypeFilter) are entered under
ProcessingFilters. This way, the list from the sequence is known to the view and it can be
processed.
Article groups for processings of A+W Business for the sequence:
 Description                       AWB article group                 A+W Type
 Drilling                          26                                1100
 Edgework                          31                                1000, 1005,1010,1015,1020
 Corner cut-out                    28                                1300
 Edge cut-out                      33                                1400
 Rounded corner                    34                                1310
 Corner cut-off                    35                                1305
 Inner cut-out                     30                                1415
 SN macro                          425                               1900
 Countersunk hole                  404                               1110


The edgework arrissing (awtyp = 1000),grinding (awtyp = 1005), polishing (awtyp = 1010),
beveling (awtyp = 1015), faceting (awtyp = 1020) are combined with a value.


15.3.             Projects and project prices
For selection of projects in A+W iQuote, the projects must be created in A+W Enterprise, assigned
to the customer (Master Data > Market Partner > [F4] > Project Assignment) and maintained
appropriately.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              100
The "Projects" workflow activity is in the "IQuote InOut" area of the Workflow Studio and must be
used in the CheckIn workflow.




The activity has to be added to the CheckIn workflow. The project number is stored in the
Card.Header.ObjectNo. In the configuration workflow, it is therefore possible to access the
project no. again. The parameterization is documented under 4.4 in the EN-CONFIG-A+W iQuote.
The CheckIn workflow created must still be activated for the A+W iQuote. You can do this directly
in the Workflow Studio (Configuration > Workflow management) or in the Infrastructure.Web
dialog Workflow.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                           101
If a customer has not been assigned a project in A+W Enterprise, the selection of projects does
not appear. If a customer has selected a project in A+W iQuote, then he cannot change the
project he has selected in the current configuration after the fact; instead, he must discard this
configuration.


15.4.   Stock inventory display of an article from
  several clients
With the ticket [AW-116098], a possibility was developed to display the stock inventory of an
article with respect to several clients.
Decisive for proper data in the front end is the back end stored procedure
"cu_lamgetcurrentstock." Stored in the back end under /develop/sql_scripts/cust/la ist eine
Basisvariante der Stored Procedure.
Without this stored procedure, no data is displayed in the front end.
CAUTION: Currently, no variant or color number from the A+W iQuote and the stored
procedure is transmitted.
Similarly, it must be communicated to the front end that you would like to display the new switch.
You do this in the Workflow Studio. There, you open the main workflow of the A+W iQuote that
should be changed.
Example:




There, you can enable the new stock inventory switch for each product type and product group.
For this, you must click the ValidatorProducts of the desired product branch and set the switch
"OptionShowStockOnSites" to "True."
The default is "False."




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             102
After that, the Web Configurator in the Service Locator Administrator must be restarted so that
the workflow can be reloaded.




If it is not possible to determine any data, then an empty dialog window opens.
This logic depends on the stored procedure mentioned above.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                           103
15.5.          Item reference text in shopping cart
With the development for [AW-74479] , it is now possible to display the item reference texts in
the shopping cart.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                           104
To activate the logic, in A+W Infrastructure 6 Workflow Studio, the current A+W iQuote workflow
has to be loaded with the extension point "0000 - A+W iQuote". There, you open the workflow
core area. Now you see the complete workflow and scroll down and at the end of the workflow,
there is the element "ValidatorItemRemarks", on which you click. The properties are loaded in the
right area of the Workflow Studio. There, you set the property "ShowInCart" to True.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                          105
Save change and restart the infrastructure services in the service locator, as well as the A+W
iQuote services.


15.6.           Images for A+W iQuote
15.6.1.         Product images
In A+W iQuote, standard images are drawn as default if no image was stored. These standard
images are delivered with A+W iQuote (C:\SANDPIPER1\WebWeb\Content\auw\products) and
assigned with the article type (artikel.atyp):

FLOAT_FM atyp=100  "1004.png"
ESG atyp=150  "4004.png"
VSG_FM atyp=170  "6012.png"
ISO atyp=200  "150000.png"
ZUBEHOER atyp=800  "14200.png"
RAHMEN atyp=210  "12006.png"

No assigned image causes application of "none.png".

In A+W Enterprise, the product images can be maintained on the article master data dialog
(Master Data > Articles > [Shift+F4] > Article Images).

The A+W Enterprise image path that is used for this dialog is stored in the environment variable
"ARTIKELBILD_PFAD".




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             106
For maintenance of the A+W iQuote images, the display data field must be set to the new value
"Online." When this has happened, the data field "Position in the image" is grayed out since this
data field is irrelevant for the A+W iQuote. In the data field path, the desired image must be
specified via path or searched for via the Explorer, with [F9]. It is only possible to maintain .PNG
image files.

So that the images that are maintained in A+W Enterprise are available in A+W iQuote, the
images must be copied to the desired subdirectory of the A+W iQuote. The default directory is
"\Content\auw\products\." For the customers, it makes more sense to create a new subdirectory
in which the product images are stored, for this default directory is overwritten in the update
process; the subdirectory remains. So that A+W iQuote knows the correct subdirectory for the
individual products, the workflow must be adjusted and the property "Content/Image" in the area
of the product widgets. There by default, "auw/product" is stored and can be adjusted.


15.6.2.         Images for product groups
In order to assign the respective product groups appropriate images, you have to store the required
images in the "\Content\auw\productgroups\" directory. So that the images are assigned to the
correct groups, you have to rename the image file with the short name of the article groups (Master
Data > Keys > Products > A+W iQuote-specific details > Article groups).




For example, you have a file "xyz.png" for the float group and rename this file "FLOAT.png." If you
now move this file into the "\Content\auw\productgroups\" folder, this file will now be displayed
as group image.


15.7.           Colors and variants
For the colors and/or variants, AWE master data, as well as adjustments to the A+W iQuote
workflow must be made.


A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                             107
Size variant was developed under ticket [AW-153568].


15.7.1.         Master Data
Color
The colors (hardware parts) for articles are maintained on the item master data dialog (Master
Data > Item > Phys. Properties) in that you set the toggle data field "Color/size variants" to color.




The individual colors can be set on the submenu ([F4] key in the article master data)
"Colors/sizes".

So that the selection possibilities for the colors in A+W iQuote are displayed in color, the RGB values
of the colors used must be maintained in the database table xxfarbe; otherwise the areas will be
displayed in black.

The RGB values must be maintained under "Master Data > Keys > Products > Variants > Colors >
Colors."
Dimensional variant
The variants for articles are activated on the article master data dialog (Master Data > Item >
Phys. Properties) with the "Maßvariante" flag.




For the variants, the flag "Maßvariante" must be active and for the colors, the toggle data field
"Colors/size variants" must be on colors. .Both possibilities cannot be active at the same time.
The individual variants can be set on the submenu ([F4] key in the item master data) "Variants".




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                              108
Size variant
The size variants for articles are maintained on the item master data dialog (Master Data > Item >
Phys. Properties) in that you set the toggle data field "Color/size variants" to sizes.




The individual sizes can be set on the submenu ([F4] key in the item master data) "Colors/sizes."


15.7.2.         Appearance of the selection possibilities in A+W iQuote
The selection possibilities of the colors can be designed in terms of their color with the above-
mentioned RGB values from the master data.




The dimensional variants are specified with a blue tone as default selection area.




The size variants require the maintenance of article images.
An image can be stored for all 3 variants. These images must be stored under the respective
content paths (to be set up in the respective validators in the workflow) and have as image names
the variant no. (var.bitnr) and the color no. (artfarbzu.farbnr).




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                109
To be heeded is that the numbering of the colors/sizes and dimensional variants in the AWE
database tables are frequently the same and if you activate both possibilities, two different content
paths should be set up for the different validators.


15.7.3.         Workflow
Note: Please heed when setting up the variants and colors that AutoSelect in the properties is set
to true. Otherwise it can happen that the newly selected article has an old color or variant stored.
Colors
So that product colors can be selected in A+W iQuote, the 0000 – A+W iQuote workflow used
must be adjusted. For this, in Workflow Studio, you load the workflow used and drag the Product
Colors widget (ValidatorColors) onto the loaded workflow. The widget is on the left of the
selection area.




The ValidatorColors widget offers some setting possibilities (see configuration instructions EN-
CONFIG-A+W iQuote).
New for the setting possibilities is the ColorCode; this data field expects a created variable (here:
colorCode). If this variable has not yet been created, it should look as follows:

A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                              110
The dialog for this is displayed as a tab at the bottom left on the loaded workflow.
Attaching the product colors widget after the ValidatorProduct and filling out of the properties of
the product color widget are sufficient to configure the colors for articles.
Dimensional variant
So that size variants can be selected in A+W iQuote, the 0000 – A+W iQuote workflow used must
be adjusted. For this, in Workflow Studio, you load the workflow used. The ValidatorColors are
also used for the dimensional variants. You drag the product colors widget (ValidatorColors) onto
it. The widget is on the left of the selection area.




The ValidatorColors widget offers some setting possibilities (see configuration instructions EN-
CONFIG-A+W iQuote).
New for the setting possibilities is the ColorCode; this data field expects a created variable (here:
colorCode). If this variable has not yet been created, it should look as follows:




The dialog for this is displayed as a tab at the bottom left on the loaded workflow.


A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                              111
The dimensional variants use the same widget as the colors and therefore, configuration is a bit
different.




The difference between variants and colors is the last data field (ProductNoIn). In the variants, the
product number is handed over as a negative to the documentservice so that we can distinguish
between color and variant. The Product No. of the colors/hardware is always positive.


Size variant
So that size variants can be selected in A+W iQuote, the 0000 – A+W iQuote workflow used must
be adjusted. For this, in Workflow Studio, you load the workflow used and drag the Product Size
Variants widget (ActionValidatorSizeVariants) onto the loaded workflow. The widget is on the left
of the selection area.




The Product Size Variants widget is attached in the workflow and is filled out similar to the image
above.
BOMs colors
It is now possible to activate the colors for a search on the BOM level.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             112
This possibility was created in order to combine dimensional variants with colors. (Ticket [AW-
153568]). The dimensional variants are, as described above, set up and still drawn from the
header article. That is, from the article that is visible on the A+W iQuote article selection. The
additional BOM colors, set up with the new property IsBomColor, are drawn from the first article
of the header article BOM, which has set artikel.farbflag=1.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                           113
16. Order release
All online orders (A+W Enterprise iQuote) are not released directly; instead, they are put in the
release pool.
For further information, see "EN-CONFIG-A+W Enterprise" section "Release pool".
For online entries in the call center, see "EN-CONFIG-A+W Enterprise Internal Client Separation"
section "Call center solution" and "EN-CONFIG-A+W Enterprise" section "Release pool"




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            114
17. Orders in the call center
In the default configuration, A+W iQuote orders that are entered in the CALLCENTER are assigned
directly to a client. If this should not be the case, this must be configured via a global environment
variable.
IQUOTE_CALLCENTER_STAY (client reference: no)
If this environment variable is active, online orders (entered in A+W iQuote) that are entered in
the CALLCENTER remain in the call center. There is no automatic site assignment.
(see also "EN-CONFIG-A+W Enterprise" section "Release pool")




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              115
18. Status
For the A+W iQuote orders and quotations, individual status messages are sent in the course of
running through the system.
This development was updated with DevOps item #92808.
The following table describes the status displayed in the order and quotation history.
 Processing name                   Number       Description
 Document created                      900      Document was entered successfully in A+W
                                                iQuote and transferred to A+W Enterprise.
 Document reworked in A+W              901      Document was changed in A+W iQuote.
 iQuote
 Document entered in A+W               902      Document was entered in A+W Enterprise and is
 Enterprise                                     now visible in the document overview.
 Document reworked in A+W              903      Document was changed in A+W Enterprise.
 Enterprise
 Order confirmation generated          904      Order confirmation was generated.
 In production (in processing)         910      Document was transferred to production. (No
                                                individual steps are listed)
 Delivery is underway                  940      Document was released for delivery.
 Invoice issued                        950      Invoice for the document was issued.
 Credit note created                   960      Credit note for the document was created.
 Cancellation of the document          990      The cancellation of the document was initiated.


The data is saved in the table kaufstat.
Status 910 - "In processing" is generally set for all messages from A+W Production or other
modules if for the order the general status messages are sent: from Status= 300 (fixed) to status
302 (released) and for all Status>502.
If you would like to activate the status display for all A+W Enterprise orders (also not online), you
can achieve this with the ENV configuration: IQUOTE_ALL_CUSTOM_STATUS = ON.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                            116
19. Okta Login Page
The Okta login page was developed under ticket [AW-158578], it is an upstream login page and
independent of iQuote. On it, the user logins are managed; users can register themselves. The
user is assigned an iQuote instance.
The standard login process for iQuote is thus overwritten and replaced with a one-time token and
previous system comparison check. It is not possible to use both login variants at the same time.
The login page and the iQuote have a trust relationship that is secured with a private key and
permitted IP addresses. Only if the private key is the same in both systems and the requesting IP
address is permitted in the back end do the systems trust one another. A user who has
authenticated himself on the login page is thus authenticated in iQuote with a one-time token.




For the Okta login page, it is necessary that the customer creates an account with www.okta.com
and creates user master data there, similar to how the customer does with the back end active
directory for A+W Enterprise.


19.1.          Installation
Via the A+W SetupLauncher, the A+W iQuote 6 Login Okta diskset under A+W Common and the
Microsoft .net 8.0.0 – Windows Server Hosting diskset under External Software must be
selected.
The installation should, like the A+W iQuote 6 Web (front end) be done on a Web server that is in
the DMZ (demilitarized zone).
Since Okta is not hosted locally, there must be internet access on the Web server so that there
can be communication withe the Okta account.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                               117
The remaining components (iQuote Web, iQuote Services, Infrastructure 6 Services, Infrastructure
6 Web and Documentservice) must be from QR [2403] or newer.


19.2.           Configuration
The configuration requires an Okta account, which the customer must have created in advance
and support. We will probably not have access to this account and therefore it is important that
we have a direct contact person during the setup of the system.


19.2.1.         Okta platform
Using the Terraform tool, it is possible to use a superior configuration language to bring a cloud or
the local infrastructure into the desired state for execution. Thus, we must first download the
command line tool from Terraform by HashiCorp.
Unpack the tool (terraform.exe) and place it together with the folder
(C:\SANDPIPER1\WebLoginOkta\Okta) in a secure place (e.g., "C:\Okta"). This is necessary since
after executing the tool, a state screen for the Okta configuration is created. This may not be lost,
which can happen after a diskset update.
Now we configure the okta.tf file in the new directory in order to import an update of the
configuration. WE open the okta.tf in Notepad.
Now we need information from the customer's Okta account.


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              118
The customer must generate a token that allows Terraform to make changes to the Okta tenant.
A new token is created for this in the Okta admin panel on the left menu under "Security->API".
Make sure that the token is copied directly after creation.




This token must be entered in the "okta.tf" file under the "api_token" element. For the
"org_name" and "base_url", see the Okta admin panel.




"dev-54857752.okta.com" is divided into in org_name and base_url aufgeteilt and changed
directly in the okta.tf file. Example:
provider "okta" {
    org_name = "dev-54857752"
    base_url = "okta.com"
    api_token = "<TOKEN>"
}
In addition, the URL that points to the "A+W Web Login Okta" must be adjusted with https://.
Example WEB_LOGIN_HTTPS_URL from test system aweawpvnext:
"https://aweawpvnext.tse.intra/Web.Login.Okta/"
variable "WebLoginUrl" {

A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                           119
    type = string
    default = "https://aweawpvnext.tse.intra/Web.Login.Okta/"
}


Now we open a command line (Windows + r, enter "cmd" and OK).




In the command line, you navigate to the created folder "C:\Okta" with the following command.

    cd C:\Okta



After we are in the correct folder, we use Terraform to configure Okta. This is done in the same
folder via the command line using the following commands:


    terraform init
    terraform plan
    terraform apply


According to "terraform plan" the information from the okta.tf is listed. Check this information
and then confirm with "Yes".
If the terraform has been executed successfully, you will find the application in the Okta account
under Applications > Applications.




19.2.2.              A+W iQuote Login Okta
To switch the new login page live, the "A+W iQuote Okta Login Page" of the Okta tenant must be
made known. This is done with the configuration file
"C:\SANDPIPER1\WebLoginOkta\appsettings.json". The "Okta" rubric must be configured in this
file.

A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                           120
   "Okta": {
      "OktaDomain": "https://<OKTA_TENENT_HERE>.okta.com",
      "ClientId": "<CLIENT_ID_HERE>",
      "ClientSecret": "<SECRET_HERE>",
      "AuthorizationServerId": "default",
      "UseRedirectModel": "true"
   },
For "OktaDomain", see the Okta admin panel as depicted in the figure. Important is that https://
is placed in front of the Okta domain.




For the "ClientId" and "Clientsecret", use the left menu to navigate to Application > Application
and selecting the iQuote application. Here, the values can be viewed as in the figure and entered
with the Copy button.




In the "Clients" area in the JSON file, the private key for the client in question must be stored. For
the clientID, see the A+W Infrastructure WEb. Or if the clients for the iQuote configuration should
be clarified and listed here.
  "Clients": {
    "default": {
      "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
    },
    "1": {
      "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
    },


A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                             121
      "2": {
        "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
      }
  }
The private ieys msut be stored here and in the environment variables of the A+W Enterprise of
the respective client.
Environment variable: IQUOTE_LOGIN_PRIVATEKEY
CAUTION: a private key must be compared between the login page and A+W Enterprise;
otherwise no connection can be established. Leaving this blank is not an option.


In addition to the private key, the IPv4 or IPv6 address of the login page server must be entered
here. Only queries from this computer are permitted.
Environment variable: IQUOTE_LOGIN_REMOTE_ADDRESSES (Separated with semicolon)
Caution: You must absoalutely also store the iPv6 (":::1" is the local host here).


To apply the configuration of the JSON file, the "Web.Login.Okta" page in the IIS manager must be
restarted.




19.2.3.         Preparation of iQuote for the Okta login
In the Infrastructure Web, the logout detour to the login page must be configured:




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                           122
Under the element "Log out redirect URL", the web address of the login page must be entered.
Important here is that the extension of the URL includes "/Account/SignOut".
NOTE: The "Okta" rubric point can be ignored initially since it does not contain any function.
To apply the configuration, the "Web.Web" page in the IIS manager must be restarted.




19.2.4.         Customization
As "deployment model", "A+W iQuote Login Okta" relies on the Okta redirect model. See here to
learn more about this. This means that the entire customization happens via Okta itself; see also
Style the sign-in page | Okta Developer.


19.3.           Okta data maintenance
The following data maintenance must be done by the customer, unless the customer gives you
the login for his Okta account. For the data maintenance on the Okta page, the A+W iQuote users
must be stored in the Okta account.
Tip: If you create data in the Okta interface and it is not displayed right away, you must wait a few
seconds and then refresh the window. Frequently, the display of the data is a bit delayed.



A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             123
19.3.1.        Group
Under Directory > Groups, use the "Add Group" button to create the groups.




                                                  First the group name is specified. A
                                                  description can improve the clarity of the
                                                  group later on.




                                              After saving, select the group on the list.




                                                 Under Application, the iQuote application must
                                                 be added that we imported into the
                                                 configuration via Terraform (15.2.1 Okta
                                                 Plattform).




                                              You will also be asked for additional information.
                                              Here, you enter the Web address to which the
                                              redirect should happen if the user has logged in
                                              successfully. In our example, this is the test
                                              systems of AWEAWPVNEXT with the client
                                              number 140. Finished.




A+W Software GmbH             EN-CONFIG-A+W Enterprise iQuote.docx                             124
19.3.2.         User
The users created need an A+W Enterprise employee with assignment to a market partner. The
master data maintenance is under 4.2.1 Okta Login Page.
Under Directory > People, use the "Add Person" button to create the users.




It is possible to add users compressed via .CSV file (under "More actions").
                                         A group can be assigned to the user. You can add groups
                                         to a user later on. To simplify the flow, it makes sense to
                                         create the group(s) first.
                                         The activation can be selected whether you would like to
                                         activate the customers directly or after the fact.
                                         Passwords can also be specified. This is a decision that
                                         the customer must make, whether he would like to
                                         specify passwords.
                                         If the user is saved, this user is sent an e-mail in which he
                                         is asked to verify his account and set a password if
                                         necessary.
These created users require their appropriate market partner number, which was maintained in
A+W Enterprise. For this, select the individual user under Directory > People. So that the market
partner number can be maintained, the user must be assigned to a group that owns an
application. In our example, we added a group directly when creating the user and thus see the
required application and from which group this application is drawn.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                                125
                                        With the pen button on the right side, the
                                        editing mode is opened for this user. After
                                        scrolling down, the market partner
                                        number maintained in A+W Enterprise is
                                        entered under ERPCustomerID.


                                        The SiteURL from the group is also
                                         displayed here. If no groups are used, you
                                         must store a Site Url for all users and link
                                         the users individually with the
                                         application.




A+W Software GmbH   EN-CONFIG-A+W Enterprise iQuote.docx                         126
20. Restrictions
20.1.            Input
Purchase order
PO items can only be entered without restriction violation. It is not possible to place articles in the
A+W iQuote shopping cart that have a price error, for example. If it happens that an article
violates a restriction, the Add button in A+W iQuote is switched off. This gate was incorporated in
order to make sure that no POs are entered that can be saved automatically in the system with
zero prices or similar violations.




Purchase order request
PO request items can be entered with restriction violations. These items can be added to the
shopping cart without a problem and the PO request can be entered completely. This is permitted
since these inquiries will always have to be reworked by an employee.
If an incorrect PO request is given, then the market partner assigned to the revenue
(mp.vertrerloe) is sent an e-mail.


20.2.            Processings
The restriction check for the processing parameters can be activated with
IQUOTE_WITH_PPARAM_TEST. This is also how the test for the double processed edges/corners is
activated.
For the processings stored in the A+W iQuote, it is possible to set that the restriction check is also
not displayed for non-existant values. Set-up is done using the environment variable
IQUOTE_LEERE_BEARB_MELDEN.
For more precise information, read the chapter: Master data consolidation > Article master data >
Processings.


20.3.            Glass
It must be noted that a product release of a non-fixed glass for the A+W iQuote always requires a
geometry validator. If there is no geometry validator in the workflow, then no dimensions can be
specified and thus no SN sketch will be displayed.
[AW-158039] // October 2023




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                              127
In A+W Enterprise iQuote, dimension restrictions are generally executed only on the product
level, not the BOM level. If necessary for IGU products that the dimension restrictions of the glass
be tested on the 1st level of the BOM, this can be done with an environment configuration.
IQUOTE_IGU_TESTLEVEL (client reference: no)
By default, A+W Enterprise iQuote checks the dimension restrictions only on the product level.
If the variable is activated and
= 1: For IG, the restriction check can be expanded to the 1st level (glass).


20.4.           Incorrect or locked quotations/PO requests
If a conflict in the entry of a product in A+W iQuote is determined, then this product can only be
saved as a quotation that should be examined after the fact. In A+W iQuote, you generally make a
distinction between the following types of conflicts for quotations:
    -   Restrictions (dimension or processing parameters)
    -   Price
    -   Restrictions + price

These quotations get a lock info record in the table kaufstat with corresponding status (max. of all
items)
800 – Restriction violation
801 – Pricing error
802 = 800 + 801




In addition, the items also get an expanded individual error status (kposstat):
800 – Dimension restriction violation
801 – Pricing error
802 = 800 + 801
803 = Processing parameter missing or restrictions of the Bearb.Parameter violated
804 = 800 + 803
805 = 801 + 803
806 = 800 + 801 + 803




As long as there is a lock due to an error status on a quotation, this quotation cannot be
transformed into an order via A+W iQuote. This action can only be performed directly in A+W
Enterprise.



A+W Software GmbH                  EN-CONFIG-A+W Enterprise iQuote.docx                         128
The lock status can be eliminated by the check in A+W Enterprise. The problem quotations must
be viewed and unlocked under a new menu element Sales > Quotation check > Online quotations.




There are also various possibilities for releasing the quotation.
   1. With <Sh+F5> or the "Quotation" button, you can enter the quotation in the document
        entry. Here, you can check and adjust the quotation. When saving the change, the
        question is asked whether the lock status should also be removed.
   2. If no changes must be made, then you can eliminate the lock and save the quotation
        directly via Ctrl+F in the quotation footer.
   3. The removal can be implemented directly from the overview by setting the release to yes
        and performing the action with <F3> or the "Release" button.
   The records from the tables kaufstat and kposstat with status of 800 to 807 are deleted and in
   the fields kauf._kontrollmanr and kauf._kontrolldate are assigned. The field
   kauf._kontrollmanr contains the employee number of the user and kauf._kontrolldate the
   current date.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                          129
21. Troubleshooting
Here is a list of all known problems that can occur and be eliminated during the configuration of
A+W iQuote.


21.1.           License server
21.1.1.         No connection to the license server
If the A+W iQuote is loaded without selection possibility after log-in, it could be that the problem
is a missing license for A+W iQuote or that the connection to the license server has failed.




To check whether the license server is reached, you can go to
"C:\ProgramData\Microsoft\Windows\Start Menu\Programs\A+W\Config Tools“ and start the
link "A+W LicenseClient Machine Settings Config Tool“ and test the connection. After you have
clicked the Test button and the tests were successful, a message box is displayed that confirms
the successful test. After that, press "Next" until the configuration is complete.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                             130
It can happen that the name resolution is not recognized; then the IP address of the license server
should be entered.


21.1.2.         License expired
The same scenario occurs if the A+W iQuote license has expired.




To check the license, the A+W LicenseServices Monitor must be opened on the Start menu and
the license on the desired server sought under "Application: A+W Sandpiper (2400)".




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                           131
Example of the multisite fair text environment.
Important: IIS must be restarted, otherwise the license is not obtained anew.


21.2.  Problems with                                 zero         workflows                   and
  predefined workflows
It happened increasingly that the set workflows were no longer detected correctly in the
Workflow Studio after an update of the front-end components of A+W iQuote.
In the WebConfigurator log, there is then an error message that the workflow used may not be
"zero."
If this problem occurs, then you can add the installed workflow again via the XAML file and
reinstall it. After that, the workflow should be recognized again.
Unfortunately, we do not understand what causes this error. If this error has occurred once,
please let Development know and if necessary, back up the A+W iQuote Services so that we can
research the issue.


21.3.          No images in the IG exchange BOM
It can happen that the drawings in the IG BOM are not displayed properly. The following sample
image shows the missing inner spacer.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                            132
The drawings and images on the IG exchange or muntin exchange screen depend on the master
data adjustments under 20.6.2 Produkte. It is important that the glass, spacers, gases, and
muntins that are used and are in the BOM of the insulated glass always have to be on +online in
the article master data.
Similarly, for the inner spacer a standard AIR has to be maintained since the iQuote user has no
opportunity to enter an AIR. If in the IG article "mandatory dimensions" were maintained, then a
record for the AIR has to be maintained there and a value specified. Otherwise you will see the
error image mentioned above.




21.4.   Problems during loading/opening                                                         of
  workflows in Workflow Studio
It happens again and again that the following error is displayed in Workflow Studio if you try to
load a workflow via XAML or from the database.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            133
Please set the correct reference path to the installation location of the A+W iQuote/Web
Configurator in Workflow Studio under "Configuration > Settings > Reference paths". (20.8.1 A+W
Infrastructure 6 Workflow Studio)




When entering/changing the path, confirm with the Update button; otherwise you will exit the
dialog without saving.
When checking the path, please pay attention that the desired service, here the Configurator, is
actually installed in the reference path. The Workflow Studio requires the service to open the
workflow.
A customer had split his system so that the WebConfigurator was neither installed on the process
server of the infrastructure nor on the service of the iQuote front end, but rather on a third
system. And only on the third system was it possible to open the workflow for A+W iQuote via the
Workflow Studio.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                           134
If the following error occurs, the Workflow Studio version might be too old and it must be
updated.


21.5.   No database connection on the host server of
  the A+W infrastructure
For one customer, there were connection problems from a separate A+W iQuote server in the
direction of the host server where the rest of the A+W infrastructure (here the A+W Production
Server) is installed. A database problem was reported in the logs of the Web.Configurator. There
was supposed to be no correct connection string for connection.
This problem was eliminated with installation of an A+W infrastructure web on the A+W iQuote
server. Normally for a separate installation of A+W iQuote, only an A+W infrastructure
middleware should be required; however somehow this was not sufficient.


21.6.           No dispatch of the OC possible
At one customer [AW-102433] there was a case where the entered A+W iQuote order could not
be printed. The reason for this was a missing department number for the user (kauf.abtnr). Since
the A+W iQuote creates the orders as the user system, as with intauf, that is, with employee
number -1, no department number is assigned.
So that a department number is entered nonetheless, the environment variable INTAUF_ABTNEU
must be set.


21.7.           Web Configurator does not start or timed out
The behavior can occur that the Web Configurator service crashes when starting. This behavior
can be detected in the Service Locator if the desired service is displayed for too long with the
green plus sign and goes out after that.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                           135
In the Web.ConfiguratorService log, the following exception should be found:
        An inner exception occurred:
        Type: System.Net.Sockets.SocketException
        Message: A connection attempt failed because the connected party did not properly
        respond after a period of time, or established connection failed because connected host
        has failed to respond
Similarly, you can see the failed generation attempt of the proxy creation of the Unix service, here
document service, in the log:
        Inner Exception Message: " | "
        An exception occured:
        Type: AWSOA.Core.Exceptions.CoreCommunicationException
        Message: Ice.ConnectFailedException while executing method 'DocumentService Proxy
        create'
Due to the communication from the Windows in the direction of Unix, this behavior is very
probably caused by a blocking firewall on the Unix system. As a test, you can switch off the
firewall and try to start the services. For a customer-oriented solution, the port of the
Web.Configurator must be released on the Unix system in the firewall. This will very probably be
done by the customer-internal IT.


21.8.           Duplicate key when saving a workflow
With one customer, we had the problem that the saving of a workflow via the Infrastructure.Web
caused an error.




After checking the trace file (Infrastructure.Web_xxx.awtrc), we noticed the following database
error.
2024-04-22 12:29:29.283 | [12304] | [0x00000023] | ERROR | Core                 |            |
Update workflow assignment | Workflow WebConfigurator Enterprise Groups
Extended_new.xaml / ExtensionPoint WebConfigurator | "Error Code 1000522, Message:
Duplicate key in database: ERROR [23000] [Informix][Informix ODBC Driver][Informix]Could not


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                            136
insert new row - duplicate value in a UNIQUE INDEX column (Unique
Index:ui_wfactivityassignments01). " | "
An exception occured:
Type: AWSOA.Core.Exceptions.Data.CoreDataDuplicateKeyException
Message: Duplicate key in database: ERROR [23000] [Informix][Informix ODBC
Driver][Informix]Could not insert new row - duplicate value in a UNIQUE INDEX column (Unique
Index:ui_wfactivityassignments01).
Source: mscorlib
Auto-Traced in constructor: at
AWSOA.Core.Exceptions.Data.CoreDataDuplicateKeyException..ctor(Int32, System.String,
System.Exception)
  at System.RuntimeMethodHandle.InvokeMethod(System.Object, System.Object[],
System.Signature, Boolean)
  at System.Reflection.RuntimeConstructorInfo.Invoke(System.Reflection.BindingFlags,
System.Reflection.Binder, System.Object[], System.Globalization.CultureInfo)
  at System.RuntimeType.CreateInstanceImpl(System.Reflection.BindingFlags,
System.Reflection.Binder, System.Object[], System.Globalization.CultureInfo, System.Object[],
System.Threading.StackCrawlMark ByRef)
  ...
"|""|
2024-04-22 12:29:29.285 | [12304] | [0x00000023] | ERROR | InfrastructureWorkflow       |
| Update workflow assignment | Workflow WebConfigurator Enterprise Groups
Extended_new.xaml / ExtensionPoint WebConfigurator | "Update existing Model failed with
Message:'Duplicate key in database: ERROR [23000] [Informix][Informix ODBC
Driver][Informix]Could not insert new row - duplicate value in a UNIQUE INDEX column (Unique
Index:ui_wfactivityassignments01).' " | " " | " " |

In the underlying Informix database, some GUIDs in the table Core_WFActivityAssignments
column Guid were entered in capital letters.
The GUIDs in the Informix table must be entered with lower-case letters.
The updating of the entries to lower-case letters corrected the problem.


21.9.          General performance problems
Under ticket [AW-220650], a lot of research has been done to improve the performance for
customers. The settings found were taken over into the installation instructions EN-INST-A+W
Enterprise iQuote. Please read it for the steps for system configuration.




A+W Software GmbH              EN-CONFIG-A+W Enterprise iQuote.docx                             137
22. Search/service
22.1.           Logs
You can learn about setting up the logs in the EN-CONFIG-A+W Enterprise System.


22.1.1.         Price report
The price log is always written regardless of a configuration. It is in $PROTOPFAD in the backend
(possibly under the client directory) and is called "WebPr<mmdd>". Here, all messages are logged
that are normally output in the foreground and cause a "price error" in iQuote.


22.2.           General
You can find a listing of all ICE services in the "Service Locator Administration" Tool, which is in the
Config Tools folder of the Desktop A+W folder (C:\ProgramData\Microsoft\Windows\Start
Menu\Programs\A+W\Config Tools). Here you can see in compact form how all services run
together.
If you open the tool, you can see the set connections with a click on the button with the green
arrow in the upper left corner.




Establish the connection, and after that, you will see the following list:




A+W Software GmbH                EN-CONFIG-A+W Enterprise iQuote.docx                               138
I will use this list as an example.

First we see the following:                       This point is called a node and has the
notation <computer name-service area> = Multiside-fair is the computer and CAD, the service
area, where particular CAD services can be found.                               For the AWE
Backend, we see that a Unix computer is entered with VMAUWX.
In Windows, a node reflects precisely one Windows service (marked in yellow):




On Unix or in the Backend, the running icegridnode is next to the node:

A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                        139
If a Windows service or the icegridnode should be deactivated, then the little hard disk in the
service locator administration turns red:




The actual services are below the nodes. If these services are switched on, they have a little green
triangle.
Notation: <computer name-service area-service name-client>


22.3.           Which services are affected for A+W iQuote?
The relevant services for the A+W iQuote are the following:
CAD-Geometry (included in A+W CAD Services):
Service provides the shape catalog, which is loaded once at when A+W iQuote is started.
Log in default Windows log directory: C:\ProgramData\A+W\Log
Ex. CAD.GeometryService_2021-10-11.38616.0.awtrc


Commercial converter
Service communicates with the documentservice (Backend) and provides the communication to
Windows services or takes over the tasks that are not possible via the Backend. Activating CAD
service, AWDesign or the fetching and provision of reports/attachments.
Log in default Windows log directory: C:\ProgramData\A+W\Log
Ex. Commercial.ConverterService_2021-09-28.13000.0.awtrc


Web configurator
Service is the main interface between Web browser and the Backend (documentservice). All
communication calls run via the Web configurator.


A+W Software GmbH               EN-CONFIG-A+W Enterprise iQuote.docx                              140
Log in default Windows log directory: C:\ProgramData\A+W\Log
Ex. Web.ConfiguratorService_2021-10-11.39272.0.awtrc


Commercial document
The service (documentservice) takes over all tasks as "A+W Enterprise clone". Each call from the
Web lands with the documentservice later on.
Log is in Unix in the log directory (gp)
Ex. awsoa_documentservice_54138_1011
In addition to the above-mentioned log, the documentservice also writes ftests if a calculation has
been run through.
Test is on Unix in the ftest directory (gft)
Ex. documentservice_54138.test


22.4.            Export of the Memrels sketches
With the DevOps item #101907 a possibility was created to export the Memrels sketches to
$REPTMP. Some information from the Memrels is written to data objects and transferred to the
ConverterService for sketch generation.
We have a crash with the call of the ConverterService at a customer's.
Following message content:
Iceutilexeption: /usr/include/IceUtil/handle.h
iceUtil:NullHandleException
The crash is probably caused by corrupt data in the data object to be transferred; that's why the
hope is that the information from the Memrels will give us something with regard to the cause of
the crash.
The export overwrites the existing files after each sketch generation.
The environment variable IQUOTE_SKETCH_MEMREL_EXPORT must be set to ON.
The exported Memrels are written to REPTMP. The environment variable REPTMP must therefore
be maintained accordingly.
Export file name: MEX_Maskenname.UserId Example MEX_KPOS.-1




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iQuote.docx                         141

