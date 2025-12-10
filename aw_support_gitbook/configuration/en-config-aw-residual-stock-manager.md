---
title: "EN CONFIG A+W Residual Stock Manager"
category: "configuration"
product: "A+W Residual Stock Manager"
doc_type: "Configuration"
language: "EN"
tags: ["CONFIG", "A+W Residual Stock Manager"]
version: "1.0"
last_updated: "2025-12-10"
description: "Configuration   A+W Residual Stock Manager                                                                          english        A+W Software GmbH                                         - -INTERNAL-                        EN-CONFIG-A+W Residual Stock Manager.docx     1 Content    1.   Requirement                                                         3 2.   Planning Web                                                        4      2.1. Rack types"
source_file: "EN-CONFIG-A+W Residual Stock Manager.pdf"
---


# EN CONFIG A+W Residual Stock Manager

         Configuration


A+W Residual Stock Manager




                                                                     english




   A+W Software GmbH                                         - -INTERNAL-
                       EN-CONFIG-A+W Residual Stock Manager.docx     1
Content



1.   Requirement                                                         3
2.   Planning Web                                                        4
     2.1. Rack types                                                     4
     2.2. Stock incl. rack                                               5
     2.3. Stock Label Printing                                           9
                 ODBC configuration                                      9
                 Printer configuration on the infrastructure web        10
3.   Realtime Optimizer                                                 12
     3.1. Xopton.cfg                                                    12
     3.2. Settings directly in the program                              13
4.   Configuration of the infrastructure web                            14
5.   Optimization kernel: Xopt.cfg                                      18




A+W Software GmbH           EN-CONFIG-A+W Residual Stock Manager.docx        2
1. Requirement
The installation was executed successfully according to the INST-A+W Planning Stock installation
instructions.




A+W Software GmbH          EN-CONFIG-A+W Residual Stock Manager.docx                          3
2. Planning Web
2.1. Rack types
For configuration of the rack types, you must take the following steps:
    •    Open the A+W Planning Web, for example via the A+W folder on the desktop. Normally this
         page is hosted under http://[processserver]/Planning.Web. Then the browser opens with
         the start page of the A+W Planning Web. (see Abbildung 2-1)
    •    Press the Stock button.




Figure 2-1 Start view of the A+W Planning Web

    •    Then click the Master data menu and there, the [Rack properties] button.




Figure 2-2 Master data of the A+W Planning Web

    •    New rack types can be created and configured here. For this, either change values of an
         existing rack type directly or create a new rack type with the [+ Add] button. The following
         fields must be configured:




A+W Software GmbH                EN-CONFIG-A+W Residual Stock Manager.docx                         4
Figure 2-3 Sample configuration of rack types

              o    Description: unique name for identification of a rack type
              o    Access type: describes how glass can be stacked up or down. Available options:
                            Free: random access to the glass (e.g. harp racks)
                            First in, First out (FiFo): only the first glass stored can be removed (e.g.
                             through passage)
                            Last in, First out (LiFo): only the last glass stored can be removed (e.g. A-
                             rack)
              o    Maximum weight: maximum weight in kg
              o    Maximum height: maximum height of the glass that can be placed on this rack type.
              o    Maximum width: maximum width of the glass that can be placed on this rack type.
                   In the case of several stacks, this value describes the maximum width of all stacks
                   together.
              o    Maximum depth: maximum depth of the rack. With a glass stack, all thicknesses of
                   the glass in a stack are added together. For harp racks, the maximum depth is set
                   equal to the width of a single slot.
              o    Minimum height: minimum height of the glass that may be placed on this rack type.
              o    Minimum width: minimum width of the glass that may be placed on this rack type.
              o    Maximum number of stacks/slots: maximum permissible number of stacks on this
                   rack type. For a harp rack, this is the number of slots. If the value -1 is set, the
                   number is unlimited; then only the other values such as maximum height, width or
                   depth are consulted for restrictions.
              o    Segment type: the type of this rack type. Available options:
                                     HarpRack: Harp racks
                            LRack: L-rack
                   For configuration of an A-rack, two L-racks must be created.


