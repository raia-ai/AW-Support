---
description: "EN AWProduction Realtime Optimizer 3.30"
---



# EN AWProduction Realtime Optimizer 3.30

A+W Realtime Optimizer      J




                            english




                A+W Production
                                                                                                               Introduction




                                          Introduction
                                          This part of the documentation contains editorial notes.


                                          Revision Overview
                                          Part
                                          Version / Date

                                          3.30 / 01-2023            New fields added

                                          3.20 / 10-2020            New fields added

                                          3.02 / 09-2018            New fields added

                                          3.01 / 01-2017            Product and company names adjusted

                                          3.00 / 03-2015            Complete revision

                                          2.01 / 07-2013            Layout adjusted to document concept 2013

                                          2.00 / 09-2007            Complete revision

                                          1.00 / 03-2003            Initial creation



                                          Editorial
                                          The editorial contains information about the following topics:
                                          •   Notes on this document
                                          •   Copyrights
                                          •   Trademarks
                                          •   Contact

                                          Notes on this document
                                          This publication is conceived exclusively for end users of A+W Realtime Opti-
                                          mizer.
                                          This documentation and the software it describes is only distributed with a li-
                                          cense and may only be used and copied according to this license. The content
                                          of the documentation serves only as information and can be changed without
                                          prior notice at any time. The greatest care was used in compiling the texts and
                                          figures. However it is not possible to exclude errors completely. A+W Software
                                          GmbH assumes no liability for errors or imprecise statements unless these
                                          can be traced back to intentional or negligent actions.
                                          This document describes the complete stage of expansion of A+W Realtime
                                          Optimizer.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-3
                 Introduction




                                Copyrights
                                 2023, A+W Software GmbH, all rights reserved, also those for reprinting, the
                                making of copies and translation.
                                The documentation may only be copied whole or in part, stored in an archiving
                                system or transmitted in any other form in accordance with the license agree-
                                ment. Without the prior written permission of A+W Software GmbH, the docu-
                                mentation may not be transmitted electronically, by recording or in any other
                                form.

                                Trademarks
                                All hardware and software designations mentioned in the documentation can
                                also be registered trademarks or other industrial property rights of third parties.
                                The property rights of third parties must be observed.

                                Contact
                                A+W Software GmbH
                                Am Pfahlgraben 4 - 10
                                D-35415 Pohlheim
                                Germany
                                    +49 6404 2051 0
                                    +49 6404 2051 877
                                Zentrale@a-w.com
                                http://www.a-w.com
3.30 / 01-2023




                 J-4                                                                   A+W Realtime Optimizer
                                                                                                                                                           Contents




                                          Contents
                                          Introduction ............................................................................................................. J-3
                                            Revision Overview ............................................................................................... J-3
                                            Editorial ............................................................................................................... J-3
                                          Contents ................................................................................................................. J-5

                                          Tutorial                                                                                                                J-7
                                          Basic Ideas ............................................................................................................. J-9
                                            Features ............................................................................................................ J-10
                                          Using A+W Realtime Optimizer ............................................................................ J-11
                                            Overview ........................................................................................................... J-12
                                            Import of Data .................................................................................................... J-13
                                               Working with A+W Production ....................................................................... J-15
                                                 Master data ................................................................................................. J-15
                                               Use as a stand-alone system ......................................................................... J-16
                                                 Import optimizations ................................................................................... J-16
                                          Input ...................................................................................................................... J-18
                                            Overview ........................................................................................................... J-19
                                               Rejects, Rush Order Lites or Filler Orders ..................................................... J-20
                                                 Manual entry of lites ................................................................................... J-21
                                               Manual Creation of Plans ............................................................................... J-24
                                               Charge Editor ................................................................................................. J-25
                                          Optimization .......................................................................................................... J-26
                                            Overview ........................................................................................................... J-27
                                            Cutting Table Optimizations .............................................................................. J-28
                                               Create Table Optimizations ........................................................................... J-28
                                               Check and Process Table Optimization Result .............................................. J-30
                                               Resolve Table Optimization ........................................................................... J-32
                                               Linking of Table Optimizations ....................................................................... J-33
                                            Create a Quick Optimization ............................................................................. J-34
                                            Linking of Batches ............................................................................................. J-35
                                            Cutting Table Control ........................................................................................ J-36
                                          Cutting .................................................................................................................. J-37
                                            Overview ........................................................................................................... J-38
                                               Selecting Batches for Cutting ......................................................................... J-39
                                               Check Optimization and Cut .......................................................................... J-41
                                               Interrupt and Continue Work .......................................................................... J-43
                                               Cutting Overview ............................................................................................ J-44
                                            Reset Cutting Status ......................................................................................... J-46
                                          Interplay with Other Modules ................................................................................ J-47
                                            Overview ........................................................................................................... J-48
                                               Residue Dispenser ......................................................................................... J-48
                                                 Use Stored Residue Plates ........................................................................ J-48
                                               A+W Production Terminal (XTV) .................................................................... J-49
                                               A+W PlanEditor ............................................................................................. J-49
                                               A+W Defect Optimizer ................................................................................... J-50
                                               A+W DynOpt Compact .................................................................................. J-51
                                                 A+W DynOpt Compact Import .................................................................... J-51
                                                 A+W DynOpt Compact Optimization .......................................................... J-51
                                                 Create A+W DynOpt Compact Batch ......................................................... J-52
3.30 / 01-2023




                                          Software Reference                                                                                                   J-55
                                          Overview ............................................................................................................... J-57
                                           Menus ................................................................................................................ J-57



                 A+W Realtime Optimizer                                                                                                                             J-5
                 Contents




                              Icons .................................................................................................................. J-57
                            Input ...................................................................................................................... J-58
                              Rush Orders ...................................................................................................... J-58
                              Input of Rush Order Lites .................................................................................. J-60
                              Input of Shapes ................................................................................................. J-62
                              Shape Number .................................................................................................. J-63
                              Manual Plan Input ............................................................................................. J-64
                              Charge Editor .................................................................................................... J-67
                            Optimization .......................................................................................................... J-68
                              Select Glass for Optimization ............................................................................ J-68
                                 Table Optimization in the Default Variant ...................................................... J-68
                                 Table Optimization in the Production Date Variant ........................................ J-71
                              Table Optimization Batch [No.] .......................................................................... J-72
                                 Overview ........................................................................................................ J-72
                              Optimize ............................................................................................................ J-74
                                   Description of fields in section Optimization Sequence .............................. J-74
                                   Description of buttons in section Sequence ............................................... J-75
                                   Description of fields in section Automatic Compilation ............................... J-75
                                   Description of fields in section Batch Parameters ...................................... J-75
                                   Description of fields in section Table .......................................................... J-76
                                   Description of fields in section Optimization Parameters ........................... J-76
                              Residue Plates and Stockplates ........................................................................ J-77
                              Parameter .......................................................................................................... J-79
                              Number of Stockplates ...................................................................................... J-81
                              Resetting a Cutting Batch .................................................................................. J-81
                              Pausing Glass Types ........................................................................................ J-83
                              Currently Changed Settings .............................................................................. J-85
                            Cutting .................................................................................................................. J-86
                              Select a Batch ................................................................................................... J-86
                              Batch [number] - Batch [number] ...................................................................... J-90
                              Optimization Sequence ..................................................................................... J-92
                              Batch: Number .................................................................................................. J-93
                              Select the Optimizations to be Linked ............................................................... J-97
                              Optimization Result ........................................................................................... J-98
                              Rejects Pool ...................................................................................................... J-99
                              Add Rejects ..................................................................................................... J-101
                              Input of Shapes ............................................................................................... J-102
                              A+W DynOpt Editor ......................................................................................... J-103
                                   Description of buttons ............................................................................... J-104
                            Settings ............................................................................................................... J-106
                              Settings ........................................................................................................... J-107
                              Table Optimization .......................................................................................... J-108
                            View .................................................................................................................... J-109
                              Import ............................................................................................................. J-109
                              Error Reports ................................................................................................... J-110

                            Partindex                                                                                                         J-111
3.30 / 01-2023




                 J-6                                                                                              A+W Realtime Optimizer
A+W Realtime Optimizer        J

                         Tutorial




                A+W Production
                 Tutorial                                                                                     Basic Ideas




                                          Basic Ideas
                                          A major potential for saving in the flat glass processing is the optimum use of
                                          the stockplates at cutting. The smaller the waste or the residue plates, the hig-
                                          her is the use of material, and the lower the material cost. Controlling cutting
                                          tables with optimized cutting plans directly from the optimization speeds up the
                                          work process.
                                          A+W Realtime Optimizer is based on two fundamental ideas:
                                          •   Cutting optimization for the linked cutting table
                                          •   Transfer of cutting codes to the linked cutting table




                                          Fig. J-1      Cutting optimization and cutting table control
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-9
                 Basic Ideas                                                                              Tutorial




                               Features
                               A+W Realtime Optimizer supports these fundamental ideas with the following
                               features:
                               •   A+W Realtime Optimizer controls cutting by means of optimized detailed
                                   scheduling data.
                               •   Rush orders, rejects or filler sizes can be automatically re-optimized in a re-
                                   sidue plate.
                               •   Cutting tables are controlled mainly online by means of communication
                                   logs supported by the table manufacturers.
                               •   Rush order lites, rejects and fillers are optimized directly at the cutting tab-
                                   le.
                               •   Existing optimizations can be checked with regards to table optimization, to
                                   be resolved and reassembled if required. By adding rejects, filler sizes and
                                   rush orders, bigger optimizations can be created. Defined sequences on A
                                   racks are maintained.
                               •   Even at the detailed scheduling stage, A+W Production allows optimizing
                                   the cutting of every batch on the scheduled cutting table.
                               •   A+W Realtime Optimizer is especially configured for a cutting table, and
                                   can transfer the scheduled and optimized batches to this cutting table, to-
                                   gether with the cutting code.
                               •   Once the appropriate cutting code has been transferred to the cutting table,
                                   the breakout pattern can be displayed via XTV.
3.30 / 01-2023




                 J-10                                                                  A+W Realtime Optimizer
                 Tutorial                                                                Using A+W Realtime Optimizer




                                          Using A+W Realtime
                                          Optimizer
                                          This subject area introduces the functions of A+W Realtime Optimizer.
                                          This subject area includes the following training sessions:
                                          •   Import of Data
                                              – Working with A+W Production
                                              – Use as a stand-alone system
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                           J-11
                 Using A+W Realtime Optimizer                                                                        Tutorial




                                        Overview
                                        Objectives

                                        • Getting to know and understanding import of data
                                        • Getting to know and understanding the connection to A+W Production.
                                        • Getting to know and understanding the operation as stand-alone system


                                        Benefit

                                        The data have to be imported correctly before working with A+W Realtime Optimizer.


                                        Definitions

                                        Pre-systems                These systems supply with orders (batches) containing
                                                                   master data and cutting optimizations.

                                        Stand alone variant        The stand alone system imports the data by means of
                                                                   save files which must be provided in a special directory.

                                        Residue stock              The residue stock manages residue plates at the cutting
                                                                   table.


                                        Note

                                        A+W Realtime Optimizer     Can be adapted to all common cutting tables.

                                        Stand alone variant        The A+W Realtime Optimizer can be used as stand
                                                                   alone.

                                        Connection                 The staff of A+W configure the import of data.
3.30 / 01-2023




                 J-12                                                                           A+W Realtime Optimizer
                 Tutorial                                                                        Using A+W Realtime Optimizer




                                              Import of Data
                                              Depending on the basic system, data are imported fully or semi-automatically.
                                              These systems supply A+W Realtime Optimizer with batches containing base
                                              data and cutting optimizations.

                      Import of data                       Input and processing                      Cutting table control
                                                                  of data

                                                         A+W Realtime Optimizer
                            Batches                         Optimization and
                                                           Cutting code creation

                                                                                                          Cutting table




                                                                 Database




                 Fig. J-2       Overview of the work with A+W Realtime Optimizer; the work shown in italics only apply in connection
                                with stand alone systems


                                              A multitude of possible configurations open up the following possibilities in
                                              connection with A+W Realtime Optimizer:
                                              •   Integrated in an A+W Production or an A+W Business Pro environment
                                              •   Adapting to all common cutting tables
                                              •   Link to a residue stock plate
                                              •   Use as a stand-alone system
                                              The system is configured and installed by A+W staff.
                                              Possible basic systems are:
                                              •   A+W Production
                                              •   A+W Business Pro

                                                  Linking to the basic system
                                                  The staff of A+W configure the basic system and the import of data.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                       J-13
                 Using A+W Realtime Optimizer                                                                 Tutorial




                                                                    A+W Realtime
                                                                      Optimizer
                                           Import files
                                                                 Importing and check.
                                                                       the data,
                                                                   importing into the
                                         A+W Production               Database




                                                              A+W Production Database



                                                               Batches incl. optimization
                                                               and master data:
                                                               Articles
                                                               Glass Types
                                                               Tables
                                                               Optimization parameters
                                                               Stockplates



                                        Fig. J-3     Data import in A+W Realtime Optimizer


                                        If A+W Realtime Optimizer works with A+W Production, A+W Realtime Opti-
                                        mizer uses the A+W Production database as well. If another system is used,
                                        A+W Realtime Optimizer needs an empty A+W Production database. Master
                                        data and optimizations included in the batches of the basic system will be ad-
                                        opted by A+W Realtime Optimizer into the empty A+W Production database.
                                        Data are checked at the same time.
                                        The system rejects data which cause errors during import. The error log shows
                                        why the individual records were rejected. The data can be processed further.
3.30 / 01-2023




                 J-14                                                                        A+W Realtime Optimizer
                 Tutorial                                                                Using A+W Realtime Optimizer




                                          Working with A+W Production
                                          When A+W Realtime Optimizer is linked to an existing A+W Production sys-
                                          tem, data are exchanged automatically. Master data, batches, rejects, rush
                                          and filler orders are directly loaded from the A+W Production database. Apart
                                          from that, status reports for the individual batches are saved in the database.

                                          Master data
                                          If the access to base data was released at configuration, these can be viewed
                                          and processes.
                                          Master data include:
                                          •   Articles
                                          •   Glass Types
                                          •   Tables
                                          •   Optimization parameters
                                          •   Stockplates
                                          Master data and their use are described in section Detailed Scheduling of the
                                          A+W Production user manual.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-15
                 Using A+W Realtime Optimizer                                                                     Tutorial




                                        Use as a stand-alone system
                                        A+W Realtime Optimizer is installed with an empty A+W Production database.
                                        When batches are imported, the database is filled with master data.
                                        The stand alone system imports the data by means of save files which must
                                        be provided to A+W Realtime Optimizer in a special directory. Save files have
                                        to stick to a defined structure and are usually available in the working directory
                                        …\Xopton\im-port\work\*save.*. Imported data are removed from the working
                                        directory, and transferred to archives.

                                        Import optimizations
                                        Function Import optimizations is only required and valid for A+W Realtime Op-
                                        timizer stand alone versions.
                                        A+W Realtime Optimizer can supply a cutting table with cutting data or create
                                        table optimizations if batches are provided by another system. If batches are
                                        supplied, A+W Realtime Optimizer can import them for further processing.
                                        The following steps can be performed in connection with the import of batches:
                                        •   Switch on import
                                        •   Switch off import
                                        •   React to error reports


                                         Switch on import
                                        1 Open the dialog Import. Select View > Import.
                                        2 Use the [Start] button to start the import.
                                            A+W Realtime Optimizer checks the working directory for import files. If im-
                                            port files are found, the data are imported into the database while the im-
                                            port files are transferred to archives.
                                            Imported batches are available for further processing in the dialogs Select
                                            a batch and Select glass for optimization.
                                            Button [Start] becomes [Stop].
                                        3 Close the dialog. Press the [Close] button.
                                            A+W Realtime Optimizer monitors the working directory until the import
                                            function is switched off.
                                            Should errors occur during import, these are recorded; and the batches in
                                            question will not be imported. Errors can be processed manually.
3.30 / 01-2023




                 J-16                                                                          A+W Realtime Optimizer
                 Tutorial                                                                 Using A+W Realtime Optimizer




                                           Switch off import
                                          1 Open the dialog Import. As long as import is switched on, a minimized dia-
                                            log is shown in the bottom left corner of the A+W Realtime Optimizer dia-
                                            log.
                                          2 Use the [Stop] button to terminate import.
                                             Import files just stored in the working directory remain there, unprocessed.
                                             Button [Stop] changes into [Start].
                                          3 Close the dialog. Press the [Close] button.


                                           React to error reports
                                             Should errors occur during import, these are recorded; and the batches in
                                             question will not be imported.
                                             Import is stopped only at an imminent loss of data. This may be the case if
                                             an existing optimization shall be overridden. Depending on the configurati-
                                             on, an error message appears.
                                          1 Answer the question in the error report dialog xopt-on.
                                            Select the appropriate button, [Yes] or [No].
                                             Import of data is resumed.
                                          2 Open dialog Error messages. Select menu View > Error reports.
                                          3 Check the error messages and respond accordingly.


                                          Additional information
                                           “React to error reports” auf Seite J-17
                                           Software Reference, “Error Reports” on page J-110
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-17
                 Input                                                                      Tutorial




                         Input
                         This section tells you how to handle the input.
                         This subject area includes the following training sessions:
                         •   Rejects, Rush Order Lites or Filler Orders
                         •   Manual Creation of Plans
                         •   Charge Editor
