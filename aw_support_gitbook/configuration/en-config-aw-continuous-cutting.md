---
title: "EN CONFIG A+W Continuous Cutting"
category: "configuration"
product: "A+W Continuous Cutting"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Continuous Cutting"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration   A+W Continuous Cutting Multi-step Automated Production System                                                                    english                     - INTERNAL -    A+W Software GmbH   EN-CONFIG-A+W Continuous Cutting.docx   1 Change history           Date        Author         Remarks                       Version         2021-07-12 Anna Bremkamp Draft                           1.0     A+W Software GmbH        EN-CONFIG-A+W Continuous Cutting.docx             2"
source_file: "EN-CONFIG-A+W Continuous Cutting.pdf"
---


# EN CONFIG A+W Continuous Cutting

         Configuration


A+W Continuous Cutting
Multi-step Automated Production System




                                                               english




                - INTERNAL -
   A+W Software GmbH   EN-CONFIG-A+W Continuous Cutting.docx   1
Change history


        Date        Author         Remarks                       Version
        2021-07-12 Anna Bremkamp Draft                           1.0




A+W Software GmbH        EN-CONFIG-A+W Continuous Cutting.docx             2
Content

1.   General information                                              4
2.   A+W Realtime Optimizer configuration                             5
3.   Configuration of A+W Continuous Cutting                          6
     3.1. Specifying standard values                                  6
     3.2. Add a filter.                                               7
4.   Use                                                              9
     4.1. Planning cutting                                            9
     4.2. Cutting                                                    10




A+W Software GmbH            EN-CONFIG-A+W Continuous Cutting.docx        3
1. General information
The following documentation shows the steps for configuration of the A+W Realtime Optimizer -
Continuous Cutting module.
The A+W Realtime Optimizer - Continuous Cutting module is a component of the A+W Realtime
Optimizer and is currently available as a prototype.
Please make sure that you have downloaded the latest installation of the A+W Realtime Optimizer
with all current hotfixes and that the database is up-to-date.




A+W Software GmbH            EN-CONFIG-A+W Continuous Cutting.docx                              4
2. A+W Realtime Optimizer configuration
Important - Make a backup of the current entries so they can be restored if needed - either by
making a duplicate copy of the XOPTON.CFG (Example - $XOPTON.CFG) file or saving the original
entry in the XOPTON.CFG.
Open the XOPTON.CFG file in the path:
%appdata%\A+W\Techsoft\Xopton


Find the section [ContinuousCutting] as shown below and make the following changes.
If the section does not exist yet, insert it.




   •   ContinuousCuttingMode: <INTEGER> [0,1,2,3] default setting = 0
Defines the mode for Continuous Cutting. The database table RTO_INTERFACE has to be present.
       0 = Standard cutting process with batch selection dialog is used.
       No Continuous Cutting available.
       1 = the dialog for overview of already-planned batches and the dialog for preparation of
       batches for Continuous Cutting is displayed (Office RTO).
       Continuous Cutting for production is not available"
       2 = No dialog for overview and preparation of batches for Continuous Cutting is displayed
       (Shopfloor-RTO).
       Only Continuous Cutting for production is available.
       3 = The dialogs for the overview and for preparation of batches for the Continuous Cutting
       are displayed. Continuous Cutting for production is also available.
   •   ParameterStation: <STRING> default setting: AUW_CONTINUOUS_CUTTING
       Station name for loading user-specific configuration of the .NET Continuous Cutting




A+W Software GmbH             EN-CONFIG-A+W Continuous Cutting.docx                               5
3. Configuration of A+W Continuous Cutting
For the planning view, standard values can be specified in the parameter administrator and filters
created. In the A+W Realtime Optimizer, open the "Continuous Cutting" menu element:




After the new dialog has loaded successfully, press CTRL+F9. After entry of the password, the
parameter administrator opens.


3.1. Specifying standard values
Enter the standard values you wish to enter here.




A+W Software GmbH              EN-CONFIG-A+W Continuous Cutting.docx                             6
3.2. Add a filter.
To add a new filter, please proceed as follows: click the button in the Parameterizable SQL Filter
field.




An overview of all existing filters opens. Now you can insert a new filter or edit an existing filter.




A+W Software GmbH               EN-CONFIG-A+W Continuous Cutting.docx                                    7
Give the filter a meaningful name and make sure the syntax of the filter is correct. You can define
a permanent filter, e.g. pool_teile.glasart = 1004 or a filter with one or two placeholders, e.g.
pool_teile.glasart = [TTV1NUM]. For filters with placeholders, the user enters the desired value
himself later on.




A+W Software GmbH              EN-CONFIG-A+W Continuous Cutting.docx                              8
4. Use
4.1. Planning cutting
Open the A+W Realtime Optimizer with the blue A+W Desktop shortcut.
Under A+W Realtime Optimizer click on Cutting > Continuous cutting from the top menu




This opens the overview with all cutting planned with A+W Continuous Cutting.
Click the "Planning" button at the bottom right.




A+W Software GmbH             EN-CONFIG-A+W Continuous Cutting.docx                    9
Now you are in the planning view and you can plan the cutting.




4.2. Cutting
Open the A+W Realtime Optimizer with the blue A+W Desktop shortcut.
Under A+W Realtime Optimizer click on Settings > Cutting from the top menu.




Now select Automatic and confirm your selection with OK.




A+W Software GmbH             EN-CONFIG-A+W Continuous Cutting.docx           10
Now open the cutting by clicking the Cutting button on the menu.




Now you see an overview of the planned cutting.




If you click the Options button, you can reset the status of the batches if necessary.
Click the Start button to start the cutting. The optimizations of the first group are transferred to
cutting.




A+W Software GmbH               EN-CONFIG-A+W Continuous Cutting.docx                              11
If the last pattern of the group has been sent to the cutting table and cut, the next group will be
loaded into cutting automatically.




A+W Software GmbH              EN-CONFIG-A+W Continuous Cutting.docx                                  12