2.2. Stock incl. rack
After the rack types were created as described under 2.1, the Stock, Stock areas, and Rack can be
configured in the Master data. The following steps are required for this:
    •    Call of the configuration page of the stock starting from the start page via Stock > Master
         data.




A+W Software GmbH                 EN-CONFIG-A+W Residual Stock Manager.docx                             5
    •    Change of the values of already existing stock or addition of a new stock via the [+ Add]
         button. The following fields must be configured:




Figure 2-4 Sample configuration of a stock

              o    ID: unique numeric key; if a new stock is created, the next ID not yet assigned will
                   be suggested. Any previous IDs that have been freed up through the deletion of a
                   stock will not be taken into account and therefore not suggested. It is possible to
                   select the ID manually. If the ID already exists, a corresponding message will point
                   this out and prevent saving.
              o    Description: a unique name of the stock area
    •    If a new stock was created, [Save] must be pressed so that the changes are taken over.
    •    Open the settings for the storage location of this stock with a click on [Edit].




Figure 2-5 Sample configuration of the storage locations for a stock

    •    Either     change    values     of     existing    storage     locations     directly
         or add a new storage location with the [+ Add] button. The following fields must be
         configured:
              o    ID: Unique numeric code, this code must be unique across all stocks. If a new
                   storage location is created, the next ID not yet assigned will be suggested. Any
                   previous IDs that have been freed up through the deletion of a storage location will
                   not be taken into account and therefore not suggested. It is possible to select the
                   ID manually. If the ID already exists, a corresponding message will point this out
                   and prevent saving.
              o    Description: A unique name of the storage location
              o    Stock types (see Abbildung 2-6 Auswahl der Lagertypen):
                            Storage location: simple stock
                            Stock receipt: a receipt/removal for the other stock
                   For each table with the corresponding table ID, a stock and a storage location with
                   the type Stock receipt should be created so that new residual plates can be created
                   manually and can be stored in other stock locations.


A+W Software GmbH                  EN-CONFIG-A+W Residual Stock Manager.docx                         6
                    The other stock types are conceived for a sortjet and are not used in the RSM.
                      Loading              Location within a buffer system. (Filling via a shuttle from a
                                           loading station, a shuttle or an in-out station).
                      Buffer               Location that can be loaded and unloaded.
                      Loading station      Temporary station if lites are transported from one
                                           location to another.
                      Shuttle              Warehouse receipt for residual lite stock.




Figure 2-6 Selection of the stock types

               o    Allocation status: here you can set whether the storage location can be used with
                    racks or is locked. A manual lock would make sense, for example, if the area is
                    blocked due to a goods delivery. Here, storage locations that were locked by the
                    system can be re-enabled.
     •    Save change with a click on [Save] so that the changes are taken over.
     •    If for the respective storage locations you click [Edit], the allocated rack one level below
          opens. Lites can only be booked on racks, therefore it is advisable to configure at least one
          rack for each storage location.
     •    With the [+ Add] button, you can create a new rack. The following fields must be configured:
               o    ID: unique numeric code, this code must be unique across all racks. If a new rack is
                    created, the next ID not yet assigned will be suggested. Any previous IDs that have
                    been freed up through the deletion of a rack will not be taken into account and
                    therefore not suggested. It is possible to select the ID manually. If the ID already
                    exists, a corresponding message will point this out and prevent saving.




A+W Software GmbH                   EN-CONFIG-A+W Residual Stock Manager.docx                               7
Figure 2-7 Sample configuration of a rack of a storage location

              o    Description: a unique name of the rack
              o    Allocation status: here you can set whether the rack can be used for lites or if it is
                   locked. A manual lock would make sense, for example, if the area is blocked due to
                   a goods delivery. Here, racks that were locked by the system can be re-enabled.
              o    Properties: the rack type can be selected from among all the previously created
                   rack types. How rack types are created is described in 2.1.