3.30 / 01-2023




                 J-18                                                        A+W Realtime Optimizer
                 Tutorial                                                                                                   Input




                                          Overview
                                          Objectives

                                          • Getting to know and understanding rejects.
                                          • Getting to know and understanding rush order lites.
                                          • Getting to know and understanding filler orders.


                                          Benefit

                                          By using rejects, rush order lites and filler orders you can improve the yield.


                                          Definitions

                                          Reject                       A lite broken during cutting.

                                          Rush order lite              A lite, that must be cut quickly

                                          Filler order                 Serves to use capacities and material efficiently.


                                          Note

                                          Rejects                      Rejects can be entered manually via A+W Realtime
                                                                       Optimizer, or at another place within a networked
                                                                       production.

                                          Rush order lites             Rush order lites are created by A+W Realtime Optimizer
                                                                       and are saved in the database.

                                          Filler orders                Filler orders can be used only if A+W Realtime Optimizer
                                                                       is used together with A+W Production.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                     J-19
                 Input                                                                           Tutorial




                         Rejects, Rush Order Lites or Filler Orders
                         Rejects can be entered manually via A+W Realtime Optimizer, or at another
                         place within a networked production. Depending on the configuration, reject is
                         directly shown in the A+W Realtime Optimizer rejects pool. At the next oppor-
                         tunity, the broken lites are automatically optimized with the residue plate, or
                         (depending on the configuration) integrated manually into a table optimization.
                         Rush orders are created by A+W Realtime Optimizer and are saved in the da-
                         tabase. Rush orders can be integrated in the next table optimization with a sui-
                         table glass type and thickness.
                         Filler orders can be used only if A+W Realtime Optimizer is used together with
                         A+W Production. In this case, filler orders are directly taken from the A+W Pro-
                         duction database.

                           Rush orders      Breakage          Filler




                                       Realtime Optimizer
                                           Cutting table
                                       optimizations create




                                    A+W Production Database
                                     Batches with optimizations
                                     and base data:
                                     Articles
                                     Glass Types
                                     Tables
                                     Optimization parameters
                                     Stockplates



                         Fig. J-4       Input and processing of data in A+W Realtime Optimizer
3.30 / 01-2023




                 J-20                                                            A+W Realtime Optimizer
                 Tutorial                                                                                             Input




                                          Manual entry of lites
                                          In addition to batches from another system, A+W Realtime Optimizer allows
                                          to enter lites, add them to table optimizations, and transfer them to the cutting
                                          table.
                                          Use the following steps to enter or delete manually:
                                          •   Enter rush orders
                                          •   Editing rush orders
                                          •   Delete rush orders
                                          •   Enter rejects
                                          •   Delete rejects


                                           Enter rush orders
                                          1 Open dialog Rush order lites.
                                            Select menu Input > Rush order lites. Dialog Rush order lites shows all ent-
                                            ered rush order lites that have not been used in an optimization so far.
                                          2 Open dialog Enter rush orders. Press the button [Add].
                                          3 In field Glass type, select the glass type for these rush orders. If various
                                            thicknesses are available, enter the required thickness in field Thickness.
                                          4 In field Rack, enter the rack onto which the rush orders shall be put after
                                            cutting. Depending on the organization, this field can also remain empty.
                                          5 Enter the number of lites in field Quantity.
                                          6 In field Shape, select the shape number if you want to enter a shape.
                                              You can also process the shapes. To do this, use the [^] button. You can
                                              also define a free shape for rush order lites. Enter shape number 99. Select
                                              the corresponding SN file (entered and exported as Block-Ind file via CAD
                                              Designer Shapes from the catalog directory).
                                          7 Enter the lite dimensions in the fields Width and Height.
                                              When you enter a shape, these fields automatically show the dimensions
                                              of the surrounding rectangle.
                                          8 Save the input of rush orders. Press the [OK] button.
                                              Entered data are saved and shown in the list.
                                          9 Enter more lites or close the dialog.
                                              To enter more lites, repeat the procedure starting from step 2.
                                              Use the [End] button to close the dialog.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                               J-21
                 Input                                                                          Tutorial




                          Editing rush orders
                         1 Open the dialog Enter rush orders.
                           Select menu Input > Rush orders. Dialog Rush order lites shows all entered
                           rush orders that have not been used in an optimization so far.
                         2 On the rush order list, tag the line you want to edit.
                         3 Press [Edit]. This opens the dialog Rush order entry. The fields show the
                           data of the lite you want to change.
                         4 Enter the required changes and quit the dialog using [OK].


                          Delete rush orders
                         1 Open the dialog Enter rush orders.
                           Select menu Input > Rush orders. Dialog Rush orders shows all entered
                           rush orders that have not been used in an optimization so far.
                         2 Tag a line in the list of rush orders.
                         3 Press the [Delete] button.
                            The tagged rush order will be deleted.
                         4 Close the dialog. Press the [OK] button.


                          Enter rejects
                            If you use A+W Production (XTV) at the cutting table, rejects can be ent-
                            ered directly at the table, and is automatically transferred to A+W Realtime
                            Optimizer. Rejects can also be entered manually:
                         1 Open the dialog Rejects pool.
                           Select menu Cutting > Rejects pool > [Add].
                         2 In section Product ID enter order number, item number and sub item num-
                           ber the broken lite belongs to.
                         3 If you are working with Barcoding you can enter the reject reason. Select
                           the appropriate entry from the combo box Reject reason.
                         4 Save the entries. Press the [Save] button.
3.30 / 01-2023




                 J-22                                                         A+W Realtime Optimizer
                 Tutorial                                                                                          Input




                                           Delete rejects
                                          1 Open the dialog Rejects pool.
                                            Select menu Cutting > Rejects pool. Dialog Rejects pool shows all broken
                                            lites that have been entered, and have not been used for optimization.
                                          2 Tag one or more lines on the reject list.
                                          3 Press the [Delete] button.
                                             The tagged reject will be deleted.
                                          4 Close the dialog. Press the [Close] button.

                                             Booking rejects
                                             Use [Booking F5] button to transfer the rejects to production. In case you
                                             have reported lites as rejects by mistake, you can also use this button the
                                             report the lites as OK.


                                          Additional information
                                           Software Reference, “Input of Shapes” on page J-62
                                           Software Reference, “Rush Orders” on page J-58
                                           Software Reference, “Rejects Pool” on page J-99
                                           Software Reference, “Add Rejects” on page J-101
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-23
                 Input                                                                              Tutorial




                         Manual Creation of Plans
                         This option allows to create a purele manual plan and save it as local optimi-
                         zation in the database. The manual plan can be edited and changed after-
                         wards. This is done by means of module A+W PlanEdit. For details on this
                         module, please refer to the corresponding documentation. No barcode infor-
                         mation will be available for manual plans.


                          How to create a new plan
                         1 Select menu Input > Manual Plan. Dialog Manual Plan Input Cutting
                           Table … appears.
                         2 In section Glass Types select the glass type you want to create the plan for.
                         3 On the left select the stock size in section Stockplates, that shall be used
                           for the manual cutting pattern.
                         4 In section Residue Plates define height and width for the residue plate to
                           be created.
                         5 Click on the icon [New]. A+W PlanEditor opens.
                         6 Enter the requested lites via context menu. Thus, select option Insert and
                           enter the specific lite data.
                         7 Via File > Save as it is possible to save the cutting plan as file.
                         8 Use Output > AWC for transfer to cutting.


                          How to edit a manual plan
                         1 To edit a manually entered cutting plan, choose Input > Manual Plan from
                           menu. Dialog Manual Plan Input Cutting Table … opens. The lower section
                           Plan shows the plan previously entered.
                         2 Use the [Edit] button to open the plan, previously entered and make the
                           modifications.
                         3 Don't forget to save the modifications or to release the data via Output >
                           AWC.


                          How to select a plan manually entered for cutting
                         1 A plan manually entered can only be cut directly via Cutting.
                         2 Use the [Cutting] button to select all batches optimized and prepared for
                           cutting.
                         3 The manually created plan appears in the list of available batches with
                           batch number >15000 and has the additional information PlanEdit.
                         4 Select the batch and prepare it for cutting ([Options] button) or cut it directly
                           ([Cutting] button).
3.30 / 01-2023




                         Additional information
                          Software Reference, “Manual Plan Input” on page J-64




                 J-24                                                           A+W Realtime Optimizer
                 Tutorial                                                                                               Input




                                          Charge Editor
                                          Via this dialog it is possible to define a charge number. Tag the checkbox and
                                          the entered charge number will be inherited to the following stockplates of the
                                          identical glass type/thickness. The last charge number is saved per glass type/
                                          thickness/stock plate. Next time, this editor will be opened the input field is pre-
                                          set with this value. The allocation always affects the selected stock size (and
                                          in case of inheritance those below).
                                          A set charge (including inheritance) can also be deleted via this editor.
                                          If the cutting process for a stock size has no batch allocation, the user has to
                                          enter a charge number first. The dialog Charge Editor appears with a corre-
                                          sponding info in A+W Production Terminal (XTV). The entered charge number
                                          is used for all lites of the respective stock size while passing the A+W Produc-
                                          tion Terminal (XTV).


                                          Additional information
                                           Software Reference, “Charge Editor” on page J-67
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                 J-25
                 Optimization                                                                      Tutorial




                                Optimization
                                This section shows you how the optimization works.
                                This subject area includes the following training sessions:
                                •   Cutting Table Optimizations
                                •   Create a Quick Optimization
                                •   Linking of Batches
                                •   Cutting Table Control
3.30 / 01-2023




                 J-26                                                               A+W Realtime Optimizer
                 Tutorial                                                                                           Optimization




                                          Overview
                                          Objectives

                                          •   Getting to know and understanding table optimizations
                                          •   Getting to know and understanding quick optimizations
                                          •   Getting to know and understanding linking of residue plates
                                          •   Getting to know and understanding cutting table control


                                          Benefit

                                          The more efficient the optimization works, the higher the yield. This saves money.


                                          Definitions

                                          Cutting table optimizations Optimizations, created with A+W Realtime Optimizer.

                                          Quick optimization           Plates, not sent yet to the cutting table can be resolved
                                                                       completely and re-optimized.


                                          Note

                                          Batch                        A batch is a composition of glass from one or more
                                                                       orders, to be considered and produced at once in
                                                                       optimization and production (e.g. same route, same
                                                                       customer, same glass types, same production dates).
                                                                       The optimizations of prior systems exist in the shape of
                                                                       batches.

                                          Lot                          A part / a glass type of a batch, that shall be processed /
                                                                       cut under identical conditions at the same time (e.g. all
                                                                       Float 4 of a batch).

                                          Cutting table control        The cutting table to be controlled by A+W Realtime
                                                                       Optimizer is defined during installation.

                                          Rejects                      Can either be cut in the re-optimization at the end of a
                                                                       batch to be cut or transferred to rejects pool and can be
                                                                       cut together with the next batch.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                      J-27
                 Optimization                                                                              Tutorial




                                Cutting Table Optimizations
                                Table optimizations are created by A+W Realtime Optimizer. Basic systems
                                provide complete optimizations which are resolved by A+W Realtime Optimi-
                                zer to be rearranged. You can combine any number of batches, provided there
                                is enough space for the racks at the cutting table.
                                When you create table optimizations, you can take into account residue plates
                                on the cutting table, use different stockplates, or use a residue stock. Rejects,
                                rush or filler orders can be excluded or integrated as required.
                                Table optimizations are saved in the database, and are used for cutting if re-
                                quired.


                                Create Table Optimizations
                                The following steps are necessary when creating a new table optimization:
                                •   Select glass type and batch for table optimization
                                •   Create table optimization


                                 Select glass type and batch for table optimization
                                1 Open the dialog Select glass for optimization.
                                  Select Optimization > Table Optimization.
                                2 From the list Glass type select the glass type to be optimized. The list Glass
                                  type shows if special orders (reject, rush orders, etc.) exist in A+W Real-
                                  time Optimizer for the glass type.
                                    If you select a glass type for which there are broken lites or rush orders,
                                    these will be automatically integrated in the new table optimization (if con-
                                    figured).
                                    If your system is configured to work with a residue plate dispenser, this list
                                    shows whether a residue plate is available for the glass type in question.
                                    The list Available optimizations shows all batches containing optimizations
                                    for the glass type and thickness selected from the list Glass type.
                                3 Tag the checkbox Permit manual cutting to show even glass types that are
                                  only meant to be cut manually.
                                4 From the list Available optimizations select the batches to be arranged in a
                                  table optimization.

                                    Select only rejects and rush orders
                                    If there are broken lites or rush orders for the selected glass type, these li-
                                    tes can be optimized without another batch. Do not select a batch from the
                                    list in this case.

                                    If you have tagged a batch but do not want to select it, change the selected
                                    glass type. When you select the required glass type again, no batch will be
3.30 / 01-2023




                                    tagged.
                                5 Click on [Select] to compile the selected batches in a table optimization.



                 J-28                                                                  A+W Realtime Optimizer
                 Tutorial                                                                                   Optimization




                                             The dialog closes. Dialog Table optimization appears in which the tab Op-
                                             timize shows the selected batches.


                                           Create table optimization
                                          1 Please make sure that in the previous step, Select batches for table opti-
                                            mization, batches have been actually selected.
                                             Dialog Table optimization appears with the tab Optimize.
                                          2 Select the necessary optimization parameters.
                                          3 Select the required parameter from register Stockplates.
                                          4 Select the required parameters from register Filler.
                                          5 To create the optimization, return to tab Optimize and press the button [Op-
                                            timize].
                                             The dialog disappears, and the optimization is run in the background. As
                                             long as the optimization is running, you can go on working with A+W Real-
                                             time Optimizer.
                                             As soon as the optimization result is available, the dialog reappears auto-
                                             matically. The optimization result is shown in register Overview.
                                          6 To save the optimization, press [Save].
                                             The optimization is now shown in dialog Select a batch and can be trans-
                                             ferred to the cutting table.


                                          Additional information
                                           Software Reference, “Select Glass for Optimization” on page J-68
                                           Software Reference, “Optimize” on page J-74
                                           Software Reference, “Residue Plates and Stockplates” on page J-77
                                           “Selecting Batches for Cutting” auf Seite J-39
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                            J-29
                 Optimization                                                                               Tutorial




                                Check and Process Table Optimization Result
                                Table optimizations can be checked anytime before they are transferred to the
                                cutting table. To change a table optimization, to add reject, rush orders, or filler
                                sizes, or to add or delete whole batches, you need to resolve the entire opti-
                                mization, and create a new one.
                                The following steps are possible when creating a table optimization:
                                •   Select other stockplates for optimization
                                •   Use residue plate from previous optimization
                                •   Add filler sizes to the optimization
                                Changes are impossible once a table optimization was saved.


                                 Select other stockplates for optimization
                                1 From dialog Table optimization, select register Stockplates.
                                    The list on the right side shows all stockplates defined in master data for
                                    this glass type and thickness, which are available for cutting.
                                2 Tag the stockplate(s) A+W Realtime Optimizer may use for cutting optimi-
                                  zation.
                                    During optimization A+W Realtime Optimizer checks how many lites of
                                    which size are needed to achieve the optimum result.
                                3 To create the optimization, switch to the register Optimize and press the
                                  [Start] button.
                                4 To save the optimization, press [Save].


                                 Use residue plate from previous optimization
                                1 From dialog Table optimization, select register Stockplates.
                                    If there is a residue plate of the same glass type and thickness on the cut-
                                    ting table as required in the present optimization, this can be integrated in
                                    the table optimization.
                                2 Enter the height and width of the residue plate on the cutting table in secti-
                                  on Residue plate.
                                3 To create the optimization, switch to the register Optimize and press the
                                  [Start] button.
                                4 To save the optimization, press [Save].