A+W Software GmbH                  EN-CONFIG-A+W Residual Stock Manager.docx                           8
2.3. Stock Label Printing
           ODBC configuration
For each database that is used, an ODBC connection must be configured. In this example, we are
using separate databases. An ALCIM database and an AWSOA database.




Figure 2-8 ODBC configuration

In both configurations of the system DSN, the Windows Authentication should be selected.




Figure 2-9 ODBC user authentication

In the end, the data source test should be successful.


A+W Software GmbH                EN-CONFIG-A+W Residual Stock Manager.docx                       9
Figure 2-10 ODBC data source test


           Printer configuration on the infrastructure web
On the Infrastructure web (url:servername/Infrastructure.Web), under Configuration - A+W
Production - Stock Label Print, the following parameters have to be configured.
 StockID                                              This stock ID is the ID of the respective
                                                      storage
 Printer                                              Printer that is used for the label printing
 Report Name                                          Is the absolute path in which the report is
                                                      located
 Station Group                                        The "Station Group" field refers to the groups
                                                      defined in the A+W Production -> Parameter
                                                      Administrator -> Approval dialog




A+W Software GmbH                   EN-CONFIG-A+W Residual Stock Manager.docx                       10
Figure 2-11 Stock label printing configuration

The printer has to be configured in the system's printer settings if it is not already configured.
Generally, the default printer is used.
Under Planning/Web - Stock - Overview, you can initiate the label printing by selecting print in
addition to an article.
Note: Please note that the user under whom the process manager is running, has to be
configured within the DB configuration in order to have access to the specific database.




A+W Software GmbH                  EN-CONFIG-A+W Residual Stock Manager.docx                         11
3. Realtime Optimizer
3.1. Xopton.cfg
So that the A+W Residual Stock Manager and A+W Realtime Optimizer can communicate with one
another, the configuration file of the A+W Realtime Optimizer, xopton.cfg, must be adjusted. This
file is under
                               %appdata%\A+W\TECHSOFT\Xopton
Basically, for this file:
     •    all lines that start with a semicolon are commented out and will not be considered. It can
          be necessary to remove semicolons in order to activate the configuration.
     •    Between parameters, assignment operator = and the value assigned, there may be no
          empty spaces. That is:
          False: Table = TB1                                               True: Table=TB1
     •    At the end of the document, there is a description of all parameters and their assignment
          possibilities.
In the Remaster section, the following parameters must be set:

; ............. Section for Hegla Remaster ..................................
[Remaster]
Remaster=Y
NumberOfRemasters=1
Remaster1=Table name, Computer name
RemasterMode=6
MinRemasterLength=1000

The table must be entered in the Table name field that should work with the stock in question in
the A+W Residual Stock Manager. The possible tables are in the xopton.cfg under

; ............. Section for cutting .........................................[Cutting]
Table=Tischname

also configured in the xopton.cfg. The StockID is the ID of the stock that the table can access. For
the ID, consult the A+W Planning Web. It is possible to configure several manual residual stocks,
then the parameter NumberOfRemasters must be adjusted accordingly and a new line with
RemasterX=Tischname,LagerID inserted for each residual stock.




A+W Software GmbH                     EN-CONFIG-A+W Residual Stock Manager.docx                  12
3.2. Settings directly in the program
In addition to the xopton.cfg, the use of a residual stock must also be activated in the A+W Realtime
Optimizer. For this, the following steps are required after the start of the A+W Realtime Optimizer:
    •   Click the Settings > Tables menu element, this will open the Settings window
    •   Place a checkmark in the 3 boxes in the Residual plate stock section. Here it is also possible
        to define the minimum storage length and decide whether residual plates should only be
        placed in or used from the stock. The settings here override the configuration in the
        xopton.cfg file.




         Figure 3-1 Activation of the residual plate stock in the A+W Realtime Optimizer




A+W Software GmbH               EN-CONFIG-A+W Residual Stock Manager.docx                          13
4. Configuration of the infrastructure web
In order to print labels for residual quantities, the following adjustment must be made in the
configuration of the infrastructure web under Stock label Print.