3.30 / 01-2023




                 J-30                                                                   A+W Realtime Optimizer
                 Tutorial                                                                                       Optimization




                                           Add filler sizes to the optimization
                                          1 From dialog Table optimization, select register Filler.
                                             The list on the right shows all filler orders defined for the glass type and
                                             thickness of this batch.
                                          2 Tag the filler orders to be integrated in the table optimization.
                                             Ideally, filler orders are used to minimize the waste, or the residue plate.
                                          3 To create the optimization, go to tab Optimize and press [Optimize].
                                          4 Continue to add or delete filler orders until the optimum result is reached.
                                          5 To save the optimization, press [Save].


                                          Additional information
                                           “Resolve Table Optimization” auf Seite J-32
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-31
                 Optimization                                                                              Tutorial




                                Resolve Table Optimization
                                Table optimizations can be resolved only if they were saved after having been
                                created. As long as dialog Table optimization is open and the table optimizati-
                                on in question has not been saved, the optimization can be rejected by pres-
                                sing the Abort button.
                                When you resolve a table optimization, the batches included are returned to
                                the batch list. Possibly included rejects, rush orders, or filler orders are retur-
                                ned to the appropriate pools, and are available again for optimization.
                                Optimizations for which cutting was started and aborted, can also be resolved.
                                Batches for which lites were cut already, are reset and treated as if cutting had
                                not taken place.


                                 Resolve created and saved table optimizations
                                1 Open the dialog Reset cutting batch.
                                  This is done in menu Optimization > Reset.
                                   Dialog Reset a cutting batch shows a list of all batches available for status
                                   changes. The list is sorted by batch numbers. Table optimizations are
                                   shown as batches with numbers starting from 15000 (can be configured).
                                2 Tag the table optimization you want to break down.
                                  Tag the corresponding batch with a number higher than 15000.
                                   You can tag several table optimizations to be resolved at the same time.
                                3 To save the optimization, press the [OK] button. A security check appears.
                                4 Confirm this query. Select the [Yes] button.
                                   The batches and lites of the selected table optimization are now available
                                   for new table optimizations. If the table optimization was using ReMaster
                                   lites, these are available again after the optimization was resolved.


                                Additional information
                                 “Create Table Optimizations” auf Seite J-28
3.30 / 01-2023




                 J-32                                                                  A+W Realtime Optimizer
                 Tutorial                                                                                      Optimization




                                          Linking of Table Optimizations
                                          To improve the waste it is possible to link table optimizations. Linking is only
                                          possible for table optimizations with identical glass types. Which means, the
                                          table optimizations must exist.
                                          To link table optimizations the following steps are required:
                                          •   Select glass type and batch for table optimization
                                          •   Create table optimization


                                           Linking of table optimizations
                                          1 Open the dialog Select glass for optimization.
                                            Select Optimization > Table optimization.
                                          2 From the list Glass type select the glass type to be optimized. The list Glass
                                            type shows if special orders (rejects, rush orders, etc.) exist in A+W Real-
                                            time Optimizer for the glass type.
                                              If you select a glass type for which there are broken lites or rush orders,
                                              these will be automatically integrated in the new table optimization (if con-
                                              figured).
                                              If your system is configured to work with a residue plate dispenser, this list
                                              shows whether a residue plate is available for the glass type in question.
                                              The list Available optimizations shows all batches containing optimizations
                                              for the glass type and thickness selected from the list Glass type.
                                          3 Tag the checkbox Permit manual cutting to show even glass types that are
                                            only meant to be cut manually.
                                          4 From the list Available optimizations select the batches to be arranged in a
                                            table optimization.


                                          Additional information
                                           “Linking of Table Optimizations” auf Seite J-33
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-33
                 Optimization                                                                                            Tutorial




                                             Create a Quick Optimization
                                             Plates / patterns already optimized (via A+W Production or via table optimiza-
                                             tion in A+W Realtime Optimizer), but still not sent to the table, can be resolved
                                             completely and re-optimized. Thus, rush order lites and rejects will also be op-
                                             timized and a completely new cutting pattern is the result for the re-optimized
                                             plates.
                                             The following steps are necessary when creating a quick optimization:
                                             •     Create table optimization
                                             •     Cutting of table optimization has been started
                                             In case of reject during cutting, this can be re-cut in real-time by using the quick
                                             optimization.




                 Fig. J-5       Cutting overview


                                             Via the context menu it is possible to resolve the optimization from the next
                                             pattern on and to re-optimize.
                                             In example Fig. J-5 (Cutting overview) the patterns / plates 1 and 2 were sent
                                             to table and cut. The plates / patterns 3-6 can be resolved and re-optimized
                                             (quick optimizations) via right click.




                                             Fig. J-6       Context menu
3.30 / 01-2023




                                             After confirming the message the plates still to be cut will be removed. Then,
                                             the broken lites and the plates still to be cut will be re-optimized.


                 J-34                                                                                A+W Realtime Optimizer
                 Tutorial                                                                                         Optimization




                                          Additional information
                                           “Cutting Overview” auf Seite J-44



                                          Linking of Batches
                                          With the linking of batches, A+W allows to avoid residue plates. In the past,
                                          residue plates had to be assembled manually. This is no longer necessary.
                                          Linking takes place during cutting.
                                          Dialog Batch: # activates the option for linking batches in section Residue pla-
                                          te management.
                                          When cutting is started, the system will send the first pattern of a batch then
                                          search - starting from the next batch - the database for a suitable batch of this
                                          glass type; the corresponding data will be loaded.
                                          The next batch must have the status Released. The batch is loaded in the
                                          background so as not to interrupt cutting. When the penultimate lite (can be
                                          configured) of a glass type has been cut, the user will be informed (optionally!)
                                          as to which batch and batch the residue plate will be linked to. The user can
                                          abort the linking at this point or choose a corresponding lot.
                                          When the user confirms this link, rush order lites and rejects of this glass type
                                          will be loaded, and added to the next optimization with priority 0. The residue
                                          plate of the currently cut batch becomes the start plate of the next optimization.
                                          Optimization is started. After the optimization, the next optimization will be lin-
                                          ked with the original optimization so that the residue plate of the original opti-
                                          mization will be filled with the lites of the first plate of the next optimization. All
                                          other patterns of the next optimization will be resolved in the last cut optimiza-
                                          tion. The system now creates and transfers a new cutting code.
                                          The first pattern of the next optimization is market Cut. Using the mechanism
                                          from the table optimization, the next optimization is first saved as a table opti-
                                          mization, after which the batch and batch number of the original, next optimi-
                                          zation are added. The status of the next optimization is changed to Started.


                                          Additional information
                                           Software Reference, “Select the Optimizations to be Linked” on page J-97
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                    J-35
                 Optimization                                                                            Tutorial




                                Cutting Table Control
                                A+W Realtime Optimizer works as a cutting control station.

                                   Parameters of the linked table
                                   The cutting table to be controlled by A+W Realtime Optimizer is defined du-
                                   ring installation. The corresponding parameters are defined at installation.
                                   Optimizations are created with the parameters set in A+w Production or
                                   A+W Realtime Optimizer.

                                A cutting code is created and transferred to the cutting table, or is made avai-
                                lable in a defined directory. Depending on the cutting table and the table con-
                                trol, the cutting table is transferred to the table by a special program, or is
                                loaded from the defined directory by the cutting table software.


                                  A+W Realtime Optimizer
                                    Cutting code creation
                                       Re-optimization
                                     Status management
                                                                             Cutting table




                                    Production database
                                           Optimizations



                                Fig. J-7        Input and processing of data in A+W Realtime Optimizer


                                Once the cutting code for a stockplate was sent to the cutting table, A+W Real-
                                time Optimizer considers this stockplate completed. If transfer of the cutting
                                code is interrupted, work can be resumed at this precise spot.
                                In connection with XTV, breakage at the cutting table is directly reported to
                                A+W Realtime Optimizer. As long as the cutting code for the last stockplate of
                                a glass type (a batch) has not been transferred to the cutting table, breakage
                                can be automatically re-optimised, to be cut with the last stockplate of the
                                batch.
3.30 / 01-2023




                 J-36                                                                    A+W Realtime Optimizer
                 Tutorial                                                                               Cutting




                                          Cutting
                                          This section tells you how to handle the cutting.
                                          This subject area includes the following training sessions:
                                          •   Selecting Batches for Cutting
                                          •   Check Optimization and Cut
                                          •   Interrupt and Continue Work
                                          •   Cutting Overview
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                   J-37
                 Cutting                                                                                Tutorial




                           Overview
                           Objectives

                           • Getting to know and understanding the cutting process.


                           Benefit

                           A+W Realtime Optimizer can be used to the best effect only if you are capable of the
                           process.


                           Definition

                           Panorama                    Part of the program that can be configured to control
                                                       complex machines or more machines (cutting lines).


                           Note

                           Batch number 1000-9999      Come from a prior system.

                           Batch number from 15000     Batches starting from number 15000 contain table
                                                       optimizations created by A+W Realtime Optimizer. The
                                                       number range can be configured.

                           Panorama                    Administration of Panorama is password-protected.
3.30 / 01-2023




                 J-38                                                               A+W Realtime Optimizer
                 Tutorial                                                                                          Cutting




                                          Selecting Batches for Cutting
                                          Optimizations exist in the shape of batches. Select the batches containing the
                                          optimizations you want to cut on the cutting table.


                                           Selecting batches for cutting
                                          1 Open dialog Select a batch.
                                            Select menu Cutting > Cutting optimization.
                                          2 Select a batch. Select an entry in the Batch list. The Optimization list shows
                                            the optimizations existing for this batch.

                                             Batch numbers
                                             Batches of the numbers 1000-9999 come from another system and contain
                                             one or more optimizations. Batches starting from number 15000 contain ta-
                                             ble optimizations created by A+W Realtime Optimizer.

                                          3 Select one or all optimizations. If no optimization is tagged, the system as-
                                            sumes that all to be selected. You can configure whether individual optimi-
                                            zations can be selected.

                                             Optimization numbers
                                             Optimizations are defined per lot (per glass type), and numbered consecut-
                                             ively for every batch.

                                          4 Press [OK]. The tagged optimizations are selected for cutting and shown in
                                            dialog Batch [number -] - batch [number].
                                          5 Close the dialog. Press the [OK] button.
                                          6 Start the cutting process. Press the [START] button.


                                           Re-cut already cut batches
                                             When all plates of an optimization have been cut, the entire batch gets the
                                             status Produced. This status can be reset to status Released, and the ent-
                                             ire batch can be cut again.
                                          1 Open the dialog Reset cutting batch.
                                            This is done in menu Optimization > Reset.
                                             Dialog Reset a cutting batch shows a list of all batches available for status
                                             changes. The list is sorted by batch numbers. Completely cut batches are
                                             shown with status Produced.
                                          2 Select the batch you want to reset from status Produced to status Relea-
                                            sed. You can tag several batches, and reset them together.
                                          3 Press the [OK] button to reset the batch.
                                             The batch is now available again for cutting as a complete optimization.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                              J-39
                 Cutting                                                                             Tutorial




                            Skip pattern
                              If you choose Skip pattern for a lite, no cutting code will be created, and no
                              cutting plan will be shown for this lite.
                           1 Open the dialog Residue plate handling.
                             Press the button [Options] in dialog Batch: [No.] - Batch: [No.] for the batch
                             you want to edit.
                           2 Tag in the Optimizations list the glass type for which individual stockplates
                             shall be cut again.
                              The Lite list shows all lites for a batch belonging to the selected glass type.
                              Column Status shows the status of each stockplate.
                              You can skip only lites with a status other than Cut.
                           3 Click the right mouse key on the lite to be skipped during cutting.
                              A context menu appears with the entries Skip pattern, and Do not send cut-
                              ting code.
                           4 Select Skip pattern to stop the system from creating a cutting code and a
                             breakout pattern for this lite.
                           5 Close the dialog. Press the [OK] button.


                            Suppress cutting code creation
                              If you select Do not send cutting code for a lite, the system will create no
                              cutting code, but the breakout pattern will be shown in A+W Production Ter-
                              minal (XTV).
                           1 Open the dialog Residue plate handling.
                             Press the button [Options] in dialog Batch: [No.] - Batch: [No.] for the batch
                             you want to edit.
                           2 Tag in the Optimizations list the glass type for which individual stockplates
                             shall be cut again.
                              The Lite list shows all lites for a batch belonging to the selected glass type.
                              Column Status shows the status of each stockplate.
                              You can send no cutting code only for lites with a status other than Cut.
                           3 Click the right mouse key on the lite to be skipped during cutting.
                              A context menu appears with the entries Skip pattern, and Do not send cut-
                              ting code.
                           4 Select Do not send cutting code to stop the system from creating a cutting
                             code for this lite, but show the breakout pattern in A+W Production Terminal
                             (XTV).
                           5 Close the dialog. Press the [OK] button.


                           Additional information
3.30 / 01-2023




                            Software Reference, “Batch: Number” on page J-93
                            Software Reference, “Select a Batch” on page J-86




                 J-40                                                             A+W Realtime Optimizer
                 Tutorial                                                                                         Cutting




                                          Check Optimization and Cut
                                          Once you have selected optimizations for cutting, you can run some checks,
                                          then transfer the optimizations to the cutting table.
                                          This chapter describes the following steps:
                                          •   Show scheduled cutting sequence
                                          •   Check residue plates
                                          •   Define start of cutting and start cutting
                                          The following descriptions are based on the assumption that you have com-
                                          pleted the previous step Selecting Batches for Cutting and that the dialog
                                          Batch: [No.] - Batch: [No.] is displayed.


                                           Show scheduled cutting sequence
                                          1 Press the button [Sequence].
                                            Dialog Cutting sequence appears.

                                              Sequence in case of several batches
                                              If several batches have been selected for cutting, the stockplates will be
                                              sorted acc. to the configuration of A+W Realtime Optimizer. All residue pla-
                                              tes can be cut at the end of the batch for example, or at the end of a glass
                                              type. A+W Realtime Optimizer can be configured to cut stockplates alter-
                                              nately (e. g. coated - uncoated).

                                          2 Press [OK] to close the dialog.


                                           Check residue plates
                                          1 Press the button [Residue plates].
                                            Dialog Residue plate handling appears.
                                          2 Check the displayed values.
                                          3 Amend the status of individual plates, or the settings for reject handling if
                                            necessary.
                                          4 If the PlanEdit module is installed on your workstation, you can view the
                                            cutting pattern for the selected stockplate by using the button Process pat-
                                            tern.
                                          5 Press [OK] to close the dialog.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-41
                 Cutting                                                                           Tutorial




                            Define start of cutting and start cutting
                           1 In the Optimizations list, tag the batch from where cutting shall start.
                           2 From the Pattern list, select the stockplate from where cutting shall start.
                           3 Press the [START] button.
                              The system creates the cutting code for the optimizations displayed, and
                              transfers it to the connected cutting table.
                              Wording and function of the button changes into [STOP].
                              If A+W Realtime Optimizer works with A+W Production Terminal (XTV), the
                              A+W Production Terminal (XTV) breakout display can be controlled by the
                              keys [Stop] and [<<].


                           Additional information
                            Software Reference, “Batch: Number” on page J-93
                            Software Reference, “Batch [number] - Batch [number]” on page J-90
3.30 / 01-2023




                 J-42                                                           A+W Realtime Optimizer
                 Tutorial                                                                                            Cutting




                                          Interrupt and Continue Work
                                          An optimization that cuts the stockplates in succession, can be interrupted due
                                          to technical interferences or the end of a shift. A+W Realtime Optimizer regis-
                                          ters the point at which the work was interrupted and allows to go on from there.
                                          The following steps are described below:
                                          •   Interrupt cutting during an optimization
                                          •   Continue cutting after an interruption


                                           Interrupt cutting during an optimization
                                          1 You are in dialog Cutting overview.
                                          2 Press [STOP].
                                          3 Close the dialog.


                                           Continue cutting after an interruption
                                              A+W Realtime Optimizer remembers optimizations that have not been cut
                                              completely.
                                          1 Select menu Cutting > Cut optimization to select an optimization for cutting.
                                              A security check appears. The system shows the incomplete batch and
                                              asks whether this shall be completed.
                                          2 To view the interrupted batch, select [Yes].
                                              A+W Realtime Optimizer shows the interrupted batch in dialog Batch: [No.]
                                              - Batch: [No.].
                                              If you answer the security check by No, the interrupted optimization will be
                                              set to Started. Already transferred cutting patterns remain on status Cut.
                                              Dialog Select a batch appears.
                                          3 To continue the interrupted cutting, press [Start].
                                              The cutting code of the already cut lites is not transferred to the cutting ta-
                                              ble again.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-43
                 Cutting                                                                                         Tutorial




                                         Cutting Overview
                                         The cutting overview shows the glass to be cut next.


                        A




                                                                                                                  B




                                                                                                                  C



                 A Menu                             B Plate view                     C Lite view
                 Fig. J-8   Cutting overview


                                         To show or hide the menu (A) on the left side of the dialog press the respective
                                         icon. It is also possible to expand and reduce the individual entries (Cutting,
                                         Panorama, Administration).
                                         The view can be configured via the options in entry cutting.




                                         Fig. J-9       Plate view