In the Stock Id field, enter the stock number that should be printed. You can configure one printer
per created stock. In the Printer field, specify the printer on which the labels should be printed and
in the Report Name field, the name of the report. Printer and Report Name must be specified as
absolute paths.
The Station Group field refers to the groups defined in A+W Production (A+W Production >
Parameter Administrator>Release dialog, Group of executing computers area):




A+W Software GmbH            EN-CONFIG-A+W Residual Stock Manager.docx                             14
The job service writes this entry to the process table.
Example: If the ProcessManager that is entered in Group 1 should print the report, then in the
Web interface, 1 should be entered in the Station Group field. Group 0 is reserved for the release
dialog.




A+W Software GmbH           EN-CONFIG-A+W Residual Stock Manager.docx                          15
The Stock Connection Settings and Table to Stock Assignment areas contain parameters for the
Stock Service, so that it can communicate with an external stock, e.g. the Hegla ReMaster.
Stock Connection Settings
In this area, you make the settings for the stock connection.




In the Stock Id field, enter the stock ID to be incorporated, and in the IP Address field the
appropriate Hegla (stock) IP address. In the Port field, the port number to be used must be
entered and in the Stock Interface Version field the interface or interface version that is used.
To add a new stock connection, click the + and fill out the fields described above accordingly.




A+W Software GmbH            EN-CONFIG-A+W Residual Stock Manager.docx                              16
Table to Stock Assignment
In this area, you can assign cutting tables to individual stocks.




In the Table Id field, enter the appropriate table number and in the Stok Id field, the appropriate
stock number. The combo box in the Stock Type field contains the entries External and Internal.
Here, the Stock ID corresponds to an internal storage of the warehouse ID in the planning web
(RSM). The Stock ID of an external stock corresponds to the ID in the Stock Connection Settings
(e.g. Hegla, ReMaster, other manufacturers are also possible).
With a click on X, the corresponding entry is removed.
After the settings were made, you should ensure here that the Stock Service is restarted. This is
necessary since otherwise the service will not connect to the ReMaster.




A+W Software GmbH             EN-CONFIG-A+W Residual Stock Manager.docx                             17
5. Optimization kernel: Xopt.cfg
In addition to the configuration in the xopton.cfg, various parameters for the optimization kernel
can be overridden. Usually this is not necessary, but it can be appropriate for test scenarios or
another fine-tuning. The parameters listed here should only be activated if the person activating
them is aware of the changes they will cause. In the worst case, the use of residual plates can be
deactivated c9ompletely or the use of an excessive number of residual plates can slow down the
production flow.
Since the parameters in the xopt.cfg file override parameters from the file opt2par.dat, a check of
these entries in advance makes sense. The opt2par.dat file can be opened with the A+W Tool
DebNET.exe. For this, just copy the program
                \\jupiter\TECHSOFT_Glasbaum\XOPT\TOOLS\DEBUG\DebNET.exe
into the directory with the individual opt2 files (for example, in the directory for table optimization
listed below) and open it with a double-click. Editing of the opt2 files is not possible.
The xopt.cfg master file is under
                                           P:\Release\Save
This xopt.cfg file is copied for each table optimization into the directory
                           %appdata%\A+W\TECHSOFT\Xopton\TOPT01
the individual opt2 files can also be copied here for each table optimization. If the master file is
changed, this change takes effect with the next optimization. No restart of the A+W Realtime
Optimizer is required. The following parameters influence the use of the residual plates from the
A+W Residual Stock Manager and replace individual parameters from the opt2par.dat file:
    •   ForceStockplateSequence
        This parameter can be used to override the StockInSequence entry in the opt2par.dat and
        controls the processing of the stock dimension.
            o   =0       (Default) All entries for stock plates are treated the same. There is no
                special logic for residual plates. Control via prices is possible now as before.
                Caution: if everything is configured for the A+W Residual Stock Manager, then the
                access sequence (>=1) is entered in the price field for the residual plates. Since in
                this case, the dimensions have a 0 in the price field, no residual plates will be used
                since they have a higher price.
            o   "1"= All stock plates are processed strictly in the order of their entries. The field
                PRICE in the opt2par.dat, record 3 (see Abbildung 5-2) is used as sort index in
                ascending order. If no prices are specified, then procedure is automatically as in
                the case = 0. If prices exist, the least expensive stockplate is necessarily processed
                first. The next stockplate in the sequence is only begun once all plates of the
                previous stage are completely used up. If there are two residual plates with
                sequence 1 and a residual plate with sequence 2, then first both residual plates
                with sequence 1 must be used before the residual plate with sequence 2 can be
                used. This ensures that residual plates used are also accessible. The sequence is
                visible on the table optimization dialog (Abbildung 2-1) or it can be checked with
                the A+W tool Deb.NET in the opt2par.dat file (Abbildung 5-2).




A+W Software GmbH            EN-CONFIG-A+W Residual Stock Manager.docx                              18
Figure 5-1 Sequence of the residual plates on the table optimization dialog

              o    =2      This is the default setting for use of the A+W Residual Stock Manager. The
                   stockplates and residuals are categorized using the entries in the RESTLAGER field
                   in the opt2par.dat, record 3 (see Abbildung 5-3). Here, the entry 0 means that this
                   is a normal stockplate; 1 that this is a residual plate from an automatic stock, and
                   2 that the residual plate is stored in a manual stock. Depending on the entry, the
                   residual plates are planned as follows:
                   Residual plates from an automatic stock are preferred if they can be occupied (a
                   plate may be too small for the current order dimensions). If these residual plates
                   have been processed or cannot be processed, normal stockplates and manual
                   residual plates are checked and used depending on the achievable yield. A manual
                   residual plate is therefore only used if a better yield is achieved as a result (which
                   will automatically be the case, for example, with small order quantities). In the case
                   of manual residual plates, additional attention is paid to whether they may stand
                   on a stack and can only be used in a certain sequence.
              o    =3        Precisely as with ForceStockplateSequence=2 with the following deviation:




                        Figure 5-2 Sequence of the residual plates in the opt2par.dat

                   The residual plates from the automatic stock are not preferred, but rather only
                   used according to the yield.




A+W Software GmbH                  EN-CONFIG-A+W Residual Stock Manager.docx                          19
Figure 5-3 Categorization of the stockplates in the opt2par.dat with 0 = normal stockplate, 1 = residual plate from an
automatic stock, 2 = residual plate from a manual stock

    •    ConsumeResidualsFirst=1
         If this parameter is set, all residual plates are used before the stockplates, regardless of the
         yield or whether the stock is manual or automatic. This happens until either all residual
         plates are used up or a residual plate to be processed manually cannot be used. A manual
         residual plate cannot be used if it is not in the first position on an A-rack stack or if it is too
         small for the lites to be cut. As soon as the optimization kernel encounters a residual plate
         that is not accessible, only stockplates are used. In this case, starting at this time, all residual
         plates are ignored for the rest of the current optimization batch (background: the other
         residual plates are then not accessible).
    •    IgnorePricemarkeForResiduals=1
         If this parameter is set, residual plates are only used if the yield increases with their use.
         Thus, residual plates are not preferred and it can happen that the residual plate stock is
         overloaded or completely loaded.
    •    InvertMIMResidueSetting=1
         If residual plates are used for a table optimization, all available residual plates are locked
         until the optimization is either saved or cut. Only then will the residual plates not used be
         released for a new optimization. This prevents double use.
         With the parameter InvertMIMResidueSetting, parameters set by the A+W Realtime
         Optimizer witnin the opt2par file so that the save files can be used for additional tests
         directly with the optimization kernel. Therefore, setting this parameter makes sense if the
         A+W Realtime Optimizer should use save files modified by a table optimization for tests
         with the optimization kernel. This parameter may not be set in live operation!




A+W Software GmbH                 EN-CONFIG-A+W Residual Stock Manager.docx                                        20