3.30 / 01-2023




                                         The plate view (B) can be configured per table. The combobox serves to con-
                                         trol which fields shall be displayed.


                 J-44                                                                         A+W Realtime Optimizer
                 Tutorial                                                                                            Cutting




                                          To reflect the plate picture activate in section Plate Picture the requested axis.
                                          The same applies to lite picture (C). Here you can also show or hide the re-
                                          quested display options.




                                          Fig. J-10    Lite view


                                          The point Shape in entry Panorama visualizes the shape saved for machine
                                          control in A+W Realtime Optimizer.
                                          The section Administration is password-protected. Here you make general
                                          settings.
                                          Press the [Start] icon to start the cutting. Press the [Stop] icon to stop the cut-
                                          ting.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-45
                 Cutting                                                                              Tutorial




                           Reset Cutting Status
                           If a batch or individual stockplates has already reached the status Cut but shall
                           be cut again, the production status can be reset, and cutting can be repeated.
                           The production status can be reset by:
                           •   Re-cut already cut lites
                           •   Re-cut already cut batches
                           If the whole optimization was reset, but only individual stockplates shall be cut
                           again, you can exclude parts of the optimization from being cut again by:
                           •   Skip pattern
                           •   Suppress cutting code creation


                            Re-cut already cut lites
                               Individual lites of whole batches can be cut again as long as A+W Realtime
                               Optimizer can still access the batches. Cutting of the corresponding batch
                               has to be selected and displayed in dialog Batch: [No.] - Batch: [No.].
                           1 Open the dialog Residue plate handling.
                             Press the button [Residue plates] in dialog Batch: [No.] - Batch: [No.] for
                             the corresponding batch.
                           2 On the Optimizations list, tag the glass type for which a stockplate shall be
                             cut again.
                               The Lite list shows all lites for a batch belonging to the selected glass type.
                               Column Status shows the status of each stockplate.
                                Software Reference, “Batch: Number” on page J-93
                           3 Click the right mouse key on the lites you want to reset from status Cut to
                             be cut again.
                               A context menu appears showing the entry Cut.
                           4 Select Cut to reset the lite.


                           Additional information
                            Software Reference, “Batch: Number” on page J-93
3.30 / 01-2023




                 J-46                                                              A+W Realtime Optimizer
                 Tutorial                                                                       Interplay with Other Modules




                                          Interplay with Other Modules
                                          Objectives

                                          •   Getting to know and understanding the work with a residue plate stock.
                                          •   Getting to know and understanding the work with A+W Production Terminal (XTV).
                                          •   Getting to know and understanding the work with A+W PlanEditor.
                                          •   Getting to know and understanding the work with A+W Defect Optimizer.


                                          Benefit

                                          The performance of A+W Realtime Optimizer can be increased by adapting other
                                          modules.


                                          Definitions

                                          Residue dispenser           The residue dispenser manages residue plates at the
                                                                      cutting table.

                                          A+W Production Terminal     Offers a breakout display at the cutting table.
                                          (XTV)

                                          A+W PlanEditor              Shows the data of patterns to be cut, tabulated and
                                                                      graphically.

                                          A+W Defect Optimizer        The intelligent defect optimization

                                          A+W DynOpt Compact          A+W entry level solution for dynamic optimization


                                          Note

                                          Configuration               A+W Realtime Optimizer can be configured to work with
                                                                      different modules.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                     J-47
                 Interplay with Other Modules                                                                       Tutorial




                                         Overview
                                         A+W Realtime Optimizer can be configured to work with different modules. For
                                         information on linking with different basic systems please refer to the previous
                                         chapter.
                                         If A+W Realtime Optimizer is configured accordingly, it can work with other
                                         modules such as:
                                         •      Residue Dispenser
                                         •      A+W Production Terminal (XTV)
                                         •      A+W PlanEditor
                                         •      A+W Defect Optimizer


                                         Residue Dispenser
                                         The residue dispenser manages residue plates at the cutting table. If a residue
                                         plate remains after cutting, it will not be rejected but stored there. Information
                                         on glass type, thickness, and size of the residue plates are entered and saved
                                         in a management program. A+W Realtime Optimizer can work with the resi-
                                         due dispenser administration program. Data concerning residue plates are ex-
                                         changed. A+W Realtime Optimizer can integrate residue plates in table
                                         optimizations. When an optimization is cut, the residue plate can be replaced
                                         by a plate from the dispenser (without re-optimization).
                                         When a residue plate is integrated in an optimization, A+W Realtime Optimizer
                                         informs the residue management program of its status. This residue plate can-
                                         not be used elsewhere.
                                         If a table is controlled with a cutting code that was optimized for a residue pla-
                                         te, the cutting code controls the dispenser, and the required residue plate is
                                         put onto the table for cutting.


                                         Additional information
                                          Tutorial, “Import of Data” on page J-13

                                         Use Stored Residue Plates
                                         This function is available only if your system has been configured to work with
                                         a residue plate dispenser.

                                                Plates from the dispenser and residue plates cannot be used at the
                                                same time!
                                                If you want to use plates from the dispenser for optimization, a previously
                                                entered residue plate will be ignored. A+W Realtime Optimizer comes up
                                                with a message to that effect.
3.30 / 01-2023




                 J-48                                                                            A+W Realtime Optimizer
                 Tutorial                                                                    Interplay with Other Modules




                                           Use dispenser plates for optimization
                                          1 Select Dispenser plates in dialog Table optimization.
                                             The list on the right shows all plates the dispenser has to offer for the ap-
                                             propriate glass type and thickness that are available for cutting.
                                          2 Tag the dispenser plate A+W Realtime Optimizer shall use for cutting opti-
                                            mization.
                                             Up to ten dispenser plates can be integrated in an optimization.
                                          3 To create the optimization, go to tab Optimize and press [Optimize].
                                             The dispenser plate is now reserved for this batch in the program that ma-
                                             nages the dispenser; they cannot be used by another batch now.
                                          4 To save the optimization, press [Save].


                                          A+W Production Terminal (XTV)
                                          A+W Production Terminal (XTV) offers a breakout display at the cutting table
                                          which, depending on the configuration, can be used to enter rejects. A+W
                                          Realtime Optimizer passes on information to A+W Production Terminal (XTV)
                                          once the cutting code for the connected table has been created. A+W Produc-
                                          tion Terminal (XTV) can then show the breakout pattern for this optimization.
                                          If A+W Production Terminal (XTV) is used to enter rejects, A+W Production
                                          Terminal (XTV) informs A+W Realtime Optimizer accordingly.


                                          Additional information
                                           For more information on A+W Production Terminal (XTV) please refer to the appro-
                                            priate documentation.


                                          A+W PlanEditor
                                          PlanEditor shows the data of patterns to be cut, tabulated and graphically. The
                                          results show the statistical evaluation of the existing patterns. You get a quick
                                          overview of the lites to be produced, stock sizes, residue plates, waste, etc.
                                          Depending on the configuration, the graphics editor shows the patterns to be
                                          cut, and offers various ways of processing. You can create and change pat-
                                          terns, add lites, save and print the pattern.
                                          If PlanEditor is installed at your workstation, you can start PlanEditor by dou-
                                          ble-clicking on an optimized plate. PlanEditor shows the cutting pattern for this
                                          plate. Amendments made by PlanEditor will be adopted by A+W Realtime Op-
                                          timizer.


                                          Additional information
                                           For more information on A+W PlanEditor please refer to the appropriate documen-
                                            tation.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                               J-49
                 Interplay with Other Modules                                                                      Tutorial




                                         A+W Defect Optimizer
                                         … the intelligent defect optimization
                                         The stock plates are scanned in conjunction with a quality scanner, e.g. from
                                         Viprotron, and any faults or defects are detected and displayed. The earlier de-
                                         fects are detected during the process, the lower the incurred costs.
                                         Defects are taken into account during optimization for the restructuring of the
                                         sectional image. If there are any orders that are to be considered, then those
                                         will of course be taken into account.
                                         Defects in residual plates are also stored, and can thus be reused later without
                                         additional inspections.
                                         If defects cannot be avoided through the optimization process (e. g. number
                                         and size of stock lites on pattern), the optimization process tries to use smaller
                                         and thus cheaper glass panes for the defects.
                                         Glass that is positioned on defects is automatically reported as reject and is
                                         recut.

                                                Requirements
                                                The production system A+W Production as well as the A+W Realtime Op-
                                                timizer are prerequisites to use the A+W Defect Optimizers.


                                         Additional information
                                          For more information on A+W Defect Optimizer please refer to the appropriate do-
                                           cumentation.
3.30 / 01-2023




                 J-50                                                                           A+W Realtime Optimizer
                 Tutorial                                                                     Interplay with Other Modules




                                          A+W DynOpt Compact
                                          A+W DynOpt Compact is the entry level solution of A+W for Dynamic Optimi-
                                          zations.
                                          The system is based on the A+W Realtime Optimizer and loads the batches,
                                          pre-optimized and sent by the prior production system A+W Production. These
                                          batch are resolved completely and re-optimized systematically and dynamical-
                                          ly. This method improves the yield and reduces the number of residue plates
                                          to be saved.
                                          You can consider A+W DynOpt Compact to be an automatic A+W Real-time
                                          Optimizer.
                                          A+W DynOpt Compact works with the following two modules:
                                          •   A+W DynOpt Compact Import
                                          •   A+W DynOpt Compact Optimization

                                          A+W DynOpt Compact Import
                                          During import, the batches released for A+W DynOpt Compact are converted
                                          into so-called Cluster. A cluster is a - initially random - production unit, e. g. a
                                          rack, a group of racks, or an individual lite.

                                          A+W DynOpt Compact Optimization
                                          After the import, the processing sequence for the clusters is defined conside-
                                          ring the available space. This more or less matches the production sequence;
                                          in special cases, clusters may be moved up in the sequence to improve the
                                          yield. You can use harp racks, A racks, or both.
                                          About half of the computed clusters become primary clusters and the rest, se-
                                          condary clusters. Primary clusters get priority 1 and are completely optimised
                                          in the optimization on hand. Secondary clusters are used as fillers; the optimi-
                                          zation itself decides whether or not they are required.
                                          Example:
                                          Available space: 6. The space for a harp rack is 1, the space for an A rack 0,5
                                          (in terms of harp racks, i.e. 1 harp rack = 2 A racks.
                                          If there are as many harp racks as there are A racks and the splitting is applied
                                          to the clusters, this means: 4 harp racks plus 4 x 0,5 A racks = 6. Half of the
                                          numbers each means: two primary and two secondary harp racks and A racks.

                                                           Imported          Used             Primary           Secondary

                                          Harp rack        16                4                2                 2

                                          A Rack           17                4                2                 2

                                          Tab. J-1      Example

                                          The following conditions are kept when calculating the time-line:
3.30 / 01-2023




                                          •   The primary sorting of clusters is the production sequence.
                                          •   As long as clusters from the current batch can fill the available space, no
                                              clusters of the following batch will be used to create the time-line.

                 A+W Realtime Optimizer                                                                                  J-51
                 Interplay with Other Modules                                                                             Tutorial




                                         •      If the secondary clusters include a glass type that does not appear in the
                                                primary clusters, there are two options:
                                                – If the cluster consists of lites of a glass type for which there are primary
                                                     lites as well, only those will be optimized. The lites of the glass type that
                                                     does not appear in the primary clusters, will be optimized when the clus-
                                                     ter becomes primary.
                                                – If the cluster consists only of lites of a glass type that does not appear
                                                     in the primary clusters, the system searches the present batch for an al-
                                                     ternative cluster which consists (at least partly) of lites of a primary glass
                                                     type. If this can be found, the clusters will be exchanged; otherwise, the
                                                     present cluster will not be included in the optimization.
                                         Every step of A+W DynOpt Compact provides all primary and all secondary
                                         clusters for optimization. The primary lites will always be used for optimization
                                         and the secondary only if required. After this step, all primary clusters have
                                         been filled and can be replaced by secondary clusters or even new ones. Pro-
                                         cessing of several clusters looks as follows:

                                         Create A+W DynOpt Compact Batch
                                         There are two ways of creating A+W DynOpt Compact batches.
                                         •      Creating A+W DynOpt Compact batches in the cluster view
                                         •      Creating a A+W DynOpt Compact batch at cutting


                                          Creating A+W DynOpt Compact batches in the cluster view
                                         1 Open the dialog Cluster view.
                                           Select Cutting > A+W DynOpt Compact.
                                         2 On the left side, select the batch(es) you want to use to create an A+W Dy-
                                           nOpt Compact batch.
                                         3 Open the context menu and select Create A+W DynOpt Compact batch.
                                         4 After the A+W DynOpt Compact batches have been created, they are di-
                                           splayed in the top left section of the dialog. They are headed by +. If you
                                           open up the tree, you can view the rack data for the batches.


                                          Creating a A+W DynOpt Compact batch at cutting
                                         1 Open dialog Select a batch.
                                           Select either Cutting > Cut optimization or use the corresponding icon.
                                         2 From the batch list, select the batch you want to use to create an A+W Dy-
                                           nOpt Compact batch.
                                         3 Open the context menu and select Create A+W DynOpt Compact for batch
                                           XXXX.
                                         4 When the A+W DynOpt Compact batch has been created, it appears in the
                                           top left section of the dialog, marked by Cut&Go. Tag the batch in the left
                                           section to display the appropriate information in section Optimizations.
3.30 / 01-2023




                 J-52                                                                                 A+W Realtime Optimizer
                 Tutorial                                                                   Interplay with Other Modules




                                             Requirements
                                             The production system A+W Production as well as the A+W Realtime Op-
                                             timizer are prerequisites to use the A+W DynOpt Compact.


                                          Additional information
                                           For more information on A+W DynOpt Compact please refer to the appropriate do-
                                            cumentation.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-53
                 Interplay with Other Modules                  Tutorial
3.30 / 01-2023




                 J-54                           A+W Realtime Optimizer
A+W Realtime Optimizer          J

                 Software Reference




                A+W Production
                 Software Reference                                                                                Overview




                                          Overview
                                          The following chapter describes all dialogs available in A+W Realtime Optimi-
                                          zer. Depending on the program version, some dialogs or fields in the dialogs
                                          are invisible. The following versions are possible:
                                          •   A+W Realtime Optimizer integrated in the A+W Production environment.
                                          •   A+W Realtime Optimizer integrated in A+W Production environment toge-
                                              ther with a ReMaster dispenser.
                                          •   A+W Realtime Optimizer stand alone.
                                          The description of the individual dialogs shows if an information applies only
                                          to a certain version.


                                          Menus
                                          The following menus appear after starting A+W Realtime Optimizer:




                                          A When starting A+W Realtime Opt.
                                          Fig. J-11    Menu of A+W Realtime Optimizer


                                          The menus contain functions, sub-menus, and dialogs. The following table de-
                                          scribes the functions and lists the sub-menus and dialogs. Description of the
                                          dialogs in the following chapters is sorted by menu.


                                          Icons
                                          Some dialogs can be directly loaded via icons:

                                          Icon          Dialog/Function

                                                        Opens the dialog “Rush Orders” auf Seite J-58

                                                        Opens the dialog “Select Glass for Optimization” auf Seite J-68

                                                        Opens the dialog “Select a Batch” auf Seite J-86

                                                        Opens the dialog “Rejects Pool” auf Seite J-99

                                                        Opens the dialog “Error Reports” auf Seite J-110

                                                        Opens the dialog “Import” auf Seite J-109
3.30 / 01-2023




                                          Tab. J-2     Icons and their function




                 A+W Realtime Optimizer                                                                                   J-57
                 Input                                                                Software Reference




                         Input
                         Open menu Input
                         The Input menu offers the following options:
                         •   Rush order lites
                             This menu allows to enter rush order lites directly in A+W Realtime Optimi-
                             zer.
                              Software Reference, “Input of Rush Order Lites” on page J-60
                         •   Manual plan
                             This menu allows to create a purele manual plan and save it as table opti-
                             mization in the database.
                              Software Reference, “Manual Plan Input” on page J-64
                         •   Master data
                             This menu gives access to the master data. These are described in detail
                             in A+W Production manual.


                         Rush Orders
                         Input > Rush order lites




                         Fig. J-12     Rush order lites


                         Rush order lites can be integrated in table optimizations. This dialog shows all
                         the entered rush order lites. The combo box for field Table allows to view the
                         rush orders per table, or for all tables. For details on rush order lites, please
                         refer to section Detailed scheduling.

                         Description of fields

                         Glass type Shows the product number of the glass type. The value is adop-
                         ted from field Glass type in dialog Enter rush order lites.
3.30 / 01-2023




                         Thickness Shows the thickness of the glass type. The value is adopted from
                         field Thickness in dialog Enter rush orders.



                 J-58                                                          A+W Realtime Optimizer
                 Software Reference                                                                                    Input




                                          Rack This field shows the rack number. The value is adopted from field Rack
                                          in dialog Enter rush orders.

                                          Quantity This field shows the number of rush order lites. The value is taken
                                          from field Quantity in dialog Enter rush order lites.

                                          Shape If the rush order is a shape, this field shows the shape number. 0
                                          stands for "no shape". The value is adopted from field Shape in dialog Enter
                                          rush order lites.

                                          Width This field shows the width of the rush order. The value is taken from
                                          field Width in dialog Enter rush order lites.

                                          Height Shows the height of the rush order. The value is adopted from field
                                          Height in dialog Enter rush order lites.

                                          Priority Shows the priority of the rush order. Default priority is 0

                                          All stations This checkbox defines the rush order lites to be displayed. Usu-
                                          ally, only those rush order lites will be displayed that were entered at this par-
                                          ticular terminal in order to edit or delete them. This prevents other terminals
                                          from changing or deleting those records. If you want to see all the rush order
                                          lites existing in the database, you can activate this checkbox. Rush order lites
                                          entered at other terminals appear in a different color in the information window
                                          below the checkbox All terminals.
                                           All entered rush order lites are displayed even those entered at other termi-
                                          nals.
                                           You will see only the rush order lites entered at this particular terminal.
                                          Technical info: Database field: FEIN_TEILE:STATIONID

                                          Table The combo box shows all cutting tables defined. This allows you to all-
                                          ocate rush order lites to a certain cutting table. Option All tables shows all rush
                                          order lites entered. If you tag a record on the list, the grey area below the
                                          checkbox All terminals shows the table on which the rush order lite is to be cut.

                                          Description of buttons

                                          Add Use this button to open the dialog Enter rush orders.

                                          Process Use this button to open the dialog Enter rush orders for the tagged
                                          record.

                                          Delete This button serves to delete the tagged rush order lite. This produces
                                          a security check. After this, the entry will be deleted.


                                          Additional information
                                           Tutorial, “Rejects, Rush Order Lites or Filler Orders” on page J-20
                                           Software Reference, “Shape No.” on page J-60
3.30 / 01-2023




                                           Software Reference, “Input of Rush Order Lites” on page J-60




                 A+W Realtime Optimizer                                                                                J-59
                 Input                                                                Software Reference




                         Input of Rush Order Lites
                         Input > Rush order lites > [Add]




                         Fig. J-13    Rush order lites


                         This dialog allows to enter rush orders. For details on rush order lites, please
                         refer to section Detailed scheduling.
                         Technical info: Database table: FEIN_TEILE

                         Description of fields

                         Glass type The combo box shows all defined glass products. Select the re-
                         quired glass type from the combo box. Glass types are defined in master data.
                         Technical info: compulsory field, database field: POOL_TEILE:GLASART

                         Thickness The combo box shows all thicknesses defined for the glass type
                         selected in field Glass type. Select the required thickness from the combo box.
                         Thicknesses are defined in master data.
                         Technical info: compulsory field, database field: POOL_TEILE:DICKE

                         Rack Enter the number of the rack onto which the rush order shall be put.
                         Racks are defined in master data.
                         Technical info: Compulsory field, 4 digit, database field: FEIN_TEILE:BOCK

                         Quantity. Enter the number of rush order lites.
                         Technical info: compulsory field, database field: FEIN_TEILE:MENGE

                         Shape No. If the rush order is a shape, enter the appropriate shape number
                         (acc. to shape catalog). When you enter the shape number and leave the field,
                         the dialog Shape input appears automatically.
                         Technical info: compulsory field, database field: POOL_MODELL:MO-
                         DELL_NR

                         Width Enter the width of the rush order lite. If it is a shape, enter the width of
                         the surrounding rectangle.
3.30 / 01-2023




                         Technical info: compulsory field, database field: POOL_MODELL:BREITE




                 J-60                                                           A+W Realtime Optimizer
                 Software Reference                                                                                    Input




                                          Height Enter the height of the rush order lite. If it is a shape, enter the height
                                          of the surrounding rectangle.
                                          Technical info: compulsory field, database field: POOL_ MODELL:HOEHE

                                          Description of buttons

                                          Magnifier Use this button to open the dialog Input of shapes.


                                          Additional information
                                           Software Reference, “Input of Shapes” on page J-62
                                           Tutorial, “Rejects, Rush Order Lites or Filler Orders” on page J-20
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                J-61
                 Input                                                                     Software Reference




                         Input of Shapes
                         Input > Rush order lites > [Add] > [Magnifier]

                                         A         B



                                                                                           C

                                                                                           D




                         F




                                     E
                         A Input required per shape                 D Shape overview
                         B Shape numbers                            E Parameter list
                         C Graphic overview of shapes               F Input field
                         Fig. J-14    Input of shapes


                         This dialog is used to enter standard shapes. The selection is determined by
                         the shape catalog you are using. The required entries for the selected shapes
                         are shown in the top left window (A) in the dialog. Your entries immediately ap-
                         pear in the right window (D) of the dialog; the shape being shown proportional-
                         ly. The bottom window (E) shows the input parameters.
                         The values in front of the required input for the selected shape have the follo-
                         wing meanings:

                         Value        Explanation

                         W            Width of the shape. In case of several widths = W, W1, W2, etc.

                         H            Height of the shape. In case of several heights = H, H1, H2, etc.

                         T            Trim. In case of several trims = T, T1, T2, etc.

                         <-->         Reflection flag. Valid input: 0: Normal 1: Vertically reflected.
3.30 / 01-2023




                         @            Rotation flag. Valid input: 90: rotate by 90° 180: rotate by 180° 270:
                                      rotate by 270°.

                         Tab. J-3     Description of input values for the selected shape


                 J-62                                                               A+W Realtime Optimizer
                 Software Reference                                                                                     Input




                                          Additional information
                                           Software Reference, “Input of Shapes” on page J-62
                                           Tutorial, “Rejects, Rush Order Lites or Filler Orders” on page J-20



                                          Shape Number
                                          Input > Rush order lites > [Add] > [Magnifier] > [Magnifier]




                                          Fig. J-15     Shape number


                                          If you do not know the exact shape number and do not have a printout of the
                                          shape catalog at hand either, this dialog will give you an overview of the exis-
                                          ting shapes. The shape number highlighted in grey. The above screenshot
                                          shows shape number 1. When you have found the shape you are looking for,
                                          double-click on it on the list; it will automatically appear as the Field no. in di-
                                          alog Input of shapes.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                 J-63
                 Input                                                             Software Reference




                         Manual Plan Input
                         Input > Manual plan …




                         Fig. J-16    Manual plan input


                         This dialog allows to create a purele manual plan and save it as table optimi-
                         zation in the database. The manual plan can be edited and changed after-
                         wards. This is done by means of module PlanEdit. For details on this module,
                         please refer to the corresponding documentation. No barcode information will
                         be available for manual plans.

                         Description of fields in section Glass Type

                         Glass type This field shows the glass type. The value is loaded from master
                         data.

                         Thickness This field shows the thickness of the glass type. The value in this
                         field is adopted from master data.

                         Glass description This field shows a description of the glass type. The value
                         is loaded from master data.

                         Left trim Left edge of the stockplate (in mm) that cannot be optimized. The
                         input in this field is adopted from the master data.

                         Right trim Right edge of the stockplate (in mm) that cannot be optimized. The
                         input in this field is adopted from the master data.
3.30 / 01-2023




                         Top trim Top edge of the stockplate (in mm) that cannot be optimized. The
                         input in this field is adopted from the master data.



                 J-64                                                        A+W Realtime Optimizer
                 Software Reference                                                                                Input




                                          Bottom trim Bottom edge of the stockplate (in mm) that cannot be optimized.
                                          The input in this field is adopted from the master data.

                                          Description of fields in section Plan

                                          Batch This field shows the number of the batch in which the manual plan shall
                                          be cut.

                                          Locked This column defines whether and by which terminal the batch has
                                          been locked for processing or optimization.

                                          Glass type Shows the glass type for which the manual plan has been crea-
                                          ted.

                                          Thickness Shows the thickness of the glass type on the manual plan.

                                          Glass description Shows the name of the glass that has been added to the
                                          manual plan.

                                          Table Shows the table on which the manual plan shall be cut.

                                          Lite quantity Shows the number of lites contained in the manual plan.

                                          Lite sqft. Shows the surface of the lites (in sqm) contained in the manual
                                          plan.

                                          Stockplates Shows the number of stockplates required for the manual plan.

                                          Waste Shows the waste (in %) this manual plan will produce.

                                          Residue plate Shows the length of the residue plate that results from the ma-
                                          nual plan.

                                          Description of fields in section Stockplates

                                          Width Shows the width of the stockplate in mm or inch (configurable).

                                          Height Height of the stockplate in mm or inch (configurable).

                                          XY? This column defines the direction of the cross cut. Valid options:
                                          X: The cross cut must be vertical to the bottom edge of the plate.
                                          Y: The cross cut runs parallel with the bottom edge of the lite.
                                          ?: The optimization can choose one of the two directions for the cross cut.

                                          Quantity Shows the number of stockplates available.

                                          Description of fields in section Residue plate
3.30 / 01-2023




                                          Width If there is a residue plate with the appropriate combination of glass
                                          type/thickness, it can be used. Enter the width of the residue plate in mm.




                 A+W Realtime Optimizer                                                                            J-65
                 Input                                                            Software Reference




                         Height If there is a residue plate with the appropriate combination of glass
                         type/thickness, it can be used. Enter the height of the residue plate in mm.

                         Description of fields and buttons in the bottom section

                         Unnamed field This field shows the number of the batch in which the manual
                         plan shall be cut.

                         Table Shows the table on which the manual plan will be cut.

                         New Use this button to start module PlanEdit. For details on this module,
                         please refer to the corresponding documentation.

                         Edit This button is active when you have added a manual plan. You can use
                         this button to edit the plan.

                         Cutting Use this button to start the cutting process.


                         Additional information
                          Software Reference, “Parameter” on page J-79
3.30 / 01-2023




                 J-66                                                        A+W Realtime Optimizer
                 Software Reference                                                                               Input




                                          Charge Editor
                                          Input > Charges [F3]




                                          Fig. J-17    Charge editor


                                          This dialog allows to enter a charge number.

                                          Description of fields in section Stockplates

                                          Glass type This field shows the glass type. The value is loaded from master
                                          data.

                                          Thickness This field shows the thickness of this glass type in mm. The input
                                          in this field is loaded from master data in mm or inch (configurable)

                                          Width Shows the width of the stockplate in mm or inch (configurable).

                                          Height Height of the stockplate in mm or inch (configurable).

                                          Charge description This field shows the entered charge description.

                                          Glass description This field shows a description of the glass type.

                                          Description of fields in section charge description

                                          Checkbox Tag the checkbox and the entered charge number will be inherited
                                          to the following stockplates of the identical glass type/thickness.

                                          Field Enter the charge description in this field.


                                          Additional information
3.30 / 01-2023




                                           Software Reference, “Charge Editor” on page J-67




                 A+W Realtime Optimizer                                                                           J-67
                 Optimization                                                               Software Reference




                                Optimization
                                Open menu Optimization
                                The Optimization menu offers the following options:
                                •   Table optimization
                                    Use this menu to create a table optimization.
                                     Software Reference, “Select Glass for Optimization” on page J-68
                                •   Reset
                                    Use this menu to reset batches.
                                     Software Reference, “Resetting a Cutting Batch” on page J-81



                                Select Glass for Optimization
                                Optimization > Table optimization
                                There are two different variants of this dialog. Which variant is displayed de-
                                pends on which settings you have made for the table optimization:
                                •   Default
                                •   Production Date
                                 Chapter “Table Optimization” on page J-108


                                Table Optimization in the Default Variant




                                Fig. J-18     Select glass for optimization - default


                                In this dialog, A+W Realtime Optimizer lists all glass types for which there are
                                batches and rush order lites to be optimized. The available batches for the se-
                                lected glass type will be displayed.
3.30 / 01-2023




                 J-68                                                                   A+W Realtime Optimizer
                 Software Reference                                                                          Optimization




                                          Description of fields in section Available Glass Types

                                          Glass type Shows the article number of the glass type for which batches are
                                          available. The value is loaded from master data.

                                          Glass description This field shows a description of the glass type.

                                          Thickness Shows the thickness of the glass type. The value is loaded from
                                          master data.

                                          Residue warehouse This column only appears if A+W Realtime Optimizer
                                          has been configured to operate with a residue plate dispenser. This column
                                          shows an entry if the residue plate dispenser contains a lite of the required
                                          glass type and thickness. The number displayed is the length of the residue
                                          plate in mm found in the residue plate dispenser. If the dispenser contains se-
                                          veral residue plates of this glass type and thickness, the longest residue plate
                                          will be displayed.

                                          Reject quantity If reject has been entered for this glass type, this field shows
                                          the number of broken lites.

                                          Reject surface If reject has been entered for this glass type, this field shows
                                          the total surface of the reject.

                                          Rush order qty. If rush orders have been entered for this glass type, this field
                                          shows the number of lites.

                                          Rush order sqft. If rush orders have been entered for this glass type, this
                                          field shows the total surface.

                                          Description of fields in section Available Optimizations

                                          Batch This column shows the number of the batch containing optimizations
                                          for the selected glass type.

                                          Lot This column contains the number of the batch that includes optimizations
                                          for the selected glass type.

                                          Locked This column defines if and from which the terminal the batch has
                                          been locked for processing or optimization.

                                          Parameter This column shows the table for which the displayed batch has
                                          been optimized.

                                          Stockplates This column defines the number of stockplates required for op-
                                          timizing the batch.

                                          Lite quantity This column shows the number of lites included in the lot opti-
                                          mization.
3.30 / 01-2023




                                          Lite sqft. This column shows the square metres of glass included in the lot
                                          optimization.



                 A+W Realtime Optimizer                                                                              J-69
                 Optimization                                                            Software Reference




                                Waste Shows the waste in % resulting from the present batch optimization.

                                Residue (mm) Shows the length of the residue plate resulting from batch op-
                                timization on the cutting table.

                                Information This column displays the batch name.

                                Date In this column, you see the production date that was calculated during
                                batch creation by capacity planning.

                                Shift This column displays the production shift that was determined during
                                batch creation by capacity planning.

                                Description of checkbox

                                Permit manual cutting If this checkbox is tagged, the list Glass types also
                                shows the glass types for optimization that were defined in master data only
                                for manual cutting.
                                 Show only glass types for automatic cutting
                                 Show glass types for manual cutting as well
3.30 / 01-2023




                 J-70                                                              A+W Realtime Optimizer
                 Software Reference                                                                            Optimization




                                          Table Optimization in the Production Date Variant




                                          Fig. J-19     Select glass for optimization - Production Date


                                          This dialog displays the production dates and allows you to filter the optimiza-
                                          tions by production date. This makes it easier to meet deadlines and plan the
                                          production process.
                                          First, select a production date from the Production Date list.
                                          The Available Glass Types area shows all glass types that are included in op-
                                          timizations with the selected production date. Select the glass type you want
                                          to cut.
                                          The Available Optimizations area shows all optimizations that should be pro-
                                          duced by the selected production date. For a better overview, the optimizati-
                                          ons are marked in color:
                                          •   Green: The production date is in the future.
                                          •   Yellow: The production date is today.
                                          •   Red: The production date is in the past.
                                          The fields in the Available Glass Types and Available Optimizations areas are
                                          identical to the fields on the Table optimization in the default variant dialog and
                                          will be explained there.
                                           Chapter “Table Optimization in the Default Variant” on page J-68


                                          Additional information
                                           Tutorial, “Selecting Batches for Cutting” on page J-39
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                 J-71
                 Optimization                                                                Software Reference




                                Table Optimization Batch [No.]
                                This dialog serves to set various optimization parameters. The dialog is split
                                into the following tabs:
                                •   Overview
                                •   Optimize
                                •   Residue Plates and Stockplates
                                •   Parameter


                                Overview
                                Optimization > Table optimization > Select glass - [Select] > Overview




                                Fig. J-20    Table optimization - Overview


                                This dialog presents the batches selected in dialog Select Glass for Optimiza-
                                tion. If an optimization has been run, its results appears here. If no optimization
                                has been run so far, the fields Plates, Waste and Residue (mm) are empty.
                                After an optimization has been run, you can double-click on the glass type to
                                start PlanEdit if this is installed at your workstation. PlanEdit shows the break-
                                out pattern for the stockplate in graphic form.

                                Description of the list at the top

                                Glass type Shows the article numbers of the glass types included in the se-
                                lected table optimization. The value is loaded from master data.

                                Thickness This field shows the thickness of the glass type. The value is loa-
                                ded from master data in mm or inch (configurable).
3.30 / 01-2023




                                Parameter When an optimization has been run, the system shows the opti-
                                mization parameters applied.


                 J-72                                                                  A+W Realtime Optimizer
                 Software Reference                                                                         Optimization




                                          Quantity This field shows the number of lites.

                                          Sqft. This field shows the total surface for the optimized glass type in square
                                          metres.

                                          Stockplates Shows the number of stockplates required for optimization (only
                                          after optimization).

                                          Waste Shows the waste in % (only after optimization).

                                          Residue (mm) Shows the width of the residue plate (in mm) remaining on the
                                          table for further use (only after optimization).

                                          Description of the list at the bottom

                                          Batch This field shows the batch numbers that are included in the table opti-
                                          mization displayed.

                                          Lot Shows the number of lots that are included in the table optimization di-
                                          splayed.

                                          Cutting racks Shows the number of cutting racks scheduled for the lites of
                                          this batch.

                                          Special glass batch Defines whether this is a special glass batch. Special
                                          glass batches contain glass types that were defined in master data as special
                                          glass types. Valid options:
                                          • Yes
                                          • No

                                          Stockplates Shows the number of stockplates scheduled for cutting this
                                          batch. This is the result of Detailed scheduling, not table optimization.

                                          Waste Shows the waste in % for this batch. This is the result of Detailed
                                          scheduling, not table optimization.

                                          Residue (mm) This field shows the width of the residue plate (in mm) remai-
                                          ning on the table after cutting this batch that can be used further. This is the
                                          result of Detailed scheduling, not table optimization.


                                          Additional information
                                           Tutorial, “Create Table Optimizations” on page J-28
                                           Tutorial, “Cutting Table Optimizations” on page J-28
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-73
                 Optimization                                                                Software Reference




                                Optimize
                                Optimization > Table optimization > Select glass - [Select] > Optimize




                                Fig. J-21    Optimize


                                This dialog serves to enter the settings for optimization. The list provides infor-
                                mation on the selected glass type.

                                Description of fields in section Optimization Sequence

                                Batch This field shows the batch(es) to be optimized.

                                Lot Shows the number of lots of the individual batch.

                                Rank Shows the optimization rank. Press the buttons  or  to change the
                                rank. Identical ranks can be mixed, different separated.

                                Items Shows the number of items included in this batch.

                                A Racks This field shows the number of A racks required for this batch.

                                Harp rack Shows the number of harp racks required for this batch.

                                Lite quantity Number of lites included in this batch.

                                Lite sqft. This field shows the lite surface (in sqm) included in this batch.

                                Stockplates Shows the number of stockplates needed to cut this batch.
3.30 / 01-2023




                 J-74                                                                  A+W Realtime Optimizer
                 Software Reference                                                                           Optimization




                                          Description of buttons in section Sequence

                                          ˄ This button is used to change the rank.If you choose a batch with rank 1 for
                                          example and press ˄, the rank will change from 1 to 2. The sorting of the table
                                          may change as well.

                                          ˅ This button is used to change the rank. If you choose a batch with rank 1
                                          for example and press ˅, the rank will change from 2 to 1. The sorting of the
                                          table may change as well.

                                          Select This combo box controls the rank. The combo box consists of as many
                                          ranks as there are batches on the table. You can select a batch from the table,
                                          open the combo box and assign the selected batch the required rank. The
                                          ranks have to be assigned consecutively, i. e. you cannot skip a rank. Rank 1
                                          is followed by rank 2, then rank 3. Rank 2 cannot be skipped. If you assign a
                                          lower tank to a batch, sorting of the table will change.

                                          Description of fields in section Automatic Compilation

                                          Split lots This checkbox defines whether lots shall be split. Valid options:
                                           Lots will not be split.
                                           Lots will be split. Activating this checkbox may affect the field Rank.

                                          Split lots by maximum number of cutting racks This checkbox defines
                                          whether lots shall be split and if so, when this is done. If you want to split up
                                          lots after a certain number of cutting racks, enable the checkbox and enter in
                                          the following field the quantity after which the batch shall be split.

                                          Use minimum lite sqft. for splitting lots This checkbox defines whether
                                          lots shall be split and if so, when this is done. If you want to split lots from a
                                          certain lite surface (in sqm) upwards, enable the checkbox and enter in the fol-
                                          lowing field the surface after which the splitting shall be done.

                                             Splitting of lots
                                             Lots can be split either by the maximum number of cutting racks, or by mi-
                                             nimum lite surface. These two checkboxes cannot be active at the same
                                             time.

                                          Description of fields in section Batch Parameters

                                          XOPT-S This parameter needs to be set if you are working with A racks. The
                                          optimization then takes into account that the lites need to be set on A racks,
                                          maintaining a certain sequence for the following processings.

                                          Rejects This parameter defines that whenever there are rejects for the selec-
                                          ted glass type, it will be automatically included in the imminent optimization.

                                          Rush order lites Selecting this parameter means that you permit than whe-
3.30 / 01-2023




                                          never there are rush order lites for the selected glass type, these are automa-
                                          tically integrated in the upcoming optimization.




                 A+W Realtime Optimizer                                                                               J-75
                 Optimization                                                                   Software Reference




                                Filler only for gaps This parameter defines that should there be filler orders
                                for the same glass type, gaps in the optimization will be filled with filler orders.
                                The residue plate will not be filled up with filler orders. Existing filler orders for
                                a glass type are displayed on tab Filler.

                                Residue stock This checkbox only appears if you have got a residue plate
                                stock.
                                 The residue plate stock will not be used
                                 The residue plate stock will be used

                                Description of fields in section Table

                                Table The combo box shows all tables configured for your production. Select
                                the required table from the combo box. The section below shows the table na-
                                me.

                                Description of fields in section Optimization Parameters

                                Optimization parameters The combo box lists the optimization parameters
                                for creating the optimization. The system presents only parameters that can
                                be used by the selected table. Select the required table from the combo box.
                                The section below shows the parameter name.

                                Description of buttons

                                Optimize Use this button to start the optimization. The optimization is run in
                                the background. The results can be viewed in tab Overview as soon as they
                                are available. The optimization result will be saved in the database only if the
                                button [Save] or [Cut] is pressed.


                                Additional information
                                 Tutorial, “Cutting Table Optimizations” on page J-28
3.30 / 01-2023




                 J-76                                                                    A+W Realtime Optimizer
                 Software Reference                                                                             Optimization




                                          Residue Plates and Stockplates
                                          Optimization > Table optimization > Residue plates and stockplates




                                          Fig. J-22     Residue plates and stockplates


                                          This dialog serves to select for the previously selected glass type the residue
                                          plates and stockplates to be used for optimization. The selected glass type is
                                          shown on the left. The right side shows the suitable stockplate or, if available,
                                          the suitable residue plates.

                                          Description of fields in section List of Stockplates (right)

                                          Width Shows the width of the stockplate in mm.

                                          Height Shows the height of the stockplate in mm.

                                          XY? This column defines the direction of the cross cut. Valid options:
                                          • X: The cross cut must be vertical to the bottom edge of the plate.
                                          • Y: The cross cut runs parallel with the bottom edge of the lite.
                                          • ?: The optimization can choose one of the two directions for the cross cut.

                                          Residue plate slot This field shows where the stockplate can be found. If it
                                          says 'stock', the plate is a stockplate. If it shows a number, e. g. 2, the plate is
                                          a residue plate which can be found in slot number 2.

                                          Storing time / quantity If the plate is a residue plate, this field shows the
                                          date and time at which the plate was added to the residue plate stock. If it
                                          shows a number, e. g. 7670, this is a stockplate of which there are still 7670
                                          pieces on stock.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                  J-77
                 Optimization                                                              Software Reference




                                Description of fields in section Residue plates

                                Height/width If there is still a residue plate of the same glass type and thick-
                                ness from the last cutting, this can be used. Enter height and width of the re-
                                sidue plate. The optimization will use this residue plate first, before using a
                                new stockplate.

                                   Residue plate and lite from residue stock cannot be used at the same
                                   time!
                                   If you are already using a residue stock plate, you cannot use a residue pla-
                                   te in addition. If A+W Realtime Optimizer has been configured to work with
                                   a residue plate dispenser, use of residue stock plates can be switched on
                                   or off on tab Optimize via checkbox Use.


                                Additional information
                                 Tutorial, “Use Stored Residue Plates” on page J-48
                                 Tutorial, “Residue Dispenser” on page J-48
3.30 / 01-2023




                 J-78                                                                  A+W Realtime Optimizer
                 Software Reference                                                                            Optimization




                                          Parameter
                                          Optimization > Table optimization > Parameters




                                          Fig. J-23    Parameter


                                          This dialog serves to enter the parameter settings for table optimization. The
                                          list shows the available stockplates.

                                          Description of fields in section Coating

                                          None/top/bottom If the stockplate is coated, use the radio buttons to define
                                          if the coating is on top or at the bottom. If the stockplate is not coated, enable
                                          radio button None.

                                          Description of the button

                                          Number of Use this button to open dialog Number of stockplates.

                                          Description of fields in section Optimization Parameters

                                          Trim The fields left trim, right trim, top trim and bottom trim show the trim ent-
                                          ered for this glass product. The grey fields refer to the values taken from the
                                          glass product master data. The values in the white fields can be overridden.
                                          This is just a temporary change of trim for the batch on hand.

                                          Auto subplate This checkbox defines whether the defined, maximum sub-
                                          plate width can be extended.
                                           The maximum subplate width can be extended.
                                           The maximum subplate width cannot be extended.
3.30 / 01-2023




                                          Max. subplate Field Max. subplate refers to the maximum subplate width for
                                          the selected glass product. The grey field refers to the values taken from the



                 A+W Realtime Optimizer                                                                                J-79
                 Optimization                                                                Software Reference




                                glass product master data. This entry can be changed in the white field. This
                                means a temporary change of the maximum subplate width for the correspon-
                                ding batch.

                                Cutting Mode This field defines the cutting mode for the XOPT(S) optimiza-
                                tions. The radio button shows the cutting mode used for detailed scheduling.
                                Selection of the appropriate cutting mode depends on the cutting table and the
                                company's requirements. Generally, cutting mode 1 will produce the best yield
                                while cutting mode 4 shows the worst results. Higher waste might be compen-
                                sated by quicker breakout and stacking (due to the simpler cutting mode). The
                                cutting mode determines the position of the lites on the subplate between two
                                adjacent Y cuts.
                                • 1: Between two Y cuts, lites of different width and height can lie next to an-
                                    other. Hence, W cuts may occur.
                                • 2: Between two Y cuts, only lites of different width and the same height can
                                    lie next to another.
                                • 3: Between two Y cuts, only lites of the same item can lie next to another.
                                • 4: Between two Y cuts, only up to two lites of the same item can lie next to
                                    another.
                                • 5-7: Special mode for Coopmes tables. This mode is identical with modes
                                    2-4.

                                Description of buttons

                                PlanEdit This button will be active after an optimization has been run. Use
                                this button to open the program PlanEdit.

                                Cutting This button will be active after an optimization has been run. Use this
                                button to start cutting.


                                More information on parameters
                                 Software Reference, “Number of Stockplates” on page J-81
3.30 / 01-2023




                 J-80                                                                A+W Realtime Optimizer
                 Software Reference                                                                        Optimization




                                          Number of Stockplates
                                          Optimization > Table optimization > Parameters > [Quantity]




                                          Fig. J-24    Number of Stockplates


                                          This dialog shows the number of stockplates available for the selected glass
                                          type.


                                          Resetting a Cutting Batch
                                          Optimization > Reset …




                                          Fig. J-25    Resetting a cutting batch


                                          This dialog allows to reset batches already started or produced, to be proces-
                                          sed again. Saved table optimizations can be resolved. Produced batches that
                                          have not been booked yet, can be booked as produced. Delete routines for old
                                          (produced) batches are taken over by the ALCIMServer. Please refer to the
                                          documentation for information on the deletion of batches.

                                          Description of the Batch List

                                          Batch Shows the numbers of the batches the status of which can be chan-
                                          ged. Numbers 1000 - 9999 represent completely optimized batches (e. g. from
                                          A+W Production) ready for cutting. Numbers 15000 - 15999 (number range
                                          can be configured) are reserved for self-created table optimizations.
3.30 / 01-2023




                                          Locked There is an entry in this column if another A+W Realtime Optimizer
                                          or another process is currently handling this batch.




                 A+W Realtime Optimizer                                                                           J-81
                 Optimization                                                                 Software Reference




                                Status Shows the processing status of the individual batches. The options
                                are:

                                   Status              Meaning

                                   Released            An optimization has been released for cutting. These
                                                       batches can be processed by a table optimization prior to
                                                       cutting.

                                   Started             Processing of the batch has been started. Lots of this
                                                       batch are already being cut, or optimized locally. This
                                                       status appears even if a table optimization was not cut but
                                                       was resolved.

                                   Produced            Batch has been produced.

                                   Tab. J-4      Status of batches

                                Description of buttons

                                Produced If a released batch is tagged and this button is selected, the batch
                                is marked as produced, and is no longer available for optimization.

                                OK If a released table optimization (batch from no. 15000) (configurable) is
                                tagged, and this button is selected, the table optimization will be resolved. The
                                included batches, rejects, rush or filler orders are available for new optimizati-
                                ons. Execution of this function is preceded by a security check.
                                If a produced batch is tagged, and this button is selected, the batch is reset
                                and can be produced again.


                                Additional information
                                 Tutorial, “Reset Cutting Status” on page J-46
3.30 / 01-2023




                 J-82                                                                   A+W Realtime Optimizer
                 Software Reference                                                                           Optimization




                                          Pausing Glass Types
                                          Optimization > DynOpt Settings




                                          Fig. J-26    Pausing glass types


                                          If a batch is imported into DynOpt, it has to be ensured that there are enough
                                          plates of this glass type in stock. You may never import a batch that includes
                                          the missing glass types.
                                          Sometimes, however, it happens that you only determine during production
                                          that some glass types are not available. With this dialog, you now have the op-
                                          portunity to lock individual glass types or remove them from production. The
                                          dialog shows you all glass types that are in production.

                                          Explanatin of the individual fields

                                          Filter With this combo box, you can restrict the list of glass types. The follo-
                                          wing values are available:
                                          • All: all glass types are displayed that are in production.
                                          • Locked: only locked glass types are displayed.
                                          • Urgent: only urgent glass types are listed. Urgent refers to such lites of this
                                              glass type that are waiting by the DynOpt exit lines.
3.30 / 01-2023




                                          Exit This combo box is only active if you have selected the Urgent setting on
                                          the combo box. Here you have the possibility to display the urgent glass types
                                          per exit. To do this, the exits have to be configured appropriately.



                 A+W Realtime Optimizer                                                                               J-83
                 Optimization                                                              Software Reference




                                Reason for pausing To lock a glass type, mark it and select the reason from
                                the combo box.

                                Stop optimization Use this button to stop the optimization. This is necessary
                                if you would like to remove a glass type completely from production. To do this,
                                you first have to stop the optimization and then remove the glass type.

                                Remove This button is only active if you have stopped the optimization for a
                                glass type. Then you can remove the glass type.

                                Lock Use this button to lock a glass type for the next optimization process.
                                First select the glass type, then the reason, then click [Lock].

                                Release Use this button to release a locked glass type. First select the glass
                                type and then click [Release].

                                Overview Use this button to open the Currently changed settings dialog with
                                an overview of the current settings.

                                Dissolve This button is only active if the production is active. Then you can
                                use this button to force a new DynOpt optimization.

                                Apply Use this button to confirm the actions. Ex: You have locked a glass ty-
                                pe, then click [Apply] to complete the action.
3.30 / 01-2023




                 J-84                                                                A+W Realtime Optimizer
                 Software Reference                                                                          Optimization




                                          Currently Changed Settings
                                          Optimization > DynOpt Settings > [Overview]




                                          Fig. J-27     Currently changed settings - overview


                                          This dialog provides a summary view of the settings for the tabs
                                          •   General
                                          •   Entries
                                          •   Exits
                                          •   Buffer
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-85
                 Cutting                                                               Software Reference




                           Cutting
                           Open menu Cutting
                           The Cutting menu offers the following options:
                           •   Cut optimization
                               Use this menu to cut a batch.
                                Software Reference, “Select a Batch” on page J-86
                           •   Reject pool
                               Use this menu to access the reject pool.
                                Software Reference, “Rejects Pool” on page J-99
                           •   Panorama
                               Use this menu to get access to Panorama (optional)


                           Select a Batch
                           Cutting > Cut optimization




                           Fig. J-28    Select a batch


                           This dialog is used to select one of the batches available. Select one or all op-
                           timizations from the selected batch. These optimizations are prepared for cut-
                           ting.

                           Description of the Batch List

                           Batch Shows the numbers of the batches the status of which can be chan-
                           ged. Numbers 1000 - 9999 represent completely optimized batches (e. g. from
3.30 / 01-2023




                           A+W Production) ready for cutting. Numbers 15000 - 15999 (number range
                           can be configured) are reserved for self-created local optimizations. If the term
                           DynOpt Compact appears at this point, this is an DynOpt Compact batch.


                 J-86                                                              A+W Realtime Optimizer
                 Software Reference                                                                                  Cutting




                                          Status Shows the processing status of the individual batches. The options
                                          are:

                                             Status             Meaning

                                             Released           An optimization has been released for cutting. These
                                                                batches can be processed by a table optimization prior to
                                                                cutting, or can be cut directly.

                                             Started            Processing of the batch has been started. Lots of this
                                                                batch are already being cut, or optimized locally. This
                                                                status appears even if a table optimization was not cut but
                                                                was resolved.

                                             Produced           Batch has been produced.

                                             Tab. J-5     Status of batches

                                          Information This column displays the batch name.

                                          Date In this column, you see the production date that was calculated during
                                          batch creation by capacity planning.

                                          Shift This column displays the production shift that was determined during
                                          batch creation by capacity planning.

                                             Change sorting
                                             By clicking on the column headers you can sort the list contents in ascen-
                                             ding or descending order.

                                          Description of list Optimization

                                          No. Batch number of the optimizations included in this batch.

                                          Status Shows the processing status of the individual batches.

                                          Glass type Article number of the glass type included in this optimization. The
                                          value is loaded from master data.

                                          Thickness Thickness of the glass type included in this optimization. The va-
                                          lue is loaded from master data.

                                          Glass description Shows the name of the glass type. The value is loaded
                                          from master data.

                                          Parameter Name of the table for which the optimization has been created.
                                          The value is loaded from master data.

                                          Stockplates Number of stockplates needed for this optimization.

                                          Waste Percentage of waste for this optimization.
3.30 / 01-2023




                                          Residue (mm) Length of the residue plate remaining after optimization.



                 A+W Realtime Optimizer                                                                                 J-87
                 Cutting                                                                 Software Reference




                           Description of fields

                           Old batches Tick this checkbox to display even the batches that have alrea-
                           dy been produced, and still have got the status Produced.
                            do not show batches of status Produced.
                            show only batches of status Produced.

                           Hide optimizations already cut When you tag this checkbox, the system hi-
                           des the optimizations that were already cut.
                            Show optimizations already cut.
                            Hide optimizations already cut.

                           Re-optimization Use this combo box to control re-optimizations. Possible va-
                           lues are:
                           • No: there is no re-optimization.
                           • Yes: there is a re-optimization without user intervention. If an optimization
                                that was not optimized for the configured table is transferred to cutting, then
                                a table optimization is created automatically without dialog display and in-
                                serted into the cutting process instead of the original optimization.
                           • Table optimization: Re-optimization with display of the Table optimization
                                dialog. If an optimization that was not optimized for the configured table is
                                transferred to cutting, then the Table optimization dialog is started. Here,
                                the optimization parameters such as edge cuts and cutting mode can be
                                changed. After the optimization has been done, the optimization can be di-
                                scarded or transferred to the cutting process with the [Cutting] button. If the
                                optimization is discarded, you have the opportunity to cut the original opti-
                                mization or to skip the optimization.
                           If the optimization was transferred to cutting accidentally, the cutting can be
                           ended and the table optimization dissolved. After that, the original optimization
                           is again available for the cutting.

                           Combo boxes The upper combo box marks the machine status. Possible va-
                           lues are:
                           • Ready: Cutting table is ready for work.
                           • Off: Cutting table is not ready for work (e.g. break).
                           Use the lower combobox to decide which batches shall be displayed. Possible
                           values are:
                           • Batches for the own table: Displays cutting batches for the own table only.
                           • Batches for alternative tables: Displays cutting batches also for alternative
                              tables.
                           • Batches for all tables: Displays batches for all cutting tables.

                           Select table The combo box can be used to restrict the display. The combo
                           box shows all cutting tables defined. You can define whether optimization bat-
                           ches of all tables shall be shown, or only those optimized for the table configu-
                           red in your A+W Realtime Optimizer installation. If A+W Realtime Optimizer
                           has been configured for "Table 9 logic", you can also choose Alternative ta-
3.30 / 01-2023




                           bles.




                 J-88                                                              A+W Realtime Optimizer
                 Software Reference                                                                                Cutting




                                          Description of buttons

                                          Options Use this button to create cutting data out of the optimization data,
                                          and transfer these to the cutting table. Cutting is started at the connected cut-
                                          ting table. The button changes to STOP.

                                          Sort This button will be active for a batch with more than one optimization on-
                                          ly. By pressing this icon the dialog Optimization sequence opens.

                                          Cut Use this button to open the dialog Cutting overview.


                                          Additional information
                                           Tutorial, “Selecting Batches for Cutting” on page J-39
                                           Tutorial, “Cutting Table Control” on page J-36
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                              J-89
                 Cutting                                                                Software Reference




                           Batch [number] - Batch [number]
                           Cutting > Cut optimization … > [OK]




                           Fig. J-29    Batch nnn - Batch mmm


                           This dialog shows batches and lots selected in dialog Select a Batch for cut-
                           ting.

                           Description of the List of Optimizations
                            Software Reference, “Description of list Optimization” on page J-87

                           Description of the Pattern List

                           No. Consecutive numbering of stockplates used in this optimization. Num-
                           bers correspond to the cutting sequence.

                           Width This field shows the stockplate width in mm. The input in this field is
                           loaded from master data.

                           Height This field shows the stockplate height in mm. The input in this field is
                           loaded from master data.

                           Opt Gr. Shows which optimization groups fill the stockplate with lites. Only
                           two groups per stockplate are valid. An optimization group may be a batch or
                           a re-optimization.

                           Status Shows the status of the individual stockplates of the optimization. The
                           following statuses are valid:
3.30 / 01-2023




                 J-90                                                              A+W Realtime Optimizer
                 Software Reference                                                                                         Cutting




                                          Status               Meaning

                                          Sent                 Cutting code was created.

                                          Skip                 No cutting code will be created for this stockplate, and no
                                                               breakout pattern will be supplied.

                                          Do not send          No cutting code will be created for this stockplate, but a
                                          cutting code         breakout pattern will be supplied.

                                          Cut                  This status is set when the cutting table has received or
                                                               picked up the cutting code (serial link or via network). The
                                                               system does not check whether the lite was actually cut.

                                          Tab. J-6       Status of batches

                                          Description of buttons

                                          Table - START Use this button to create cutting data out of the optimization
                                          data, and transfer these to the cutting table. Cutting is started at the connected
                                          cutting table. The button changes to STOP.

                                          Table - STOP Press this button to stop the transfer of cutting data to the cut-
                                          ting table. The cutting table finishes cutting the started stockplate. The button
                                          changes to START.

                                          Pattern - sequence Use this button to open the dialog Optimization Sequen-
                                          ce.

                                          Pattern - options Use this button to open the dialog Batch: Number.

                                          XTV - stop This button serves to stop the communication. The previous cut-
                                          ting pattern remains.

                                          XTV - << This button scrolls back the breakout display in the connected XTV.

                                          Close This button closes the dialog. This is possible only if the system cur-
                                          rently creates no cutting code. If cutting code creation is under way, use
                                          [STOP] first to stop it.


                                          Additional information
                                           Software Reference, “Optimization Sequence” on page J-92
                                           Software Reference, “Batch: Number” on page J-93
                                           Tutorial, “Check and Process Table Optimization Result” on page J-30
                                           Tutorial, “Cutting Table Optimizations” on page J-28
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                                       J-91
                 Cutting                                                             Software Reference




                           Optimization Sequence
                           Cutting > Cut Optimization > Select Optimization > [Sorting]




                           Fig. J-30    Optimization sequence


                           If the selected batch contains several glass types to be optimized, this dialog
                           shows the scheduled cutting sequence for these glass types. To change the
                           sequence use the arrow keys.

                           Description of fields

                           Status Shows the status of the optimization.

                           Glass type Shows the product number for the glass type. The value is loaded
                           from master data.

                           Thickness This field shows the thickness of this glass type in mm. The input
                           in this field is loaded from master data.

                           Glass name This field shows the name of the glass type. The value is loaded
                           from master data.

                           Parameter Shows the cutting table on which the optimization shall be cut.

                           Stockplates Shows the number of stockplates used for optimisation.

                           Waste Shows the optimization waste.

                           Rest Shows the residue plate.
3.30 / 01-2023




                 J-92                                                           A+W Realtime Optimizer
                 Software Reference                                                                               Cutting




                                          Batch: Number
                                          Cutting > Cut Optimization> Select Optimization > [Options]




                                          Fig. J-31    Batch: number


                                          This dialog defines what may or shall happen to the rejects and residue plates
                                          of each glass type of the selected optimization.

                                          Description of the Optimization List

                                          Lot Batch number of the displayed glass type within the optimization.

                                          Glass type Shows the product number for the glass type. The value is loaded
                                          from master data.

                                          Thickness This field shows the thickness of this glass type in mm. The input
                                          in this field is loaded from master data.

                                          Glass description This field shows the name of the glass type. The value is
                                          loaded from master data.

                                          Parameter Shows the cutting table the optimization is meant for.

                                          Stockplates Number of stockplates required to cut this batch.

                                          Waste Percentage of waste for this optimization.
3.30 / 01-2023




                                          Residue (mm) Length of the residue plate remaining after optimization.




                 A+W Realtime Optimizer                                                                             J-93
                 Cutting                                                                   Software Reference




                           Description of the Stockplate List

                           No. Number of the stockplate which is needed for the optimization tagged on
                           the Optimizations list.

                           Width This field shows the stockplate width in mm. The input in this field is
                           loaded from master data.

                           Height This field shows the stockplate height in mm. The input in this field is
                           loaded from master data.

                           Opt Gr. Shows which optimisation groups fill the stockplate with lites. Only
                           two groups per stockplate are valid. An optimization group may be a batch or
                           a re-optimization.

                           Cutting status Shows the cutting status of the individual stockplates of the
                           optimization. The following statuses are valid:

                              Status               Meaning

                              Sent                 Cutting code was created.

                              Skip                 No cutting code will be created for this stockplate, and no
                                                   breakout pattern will be supplied.

                              Do not send          No cutting code will be created for this stockplate, but a
                              cutting code         breakout pattern will be supplied.

                              Cut                  This status is set when the cutting table has received or
                                                   picked up the cutting code (serial link or via network). The
                                                   system does not check whether the lite was actually cut.

                              Tab. J-7       Cutting status of batches

                           Description of fields in section Rejects

                           Optimize rejects Here you specify the way A+W Realtime Optimizer shall
                           handle rejects transferred to cutting. The following settings are possible:
                           • No: no re-optimization,
                           • Separate: The new re-optimization was added at the end of the existing op-
                              timisation. This results in a cross cut between the existing optimization and
                              the new part.
                           • Mix: The previous stock plate will be re-optimized completely. This often re-
                              sults in a better yield.

                           Cut rejects by residue plate length This checkbox defines whether the bro-
                           ken lites shall be optimized with a new residue plate if the existing residue pla-
                           te does not suffice. If this checkbox is tagged, the entry in the following field is
                           important.
                            Do not start new stockplate to cut rejects.
3.30 / 01-2023




                            Start new stockplate if the new residue plate is smaller than the new residue
                           plate length defined in the following field, Length.




                 J-94                                                                A+W Realtime Optimizer
                 Software Reference                                                                               Cutting




                                          Cut residue plate below a length of This field is active only if the previous
                                          checkbox was tagged. Enter the maximum size for the new residue plate. No
                                          new residue plate will be started if reoptimization results in a bigger residue
                                          plate. Reject is collected in the reject pool.

                                          Description of fields in section Residue Plate Management

                                          Link Here you specify the way A+W Realtime Optimizer shall handle residue
                                          plates. The following settings are possible:
                                          • No: no linking,
                                          • Separate: The new re-optimisation was added at the end of the existing op-
                                             timization. This results in a cross cut between the existing optimization and
                                             the new part.
                                          • Mix: The lites will be resolved on the residue plate and re.optimized toge-
                                             ther with the quantity to be optimized.

                                          Edit residue plate before cutting If this checkbox is ticked, the system will
                                          ask whether PlanEdit shall be started.

                                          Description of fields in section Quick Optimization

                                          Quick Optimization The following settings are possible:
                                          • Standard: In this mode, you can dissolve and re-optimize the pattern of a
                                            glass type for which no cutting code was transmitted during the cutting pro-
                                            cess. The idea is that for optimizations with many patterns, the broken lites
                                            are not only optimized on the last lite. The broken lites are placed in the
                                            new optimization at the start (without further user intervention)..
                                          • Expanded: In this mode, additional user inputs are required. The glass se-
                                            lection menu for the table optimization is called up automatically. There, ho-
                                            wever, only the glass type of the dissolved optimization is visible. Here you
                                            can add additional optimizations. Then the Table optimization dialog opens.
                                            There, you can change edges, etc. When the optimization is finished, the
                                            optimization can be transferred directly to the cutting process using the
                                            [Cut] button.

                                          Reload Use this setting to load a further batch. The following settings are pos-
                                          sible:
                                          • Manual: Reloading is done manually.
                                          • Requirement: The user gets a message as soon as the number of uncut
                                              patterns in A+W Realtime Optimizer falls below a defined threshold. The
                                              user can reject reloading, or select a new batch to be loaded from the se-
                                              lection.
                                          • Automatic: Reloading is done automatically.

                                          Description of fields in section Label Print

                                          Active Use this checkbox to enable or disable label printing.
3.30 / 01-2023




                                           Label printing is disabled.
                                           Label printing is enabled. You can print labels directly.




                 A+W Realtime Optimizer                                                                             J-95
                 Cutting                                                                Software Reference




                           Description of buttons

                           PlanEdit If you select this button, and module Plan Edit is installed on your
                           system, PlanEdit is started and gives a graphic display of the optimization.

                           Cutting Use this button to start the Cutting overview.

                           Description of the context menu
                           Click the right mouse key on a lite with status Cut to delete the status Cut and
                           allow to cut the lite again.
                           Click the right mouse key on a lite without a status to set the status Do not send
                           cutting code or Skip can be set for the selected lite.


                           Additional information
                            Tutorial, “Use Stored Residue Plates” on page J-48
                            Tutorial, “Residue Dispenser” on page J-48
3.30 / 01-2023




                 J-96                                                             A+W Realtime Optimizer
                 Software Reference                                                                               Cutting




                                          Select the Optimizations to be Linked
                                          Cutting > Cut optimization > Select Batch > [OK] > Dialog Active Batch: xxx
                                          opens > Select optimization > [Start]




                                          Fig. J-32    Select the optimizations to be linked


                                          The list Available optimizations shows all batches containing optimizations for
                                          the glass type and thickness selected from the Glass type list. The dialog
                                          header contains the selected batch, the lots, and the glass type. Select the
                                          batch to be linked with from the table and press [Use].

                                          Description of fields in section Selection Parameters and Residue
                                          Plate

                                          All tables This checkbox defines the optimizations to be displayed. If this
                                          checkbox is ticked optimizations for other tables will be displayed, too.

                                          Permit manual cutting If this checkbox is ticked, the list Available optimiza-
                                          tions shows even the glass types designed only for manual cutting in master
                                          data.

                                          Residue plate Shows the length of the residue plate resulting from the selec-
                                          ted optimization (dialog Active batch: xxx).
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                             J-97
                 Cutting                                                               Software Reference




                           Optimization Result
                           Cutting > Cut optimization > Select batch > [OK] > Dialog Active batch: xxx
                           being opened > Select optimization > [Start] > Select batch > [Link]




                           Fig. J-33     Optimization result


                           This dialog shows the optimization result after linking. It consists of two secti-
                           ons. Section New optimization after linking shows the result after linking. Sec-
                           tion Original optimization shows the result prior to/without linking.
                           The grey area above the buttons tells you what and which quantity has been
                           additionally optimized.

                           Description of buttons

                           Repeat Press this button to return to the selection for link optimization where
                           batches can be selected.
                            Software Reference, “Select the Optimizations to be Linked” on page J-97

                           Linking This button is used to confirm the result and start cutting of the opti-
                           mization.


                           Additional information
                            Tutorial, “Linking of Table Optimizations” on page J-33
3.30 / 01-2023




                 J-98                                                              A+W Realtime Optimizer
                 Software Reference                                                                               Cutting




                                          Rejects Pool
                                          Cutting > Rejects pool




                                          Fig. J-34    Rejects pool


                                          This dialog shows all lites entered as or reported broken. If glass type and
                                          thickness fit, lites from the rejects pool can be optimized once more in table
                                          optimizations or reoptimization.

                                          Description of the Rejects List

                                          Glass type Shows the product number for the glass type. The value is loaded
                                          from master data.

                                          Description This field shows the name of the glass type. The value is loaded
                                          from master data.

                                          Thickness This field shows the thickness of this glass type in mm. The input
                                          in this field is loaded from master data.

                                          Width This field shows the stockplate width in mm. The input in this field is
                                          loaded from master data.

                                          Height This field shows the stockplate height in mm. The input in this field is
                                          loaded from master data.
3.30 / 01-2023




                                          Batch Shows the batch number the lites originally belonged to.




                 A+W Realtime Optimizer                                                                             J-99
                 Cutting                                                                  Software Reference




                           DynOpt This field allows you to set a DynOpt flag for individual broken lites,
                           so that they can be reoptimized by DynOpt. To do this, select the correspon-
                           ding lite(s) and then click on the DynOpt button. Only lites for which no blo-
                           cking station is entered can be selected.

                           Customer Shows the name of the customer the broken lite belongs to.

                           Order Shows the number of the order the broken lite belongs to.

                           Itm Shows the item number of the order the broken lite belongs to.

                           Quantity Shows the number of lites.

                           ShapeNo If the broken lite is a shape, the shape number appears in this field.

                           Rack Number of the (harp) rack that would have held the lite were it not bro-
                           ken.

                           Label no. Label number of the broken lite.

                           Lot This field is used only for program-internal purposes and has no meaning.

                           Description of buttons

                           Update If more broken lites are reported (e. g. A+W Production Terminal
                           XTV) while you are using this dialog, these will be shown only after the dialog
                           display was updated by means of this button.

                           Delete Use this button to delete the tagged broken lite from the rejects pool.
                           You can tag and delete several lites at the same time. If you work with barco-
                           ding, you can also book the lites.

                           Shape info This button starts the shape display of A+W Production.

                           Printing This button starts a printout listing the contents of the rejects pool.
                           This button is available only if the system was configured accordingly.

                           Add This button opens the Reject input dialog.

                           Explanation of the combo box
                           With the combo box, you can select to which table the break that you want to
                           add should be booked.
                           If you open the breakage pool for the first time, by default the table is selected
                           on which the A+W Realtime Optimizer is attached.


                           Additional information
                            Tutorial, “Rejects, Rush Order Lites or Filler Orders” on page J-20
3.30 / 01-2023




                            Software Reference, “Input of Shapes” on page J-62
                            Software Reference, “Add Rejects” on page J-101




                 J-100                                                              A+W Realtime Optimizer
                 Software Reference                                                                                Cutting




                                           Add Rejects
                                           Cutting > Rejects pool > [Add]




                 Fig. J-35   Add rejects


                                           This dialog can be used to enter broken lites that shall be included in an opti-
                                           mization once more.

                                           Description of fields

                                           Order Enter the order number the broken lite belongs to.

                                           PItem Enter the item number of the order the broken lite belongs to.

                                           Reject reason Select the reject reason from this combo box. You can select
                                           only reject reasons defined in master data.

                                           Description of the Part list

                                           Ordno Order number the broken lite belongs to.

                                           PartNo Element number of the lite.

                                           Description This field shows the name of the glass type. The value is loaded
                                           from master data.

                                           Width Shows the width of the glass type in mm or inch (configurable).
3.30 / 01-2023




                                           Height Shows the height of the glass type in mm or inch (configurable).




                 A+W Realtime Optimizer                                                                             J-101
                 Cutting                                                                  Software Reference




                           Additional information
                            Tutorial, “Rejects, Rush Order Lites or Filler Orders” on page J-20



                           Input of Shapes
                           Cutting > Rejects pool > [Shape info]

                                            A          B



                                                                                          C

                                                                                          D



                           F




                                        E
                           A Input required per shape                D Shape overview
                           B Shape numbers                           E Parameter list
                           C Graphic overview of shapes              F Input field
                           Fig. J-36     Shape input


                           The fields and buttons in this dialog are the same as in dialog Shape input in
                           the rush order section. The dialog is described there.


                           Additional information
                            Software Reference, “Input of Shapes” on page J-62
3.30 / 01-2023




                 J-102                                                              A+W Realtime Optimizer
                 Software Reference                                                                                  Cutting




                                          A+W DynOpt Editor
                                          Cutting > DynOpt Compact …




                                          Fig. J-37    Editor


                                          On the left, the editor shows in section Released batches all batches from de-
                                          tailed planning that can be processed by DynOpt Compact.

                                          Description of fields in section Released batches

                                          Batch Shows the batch number from detailed scheduling.

                                          Text This field shows the name of the batch number.
                                          Section Imported batches contains already optimized or imported batches.
                                          Open the tree structure to view more information on the batch in question. The
                                          first level of the tree shows the batch number, the second contains the rack
                                          number while the third tells you the status, the number of lites, and the rack
                                          type. If you click on the second level (rack number) of the tree, the list Imported
                                          lites provides detailed information on the individual lites.
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                               J-103
                 Cutting                                                              Software Reference




                           Description of buttons

                           > Use this button to move a tagged batch from section Released batches to
                           section Imported batches.

                           < Use this button to move a tagged batch from section Imported batches back
                           to section Released batches.

                           ˄ This button is used to change the sequence. Select a batch in section Re-
                           leased batches and press ˄ to move it one slot upwards on the list.

                           ˅ This button is used to change the sequence. Select a batch in section Re-
                           leased batches and press ˅ to move the batch one position down on the list.

                           Description of fields in section Imported Lites

                           Batch Shows the batch number from detailed scheduling.

                           Batch sequence Shows the sequence of the rack. This is a serial number for
                           imported racks within a batch.

                           Serial No. This field lists, in ascending sequence, the serial number within the
                           batch.

                           Slot No. If the rack is a harp rack, this field shows the slot number. For A
                           racks, it shows 0.

                           Glass type Shows the product number of the glass type.

                           Thickness Shows the lite thickness in mm or inch (configurable).

                           Width Shows the lite width in mm or inch (configurable).

                           Height Shows the lite height in mm or inch (configurable).

                           Order This field shows the order number.

                           Itm Shows the item number of this order.

                           Status This field shows the status. For details, please see below.

                           DynOpt Compact batch Shows the batch number of DynOpt Compact opti-
                           mization.

                           DynOpt Compact lot Shows the lot number of the DynOpt Compact optimi-
                           zation.

                           DynOpt Compact pattern Number of the pattern the corresponding lite be-
                           longs to.
3.30 / 01-2023




                           Tag a batch in the bottom left section to view detailed information on the indi-
                           vidual lites in the window on the left.



                 J-104                                                          A+W Realtime Optimizer
                 Software Reference                                                                                 Cutting




                                          A time bar appears at the bottom of the dialog. Every colored rectangle marks
                                          the status of a rack.
                                          The following colors are valid:

                                          Color        Explanation

                                                       All lites of the rack have been cut.

                                                       All lites of the rack have been optimized.

                                                       Lites of the rack have been partly optimized.

                                                       Rack has not been optimized yet.

                                          Tab. J-8     Explanation of symbols

                                          The numbers below the colored rectangle indicate the batch and rack number.
                                          Example: 1187/9951 means: batch number 1187 and rack number 9951.

                                          Description of fields

                                          Status The combo box lists the statuses relevant for DynOpt Compact. Valid
                                          options:
                                          0: unprocessed
                                          100: entire racks which have been only partly optimized.
                                          200: Optimized.
                                          300: Cut.
                                          500: If errors have occurred during optimization, the corresponding lites will
                                          get status 500. Apart from that, they appear in the right section of the editor in
                                          a red bar.

                                          Time bar view The time bar view defines the type of view. The editor is avai-
                                          lable for Cutting and for Optimization.

                                          Description of buttons

                                          Update This button serves to update the editor.

                                             Create DynOpt Compact batches
                                             DynOpt Compact batches can be created in the editor or at cutting. In the
                                             cluster view, you can tag one or more batches then create in the context
                                             menu the function Create DynOpt Compact batches. At cutting, this is pos-
                                             sible only for one batch at a time.


                                          Additional information
                                           Tutorial, “A+W DynOpt Compact” on page J-51
3.30 / 01-2023




                 A+W Realtime Optimizer                                                                              J-105
                 Settings                                                             Software Reference




                            Settings
                            Open menu Settings
                            The Settings menu offers the following items:
                            •   Tables
                                Use this menu to access the configured tables.
                                 Software Reference, “Settings” on page J-107
                            •   Table optimization
                                Use this menu to access the table optimization.
                                 Software Reference, “Settings” on page J-107
3.30 / 01-2023




                 J-106                                                            A+W Realtime Optimizer
                 Software Reference                                                                            Settings




                                          Settings
                                          Settings > Tables




                                          Fig. J-38    Tables


                                          This dialog is available for all configured tables.
                                          It offers the opportunity to change settings at runtime, which can otherwise
                                          only be adjusted with the configuration file (xopton.cfg). Thus, the A+W Real-
                                          time Optimizer does not have to be exited and re-started.

                                          Explanation of the fields in the residual plate stock

                                          Active The checkbox controls whether or not the residual plate stock is used..
                                           The residual plate stock is used.
                                           The residual plate stock is not used.

                                          Store plates The checkbox controls whether or not residue plates are stored
                                          in the residual plate stock..
                                           Residual plates are stored in the residual plate stock.
                                           Residual plates are not stored in the residual plate stock.

                                          Use plates The checkbox controls whether or not the optimization uses the
                                          residual plates from the residual plate stock.
                                           Residual plates from the residual plate stock are used.
                                           Residual plates from the residual plate stock are not used.

                                          Minimum storage length In this field, you enter the minimum length in mm
                                          starting with which a residual plate is stored.

                                          Explanation of the fields in the Cutting area

                                          Active The checkbox controls the label printing during cutting.
3.30 / 01-2023




                                           Labels are printed during cutting.
                                           Labels are not printed.




                 A+W Realtime Optimizer                                                                          J-107
                 Settings                                                                Software Reference




                            Edit residual plate In this field, you enter the minimum length of a residual
                            plate in mm, so that editing can be done with PlanEdit during cutting.

                            Description of buttons

                            Accept If you click this button, the changes are applied.

                            Reject If you click this button, the changes are discarded.


                            Table Optimization
                            Settings > Table optimization




                            Fig. J-39    Table optimization


                            With this dialog, you control whether with the selection of the table optimization
                            the production date is displayed or not.
                            The combo box has the following modes:
                            •   Default
                            •   Production date
                            If you select the Default mode, you will see the table optimization without pro-
                            duction date.
                             Chapter “Table Optimization in the Default Variant” on page J-68
                            If you select the Production date mode, you will see the table optimization 
                            production date.
                             Chapter “Table Optimization in the Production Date Variant” on page J-71
3.30 / 01-2023




                 J-108                                                             A+W Realtime Optimizer
                 Software Reference                                                                                  View




                                          View
                                          Open menu View
                                          The View menu offers the following items:
                                          •   Start and exit the import (only for A+W Realtime Optimizer stand alone)
                                              Use this menu to start and to exit the import.
                                          •   Software Reference, “Import” on page J-109
                                          •   Error messages
                                              Use this menu to access the error messages.
                                               Software Reference, “Error Reports” on page J-110
                                          •   Status bar
                                              Use this menu to show or hide the status bar.


                                          Import
                                          View > Import




                                          Fig. J-40     Import


                                          This dialog monitors the working directory for import files and shows the import
                                          status.
                                          Batches that have been imported without an error message, appear in dialog
                                          Select a Batch for further processing. Imported data are saved in the database
                                          while the imported files are moved to archives.

                                          Description of buttons

                                          Start When you use this button, the import function will monitor the working
                                          directory. When new import files are transferred to the working directory, these
3.30 / 01-2023




                                          are automatically checked and imported into the database. The button now re-
                                          ads Stop.



                 A+W Realtime Optimizer                                                                            J-109
                 View                                                                Software Reference




                         Stop Using this button terminates the import. When new import files are
                         transferred to the working directory, these remain unprocessed until the import
                         function is restarted. The button now reads Start.


                         Additional information
                          Tutorial, “Import optimizations” on page J-16



                         Error Reports
                         View > Error reports




                         Fig. J-41     Error reports


                         This dialog shows a new error as well as all errors occurred since the program
                         was last started.

                         The following error occurred A new error is shown in this area.

                         Previous errors This section shows all previously occurred errors.

                         Error file Use this button to save the contents of this dialog in an error file.
3.30 / 01-2023




                 J-110                                                         A+W Realtime Optimizer
A+W Realtime Optimizer         J

                         Partindex




                A+W Production
                 Partindex                                                  Index A+W Realtime Optimizer




                 Index A+W Realtime Optimizer
                 A                                      D
                 A+W Production Terminal (XTV)   J-49   Data import
                 Add                                    – A+W Production J-15
                 – broken lite J-101                    – method J-13
                                                        – stand-alone system J-16, J-109
                 B                                      Data input
                 Basic idea                             – breakage J-20
                 – cutting code creation J-9            – filler orders J-20
                 – cutting optimisation J-9             – rush orders J-20
                 Batch                                  Data processing
                 – reset J-81                           – local optimisation J-28
                 – select J-86                          Defect Optimizer J-50
                 – sequence J-41                        Delete
                 Batches                                – breakage J-24
                 – link J-35                            – high-priority sheet J-22
                 Break down                             – rejects J-23
                 – table optimisation J-32
                 Breakage                               E
                 – delete J-24                          Einstellungen
                 – optimize J-28                        – Tischoptimireung J-108
                 – select J-28                          Enter
                 Broken sheet                           – high-priority sheet J-21
                 – Pool J-99                            – rejects J-22
                                                        – Rush order lites J-60
                 C                                      Error report J-17, J-110
                 Cluster view J-103
                 Continue                               F
                 – cutting J-43                         Features J-10
                 Control                                Filler order
                 – Table J-90                           – use J-31
                 Control unit J-36
                 Create                                 G
                 – cutting code J-90                    Glass type
                 – local optimisation J-52              – select J-68
                 – table optimisation J-29
                 Cut
                 – Job J-90                             H
                 Cutting                                High-priority sheet
                 – continue J-43                        – delete J-22
                 – interrupt J-43                       – enter J-21
                 – repeat J-39, J-81                    – optimize J-28
                 – sequence J-41, J-92                  – show J-58
                 – skip J-40                            High-priority sheet order
                 – start J-42, J-90                     – select J-28
                 Cutting code
3.30 / 01-2023




                 – create J-90                          I
                 – do not create J-40                   Icons
                 Cutting table J-36                     – overview   J-57


                 A+W Realtime Optimizer                                                           J-113
                 Index A+W Realtime Optimizer                                                Partindex




                 Import                                 – Pausing glass types J-83
                 – Data J-109                           – select J-86
                 – job J-16                             Optimize
                 – switch off J-17                      – Select glass type J-68
                 – switch on J-16                       – Table optimization J-74
                 Input of shapes J-62                   Overview
                 Interrupt                              – icons J-57
                 – cutting J-43                         – Local optimisation J-72
                                                        – method J-11, J-18, J-26, J-37
                 J                                      – Software J-57
                 Job
                 – cut J-39, J-90                       P
                 – select J-28, J-52                    Pausing glass types J-83
                                                        PlanEditor J-49
                 L                                      Plate
                 Link J-35                              – cut again J-46
                 – table optimization J-33              – do not cut J-40
                 Lite                                   Process
                 – enter J-21                           – Residue plate J-93
                 Local optimisation J-28                Production status
                 – create J-52                          – reset J-46
                 – Number of stockplates J-81
                 – overview J-72                        R
                 – Stockplate J-77                      Rejects
                                                        – add J-101
                 M                                      – delete J-23
                 Master data J-15                       – enter J-22
                 Menu                                   Repeat
                 – Software J-57                        – cutting J-46, J-81
                 Method                                 – job J-39
                 – data import J-13                     Reset
                 – overview J-11, J-18, J-26, J-37      – status J-46, J-81
                 – table control J-36                   Residue plate
                 Modules                                – optimise J-49
                 – A+W Production Terminal (XTV) J-49   – process J-93
                 – connected J-47                       – show J-41
                 – Defect Optimizer J-50                – use J-30
                 – PlanEditor J-49                      Residue plate dispenser
                 – Residue stock J-48                   – use J-48
                                                        Rush order lites
                                                        – enter J-60
                 O
                 Optimisation
                 – check J-41                           S
                 – cut J-41                             Select
                 – import J-16                          – batch J-86
                 – select stockplate. J-30              – breakage J-28
                 Optimise                               – Glass type J-68
                 – breakage J-28                        – high-priority sheet J-28
3.30 / 01-2023




                 – high-priority sheet J-28             – job J-28, J-39, J-52
                 – residue plate J-49                   – Optimization J-68, J-86
                 Optimization                           – stockplate J-77
                                                        Sequence


                 J-114                                                         A+W Realtime Optimizer
                 Partindex                                            Index A+W Realtime Optimizer




                 – batch J-41                        X
                 – cutting J-41, J-92                XOPT-ON Plus
                 Shape J-102                         – Cluster view J-103
                 Show                                – general J-51
                 – high-priority sheet J-58          – Import J-51
                 Skip                                – Optimisation J-51
                 – cutting J-40
                 Software
                 – Menu J-57
                 – Overview J-57
                 Stand alone system
                 – Data import J-109
                 Start
                 – cutting J-90
                 Stockplate
                 – select J-30, J-77
                 Switch off
                 – import J-17
                 Switch on
                 – import J-16

                 T
                 Table
                 – control J-90
                 Table optimisation
                 – break down J-32
                 – create J-29
                 Table optimization
                 – link J-33
                 – Parameters J-74, J-79
                 Tableoptimisation
                 – check result J-30
                 Tischoptimierung
                 – Einstellungen J-108

                 U
                 Use
                 – filler order J-31
                 – residue plate J-30
                 – residue plate dispenser    J-48

                 V
                 View
                 – Broken sheets    J-99

                 W
                 Work
                 – continue J-43
3.30 / 01-2023




                 – interrupt J-43




                 A+W Realtime Optimizer                                                     J-115
                 Index A+W Realtime Optimizer                 Partindex
3.30 / 01-2023




                 J-116                          A+W Realtime Optimizer

