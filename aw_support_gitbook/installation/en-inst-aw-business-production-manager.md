---
title: "EN INST A+W Business Production Manager"
category: "installation"
product: "A+W Business Production Manager"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Business Production Manager"]
version: "1.0"
last_updated: "2025-12-10"
description: "Installation and Configuration Instructions            A+W Production Manager and iCut     10.12.2021             EN-INST-A+W Business Production Manager.docx   1      Date      by     Comments                                                                       Rel      2013-10-31 MT    Release version                                                                1.0      2014-01-20 MT    Release version, AWB Pro-Config-Tool                                           1.1      2014-05-"
source_file: "EN-INST-A+W Business Production Manager.pdf"
---


# EN INST A+W Business Production Manager

        Installation and Configuration Instructions



        A+W Production Manager and iCut




10.12.2021             EN-INST-A+W Business Production Manager.docx   1
     Date      by     Comments                                                                       Rel
     2013-10-31 MT    Release version                                                                1.0
     2014-01-20 MT    Release version, AWB Pro-Config-Tool                                           1.1
     2014-05-30 WB    Review                                                                         1.2
     2014-06-16 WB    Add chapter “Meaning of variables in formulas”                                 1.3
                      Add chapter “Configuring machine drivers for cutting, bending and
     2014-09-24 DLA                                                                                  1.4
                      sealing”
     2015-06-01 MH    Requested changes by DLA (AWDesk case #346744)                                 1.5
                      Create drilled hole marking and new ParameterID 18 and Chapter 6.8
     2015-07-17 MST                                                                                  1.6
                      (#345910)
     2015-08-06 MST   ParameterID 14 (Rack numbering) is out of date (#327524)                       1.7
     2015-08-10 MST   New ParameterID 19 (image settings for hand cut labels, #351540)               1.8
     2015-09-07 MST   Change Prod_Parameter table with ConfigTool 6.9                                1.9
                      Configure bender text in AWBusiness 5.8
     2015-10-23 MST                                                                                  2.0
                      Placeholders for bender text 5.8.1
     2015-11-06 MST   New ParameterID 20 display processing text 1 (see #357127)                     2.1
     2016-02-05 MST   3.4 Setting up productive and archived databases                               2.2
     2016-02-24 MST   New ParameterID 21 Set optimization mode for lot type (see #352642)            2.3
     2016-03-01 MST   7.1.1.1 Update of 12.x to 13.x or higher number range for break                2.4
     2016-03-01 MST   7.1.2    New reports and labels since Version 6                                2.5
                      6.1.3 New fields in database for position split and breakage since
     2016-03-02 MST                                                                                  2.6
                      Version 6
     2016-03-02 MST   7.1.4    New table PROD_BREAKAGE since Version 6                               2.7
     2016-03-21 MST   7.1.5    Stockplates since Version 6                                           2.8
                      7.3 New features in V6
                      7.3.1New columns in Prod_OPTI_STATISTICS (#361422)
     2016-05-20 MST   7.3.2 Use of the latest user input for a new optimization variant in the       2.9
                      Optimization Manager (#360709).
                      7.3.3             Send waste to AWB for cost calculation (#363566)
                      New formula variables NumberOfDifferentMachinesForProcessings,
     2016-05-31 MST                                                                                  3.0
                      NumberOfDifferentMachinesForProcessingsOfParent and TourOrder 6.6




10.12.2021                EN-INST-A+W Business Production Manager.docx                           2
     Date      by     Comments                                                                     Rel
                      New Release version 6.1
                      No support for: Microsoft remove 260 length path limit since Win10 and
     2016-06-07 MST   Server 2016 3.10                                                             3.1
                      Update to version 6.1 2.4
                      New driver scripts 7.3.4
                      xOptMult and xrecalc batches and problem of glass after optimization
     2016-07-08 MST                                                                                3.2
                      7.2.2
     2016-07-19 MST   NewFormula NumberOfSheetsWithProcessingInUnit6.6f                            3.3
                      New function tolerance for Max/Mix optimization parameter (#375052)
     2016-07-23 MST                                                                                3.4
                      7.1.6
                      Multi selection in lists (#378635) 7.3.5
                      User-defined edge stripping (#376802) 7.3.6
                      New columns in table PROD_OPTI_STATISTICS (#378569) 7.3.7
     2016-10-07 MST   Save residual plates in AWB DB (#378522) 7.3.8                               3.5
                      Block entry has incorrect dimensions7.1.7
                      Marking stepped drilled holes in cutting code 7.3.9
                      Use of residual plates rather than stockplates in optimization 7.1.8
     2016-12-01 MST   New Parameter ID 22 Residual plates decrease in ConfigTool                   3.6
                      #385099: Print cutting labels via machine driver 7.3.10 and new
     2017-05-10 MST                                                                                3.7
                      Parameter ID 23
                      New Formula/Orga variables (6.6):
                      ParentProductClass
     2017-07-17 MST   GrandParentProductType                                                       3.8
                      GrandParentProductClass
                      EndProductClass
                      #404089: The Production Manager could print labels for Glass from stock,
                      customer own glass or order glass and uses the new Parameter ID 24
     2017-09-30 MST   AdditionalGlassLabel for report settings                                     3.9

                      Info about version 6.4 2.4.1
     2017-09-20 MST   #399962: Use Crystal Report Runtime 13 7.3.11                                4.0




10.12.2021                EN-INST-A+W Business Production Manager.docx                         3
     Date      by     Comments                                                                    Rel
                      #405953: How to edit Opt2* files before optimization runs 7.1.9.
                      Configuration of Realtime Optimizer Standalone 5.10
                      5.10.1 Config AWB Pro and RTO
     2017-09-21 MST                                                                               4.1
                      5.10.2 Use RTO as stand-alone system
                      5.10.3 Hints for RTO xopton.cfg file settings
                      5.10.3.7 Use Hegla article code
                      New AWB feature: standard shapes rotation on order entry screen
     2017-10-06 MST                                                                               4.2
                      (#377601) 7.1.10
                      New INTVALUE2 for ParameterId 18 in PROD_PARAMETER for cut-out
     2017-10-20 MST                                                                               4.3
                      marking (#408035)
     2017-11-07 MST   Different stocks and plate booking via XTV feedback 7.1.11                  4.4
                      Export of rounded corners for the cutting table. New INTVALUE3 for
     2017-11-08 MST                                                                               4.5
                      ParameterId 18 in PROD_PARAMETER (#409300)
     2017-11-24 MST   Errors in XRecalc at optimization 7.2.3                                     4.6
                      Notes about shape 770, 771, 7727.3.12
     2017-11-28 MST                                                                               4.7
                      Refinements in Hotfix 899, 915, 952, 980 7.3.13
                      #407260: Feedback from Realtime optimizer (RTO) to AWB to discount
     2018-01-18 MST                                                                               4.8
                      stockplates in AWB 7.3.14
                      7.3.15 Some problems raised


                      #4170277.3.15.1 sheets that are not set into the cutting state.
     2018-02-26 MST   #416756 7.3.15.2 Hardware articles in order selection search                4.9
                      #417132 7.3.15.3 Bavelloni driver support optimization numbers larger
                      than 3 digits
                      #4168877.3.15.4 faster GetFRM
                      New Feature:
     2018-03-08 MST                                                                               5.0
                      #408305: Label printing with Macotec cutting table 7.3.10
                      April 2018 Release:
                      Archive reports as pdf 7.3.16
     2018-04-16 MST   New Job status at job status dialog 7.3.17                                  5.1
                      Some Bugfixes 7.3.18:
                      #420104: Residual plates size not correct




10.12.2021                EN-INST-A+W Business Production Manager.docx                        4
     Date      by     Comments                                                                            Rel
                      June 2018 release:
                      - Add stockplate supplier info 7.3.19
     2018-06-13 MST                                                                                       5.2
                      - New parameter 25 to change base archive folder path
                      - New filter criteria at optimization summary TAB 7.3.20
                      Default PDF printer to show Optimization Result and Pattern report on
     2018-07-26 MST                                                                                       5.3
                      Screen from PlanEdit 7.3.21
                      3 new criteria for formula 6.6
                      - CustomerItem
                      - CommissionReference
     2018-09-04 MST                                                                                       5.4
                      - ProjectNumber
                      - ItemText3
                      - ItemText4
                      October 2018 release
                      New criteria for formula 6.6
     2018-10-01 MST                                                                                       5.5
                      NumberOfLaminatedGlassInInsulatedUnit
                      Mark macro processings 7.3.22
                      November release 2018
                      New criteria for formula 6.6
                      - RouteNumber (#410859)
                      Some fixes:
     2018-11-16 MST   - Error in the residual plate size during stock booking fixed                       5.6
                      - Error during the search for all additional glass surfaces for reports fixed
                      - Refinements of the dialog for cutting shapes
                      - Refinements for the selection of float from a tempered glass at order
                      selection
                      Wizard mode ends after order creation (#437306).
                      The user does the detailed scheduling and optimization manually.
                      You have to set the ParameterID 26.
     2019-01-25 MST   RTO sends status feedback to Production Manager                                     5.7
                      (#410492) 5.10.3.10
                      Some hints for special shapes 901 and 902 7.3.23
                      New parameter for ParameterID 22 to get the smaller residual plate


10.12.2021                EN-INST-A+W Business Production Manager.docx                                5
     Date         by    Comments                                                                    Rel
                        New parameter for ParameterID 18 for different markings on different
     2019-01-29 MST                                                                                 5.8
                        cutting tables
                        February Release 7.3.24:
     2019-02-07
                  MST   Print archive and output reports in the background                          5.9
                        Edge correction during the machine assignment
                        March release 7.3.25
                        Filter and search short keys
     2019-02-28 MST     Obsolete DB script in v12.5                                                 6.0a
                        ConfigTool is wanred if the order number range overlaps with the break or
                        the quotation number range.
     2019-02-28 MST     March release 7.3.25 Deleting entries in the block file                     6.0b
     2019-04-09 MST     AWB Pro Partial Deliveries 5.11                                             6.1
                        #440101 – Write muntin section in AWISO.dat for TFB Bender driver to
                        make drilled holes for muntins in the spacer 7.3.26
     2019-04-26 MST                                                                                 6.2
                        #445624 - Different batch numbers at RTO and Production Manager
                        5.10.3.11
                        #446108 - Send the finished cutting report for the RTO Remaster
     2019-05-08 MST                                                                                 6.3
                        environment ParameterID 27
     2019-06-04 MST     #444661 – Partial deliveries in AWB 7.3.27                                  6.4
     2019-08-01 MST     #449810 – Selected plate as first plate in optimization 7.3.28              6.5
                        #450801 - Support of bent IG and LAMI and use of the right cutting
     2019-08-19 MST                                                                                 6.6
                        size7.3.29
                        #451823 – XTV Mode 7.3.30
                        Information about September release 2019 7.3.31
                        Tool tip about job, optimization, breakage numbers
     2019-09-11 MST                                                                                 6.7
                        Minimized ribbon bar
                        Faster order creation and detailed scheduling
                        Rack numbers with more than 4 digits and ALCIM_BOOK_FACH in label.set




10.12.2021                  EN-INST-A+W Business Production Manager.docx                       6
     Date         by     Comments                                                                       Rel
                         Information about November release 2019 7.3.32
                         ParameterID 28: Keep float glass together on same rack if the shape is a
                         shape 99 and IG/LAMI.
     2019-10-08 MST      Job summary tab shows the correct cutting size for shape 99.                   6.8
                         #453238 New formula variables6.6 Machine1AfterCutting,
                         Machine2AfterCutting, Machine3AfterCutting, Machine4AfterCutting,
                         Machine5AfterCutting
     2020-04-22 DNI      Barcoding - unique label identification per glass 6.3.33                       6.9
     2020-06-07 DL       A+W iCut Installation and Configuration 8                                      13.4


                         ParameterID 30: Use Crystal Reports for cutting plans (#457082)
     2020-07-14 DNI                                                                                     13.4
                         ParameterID 31: Default optimization mode (for iCut #450838)


     2021-11-17 DNI      Barcoding – Production racks 6.3.34                                            13.4


This document enables the competent reader to install the software described.
You should generally proceed in the following sequence:



    1. Check the installation requirements.

    2. Compile the required data, additional programs, drivers, etc.

    3. Note or determine the time required.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                          7
Contents

   Installation and Configuration Instructions ................................................ 1

   1         New installation of Version 6 ........................................................ 14
   1.1       Prerequisites .......................................................................................................14
   1.2       Overview and fundamentals ...............................................................................14
   1.3       Time requirement ...............................................................................................14
   1.4       Update to version 6.1 or higher ..........................................................................15
   1.4.1     Version 6.4 ....................................................................................................................... 15

   2         Preparations ................................................................................. 16
   2.1       Other applicable documents...............................................................................16
   2.1.1     Installation instructions A+W Business............................................................................ 16

   2.1.2     Configuration instructions A+W Business ....................................................................... 16

   2.1.3     Installation instructions license server ............................................................................ 16

   2.1.4     Installation instructions license client ............................................................................. 17

   2.1.5     Installation instructions A+W CAD Designer (Shapes) ..................................................... 17

   2.1.6     Installation instructions A+W CAD Designer (Bars) ......................................................... 17

   2.1.7     Installation instructions A+W Plan Editor ........................................................................ 17

   2.1.8     Installation instructions A+W Business Interface Service................................................ 17

   2.1.9     Installation instructions A+W Business 6 ServiceMonitor ............................................... 18

   2.1.10    Configuration of machine code, bender code ................................................................. 18

   2.1.11    Installation Instructions for A+W Business Production Terminal (EL) ............................. 18

   2.2       Current system environment ..............................................................................18
   2.3       Database server setup ........................................................................................18
   2.4       Setting up productive and archived databases ...................................................19
   2.5       Creating database users .....................................................................................19
   2.6       .Net Framework 4.5 ............................................................................................19

10.12.2021                              EN-INST-A+W Business Production Manager.docx                                                             8
   2.7       Releasing the server directory ............................................................................19
   2.8       Windows user .....................................................................................................20
   2.9       License servers....................................................................................................20
   2.10      Removal of 260 path length limit since Win 10 and Server 2016........................21

   3         Installation A+W Business Pro ...................................................... 22
   3.1       Starting the SetupStarter ....................................................................................22
   3.2       Installation with the SetupLauncher ...................................................................22
   3.2.1     Welcome screen .............................................................................................................. 22

   3.2.2     Choose diskset ................................................................................................................. 22

   3.2.3     Setup directory ................................................................................................................ 23

   3.2.4     Previously installed components ..................................................................................... 24

   3.2.5     Select the components to install ..................................................................................... 24

   3.2.6     Interface Service configuration........................................................................................ 25

   3.2.7     Production Settings configuration ................................................................................... 27

   3.2.8     A+W Business 6 settings .................................................................................................. 28

   3.2.9     AWSOA Communication configuration ........................................................................... 29

   3.2.10    AWSOA Service User ........................................................................................................ 29

   3.2.11    A+W Business configuration ............................................................................................ 30

   3.2.12    Start the installation process ........................................................................................... 31

   3.2.13    Installation maxx PDFMAILER or eDoc PDF Printer ......................................................... 33

   3.3       Configuration after installation via SetupLauncher ............................................34
   3.4       Execute the OS restart ........................................................................................40
   3.5       No Windows domain and use SQL Server Authentication ..................................41

   4         A+W Business Pro configuration ................................................... 42
   4.1       Database update.................................................................................................42
   4.2       Adjustment of the company master data ...........................................................42
   4.2.1     Tab 4. Documents ............................................................................................................ 43

10.12.2021                             EN-INST-A+W Business Production Manager.docx                                                           9
   4.3       Adjustment of the order master data .................................................................43
   4.4       Adjustment of the production master data ........................................................45
   4.5       Adjustment of B2B master data ..........................................................................46
   4.6       Create workflow task transfer to A+W Production Manager ..............................47
   4.7       Create workflow task for archiving production manager jobs ............................52
   4.8       Configuring machine drivers for cutting, bending, and sealing ...........................56
   4.9       Configure Bender text in AWBusiness ................................................................56
   4.9.1     Bender text placeholders................................................................................................. 57

   4.10      Realtime Optimizer (EL) stand-alone ..................................................................59
   4.10.1    Configuration of AWB Pro and Realtime Optimizer (EL) stand-alone ............................. 59

   4.10.2    Use as stand-alone system .............................................................................................. 61

   4.10.3    Configure RTO in AWB Pro environment (Some hints) ................................................... 63

   4.11      Partial deliveries in AWB Pro ..............................................................................68

   5         Checking the installation and configuration .................................. 70
   5.1       Checking storage place organization ..................................................................70
   5.2       Checking capacity planning .................................................................................70
   5.3       Checking grinding allowances .............................................................................70
   5.4       Check BLOCK.pth and Opt2txt.dat ......................................................................71
   5.5       LABEL.SET ...........................................................................................................71
   5.6       Meaning of variables in formulas .......................................................................72
   5.7       Description of values for fields BOM_ID, BOM_POS, BOM_NODE and
             BOM_LEVEL ........................................................................................................82
   5.8       Implementation of markings for drilled holes or cut-outs ..................................82
   5.9       Configuration via table PROD_PARAMETER........................................................83

   6         Tips and tricks............................................................................... 93
   6.1       FAQs ...................................................................................................................93
   6.1.1     Update from 12.x to 13.x or higher check breakage job number range ......................... 93

10.12.2021                            EN-INST-A+W Business Production Manager.docx                                                    10
   6.1.2     New reports and labels since Version 6........................................................................... 93

   6.1.3     New fields in database for position split and breakage since Version 6 ......................... 93

   6.1.4     New table PROD_BREAKAGE since Version 6 .................................................................. 93

   6.1.5     Stockplates since version 6 .............................................................................................. 94

   6.1.6     Tolerance optimization parameter Max X-X, Max Y-Y, Min X-X, Min Y-Y (since V6.2) .... 95

   6.1.7     Block entry has not the correct dimension...................................................................... 96

   6.1.8     Use residual plates rather than stockplates in optimization ........................................... 97

   6.1.9     How to edit Opt2* files before optimization runs ........................................................... 98

   6.1.10    New AWB function: turning of standard models on the order entry screen (#377601)
             ....................................................................................................................................... 101

   6.1.11    Different stock and plate bookings via XTV reporting ................................................... 101

   6.2       Known errors and workarounds ....................................................................... 102
   6.2.1     Problems installing Microsoft components ................................................................... 102

   6.2.2     xOptMult and xRecalc batches ...................................................................................... 102

   6.2.3     XRecalc errors ................................................................................................................ 104

   6.3       New features in V6 ........................................................................................... 104
   6.3.1     New columns in Prod_OPTI_STATISTICS (#361422) ...................................................... 104

   6.3.2     Use the latest user input for new variant of optimization in Optimization Manager
             (#360709) ....................................................................................................................... 105

   6.3.3     Send waste to AWB for cost calculation (#363566) ...................................................... 105

   6.3.4     New driver scripts .......................................................................................................... 105

   6.3.5     Multi selection in lists .................................................................................................... 106

   6.3.6     Customized edge deletion ............................................................................................. 106

   6.3.7     New columns in table PROD_OPTI_STATISTICS ............................................................. 108

   6.3.8     Save residual plates in AWB DB ..................................................................................... 109

   6.3.9     Marking stepped drilled holes in cutting code .............................................................. 112

   6.3.10    Print cutting labels via machine driver .......................................................................... 112

   6.3.11    Crystal report Runtime 13 (#399962) ............................................................................ 122

   6.3.12    Notes about shape 770, 771, 771, 772 .......................................................................... 123


10.12.2021                               EN-INST-A+W Business Production Manager.docx                                                               11
   6.3.13    Refinements in Hotfix 898, 915, 952, 980 ..................................................................... 123

   6.3.14    Feedback from Realtime Optimizer (RTO) to AWB to discount stockplates in AWB
             (#407260) ....................................................................................................................... 123

   6.3.15    Fix some issues 417027, 416756, 417132, 416887 ....................................................... 127

   6.3.16    Archive reports as pdf .................................................................................................... 128

   6.3.17    New Job Status at Job Status dialog .............................................................................. 130

   6.3.18    Residual plates size not correct (420104)...................................................................... 131

   6.3.19    Add supplier info............................................................................................................ 131

   6.3.20    New filter criteria at optimization summary TAB .......................................................... 132

   6.3.21    Default PDF printer to show Optimization Result and Pattern report on screen from
             PlanEdit .......................................................................................................................... 133

   6.3.22    Mark macro processings ................................................................................................ 133

   6.3.23    Some hints for specials shapes 901 and 902 ................................................................. 133

   6.3.24    February Release 2019 .................................................................................................. 135

   6.3.25    March release 2019 ....................................................................................................... 136

   6.3.26    Write Muntin section in AWISO.dat for TFB Bender driver to make drilled holes for
             muntins in the spacer .................................................................................................... 138

   6.3.27    Partial deliveries in AWB (#444661) .............................................................................. 139

   6.3.28    Selected plate as first plate in optimization (#449810) ................................................. 140

   6.3.29    Support of bended IGU and LGU (#450801) .................................................................. 140

   6.3.30    XTV Mode (#451823) ..................................................................................................... 140

   6.3.31    Changes in September 2019 release ............................................................................. 143

   6.3.32    Changes in November 2019 release .............................................................................. 144

   6.3.33    Barcoding - unique label identification per glass (#439200) ......................................... 145

   6.3.34    Production racks [AW-59393]........................................................................................ 147

   7         Uninstalling ................................................................................ 151

   8         A+W iCut .................................................................................... 152
   8.1       Prerequisite ...................................................................................................... 152


10.12.2021                              EN-INST-A+W Business Production Manager.docx                                                            12
   8.1.1     Software......................................................................................................................... 152

   8.1.2     Modules of the license server ....................................................................................... 154

   8.2       Installation SQLServer Express and the database ............................................. 155
   8.3       Installation of the software with the A+W Setup Launcher .............................. 159
   8.3.1     Creating the fingerprint for the soft lock....................................................................... 159

   8.3.2     Installing the Setup Launcher and license server .......................................................... 160

   8.4       Installation of A+W iCut software ..................................................................... 162
   8.5       iCut activation in script management ............................................................... 165
   8.6       MDI window and the main menu ..................................................................... 167
   8.7       Master Data ...................................................................................................... 168
   8.7.1     Customers ...................................................................................................................... 168

   8.7.2     User rights ...................................................................................................................... 168

   8.7.3     Number ranges .............................................................................................................. 169

   8.7.4     Product Management .................................................................................................... 170

   8.8       Documents ....................................................................................................... 170
   8.8.1     Number manager ........................................................................................................... 170

   8.8.2     Document entry ............................................................................................................. 171

   8.8.3     Form printing ................................................................................................................. 172

   8.8.4     Archive transfer ............................................................................................................. 172

   8.8.5     Exchange Service ........................................................................................................... 172

   8.8.6     Data back-up .................................................................................................................. 176

   9         Appendix .................................................................................... 177
   9.1       Table of figures ................................................................................................. 177




10.12.2021                              EN-INST-A+W Business Production Manager.docx                                                           13
1 New installation of Version 6
The following installation instructions assume that no prior version has been installed. Setup and
additional configuration options may also be described in detail in the other applicable documents
see 2.1)

1.1 Prerequisites
    •   Follow the instructions described here exactly!
    •   Use the setups and configuration tools provided.
    •   Don’t use other tools such as XCOPY or REGEDIT, only the tools provided by the setup.

1.2 Overview and fundamentals
The following list provides an overview of the steps that need to be performed during installation
one after the other:
    •   Perform/check preparations, see 3.
    •   Installation, see 4.
    •   Configuration, see 5.
    •   Check the result, see 5.5.

1.3 Time requirement
Depending on the type of computer, disk space and configuration, the installation time will vary
with different computers. The installation time defined here is based on a reference device with the
following features:
    •   Processor:             Intel Xenon 2.4 GHz
    •   Main memory:           2 GB
    •   Other:                 Windows Server 2008 R2 or 2012 or 2012 R2 or 2016, 64 bit
                               in a virtual machine
    •   Database:              SQL server installed and preconfigured.
    •   License server:        installed and configured.
    •   .Net:                  Version 4.5 will be installed during the installation.
                               (Framework 3.5 must be installed for Production Manager 5.)
The installation time for a first-time or new installation on the reference device is 180 minutes. For
higher or lower performing hardware the installation times will be accordingly shorter or longer.




10.12.2021                        EN-INST-A+W Business Production Manager.docx                       14
1.4 Update to version 6.1 or higher
We are not patching version 6.0 with hotfixes because we are going ‘Fast-To-Market’.


To fix some errors, you have to do follow:


    -   You have to install the setup of newest version, if the customer has a lower version (6.0,
        too).
    -   Then you could install all hotfixes and SQL scripts.
    -   FYI: You could use the V6 database version with the Production Manager 6.1 or higher


Please, check chapter 7.1 (FAQ), 7.3 (New Features) and 3.10 (If you use Win Server 2016 or
higher)


1.4.1 Version 6.4


We will not provide a new version on a particular date. We will remain with version 6.4.


We make only 0er hotfixes. I am writing new features in this document. Please check this. This
Version can be used with a AWB 6.x.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                          15
2 Preparations
The following preparations must be made before performing the installation.

2.1 Other applicable documents
The following documents provide a detailed description of further steps that may also need to be
performed.
You can also find these documents in the Intranet > Online service area > Documentation > Internal
documentation in the respective product area.
2.1.1 Installation instructions A+W Business


Generally, the installation instructions for A+W Business 6 can be found here:
\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W Business Pro.pdf


2.1.2 Configuration instructions A+W Business


Old configuration instructions:
\\jupiter\doku_docuware\ALFAK2000\!General\Installation_Configuration\EN-
Installationshinweise.pdf
German:
\\jupiter\doku_docuware\ALFAK2000\!General\Installation_Configuration\DE-
Installationshinweise.pdf



New Configuration document:

English
\\Jupiter\SW_Install\v6\ConfigurationDocumentation\EN-CONFIG-A+W Business.pdf
German
\\Jupiter\SW_Install\v6\ConfigurationDocumentation\DE-CONFIG-A+W Business.pdf


2.1.3 Installation instructions license server


The current documentation can be found in the directory
\\Jupiter\SW_Install\2012\InstallationDokumentation\EN-INST-A+W License Server.pdf


10.12.2021                        EN-INST-A+W Business Production Manager.docx                     16
2.1.4 Installation instructions license client


The current documentation can be found in the directory
\\Jupiter\SW_Install\2012\InstallationDokumentation\EN-INST-A+W Lizenz Client.pdf


2.1.5 Installation instructions A+W CAD Designer (Shapes)


The current documentation can be found in the directory
\\Jupiter\SW_Install\V6\InstallationDokumentation\EN-INST-A+W
\\Jupiter\SW_Install\V6\InstallationDocumentation\EN-INST-A+W CAD Designer Shapes.pdf


2.1.6 Installation instructions A+W CAD Designer (Bars)


The current documentation can be found in the directory
\\Jupiter\SW_Install\v6\InstallationDokumentation\EN-INST-A+W
\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W CAD Designer Bars.pdf


2.1.7 Installation instructions A+W Plan Editor


V6 or higher: The A+W Plan Edit should be installed with the A+W Setup Launcher. There are no
installation instructions or documents.


The following text is obsolete since V6 but if you use version 2012:
The documentation of 2012 can be found in the directory
\\Jupiter\SW_Install\2012\InstallationDokumentation\DE-INST-A+W
\\Jupiter\SW_Install\2012\InstallationDocumentation\DE-INST-A+W Plan Editor.pdf


2.1.8 Installation instructions A+W Business Interface Service


The current documentation can be found in the directory
\\Jupiter\SW_Install\v6\InstallationDokumentation\EN-INST-A+W
\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W Business Interface Service.pdf



10.12.2021                     EN-INST-A+W Business Production Manager.docx                     17
2.1.9 Installation instructions A+W Business 6 ServiceMonitor


The current documentation can be found in the directory
\\Jupiter\SW_Install\v6\InstallationDokumentation\EN-INST-A+W
\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W Business Service Monitor.pdf


2.1.10 Configuration of machine code, bender code


The current instructions are found here:
\\Jupiter\SW_Install\v6\ConfigurationDocumentation\EN-CONFIG-A+W Production
MachineControl.pdf


2.1.11 Installation Instructions for A+W Business Production Terminal (EL)


The current documentation can be found in the directory:
\\Jupiter\SW_Install\v6\InstallationDocumentation\EN-INST-A+W Business Production Terminal
(EL).pdf


German


\\Jupiter\SW_Install\v6\InstallationDocumentation\DE-INST-A+W Business Production Terminal
(EL).pdf



2.2 Current system environment
The operating system must be updated to the most recent version. Windows updates must be
performed. Once the system has been updated, the system may need to be restarted before
commencing with the installation.

2.3 Database server setup
A+W Business Pro 6 is only released for SQL Server databases.
Please observe the general A+W standards when setting up the database servers. The standards can
be requested from A+W's ICT department.


10.12.2021                    EN-INST-A+W Business Production Manager.docx                    18
Special attention should be paid to the configuration of default database users and roles.

2.4 Setting up productive and archived databases
No databases are released with the diskset.
In this case, please also contact A+W's ICT department or the project manager.
We recommend setting up at least two archive databases.
Set up one productive database and two archive databases pursuant to A+W-standards in the
database server.

2.5 Creating database users
All persons who are to use the database have to be set up as database users with the authorization
db_owner. Access must be possible for the productive database as well as the archive databases.

2.6 .Net Framework 4.5
.Net-Framework 4.5 is required for the SetupLauncher (since Version 6) that guides you through the
installation of the program components.
Ensure that you have sufficient authorizations to install the .Net Framework.
Production Manager requires .Net Framework 4.5 since version 6.
Production Manager 5 requires .Net Framework 3.5



2.7 Releasing the server directory
Release the so-called server directory for Techsoft/production components, which should be set up
as a shared folder under the name TRANS, with read and write authorizations for all users ("Jeder").




10.12.2021                    EN-INST-A+W Business Production Manager.docx                        19
Figure 1: Release server directory


2.8 Windows user
A Windows user will be required for the A+W Business InterfaceService.
Important: This user must be able to authenticate to the SQL server, if necessary therefore in the
same domain.
    •    Make sure that the AWServices user exists.
    •    The AWServices user must possess sufficient authorizations in the network and on the
         machine. Read and write access must be ensured in all directories and all releases set up in
         the entire configuration.
    •    Please contact ICT for further details.

2.9 License servers
Install the license server on the basis of the existing documentation.




10.12.2021                           EN-INST-A+W Business Production Manager.docx                    20
2.10 Removal of 260 path length limit since Win 10 and Server 2016
For your information


The Administrator could remove the path length limit in Win10 (Anniversary Release, released begin
of August 2016, Build higher than 14352) and Server 2016. The A+W Production Manager cannot
support this because some modules could fail if the path size is greater than 260.


You can check the path size limit at your OS:


Launch the Registry Editor by clicking the Start menu and typing “regedit.exe,” and then navigate to
the following path:


HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Group Policy Objects\{48981759-
12F2-42A6-A048-028B3973495F}Machine\System\CurrentControlSet\Policies



Look for an entry called LongPathsEnabled and if it does not exist, create the entry:
- simply right-click on Policies to see the context menu
- click New DWORD (32-bit)
- name it LongPathsEnabled
- enter value 1 to enable long path length (more than 260 characters) or otherwise 0 to disable.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                        21
3 Installation A+W Business Pro
Installation and configuration must be performed with full administrator rights.

3.1 Starting the SetupStarter
Start the program SetupStarter.exe from your installation diskset.
Depending on the configuration of your system, the .Net Framework will first be installed in the
required versions.

3.2 Installation with the SetupLauncher
3.2.1 Welcome screen
The welcome screen of the SetupLauncher opens.




Figure 2: Welcome screen of the SetupLauncher

    •    Click [Next].
3.2.2 Choose diskset
A dialog appears to choose or create a new diskset.


10.12.2021                        EN-INST-A+W Business Production Manager.docx                     22
A diskset saves selected components as well as individual configurations of these components in a
file for simple reuse or repetition of the installation process.




Figure 3: Dialog Choose or create diskset

    •    Select A+W Business Pro Process Server or A+W Business Pro Terminal Server.
         If the application should be installed on a single workstation PC or a single server, then the
         disk set A+W Business Pro Process Server should be used. When installing and using the
         application on a terminal server, the disk set A+W Business Pro Terminal Server should be
         used.
    •    Click [Next].
3.2.3 Setup directory
A dialog appears to enter a source and target directory for the installation. If you create a new
diskset, the directory from which you started the SetupLauncher is preset as source directory.
Generally the settings can stay as they are.




10.12.2021                           EN-INST-A+W Business Production Manager.docx                     23
Figure 4: Setup directory

    •    Enter the source directory for the installation.
    •    Select the target directory for the installation.
    •    Click [Next].
3.2.4 Previously installed components
A dialog appears that lists the components that have already been installed in the system.
    •    Click [Next].
3.2.5 Select the components to install
A dialog opens to select the components to install. The chosen diskset (see chapter 3.2.2 Choose
diskset) selects all necessary components automatically. The only component that needs to be
changed manually is the correct language version of A+W Business.




10.12.2021                       EN-INST-A+W Business Production Manager.docx                      24
Figure 5: Components to be installed

No other changes need to be made to these settings.
    •    Click [Next].
3.2.6 Interface Service configuration
Configure the Interface Service.




10.12.2021                         EN-INST-A+W Business Production Manager.docx   25
Figure 6: Configuration Interface Service

    •    Enter <Domain>\AWSERVICES as user.
    •    Enter the password.
    •    Click [Next].
If the user is not authorized to log on as Service, you are asked whether you want to grant the user
this right.
    •    Click on [Yes].




10.12.2021                           EN-INST-A+W Business Production Manager.docx                  26
Figure 7: Grant "Service Account" right

3.2.7 Production Settings configuration
Configure communication with the Production components.




Figure 8: ALCIM settings configuration

    •    Enter the server directory (see 3.7).
    •    Enter the server drive; use drive P:
    •    Click [Next].




10.12.2021                          EN-INST-A+W Business Production Manager.docx   27
3.2.8 A+W Business 6 settings




Figure 9: A+W Business 6 Setup settings dialog

    •    Choose your language in the first combo box.
    •    Use the next controls to select your user for the Web configurator (AWSOA) service. With a
         click on the Browse button, the Windows user selection is started in order to make entry
         easier.




Figure 10: Service user dialog




    •    If you have chosen the user, click [OK].

    • Click in the dialog field of the Setup starter on [Next] and you will see the next dialog.


10.12.2021                          EN-INST-A+W Business Production Manager.docx                  28
3.2.9 AWSOA Communication configuration




Figure 11: AWSOA Communication configuration dialog




        •    Now the connection to the Service Locator must be configured. For the host, enter
             the name of the computer on which the Service Locator was installed. The port is
             always 12000.
        •    Click [Next].



3.2.10 AWSOA Service User




10.12.2021                       EN-INST-A+W Business Production Manager.docx               29
Figure 12: AWSOA Service User dialog

         You can determine under which user the services will run. With a click on the [Browse]
         button, the Windows user selection is started in order to make entry easier.




Figure 13: Service user dialog




         •    Here the user should coordinate the services with the user of the A+W Business
              Com.
         •    If you have chosen the user, click [OK].

         •    Click [Next] in the setup Launcher dialog and see the next dialog.



3.2.11 A+W Business configuration
Configure A+W Business.




10.12.2021                        EN-INST-A+W Business Production Manager.docx               30
Figure 14: A+W Business configuration

    •    Select the default language.
    •    Click [Next].
3.2.12 Start the installation process
Not all information for the installation is available.




10.12.2021                         EN-INST-A+W Business Production Manager.docx   31
Figure 15: Start the installation

     •    Select Install Software to perform the installation in line with your settings without saving
          these settings.
               o    This is not recommended.
     •    Select Install software and save setup configuration to an XML file to save the setup
          configuration to use again at a later time and then execute the installation.
               o    This selection is recommended.
     •    Select Only save setup configuration to an XML file to save the settings and perform the
          installation at a later time.
               o    This selection is recommended to prepare an installation and to execute later (e.g.
                    at the customer site).
     •    Select Manage Hotfixes to import existing hotfixes or to uninstall them.
Perform the installation.
     •    Click [Next].
If you want to save the configuration of the setup:
     •    Enter a meaningful name.


10.12.2021                          EN-INST-A+W Business Production Manager.docx                          32
    •    Click [Save].




Figure 16: Save the installation configuration

The installation is executed. The duration of this process may vary depending on the system and the
selection of components.
3.2.13 Installation maxx PDFMAILER or eDoc PDF Printer
You will find the following information in detail in the A+W Business instruction manual, see 2.1.1.




10.12.2021                           EN-INST-A+W Business Production Manager.docx                      33
3.3 Configuration after installation via SetupLauncher




Figure 17: A+W Production Manager configuration – Database login

    •    Enter the database server.
    •    Enter the database.
    •    Enter the user name.
    •    Enter the password.
    •    Click [Next].




10.12.2021                        EN-INST-A+W Business Production Manager.docx   34
Figure 18: A+W Production Manager configuration – ODBC-settings

    •    Enter the name of ODBC Data Source.Enter the name of ODBC Data Source
         By default the name stored in the selected A+W Business database will be proposed and no
         changes need to be made to these setting.
    •    Enter the description of ODBC Data Source (optional)
         If the ODBC Data Source already exists the description of this ODBC Data Source will be
         proposed as description.
    •    Click [Next].




10.12.2021                        EN-INST-A+W Business Production Manager.docx                     35
Figure 19: A+W Production Manager configuration – Transfer directory

    •    Click [Next].




10.12.2021                         EN-INST-A+W Business Production Manager.docx   36
Figure 20: A+W Production Manager configuration– CAD-Designer-directory

    •    Click [Next].




10.12.2021                        EN-INST-A+W Business Production Manager.docx   37
Figure 21: A+W Production Manager configuration – BLOCK.PTH-files

    •    The desired target file can be found at P:\SN\BLOCK.ZIP. You can use the UNC path to
         BLOCK.ZIP, which is used as standard (e.g. \\<Server>\Trans\SN\BLOCK.ZIP).
    •    Right click this entry and select Set new BLOCK database F2:




Figure 22: A+W Production Manager configuration– BLOCK.PTH-files – copy target

    •    Press <Ctrl>+<C> to copy the entry.
    •    Right click the entry Set new BLOCK database F2 for all other entries.




10.12.2021                        EN-INST-A+W Business Production Manager.docx                  38
    •    Press <Ctrl>+<V> to standardize the entries. Duplicate entries are automatically deleted by
         the dialog:
         Instead of P:\.... use UNC paths, i.e. \\Rechner\Trans\SN\BLOCK.ZIP




Figure 23: A+W Production Manager configuration – BLOCK.PTH-files standardized

    •    Click [Next].




10.12.2021                        EN-INST-A+W Business Production Manager.docx                     39
Figure 24: A+W Production Manager configuration – General settings

    •    Click [Next]
    •    Click [Finish].

3.4 Execute the OS restart
Configuring and installing some services may require the system to be restarted. In this case, the
SetupLauncher will point this out to you,




Figure 25: Reboot query

    •    Click on [Yes].


10.12.2021                         EN-INST-A+W Business Production Manager.docx                      40
3.5 No Windows domain and use SQL Server Authentication


If the company will not have a Window domain, you have to make settings in the AWBusiness
Config Tool.




Figure 26: No Windows domain and use SQL Server Authentication



You have to check the Use SQL Server Authentication checkbox and add the user and password for
SQL authentication. If the checkbox is not checked, the Production Manager uses the settings, which
come from AWBusiness Program.




10.12.2021                        EN-INST-A+W Business Production Manager.docx                   41
4 A+W Business Pro configuration
This chapter describes the changes required in the A+W Business master data to put the Production
Manage into operation.

4.1 Database update
Install all existing database update scripts.

4.2 Adjustment of the company master data
    •   Start A+W Business in the desired language.
    •   Should error messages appear during program start due to the current path/IP
        configuration, you can ignore them.
    •   Call Master data > Company > Company data.
    •   Note: Do NOT press [Save] during this process, but wait until the end of the configuration!




10.12.2021                      EN-INST-A+W Business Production Manager.docx                          42
4.2.1 Tab 4. Documents




Figure 27: Company master data – Documents

    •   Change or check the path for file attachments to a suitable directory.
    •   You have to exit this directory. If necessary, create it manually.
    •   Recommended: Sub-directory of the TRANS directory (see 3.7).

4.3 Adjustment of the order master data
    •   Call Master data > Order > Status allocation.




10.12.2021                       EN-INST-A+W Business Production Manager.docx    43
Figure 28: Order master data – Status allocation

    •    Enter the following data:
    •    Status 041:
              o    User status: 415
              o    Min. status: 001
              o    Lock status: 540
              o    Click [Save].
    •    Status 042:
              o    User status: 420
              o    Min. status: 001
              o    Lock status: 000
              o    Click [Save].
    •    Status 043:
              o    User status: 430
              o    Min. status: 001
              o    Lock status: 000


10.12.2021                          EN-INST-A+W Business Production Manager.docx   44
              o    Click [Save].
    •    Status 045:
              o    User status: 450
              o    Min. status: 001
              o    Lock status: 000
              o   Click [Save].
    •    Click [Close].

4.4 Adjustment of the production master data
    •    Call Master data > Production > Registration points production.




Figure 29: Production master data – Registration points production

    •    Make sure that the following points are activated as product types for feedback:
    •    Registration point 0:


10.12.2021                          EN-INST-A+W Business Production Manager.docx            45
             o   Simple tempered
             o   Tempered glass
             o   IG
             o   Laminated glass
    •   Registration point 100:
             o   Simple tempered
             o   Tempered glass
             o   IG
             o   Laminated glass
    •   Registration point 150:
             o   Simple tempered
             o   Tempered glass
             o   IG
             o   Laminated glass
    •   Registration point 200:
             o   Simple tempered
             o   Tempered glass
             o   IG
             o   Laminated glass
    •   Click [Close].

4.5 Adjustment of B2B master data
The following settings need to be made to make sure that SN generates image files during transfer
to capacity planning that may need to be shown on the lists under certain circumstances:
    •   Call Master data > B2B > Customer > SN file rules.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                          46
Figure 30: B2B-master data – SN file rules

    •    Make sure that the two records above exist.
              o    Product type Modelle/Shapes (code: 12), product class Modelle/Shapes (code: 5)
              o    Product type Modelle/Shapes (code: 12), product group Stufe/Stepped unit (code:
                   50)

4.6 Create workflow task transfer to A+W Production Manager
A workflow task has to be set up to ensure that the entered orders are automatically transferred to
capacity planning.
    •    Call Master data > Company > Formulas.




10.12.2021                           EN-INST-A+W Business Production Manager.docx                   47
Figure 31: Formula search



    •    Click the [Search] button.
    •    Check whether the formula 9008 – Automatic transfer to AWB Capa exists.
              o   If not, click the [New] button.
              o   Switch to the Formula tab.




10.12.2021                       EN-INST-A+W Business Production Manager.docx      48
Figure 32: Workflow-task configuration – Formula

             o    Enter the number 9008.
             o    Enter the description Automatic transfer to AWB Capa.
             o    As formula, enter the content of the file C:\Program Files (x86)\A+W\ALFAK
                  2012\Formula\ Workflow_TransferToCapacityPlanning.txt which you can copy
                  entirely from this file.
             o    Click [Save].
    •    Click [Close].
    •    Call Master data > Company > Customizing, tab 3. Workflow tasks. Workflow tasks.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                49
Figure 33: Workflow task configuration – Workflow task

    •    Check whether the workflow task Workflow task for AWB Capa – 9008 – Automatic transfer
         to AWB Capa is available.
             o    If not, click the [New] button.
             o    Enter the description Workflow task for AWB Capa.
             o    Select the formula 9008 - Automatic transfer to AWB Capa.
             o    Click [Save].
    •    Switch to tab 4. Autom. process execution.




10.12.2021                         EN-INST-A+W Business Production Manager.docx              50
Figure 34: Workflow task configuration – Autom. process execution

    •    Check whether the workflow task Workflow task for AWB Capa is available at the desired
         interval and in the execution 00 - cyclical.
             o    If not, click the [New] button.
             o    Select the workflow task to be set up.
             o    Do not change the pre-set sequence.
             o    Enter the required interval, e.g. 00:01 for minute-based execution.
             o    Leave the execution 00- cyclic.
             o    Click [Save].
    •    Click [Close].
    •    The cyclical execution of the transfer to A+W Business capacity planning can be checked
         with the A+W Business 6 Service Monitor l.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                    51
4.7 Create workflow task for archiving production manager jobs
A workflow task has to be set up in order to ensure that the finished orders of the Production
Manager are transferred automatically to the archive.
    •    Call Master data > Company > Formulas.




Figure 35: Formula search



    •    Click the [Search] button.
    •    Check whether a formula such as the Workflow task AWBPRO Archiving Jobs exists.
              o   If not, click the [New] button.
              o   Switch to the Formula tab.




10.12.2021                       EN-INST-A+W Business Production Manager.docx                    52
Figure 36: Workflow task configuration – Formula

             o    Enter any formula number.
             o    Enter a description such as Workflow Task AWBPRO Archiving Jobs.
             o    As formula, enter the content of the file C:\Program Files (x86)\A+W\Business
                  6\Formula\ Workflow_ArchiveProductionManager.txt which you can copy from
                  this file.
             o    Click [Save].
    •    Click [Close].
    •    Call Master data > Company > Customizing, tab 3. Workflow tasks. Workflow tasks.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                   53
Figure 37: Workflow-Task configuration – Workflow task

    •    Check whether a workflow task such as, e.g.
         Workflow-task AWBPRO Archivierungsjobs - 9070 - Workflow-Aufgabe AWBPRO
         Archivierungsjobs is available.
             o    If not: Click [New].
             o    Enter a description like Workflow Task AWBPRO Archiving Jobs.
             o    Select the created formula Workflow task AWBPRO Archiving jobs.
             o    Click [Save].
    •    Switch to tab 4. Autom. process execution.




10.12.2021                        EN-INST-A+W Business Production Manager.docx      54
Figure 38: Workflow-Task configuration – Autom. process execution

    •    Check whether a workflow task for archiving of the Production Manager orders is available,
         e.g. with a fixed execution time of 10:00 PM (hh:mm).
             o    If not, click the [New] button.
             o    Select the workflow task to be set up.
             o    Decide whether the workflow task should be executed at a fixed poin in time or
                  cyclically, e.g. every 10 hours.
             o    Click [Save].
    •    Click [Close].
    •    The execution of archived Production Manager jobs can be checked with the A+W Business
         6 Service Monitor I.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                    55
4.8 Configuring machine drivers for cutting, bending, and sealing
A+W Business Pro uses the same driver and batch scripts like A+W Production. The main difference
is that A+W Business Pro uses the installed driver from the TRANS directory (e.g. P:\Release\) and
not the PROGRAMS directory.
For more information read the following documents which you will find in directory

AUW_Configuration_Cutting.docx

AUW_Configuration_sealer_bender.docx



4.9 Configure Bender text in AWBusiness


AWProduction creates the bender text. The bender text that is created by AWBusiness is used in
Business Pro.


You can set the bender text in the IGU under Master Data > Product > Products.
See this screenshot:




Figure 39: A+W Business bender text configuration



The 10000 marks the standard bender text (normally used). The character string between the < >
signs are the placeholders for bender text (See 5.9.1).


How to check the bender text in AWBusiness? Look at the next screenshot:




10.12.2021                         EN-INST-A+W Business Production Manager.docx                  56
Figure 40: A+W Business bender text check in order item



See the text under Spacer/Text (on right side). If there no text, you have to set the text at the IGU
product.
Look at the product 720. It’s the product from the first screen shot.


Flow:


A+W Production Manager writes the file AWISO.DAT. The file is used as input for the xt_awiso. The
AWISO.dat file contains a spacer section which contains the entry “Text=xxx” and this text is passed
into the bender driver file.
So make sure that there will be some frame text generated during order.


For your information:


AWBusiness text is limited to 80 characters.


4.9.1 Bender text placeholders




10.12.2021                         EN-INST-A+W Business Production Manager.docx                         57
The frame text can be assigned at the product and is reading a standard text. The text can
contain follow placeholders:


<pn> = Productnummer
<p1> = Productdescription 1
<p2>> = Sheets in units
<g> = Gas
<cn> = Customernumber
<c1> = Customername 1
<pd> = Productiondate
<no>> = Order no./Item no.
<wh> = Dimension
<ab> = Short description of frame
<vsg> = Lam short description
<esg> = Temp short description
<kp> = Customer position
<br> = width without leading 0 or blank
<ho> = height without aeration 0 or blank
<an> = ordern without leading 0 or blank
<ps> = Item no. without aeration 0 or blank
<po> = Item no. with aeration 0 or blank
<ak> = spacer type
<vs> = LAMI description
<sn> = keynumber
<gt> = CE code
<@Formelnummer@> = Execute your own formula




10.12.2021                   EN-INST-A+W Business Production Manager.docx                    58
Example :       „<c1> <p1> <p2> <wh> <no>“
Output :         „John+Partner Standard ISO FL4/18/ORN528 540x1030 109384/001


Also with order transfer
<kk> = Customer kommission
<jn>         jobnumber
<js>         production sequence



4.10 Realtime Optimizer (EL) stand-alone


4.10.1 Configuration of AWB Pro and Realtime Optimizer (EL) stand-alone


You can use the stand-alone Realtime Optimizer. You have to configure the XTV cutting driver for
cutting code in A+W Business under Capacity Planning->Master Data->Aggregate.




Figure 41: Configure XTV cutting code for Realtime Optimizer



The XTV driver saves the Opt2* file to directory as *.savefile. That do the XTV.bat (under
P:\Trans\Release\Tables\XTV). You can set the naming of the savefile. The stand-alone Realtime
Optimizer looks at this directory, opens the savefile and import the savefiles to a AWP database.

10.12.2021                          EN-INST-A+W Business Production Manager.docx                    59
The stand-alone Realtime Optimizer needs an empty AWP database. You have to configure the cfg
file (xopton_g.cfg! not xopton.ini) of the Realtime Optimizer. You have to set the AlcimVersion in
partition [Version] and the UseOpt2DatTableID in [Import] partition. The xopton_g.cfg is in the user
P:\Release\Save\ directory.


; .......................... [Import] ...................................
; This section is used only with the ALCIM Standalone version.
;
; UseOpt2DatTableID : <Boolean>, Default=N
;          Y will use the TableId of the Opt2Dat.dat to import Savefiles.
;          If the "TableId" is empty or has 4 blanks the table of
;          XOPTON.CFG will be used


You have to set the version for the stand-alone Realtime Optimizer (Version=2 in xopton_g. cfg).


; ............. Section for version .........................................
[Version]
AlcimVersion=2


You have to set the WorkingPath, ArchivePath, ProblemPath and SaveFileMask in the xopton.ini
partition [Import].




WorkingPath=P:\Prod\TB1
ArchivePath=P:\Prod\TB1\Archiv
ProblemPath =P:\Prod\TB1\Problem


SaveFileMask=Opt*.sav


The xopton_g. cfg is in follow directory which is defined in xopton.ini partition [Common]:


; XoptSavePath : <Valid path> : Default = Techsoft Server directory path from registry


10.12.2021                                   EN-INST-A+W Business Production Manager.docx          60
;                         + 'RELEASE\SAVE'
;      Path to the directory where the XOPTON_G.CFG, XOPT.CFG, OPT2TXT.DAT are located.
;       and the LABEL.SET are stored. All XOPTSAVE files should be stored
;       in this directory.
;       All instances of XOPTON must point to the same directory.


Please check the DeleteDBAfterDays (Default is 20 days) in the xOptOn.cfg file:


; ............. Section Import (Required only for standalone version).........
[Import]
DeleteDBAfterDays=5


FYI: This is the minimal configuration. There are many more switches.


4.10.2 Use as stand-alone system


A+W Realtime Optimizer is installed with an empty A+W Production database.
When batches are imported, the database is filled with master data.
The stand-alone system imports the data using memory files, which are generally made available in
a special directory by the A+W Realtime Optimizer. Save the files in order to stick to a defined
structure; these are usually available in the working directory.
...\Xopton\im-port\work\*save.*... Imported files are removed from the working directory and
transferred to the archive.


4.10.2.1 Importing optimizations


Importing the optimization functions is only required and valid for the stand-alone versions of the
A+W Realtime Optimizer.
A+W Realtime Optimizer can supply a cutting table with cutting data or create a table optimization if
batches are provided by another system. If batches are delivered, the A+W Realtime Optimizer can
import them for further processing.
The following steps can be performed in connection with the import of batches:



10.12.2021                        EN-INST-A+W Business Production Manager.docx                        61
• Switch on import
• Switch off import
• React to error reports


4.10.2.2 Switch on import


    1)   Open the Import dialog. Select View > Import.
    2)   Use the [Start] button to start the import.
    A+W Realtime Optimizer checks the working directory for import files. If import files are found,
    the data are imported into the database while the import files are transferred to archives.
    Imported batches are avaialble for the optimization on the Batch Selection and Select Glass
    dialogs for further processing.
    The [Start] button becomes [Stop].


    3)   Close the dialog. Press the [Close] button.
    A+W Realtime Optimizer monitors the working directory until the import function is switched
    off.
    Should errors occur during import, these are recorded; and the corresponding batches are not
    imported. Errors can be processed manually.3.01 / 01-2017


4.10.2.3 Switching off import


    1) Open the dialog Import. As long as import is switched on, a minimized dialog is shown in the
       bottom left corner of the A+W Realtime Optimizer dialog.
    2) Use the [Stop] button to end the import.
    Import files just stored in the working directory remain there, unprocessed.
    The [Stop] button changes to [Start].
    3) Close the dialog. Press the [Close] button.


4.10.2.4 Reacting to error reports




10.12.2021                     EN-INST-A+W Business Production Manager.docx                        62
Should errors occur during import, these are recorded; and the corresponding batches are not
imported.
Import is stopped only at an imminent loss of data. This can be the case if an existing optimization
should be overwritten. Depending on the configuration, an error message appears.


     1) Answer the question on the error report xopt-on dialog.
     Select the appropriate button, [Yes] or [No].
     Import of data is resumed.
     2)     Open dialog Error messages. Select menu View > Error reports.
     3)     Check the error messages and respond accordingly.


4.10.3 Configure RTO in AWB Pro environment (Some hints)


4.10.3.1 RTO shows the wrong glass article number


You can set this in the XOPTON.CFG and in theAlcimTools.ini.
XOPTON.CFG:
; .............. Section for views ...........................................
[View]
ShowArticlecodeForGlasArticle=Y


AlcimTools.ini:
[RUSH SHEETS]
ShowArticlecodeForGlasArticle=Y
; Yes displays the XOPT_ART.ARTNR instead of XOPT_ART.GLASART. Default=No


4.10.3.2 Create a manual plan


In order to create a manual plan, this has to be enabled in the XOPTON.CFG


; .............. Section for Input .................................


10.12.2021                                 EN-INST-A+W Business Production Manager.docx                63
[Input]
PLAN=Y


4.10.3.3 Shape 99 import


For shape 99 you can use the rush sheet input (AlcimTools)
You have to enable this in the Alcimtools.ini.


[RUSH SHEETS]
EnableForm99=Y
; Default: N
N -> Input of shape 99 "Block.zip/Block.ind" for rush sheets disabled
Y -> Input of shape 99 "Block.zip/Block.ind" for rush sheets activated
You can enable the input of priority.
Maybe you don't want to optimize shape 99 with priority 0.


[RUSH SHEETS]
EnableInputOfPrio=0,1
Enables the input of priorities listed in a combo box, but only values you have configured here. For
ex. 0,1,4
; Important: Do not take values greater than 4!


You will need a “block.pth” and the “Get99.dll” in the XOPTON program directory.


4.10.3.4 Using Opt2Dat Artnr as article number


You have to change the XOPTON.CFG:


[Import]
UseOpt2datArtnrAsGlasart=Y




10.12.2021                     EN-INST-A+W Business Production Manager.docx                            64
; UseOpt2datArtnrAsGlasart=<BOOL> Default=N
; UseOpt2datArtnrAsGlasart=N
;   The import will create a unique id for the field XOPT_ART.GLASART.
;   The Opt2dat headerrecord field "ARTNR" will be used for XOPT_ART..ARTNR.
; UseOpt2datArtnrAsGlasart=Y
;   The import is done using the Opt2dat-Kopfzeilenfeld "ARTNR".
;   as unique key the field XOPT_ART.GLASART. If the input
;   is not numeric, an import from the Savefile is not possible.


Now you may change the Articelcode and no new record for the will be created during the next
import.


4.10.3.5 Using the old breakage dialog


Made the following changes to the xopton.cfg for all the RTO user accounts


BreakageMode=1


[BrokenSheetPool]
Mode=0


4.10.3.6 Order numbers with more than 6 digits.


Change the entry to the XPTON.CFG:


[Import]
LabelSetOrder=ORDERNUMBER


If "LabelSetOrder" is not blank, there is an attempt to read the configured variable Label.set as
order number.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                         65
4.10.3.7 Use Hegla article code


The HEGLA article code should only appear in the HEGLA NC code and not somewhere else.


The A+W Production Manager has 2 opportunities to fill out the opt2dat ARTN:



    1)       If there is a technical article number, we use this. This is the field ALC_TECHART in the
             database table BA_PRODUKTE or at
             Master Data>Product>Products TAB4 Stock/Purchasing Text field Technical Product
             Code' (marked in red) in the AWB program.
             If you would like to set the technical product code, you have to set the supply type to
             Cutting/Zuschnitt (marked in green). See screenshot:




             Figure 42: Helga technical article code settings




    2)       If there no technical article number, we use the field BA_PRODUKT in the database table
             BA_PRODUKTE as fallback



4.10.3.8 Optimization number range in RTO and Production Manager


The RTO uses an optimization number that is higher than 9999. The optimization number range
have to be smaller than 10000 in the Production Manager settings. You have to set the ParameterID
= 2 in Prod_Parameter Table. Check 6.9 (Prod_Parameter Table), ParameterId 2


4.10.3.9 Remaster in AWB PRO / RTO enviroment


See RTO Configuration


10.12.2021                            EN-INST-A+W Business Production Manager.docx                       66
RTO currently writes no feedback file for residual plates. No sheet information (Order/Item)
will be passed to AWB for residual plates. In the section [FeedBackFile] wird a new flag
"ResidualPlates" is added. For "ResidualPlates=Y" a report file is also written for residual
plates. AWB will not find the stockplate size and has to ignore it. AWB will only use the
“Order/Itm” information of the sheet records.
You have to set WriteSheetRecord=N in [FeedBackFile] in order to write no sheets to the
report file. If you want send the Status order is cut, check ParameterID 27 for automatic
feedback.


4.10.3.10       RTO sends status feedback to Production Manager (#410492)
The following switch in the RTO Config file is used for this:
Partition
[BusinessPro Feedback]
Key
FeedbackFilePath=


The functionality is activated by entering a valid path in "FeedbackFilePath=" which can be accessed
by both the A+W Realtime Optimizer and the A+W Business Pro. If an optimization with the A+W
Business Pro optimization number 1045 was imported, as soon as the first sheet of the imported
A+W Business Pro optimization was cut, an empty file with the name "1045.300" is created in this
directory. If the last sheet was cut, an empty file with the name “1045.700“ is created so that A+W
Business Pro can remove the stockplates in A+W Business. The files will be deleted by A+W Business
Pro after the booking.
For your information
The path may not be the same as the one where the optimization save files are located.


The RTO has to be configured for the "New cutting process“ in this section.


[Cutting]
NewCuttingProcess=Y
Since years we develop new features only for the new cutting process.


Check the AWB Pro Configuration 7.3.14



10.12.2021                      EN-INST-A+W Business Production Manager.docx                      67
4.10.3.11         See incorrect batch number in RTO (# 445624)


Set the following switch in RTO Cfg file.
; ............. Import section (required only for standalone version).........
[Import]
UseOptrunForJob=N


The RTO shows the Production Manager order number in the ‘Batch’ column on the "Select batch"
dialog.




Figure 43: RTO batch number




4.11 Partial deliveries in AWB Pro


You have to enable this checkbox under Master Data->Company->Company Data




10.12.2021                        EN-INST-A+W Business Production Manager.docx                  68
Figure 44: AWB Pro Partial deliveries



If you do not set this switch, you will get some error messages.




10.12.2021                          EN-INST-A+W Business Production Manager.docx   69
5 Checking the installation and configuration
5.1 Checking storage place organization
The data under Master data > Manufacturing > Storage place organization are output as default
storage place organization by the setup via the script 20131009a.sql.
    •    Master data > Production > Storage place organization: A-rack and harp rack organization
         are place as well as an underlying set of rules.

5.2 Checking capacity planning
Capacity master data is available in the default database. Check if the following data is available in
particular.
    •    Capacity planning > Master data > Organization > Aggregates
             o   General: Options, additional options
             o   Restrictions: Technical restrictions, distances between cuts

5.3 Checking grinding allowances


        During batch creation, cutting correction to the glass will be calculated depending on edge
        processing articles that are assigned to edge processing machines. The program will issue a
        warning when coupling.
        Edge processing article/edge processing machine have no appropriate entry in the grinding
        allowance table.
        To avoid these messages, the grinding allowances table should be maintained before working
        with the system


    •    Check grinding allowance under Master data > Manufacturing > Cutting correction.
    •    Correction values should be set up for existing machines for the following processings;
         whereby the correction values depend on the glass thickness
             o   900 – Edging
             o   901 – Grinding
             o   902 – Polishing
             o   903 – Miter
             o   904 - Bevel




10.12.2021                      EN-INST-A+W Business Production Manager.docx                             70
5.4 Check BLOCK.pth and Opt2txt.dat
    •    In the directory C:\ProgramData\A+W\Techsoft\SN\User\Default, check whether the
         correct files Opt2txt.dat and Block.pth are there. If not, copy them from the directory
         Common from the Server Directory (P:\COMMON and see 3.7). The SN needs the
         Opt2txt.dat to get the block file measurements. SN reads the record 30 of the Opt2txt.dat
         file. The first four characters (1-4) define the internal measurements. That is, for example,
         the measurement of the block file. Characters 11-14 define the mapping of display. Follow
         values are possible for both entries in Opt2txt.dat:
    •    0000 = mm
    •    0005 = 0.2 mm
    •    0010 = 0.1 mm
    •    0020 = 0.01 mm
    •    0032 = 1/32 Inch
    •    0128 = 1/128 Inch
    •    The files will be copied to the %Appdata%\A+W\TECHSOFT\SN directory from the SN
         default user at the first SN start. SN needs the Block.pth to get the directory of the Block
         File. You could open the SN Config tool to see what for Block file SN uses.
    •    In the directory %Appdata%\A+W\TECHSOFT\SN, check whether the correct files
         Opt2txt.dat and Block.pth. If not, copy them from the directory Common from the Server
         Directory (see 3.7).
    •    The remaining user files are taken from the directory
         C:\ProgramData\A+W\Techsoft\SN\User\Default.



5.5 LABEL.SET
        The Production Manager uses entries in the LABEL.SET file
        ( original in directory P:\COMMON )


    These are the standard fields in the LABEL.SET file after the setup
        'ORDERNUMBER',1,10,0,'',-1,' /',3,77,0,'',0,0
        'JOBNUMBER',11,14,0,'',-1,' /',3,77,0,'',0,0
        'PARENTBOMID',15,17,0,'',-1,' /',3,77,0,'',0,0
        'BOMID',18,20,0,'',-1,' /',3,77,0,'',0,0
        'RACKTYPE',21,21,0,'',-1,' /',3,77,0,'',0,0


10.12.2021                      EN-INST-A+W Business Production Manager.docx                             71
      'SHEETS',22,22,0,'',-1,' /',3,77,0,'',0,0
      'XRENUM_SHEET_MAP',23,28,0,'',-1,' /',3,77,0,'',0,0
      'ALCIM_SCHEIBEN_PRO_FACH',29,29,0,'',-1,' /',3,77,0,'',0,0


These additional fields can be added dynamically by the program when needed.
(Cutting plan editing with PLANEDIT, for XOPTON, for ShapeOpt)


      'PLANEDIT',30,30,0,'',0,'',0,0,0,'',0,0
      'XOPTON_BOCK',31,31,0,'',-1,' /',3,77,0,'',0,0
      'ALCIM_BOCK',32,34,0,'',-1,' /',3,77,0,'',0,0
      'BYSHOW',35,50,0,'',-1,' /',3,77,0,'',0,0
      'NESTED_SHAPE',51,61,0,'',0,'',0,0,0,'',0,0


     If an optimization is saved, the file LABEL.SET and the files opt2*.dat belong to the set of files
that are packed together and saved in the database.


5.6 Meaning of variables in formulas

Enclosed a list of all variables which can be used in the formulas within the rack organization part
for testing, sorting, grouping ( Menu master data, production, criteria )
When comparing strings, the string value must be put in single strokes
Example: ProductGroup=='200'

In A+W Business, the fields SealingType, SpacerType, SpacerColor are specified in the spacer article
of an IGU ( the first spacer )




Figure 45: A+W Production Manager spacer code




However, the above mentioned spacer related variables, are available as variables in the IGU rack
organization


10.12.2021                       EN-INST-A+W Business Production Manager.docx                             72
Name                   Type                 Meaning                  Values / Example
                       Int32                Batch type of the        100 = Single Glass, tempered glass or glasses with
LotType
                                            item                     processings
                                                                     200 = Laminated Glass
                                                                     300 = Insulated Glass
                                                                     0 = Other
                       String               Location in bill of      Example:
BomPosition
                                            material                 1.2 means: Second sub item of first sub item of
                                                                     head item.
                       Int32                Product code of the      BW_AUFTR_POS.PROD_ID or
Product
                                            item                     BW_AUFTR_STKL.BOM_PRODUKT
                       Int32                Procurement type of      BW_AUFTR_POS.
Procurement
                                            the item                 BW_AUFTR_POS.FER_BESCHAFFARTNR or
                                                                     BW_AUFTR_STKL.FER_BESCHAFFARTNR
                       Int32                Order number             BW_AUFTR_POS.ID or BW_AUFTR_STKL.ID
OrderNumber
                       Int32                Item number              BW_AUFTR_POS.POS_NR
LineItem
                       Int32                Level in bill of         BW_AUFTR_STKL.BOM_LEVEL
BomLevel
                                            material
                       Int32                Item number in level     BW_AUFTR_STKL.BOM_POS
BomPos
                                            in bill of material
                       Int32                Item number in bill      BW_AUFTR_STKL.BOM_ID
BomId
                                            of material
                       Nullable<Int32>      Item number of           BW_AUFTR_STKL.BOM_NODE
ParentBomid
                                            parent item in bill of
                                            material
                       String               First description text   BW_AUFTR_POS.PROD_BEZ1 or
ProductDescription1
                                            for product of item in   BW_AUFTR_STKL.STL_BEZ
                                            bill of material
                       String               Second description       BW_AUFTR_POS.PROD_BEZ2
ProductDescription2
                                            text for product of
                                            item in bill of
                                            material (available
                                            only for head items)
                       String               Short description of     BW_AUFTR_POS.PROD_KURZ_BEZ or
ShortInfo
                                            item in bill of          BW_AUFTR_STKL.STL_KURZ_BEZ
                                            material
                       Decimal              Amount of item in        BW_AUFTR_POS.PP_MENGE or
Quantity
                                            bill of material         BW_AUFTR_STKL.STL_MENGE
                       Decimal              Width of the item in     BW_AUFTR_POS.PP_BREITE or
Width
                                            bill of material.        BW_AUFTR_STKL.STL_BREITE



          10.12.2021              EN-INST-A+W Business Production Manager.docx                               73
                       Decimal              Height of the item in     BW_AUFTR_POS.PP_HOEHE or
Height
                                            bill of material.         BW_AUFTR_STKL.STL_HOEHE
                       Decimal              Thickness of the item     BW_AUFTR_POS.PP_DICKE or
Thickness
                                            in bill of material       BW_AUFTR_STKL.STL_DICKE
                       Decimal              Area of item in bill of   BW_AUFTR_POS.PP_QM (for head items) or
Area
                                            material                  BW_AUFTR_STKL.STL_QM (for all other items)
                       Decimal                                        BW_AUFTR_POS. STL_QM_FAKT (for head items)
InvoiceArea                                 Invoice area of the
                                                                      or BW_AUFTR_STKL.PP_QM_FAKT (for all other
                                            sheets
                                                                      items) PP_QM_FAKT (for all other items)
                       Int32                Shape Number of           BW_AUFTR_MODELL.MOD_NUMMER
ShapeNumber
                                            item in bill of
                                            material
                       Int32                Product Type of item      BW_AUFTR_POS.PROD_PRODART or
ProductType
                                            in bill of material       BW_AUFTR_STKL.STL_PRODART
                       Int32                Product Class of item     BW_AUFTR_POS.PROD_PRODGRP or
ProductClass
                                            in bill of material       BW_AUFTR_STKL.STL_PRODGRP
                       String               Product Group of          BW_AUFTR_POS.PROD_WGR or
ProductGroup
                                            item in bill of           BW_AUFTR_STKL.STL_WGR
                                            material
                       Int32                Product type of           BW_AUFTR_POS.PROD_PRODART or
ParentProductType
                                            parent item in bill of    BW_AUFTR_STKL.STL_PRODART
                                            material
                       DateTime             Production date of        ZW_AUFTR_ZEIT.DATUM_PROD
ProductionDate
                                            item in bill of
                                            material
                       Nullable<Int32>      ID of the machine         ZW_AUFTR_ZEIT.AGG
Aggregate
                                            that was assigned by
                                            capacity planning.
                       String               Description of the        ZW_AGGREGATE.AGG_BEZ
AggregateDescription
                                            aggregate, which was
                                            assigned by capacity
                                            planning.
                       Int32                Position of coating       BW_AUFTR_POS.FER_BESCHICH_SEITE or
CoatingPosition
                                                                      BW_AUFTR_STKL.FER_BESCHICH_SEITE
                       Int32                Position of structure     BW_AUFTR_POS.FER_STRUKTURSEITE or
StructurePosition
                                                                      BW_AUFTR_STKL. FER_STRUKTURSEITE
                       Int32                Direction of structure    BW_AUFTR_POS.FER_STRUKTURVERL or
StructureDirection
                                                                      BW_AUFTR_STKL .FER_STRUKTURVERL
                                                                      BW_AUFTR_POS.FER_STRUKTURVERL or
                                                                      BW_AUFTR_STKL .FER_STRUKTURVERL
                       Boolean              Indicate whether the      True = unit includes steps
Step
                                            unit includes steps.      False = unit does not include steps



         10.12.2021               EN-INST-A+W Business Production Manager.docx                              74
                                                                Checks for products with product type 12 and
                                                                product class 50 in the BOM.
                    Boolean             Identify if the unit    True = unit includes muntins
GeorgianBars
                                        includes muntins.       False = unit includes no muntins
                                                                Checks for products with product type 11
                    String              Sealing type of first   Second character of BA_PRODUKTE.FER_SZR_KZ
SealingType1
                                        frame in IG unit
                    String              Sealing type of         Second character of BA_PRODUKTE.FER_SZR_KZ
SealingType2
                                        second frame in IG
                                        unit
                    String              Sealing type of third   Second character of BA_PRODUKTE.FER_SZR_KZ
SealingType3
                                        frame in IG unit
                    Int32               First processing        ZW_AUFTR_ZEIT.AGG sorted by
Machine1
                                        machine after           ZW_AUFTR_ZEIT.RFOZ
                                        cutting.
                    Int32               Second processing       ZW_AUFTR_ZEIT.AGG sorted by
Machine2
                                        machine after           ZW_AUFTR_ZEIT.RFOZ
                                        cutting.
                    Int32               Third processing        ZW_AUFTR_ZEIT.AGG sorted by
Machine3
                                        machine after           ZW_AUFTR_ZEIT.RFOZ
                                        cutting.
                    Int32               Fourth processing       ZW_AUFTR_ZEIT.AGG sorted by
Machine4
                                        machine after           ZW_AUFTR_ZEIT.RFOZ
                                        cutting.
                    Int32               Fifth processing        ZW_AUFTR_ZEIT.AGG sorted by
Machine5
                                        machine after           ZW_AUFTR_ZEIT.RFOZ
                                        cutting.
                    Int32               Product code of the     BW_AUFTR_STKL.BOM_PRODUKT
ProcessArticle1
                                        first processing
                                        machine after
                                        cutting.
                    Int32               Product code of the     BW_AUFTR_STKL.BOM_PRODUKT
ProcessArticle2
                                        second processing
                                        machine after
                                        cutting.
                    Int32               Product code of the     BW_AUFTR_STKL.BOM_PRODUKT
ProcessArtice3
                                        third processing
                                        machine after
                                        cutting.
                    Int32               Product code of the     BW_AUFTR_STKL.BOM_PRODUKT
ProcessArtice4
                                        fourth processing
                                        machine after
                                        cutting.
                    Int32               Product code of the     BW_AUFTR_STKL.BOM_PRODUKT
ProcessArtice5
                                        fifth processing




       10.12.2021             EN-INST-A+W Business Production Manager.docx                            75
                                            machine after
                                            cutting.
                        Int32               Product class of the     BW_AUFTR_STKL.STL_PRODGRP
ProcessProductClass1
                                            first processing after
                                            cutting.
                        Int32               Product class of the     BW_AUFTR_STKL.STL_PRODGRP
ProcessProductClass2
                                            second processing
                                            after cutting.
                        Int32               Product class of the     BW_AUFTR_STKL.STL_PRODGRP
ProcessProductClass3
                                            third processing after
                                            cutting.
                        Int32               Product class of the     BW_AUFTR_STKL.STL_PRODGRP
ProcessProductClass4
                                            fourth processing
                                            after cutting.
                        Int32               Product class of the     BW_AUFTR_STKL.STL_PRODGRP
ProcessProductClass5
                                            fifth processing after
                                            cutting.
                        String              Product group of the     BW_AUFTR_STKL.STL_WGR
ProcessProductGroup1
                                            first processing after
                                            cutting.
                        String              Product group of the     BW_AUFTR_STKL.STL_WGR
ProcessProductGroup2
                                            second processing
                                            after cutting.
                        String              Product group of the     BW_AUFTR_STKL.STL_WGR
ProcessProductGroup3
                                            third processing after
                                            cutting.
                        String              Product group of the     BW_AUFTR_STKL.STL_WGR
ProcessProductGroup4
                                            fourth processing
                                            after cutting.
                        String              Product group of the     BW_AUFTR_STKL.STL_WGR
ProcessProductGroup5
                                            fifth processing after
                                            cutting.
                        Decimal             Airspace of the first    BW_AUFTR_STKL.STL_DICKE
Airspace1
                                            frame.
                        Decimal             Airspace of the          BW_AUFTR_STKL.STL_DICKE
Airspace2
                                            second frame.
                        Decimal             Airspace of the third    BW_AUFTR_STKL.STL_DICKE
Airspace3
                                            frame.
                        Int32               Number of sheets in
NumberSheetsInUnit
                                            the unit.
                        Decimal             Total of the
ThicknessSheetsinUnit
                                            thicknesses of all
                                            sheets in the unit.
                        String              List of distinct         Example:
DistinctSheetsInUnit
                                            products in unit         IG with three sheets (104, 106, 104)
                                            (separated by ;)         Result: 104;106



       10.12.2021                 EN-INST-A+W Business Production Manager.docx                              76
                          Int32               Number of tempered
TemperedInUnit
                                              sheets in the unit.
                          Nullable<DateTime   Delivery date           BW_AUFTR_KOPF.DATUM_ANLIEFERUNG
DeliveryDate
                          >
                          Int32               CustomerNumber          BW_AUFTR_KOPF.AH_IDENT
CustomerNumber
                          String              Route                   BW_AUFTR_KOPF.OR_TOUR
Route
                          Int32               Number of coated
CoatedInUnit
                                              sheets in the unit.
                          Int32               Number of
StructuredInUnit
                                              structured sheets in
                                              the unit.
                          String              Type of the first       Third character of BA_PRODUKTE.FER_SZR_KZ
SpacerType1
                                              frame in the IG unit
                          String              Type of the second      Third character of BA_PRODUKTE.FER_SZR_KZ
SpacerType2
                                              frame in the IG unit


                          String              Type of the third       Third character of BA_PRODUKTE.FER_SZR_KZ
SpacerType3
                                              frame in the IG unit


                          String              Color of the first      The value depends on existing color variants of
SpacerColor1
                                              frame in the IG unit.   the spacer article



                                              Color of the second     The value depends on existing color variants of
SpacerColor2              String                                      the spacer article.
                                              frame in the IG unit.

                          String              Color of the third      The value depends on existing color variants of
SpacerColor3
                                              frame in the IG unit.   the spacer article

                          Boolean             Order Item contains     True = Bill of Material contains at least one item
LeadedItem
                                              at least one item of    with product type 13
                                              product type 13         False = Bill of Material does not contain an item
                                              (leaded product)        with product type 13
                          String              Fifth item text in      BW_AUFTR_POS.POS_TEXT5
ItemText5
                                              order item line
                          Int32               Production Line of      BW_AUFTR_POS.FER_LINIE
ItemProdLine
                                              order line item.
                          Decimal             Max. thickness of a     BW_AUFTR_POS.PP_DICKE or
MaxThicknessSheetInUnit
                                              sheet in the unit       BW_AUFTR_STKL.STL_DICKE
                          Decimal             Min. thickness of a     BW_AUFTR_POS.PP_DICKE or
MinThicknessSheetInUnit
                                              sheet in the unit       BW_AUFTR_STKL.STL_DICKE
                          String              Name of the number      BW_NUMVERW.NV_NAME
NumberManager
                                              manager                 BW_NUMVERW.NV_NAME




        10.12.2021                  EN-INST-A+W Business Production Manager.docx                               77
                          Int32             Sort id of document      BW_NUMVERW.NV_SORTID
NumberManagerSortID
                                            number                   BW_NUMVERW.NV_SORTID
                          Int32             Product type             ProductType of root item (IGU, LGU or Tempered
EndProductType
                                            root/header glass        glass/single glass)
                                            (For description see     BW_AUFTR_POS.PROD_PRODART
                                            Figure)
                          Int32             Max number of Lisec      Max number of BW_AUFTR_STKL.LIORDER_NR
MaxValueOfBomProdLine
                                            order number             Only if IGU or LGU.
                          Int32             Lisec order number       BW_AUFTR_STKL. BW_AUFTR_STKL.LIORDER_NR
BomProdLine
                          Int32             Number of different
NumberOfDifferent-
                                            processing machines
MachinesForProcessings
                                            for item
                          Int32             Number of different
NumberOfDifferent-
                                            processing machines
MachinesForProcessings-
                                            for parent part of the
OfParent
                                            item
                          Int32             Tour order number        SYSADM.BW_AUFTR_KOPF.
TourOrder
                                                                     TOUREN_RANGFOLGE
                          Int32             Number of sheets
NumberOfSheetsWith-
                                            with processing in
ProcessingInUnit
                                            unit (sheets have to
                                            have the batch type
                                            = 100 (SingleGlass)).
ParentProductClass        Int32             Product class of the     BW_AUFTR_POS.PROD_PRODGRP or
                                            parent part in the       BW_AUFTR_STKL.STL_PRODGRP
                                            BOM (0 = no product
                                            class);
                                            For description see
                                            Figure)
GrandParentProductClass   Int32             Product class of the     BW_AUFTR_POS.PROD_PRODGRP or
                                            grandparent item in      BW_AUFTR_STKL.STL_PRODGRP
                                            the BOM (0 = no
                                            product class);
                                            For description see
                                            Figure)
EndProductClass           Int32             Product class            BW_AUFTR_POS.PROD_PRODGRP or
                                            root/header glass        BW_AUFTR_STKL.STL_PRODGRP
                                            (For description see
                                            Figure)
GrandParentProductType                      Product type of the      BW_AUFTR_POS.PROD_PRODART or
                          Int32
                                            grandparent item in      BW_AUFTR_STKL.STL_PRODART
                                            the BOM (0 = no
                                            product class);
                                            For description see
                                            Figure)


       10.12.2021                 EN-INST-A+W Business Production Manager.docx                            78
A example to describe Grandparent, parent and Endproduct type or class




Figure 46: Describes grandparents, parents, end product type or class

                                   String                   Third Item text in order item line    BW_AUFTR_POS.POS_TEXT3
ItemText3

                                   String                   Fourth Item text in order item line   BW_AUFTR_POS.POS_TEXT4
ItemText4

                                   String                   Customer item from position           BW_AUFTR_POS.
CustomerItem
                                                                                                  POS_KUNDENPOS
                                   String                   Commission reference from item        BW_AUFTR_POS.
CommissionReference
                                                                                                  POS_KOMMISSION




        10.12.2021                           EN-INST-A+W Business Production Manager.docx                          79
Figure 47: Customer item and commission reference in AWB

                                  Int32                    Project number from order or offer   BW_AUFTR_KOPF.
ProjectNumber
                                                                                                KO_OBJEKT_KUNDE
                                  Int32                    Number of laminated glass in
NumberOfLaminatedGlassInI
                                                           Insulated unit.
nsulatedUnit




Figure 48: ProjectNumber in AWB




        10.12.2021                        EN-INST-A+W Business Production Manager.docx                        80
RouteNumber            String                         RouteNumber                KA_TOUREN.TOUR_NR

Machine1AfterCutting   Int32                          First unique processing    ZW_AUFTR_ZEIT.AGG sorted
                                                      machine after cutting.     by ZW_AUFTR_ZEIT.RFOZ

Machine2AfterCutting   Int32                          Second unique processing   ZW_AUFTR_ZEIT.AGG sorted
                                                      machine after cutting.     by ZW_AUFTR_ZEIT.RFOZ

Machine3AfterCutting   Int32                          Third unique processing    ZW_AUFTR_ZEIT.AGG sorted
                                                      machine after cutting.     by ZW_AUFTR_ZEIT.RFOZ

Machine4AfterCutting   Int32                          Fourth unique processing   ZW_AUFTR_ZEIT.AGG sorted
                                                      machine after cutting.     by ZW_AUFTR_ZEIT.RFOZ

Machine5AfterCutting   Int32                          Fifth unique processing    ZW_AUFTR_ZEIT.AGG sorted
                                                      machine after cutting.     by ZW_AUFTR_ZEIT.RFOZ




       10.12.2021               EN-INST-A+W Business Production Manager.docx                     81
5.7 Description of values for fields BOM_ID, BOM_POS, BOM_NODE and
    BOM_LEVEL

    BW_AUFTR_POS                                    IG                      BW_AUFTR_STKL



    1             TG        1                      Frame     2               LG    3
              0           1                    0             2          0          3




    2             Float 1                                    TG     2       Foil   3       Float 4
              1           4                              3         5    3          6   3       7




    3                                                        Float 1
                                                         5         8


 BOM_LEVEL                               BOM_ID                         BOM_POS            BOM_NODE
Figure 49: A+W Business item structure




5.8 Implementation of markings for drilled holes or cut-outs


First, you have to set a SN.INI Value for drilled hole or cut-out marking.
Set the value UNICUTremoveInsideContours in section [VIEW] to UNICUTremoveInsideContours = 0


Second, see under 6.9 ParameterID 18 to set the right value in the Database.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                      82
FYI: If you want to export corner rounding on the cutting table, you have to set the SN.INI value.


Partition [USER], Value ExecuteTechnologicalRoundingsInCutTechnologies = 1


The Production Manager set the values for the block export.



5.9 Configuration via table PROD_PARAMETER
       The database table PROD_PARAMETER contains certain configuration parameters for the
       Production Manager which can be modified by A+W service personal

       The parameter ID14 (reset rack number) is obsolete since Release 12.5 Build 2157. See
       #327524




Figure 50: A+W Production Manager PROD_PARAMETER table

       The Production Manager Config Tool has a new Tab since Version 6. You can change the
Prod_Parameter Values via this Tab and not only via SQL statements. Here is a picture from this Tab:




10.12.2021                     EN-INST-A+W Business Production Manager.docx                          83
Figure 51: A+W Production Manager Config Tool to update PROD_PARAMETER table



You can change all black text (e. g. green marking) entries. The gray texts (e. g. yellow marking) are
disabled and you can not change this entries.


     Meaning of the individual fields (primary key is PARAMETERID)
 PARAMETE Description
 RID
             Range of job numbers in order mode
 1



10.12.2021                      EN-INST-A+W Business Production Manager.docx                         84
             INTVALUE1 = Min. job number
             INTVALUE2 = Current job number
             INTVALUE3 = Max job number
             Range of optimization numbers in order mode
 2

             INTVALUE1 = Min. optimization number
             INTVALUE2 = Current optimization number
             INTVALUE3 = Max. optimization number

 3           Setting of the optimization of the cutting labels (optimization performance)

             INTVALUE1 = quantity for series (high quantity)
             INTVALUE2 = 1 print one label per item for series products
                         = 2 print one label per INTVALUE3 sheets with series products.
             INTVALUE3 = packaging quantity with INTVALUE2=2=2
             STRVALUE1 = identifier if cutting labels should only be printed for all optimized
             sheets or only for processed sheets (Lostyp=100).

             When calling the report Prodman_CuttingLabel_Optimisation.rpt the value of the
             field STRVALUE1 is passed as parameter CONFIGPARAMETER to the report. If the
             string STRVALUE1 contains the string DO_NOT_CHECK_LOTTYPE, then labels are
             also printed for sheets with lot type=0 (for example non processed Float in IG). The
             default string is zero or empty.

 4           Setting of the cutting label manual cutting (job output)

             INTVALUE1 = quantity for series (high quantity)
             INTVALUE2 = 1 print one label per item for series products
                        = 2 print one label per INTVALUE3 sheets for series products
             INTVALUE3 = packaging quantity for INTVALUE2=2=2
             STRVALUE1 = ID if cutting labels should be printed for all optimized sheets or only
             for processed sheets (Lostyp=100).

             When calling the report Prodman_CuttingLabel_Handcut.rpt the value of the field
             STRVALUE1 is passed as parameter CONFIGPARAMETER to the report If the string
             STRVALUE1 contains the string DO_NOT_CHECK_LOTTYPE, then labels are also
             printed for sheets with lot type=0 (for example non processed Float in IG). The
             default string is zero or empty.

 5           Setting production label for laminated glass (job output)

             INTVALUE1 = Quantity for series ( high quantity )
             INTVALUE2 = 1 Print one label per item for high quantity item


10.12.2021                  EN-INST-A+W Business Production Manager.docx                           85
                       = 2 Print one label per INTVALUE3 sheets when high quantity item
             INTVALUE3 = Packaging quantity when INTVALUE2=2

 6           Setting of the dispatch label for IG (job output)

             INTVALUE1 = quantity for series (high quantity)
             INTVALUE2 = 1 print one label per item for series products
                       = 2 print one label per INTVALUE3 sheets for series products.
             INTVALUE3 = Packaging quantity when INTVALUE2=2

 7           Shape drawing in the manual cutting list

             INTVALUE1 = width of the drawing
             INTVALUE2 = height of the drawing
             INTVALUE3 = color depth
             DECVALUE1 = filling (1.0) otherwise no filling
             DECVALUE2 = display side view (1.0 = yes)
             DECVALUE3 = set grayscales (1.0 = yes)
             STRVALUE1 = Format: emf, jpg, png, bmp, bmp, gif

 8           Shape drawing in IGU and LAMI production list

             INTVALUE1 = Width of drawing
             INTVALUE2 = Height of drawing
             INTVALUE3 = Color depth
             DECVALUE1 = Filling (1.0) otherwise no filling
             DECVALUE2 = Show side view (1.0 = yes)
             DECVALUE3 = Create gray steps (1.0 = yes)
             STRVALUE1 = Format: emf, jpg, png, bmp, gif
             Shape drawing on the shipping label
 9

             INTVALUE1 = Width of drawing
             INTVALUE2 = Height of drawing
             INTVALUE3 = Color depth
             DECVALUE1 = Filling (1.0) otherwise no filling
             DECVALUE2 = Show side view (1.0 = yes)
             DECVALUE3 = Create gray steps (1.0 = yes)
             STRVALUE1 = Format: emf, jpg, png, bmp, gif
             Additional value for the frame length in the spacer list Prodman_Spacerlist.rpt
 10
             DECVALUE1 = this value is added to the actual length of the spacer.
             Automatic setting of optimization groups
 11
             INTVALUE1 = 0 Change of optimization group doesn’t care the jobnumber


10.12.2021                  EN-INST-A+W Business Production Manager.docx                       86
                         =1 a new job gets a new optimization group.
             Shape drawing in the list of cutting labels
 12

             INTVALUE1 = Width of drawing
             INTVALUE2 = Height of drawing
             INTVALUE3 = Color depth
             DECVALUE1 = Filling (1.0) otherwise no filling
             DECVALUE2 = Show side view (1.0 = yes)
             DECVALUE3 = Create gray steps (1.0 = yes)
             STRVALUE1 = Format: emf, jpg, png, bmp, gif
             Shape drawing of the processing list
 13

             INTVALUE1 = Width of drawing
             INTVALUE2 = Height of drawing
             INTVALUE3 = Color depth
             DECVALUE1 = Filling (1.0) otherwise no filling
             DECVALUE2 = Show side view (1.0 = yes)
             DECVALUE3 = Create gray steps (1.0 = yes)
             STRVALUE1 = Format: emf, jpg, png, bmp, gif
             Rack numbering
 14
             Possibility to start always with the same rack number for a new job (when record
             with PARAMETERID=14 doesn’t exist, the default behavior is to continue with next
             rack number inside range - see AWDESK 325244 Anatoli )

             STRVALUE1 contains the list of logical racks (separated by ,) for which the rack
             numbering should always start with the min. rack number.

             As Release 12.5 Build 2157 (= Version 5.5 Update 2) deprecated. See #327524.
             Now, you can set this option with the logical rack dialog from AWB. See #327524.
             Range of job numbers in offer mode
 15

             INTVALUE1 = Min. Job Number
             INTVALUE2 = Current Job Number
             INTVALUE3 = Max. Job Number
             Range of optimization numbers in quotation mode
 16

             INTVALUE1 = Min. optimization number
             INTVALUE2 = Current optimization number
             INTVALUE3 = Max. optimization number
             Range of breakage job numbers in order mode
 17


10.12.2021                  EN-INST-A+W Business Production Manager.docx                        87
             INTVALUE1 = Min. breakage job number
             INTVALUE2 = Current breakage job number
             INTVALUE3 = Max breakage job number
             Marking drilled holes
 18
             INTVALUE1 = 1, otherwise not marking drilled holes
             (See #345910 or 6.8)

             Marking cut-outs
             INTVALUE2 = 1, otherwise not marking cut-outs
             (see, #408035 or 6.8)

             Export corner rounding for cutting tables
             INTVALUE3 = 1, otherwise do not export corner roundings (see, #409300 or 6.8)

             Add different marking for different aggregates
             STRVALUE1 = 1000,1,0,1;1020,0,1,1;1030…
             The aggregate ID is the first entry. The next 3 entries are the different markings.
             These 4 entries are separated with comma ‘,’.
             First marking is the drilled hole marking 0 = off and 1 = on.
             Second marking is the cut-out marking 0 = off and 1 = on.
             Third marking is the corner rounding marking 0 = off and 1 = on.
             If you add a new machine with marking entry, you have to add a semicolon '; '; '
             after the last entry.
             Shape drawing in the list of manual cutting labels
 19

             INTVALUE1 = Width of drawing
             INTVALUE2 = Height of drawing
             INTVALUE3 = Color depth
             DECVALUE1 = Filling (1.0) otherwise no filling
             DECVALUE2 = Show side view (1.0 = yes)
             DECVALUE3 = Create gray steps (1.0 = yes)
             STRVALUE1 = Format: emf, jpg, png, bmp, gif
             (Version 5.5 update 2 feature. You get the new report from Wolfram Brecht, see
             #351540)
             INTVALUE1 = ID to indicate additional processing texts. 0 is the default and no
 20
             processing text is displayed. The processing text is displayed if the value is 1 (see
             #357127). The additional text will only shown for edge processing (2016/v13). See
             this Picture:




10.12.2021                  EN-INST-A+W Business Production Manager.docx                             88
             Figure 52: Additional processing text (edge processing)

             INVALUE1 = Flag to set the xopt optimization mode for lot type float. If the value is
 21
             1, the batch type is optimized in xopt mode. If the value is 0, the batch type is
             optimized in xopts mode. Default is 1.
             INTAVLUE2 = Flag for laminted glass unit lot type (0 = xopts mode, 1 = xopt mode).
             Default is 0.
             INTAVLUE3 = Flag for insulated glass unit lot type (0 = xopts mode, 1 = xopt mode).
             Default is 0.
             Values for reducing the width or height of the residual plate.
 22

             DECVALUE1 = reduce residual plate width
             DECVALUE2 = reduce residual plate height

             Value have to be in the metric measurement: millimeter. Please, take positv values
             to decrease the width or height of the plate.

             You can substract the bottom trim from the height of residual plate to get the
             smaller plate

             INTVALUE1 = 0 (do not substract and is default)
             INTVALUE1 = 1 (substract the trim and get the smaller residual plate)
             Machine ID to print cutting labels via machine driver
 23

             STRVALUE1 = AggregateId/MachineID for print a label.dat via report (labelDat.rpt)

             Value is comma separated to write more than one machine. E. g. the value could
             be 1000, 1005. Please use only 4 digits for the aggregateId/MachineID. (See
             7.3.10)

             STRVALUE2 = AggregateId/MachineID for print a PrintCuttingLabels.pdf via report
             (PrintCuttingLabels[AggregateId].rpt)

             Value is comma separated to write more than one machine. E. g. the value could
             be 1000, 1005. Please use only 4 digits for the aggregateId/MachineID. (See
             7.3.10). Every machine could have a own PrintCuttingLabel.rpt named
             PrintCuttingLabels[AggregateId].rpt. E. g. if the aggregate Id 1000, the report file is
             is PrintCuttingLabels1000.rpt




10.12.2021                    EN-INST-A+W Business Production Manager.docx                             89
             Label setting for additional glass in job output (see # 404089)
 24

             You get all glass with
             PRODUKTART in (1, 2, 3, 50) and
             LOTTYPE in (0, 100, 300) and
             FER_BESCHAFFARTNR not in (0, 102)

             That means you the Production Manager writes all stock items, order item and
             customer own glass into DR_SESSION table and the report can choose the items
             needed. The identifier is ADDITIONALGLASS in column CHAR_COL2 in table
             DR_SESSION for the report data which needed for the report.
             The new report has the ID 824 and is named ProdMan-AdditionalGlass.rpt. The ID
             in table DR_DRUCKPUNKTE and PUNKTE_ID in DR_REPORTE must have the same
             value 824.

             It exists the sql update script 20171019a to insert the data into the DB tables and
             we create a new report PROD_ADDITIONALGLASS.rpt, which will deployed with the
             AWB setup. If there is no report in the AWB Report directory, you can use an old
             version. Ask MST or JSE for the new Report.




             Figure 53: DR_DRUCKPUNKTE Table ID 824




             Figure 54: DR_REPORTE Table ID 824

             Laminted glass has the lot type 100 and not 200 (= means produced laminated
             glass)
             The quotation mode do not use this report and items. We do not anymore insert
             the items (stock items, order item and customer own glass) into the production
             sequence in offer and order mode.

             Parameter for ID 24:

             INTVALUE1 = quantity for series (high quantity)
             INTVALUE2 = 1 print one label per item for series products
                       = 2 print one label per INTVALUE3 sheet for series.
             INTVALUE3 = Packaging quantity when INTVALUE2=2
             Define the base archive folder path with STR1VALUE
 25
             The default is the AWB file attachment path from the AWB master data. See 7.3.16



10.12.2021                   EN-INST-A+W Business Production Manager.docx                      90
 26          Wizard mode settings (#437306)


             INTVALUE1 = 1 pause after job creation in quotation mode. 0 is the default and
             does the detailed scheduling and an optimization.

             INTVALUE2 = 1 pause after job creation in quotation mode. 0 is the default and
             does the detailed scheduling and an optimization.

 27          Send the status finished cutting in the RTO Remaster environment.


             INVALUE1 = 1 A+W Production Manager sends the status finished cutting to
             AWB. If the Production Manager reads a file named
             ‘OptimizationNumber.700’ (written by RTO), the Production Manager send
             the status for the sheets from the Production Manager Optimization with
             this number. The RTO writes the file only, if all sheets from this
             Optimization number are cut. Default is 0 and no status will be send.

 28          Keep the float glass together if shape, IGU/LAMI, and shape 99. The float
             glass is placed on the same rack after cutting. We have follow restrictions:


                -   IGU/LGU
                -   Shape99
                -   Float glasses have same cutting sizes/rectangles
                -   Float glasses have same glass articles
                -   Float glasses have same order and line/item numbers


             INVALUE1 = 1 A+W Production Manager places the float glass on the same rack if
             the shape is a shape 99 and IG/LAMI item. The float shapes have to be the
             same cutsizes. Default is 0 and old behavior works.

 29          Unique barcode number per glass (#439200)


             Now the glass has a unique barcode number per glass. The customer can set
             the last barcode number starting with which the ProductionManager should
             begin counting sequential barcodes.




10.12.2021                 EN-INST-A+W Business Production Manager.docx                       91
             DECVALUE1 = last unique barcode number (set to 1000 by default)



 30          Use Crystal Reports for cutting plans (#457082)


             Particular customers want to use the new Crystal Reports for cutting plans. For
             these customers, the new cutting plan report has to exist and this option
             has to be set to 1.


             INVALUE1 = 1 – Use new cutting plans. 0 – Use PlanEdit for cutting plans.
             Default is 0.
             Default optimization mode (for iCut #450838)
 31

             By default, the optimization manager can now either start with the XOPT-S mode
             or XOPT mode. Currently, the optimization mode is always set to XOPT-S. With this
             parameter, you can select the mode. iCut starts with the optimization mode set to
             XOPT.

             INVALUE1 =
             0 – XOPT-S mode or
             1 – XOPT Modus.
             Default for the ProductionManager is 0 and the old behavior works.




10.12.2021                 EN-INST-A+W Business Production Manager.docx                      92
6 Tips and tricks
6.1 FAQs
6.1.1 Update from 12.x to 13.x or higher check breakage job number range


If the customer uses the breakage function, you have to check the job number range with the new
breakage number range. The breakage number range is from 9000 to 9999 (default). If the number
ranges are not different (they overlap), you have to store normal jobs in the archive (See 3.4). You
can change the breakage number range with a SQL editor (see ParameterID in Prod_Parameter 17)
and use another number range for breakage jobs.


6.1.2 New reports and labels since Version 6


You have to install the new reports and labels because of the position split feature in version 6. The
old reports and labels do not work anymore.


6.1.3 New fields in database for position split and breakage since Version 6


6.1.3.1      Item split


We have a new field SUB_POS in many Prod_* tables. You could use this field to create joins
between tables from AWB and Production Manager.


6.1.3.2 Breakage


We have a new field KEYINDEX (Primiary key) in many Prod_* tables. This field creates an
unambiguously entry in the table to different the original entry (Item from BOM) from the breakage
entry. If you create a breakage item, the new entry is the almost same and only the field KEYINDEX
is different. The field KEYINDEX is always 0 and uses the entry from the field SUB_POS as first entry.
That means, if there a split position the field KEYINDEX could be not 0. If there any breakage, the
field KEYINDEX from the new entry is increased by 1 from the original entry.
You should use this field to create joins between tables from the Production Manager.
6.1.4 New table PROD_BREAKAGE since Version 6



10.12.2021                     EN-INST-A+W Business Production Manager.docx                          93
We have a new table PROD_BREAKAGE. You could check a breakage entry by field IS_BREAKAGE. 0
means no breakage item and 1 means breakage item. The field JOBNUMBER_NEW is null, if the item
not in a breakage job. If the field JOBNUMBER_NEW is not null, the item is in a breakage job with
this number from this field. JOBNUMBER_ORG field gets you the origin job which contains the
breakage item.
BREAKAGE_FROMSCANNER field have follow entries:
0 = breakage record from A+W Business Scanner
1 = breakage record from A+W Production Manager


BREAKAGE_REGISTRATION entry from AWB table SYSADM.KA_REKLA_ORT field NUMMER
BREAKAGE_REASON entry from AWB table SYSADM.KA_REKLA_GRND field NUMMER


6.1.5 Stockplates since version 6


    -   If the Flag “Production” is set at the “Stock Definition”, the Optimization has access to the
        stockplates




10.12.2021                     EN-INST-A+W Business Production Manager.docx                             94
Figure 55: Production flag in stock definition



     -    If the flag “Production” is NOT set at the “Stock definition”, the optimization has access only
          to stockplates with active “Default Storage Place” (old program behavior before V6)




Figure 56: Default storage place flag for plates

6.1.6 Tolerance optimization parameter Max X-X, Max Y-Y, Min X-X, Min Y-Y (since V6.2)


The option offers to enlarge Max X-X and Max Y-Y for the optimization in case there are sheets to
optimize having size larger than Max X-X or Max Y-Y.
The option for Min X-X, Min Y-Y decrease the size of Min X-X, Min Y-Y, if the sheets fit.


You could set this options in the optimization parameter control. The orange rectangle shows the
min max values for cutting. The green rectangle shows the new switches to set the options (on = use
the option at the optimization. off = ignore the option at the optimization):




10.12.2021                            EN-INST-A+W Business Production Manager.docx                     95
Figure 57: Parameter control to set the max/min options



You could set default for every aggregate in the AWB masterdata.
You need the SQL script with number 20160803a.
See case 375052.


6.1.7 Block entry has not the correct dimension




10.12.2021                         EN-INST-A+W Business Production Manager.docx   96
You get an optimization error from xrecalc XMM10028 till XMM10036
The block export makes the A+W CAD Designer (Shapes)/SN. Please, check the Opt2Txt.dat file in
the %APPDATA% and P:\SN\User\Default (Techsoft server Dir\ SN\User\Default), because SN use
the measurement entry from the Opt2txt.dat. Only the following entries are possible:


     1) 0032 (fractional Inch 1/32)
     2) 1000 (decimal inch)
     3) Default is mm


See chapter 6.4


6.1.8 Use residual plates rather than stockplates in optimization


If you would like to use the residual plates in the optimization, you can classify them higher (= larger
numeric value) than the normal stockplates. You can do this on the 'Stockplates' sidebar
'Optimization manager' TAB column 'Priority'.
This looks as follows:




Figure 58: Prioritization of residual plates



Now, the optimization uses the residual plates rather than the stockplate because the priority (33) is
greater than the stockplate priority (1).


Please consider that:


10.12.2021                             EN-INST-A+W Business Production Manager.docx                   97
You have to add one or more stockplates (plates with blue circle in picture), if you want to optimize.


6.1.9 How to edit Opt2* files before optimization runs


You could call a batch file before the optimization runs. The batch file has to be in the P:\Common
directory and is named PreOptimizationStep.bat. The batch has one argument, the machine ID. The
batch is executed in the current Opt2* fil directory
%appdata%\A+W\Techsoft\ProductionManager\Var*\. The batch shows no window and you
should enter a PAUSE in the batch. The batch output is written to the Production Manager Log with
TraceLevel Info. The lines begin with the following text:


“RunPreOptimizationBatch. Output line from batch:”


Example:


"RunPreOptimizationBatch. Output line from batch:
C:\Users\mschubert\AppData\Roaming\A+W\Techsoft\ProductionManager\VAR_1\f7a1349c-208a-42c6-
803b-0efb51d2120c>echo 1000 " | " " | " " |



Batch errors begins with the line (TraceLevel Error):
“RunPreOptimizationBatch. Error from the batch:"


The program flow is as follows:


1)    The program copies all opt2 files into the %appdata% dir. The opt2txt is copied from the
p:\common dir. The other opt2* files are created by the Production Manager.
2)      The program runs the PreOptimizationStep.bat
3)      The program start the optimization
        a)     First: The optimization runs the pre-step batch. That mean the xReCalc.bat. The
        xReCalc.bat changes some values in the opt2dat.txt. The size of the cutting rectangle
        b)      Second: the optimization is running.
        c)      Third: The post step batch runs. That means the xOptMult.bat runs.



10.12.2021                     EN-INST-A+W Business Production Manager.docx                         98
The PreOptimizationStep.bat could contains follow:




Figure 59: PreOptimizationStep.bat file

Batch as text:


echo on
setlocal ENABLEEXTENSIONS
@for /f "tokens=3*" %%i in ('reg query "HKLM\Software\Albat+Wirsam\Techsoft" /v "Root
Directory"') do @Set "RootDir=%%~j"
echo RootDir = %RootDir%


echo %1


if '%1' == '1000' goto 1000
if '%1' == '1010' goto 1010
if '%1' == '1050' goto 1050
if '%1' == '1060' goto 1060
goto end


:1000


10.12.2021                          EN-INST-A+W Business Production Manager.docx        99
copy P:\common\opt2txt_1000.dat opt2txt.dat
goto end


:1010
copy P:\common\opt2txt_1010.dat opt2txt.dat
goto end


:1050
copy P:\common\opt2txt_1050.dat opt2txt.dat
goto end


:1060
copy P:\common\opt2txt_1060.dat opt2txt.dat
goto end


:end




6.1.9.1 Batch arguments


 PreOptimizationStep         Description
 Argument

 1                           That is the aggregate ID argument. The value is the entry in the table
                             ZW_AGGREGATE column AGG_ID. The argument is used since hotfix of
                             v6.4 .



The Opt2* files docu link:
\\jupiter\Doku_DocuWare\XOPT_XOPTS\XOPTFiles\User_Manuals


You could use the dl.exe tool to change the Opt2txt.dat file.



10.12.2021                     EN-INST-A+W Business Production Manager.docx                      100
6.1.10 New AWB function: turning of standard models on the order entry screen
       (#377601)
Please, check the minimal Program requirements (October 2017)
         1) AWB version: 13.4.47
         2) Production Manager version: 13.4.629
         3) AWB DB Skript: 20170927a.sql


6.1.11 Different stock and plate bookings via XTV reporting


The Production Manager writes a PRODBDA into the FS_POOL_KOPF table and P and S records into
the FS_POOL table to book the stockplates (used by optimization) in AWB. The extension of the
PRODBDA tells the AWB the stock from the stockplate. The extension is a number like 002 or 013
and means stock with id 2 or 13. You have to set one thing in the stock masterdata of AWB and then
AWB books correct.


Goto: MasterData > Stock > Stock Definition




Figure 60: Stock ID for the booking of stockpates



You have to enter the Name text field (orange marked). You can enter the Stock Ids (semicolon
separated) In the Name text field: 1;2;3;4. If the PRODBDA file name has one this extension, AWB
books the plate from this stock.


You should write follow in the Name text field in the Production Manager environment:


StockId;Stock name



10.12.2021                           EN-INST-A+W Business Production Manager.docx                  101
2;Hegla Stock


This means for XOPTON that a stock is used. The Stock ID comes from the column Barcode-ID (green
marked).




6.2 Known errors and workarounds
6.2.1 Problems installing Microsoft components
    •    Problem
         Installation of the SQL Server Native Client and/or MS C++ Redistributable fails.
    •    Cause
         Regular Windows updates have been run previously and require the system to be rebooted.
    •    Remedy
         The system first has to be brought to a consolidated status. Any updates need to be
         performed as well as any required reboots.


6.2.2 xOptMult and xRecalc batches


If you have problems with the order of sheets after the optimization, it could be that the
optimization does not call xOptMult and xReCalc.


Issue: We have to use the short path in the batches, but we used the long path.
Please, check this registry entry to check the Techsoft RootDirectory path:




Figure 61: Registry Techsoft root directory



Open the directory ServerDir\Common (mostly P:\Common):

10.12.2021                           EN-INST-A+W Business Production Manager.docx              102
    1) Open the xOptMult.bat




Figure 62: p:\Common directory



If the batch looks like this:




Figure 63: xOptMult batch long path name



Change the marked place to:


"RootDir=%%~sj"




10.12.2021                        EN-INST-A+W Business Production Manager.docx   103
See here:




Figure 64: xOptMult batch short path name




You have to do the same at the xReCalc.bat.


6.2.3 XRecalc errors


We get sometimes errors at optimization from the XRecalc. Check the follow files:
    -    Block.pth and Opt2txt.dat in SN Default user directory and SN user
         %Appdata%\A+W\TECHSOFT\SN (see 6.4)


Either the Block file path is wrong and/or the block entry has the wrong dimension. That means that
you have Shape 99 in the optimization because:
    -    There is a Shape 99 in the Job
    -    The customer marks some processing on the cutting table (drill holes, cut-out or corner
         rounding).




6.3 New features in V6
The features 6.3.1 till 6.3.4 implemented in latest hotfix of V6 and V6.1 or higher.
Check chapter 2.4 because we do not patch V6 anymore.


6.3.1 New columns in Prod_OPTI_STATISTICS (#361422)


You need the SQL script with the number 20160405.

10.12.2021                        EN-INST-A+W Business Production Manager.docx                     104
The new columns (all decimal(28,8)) could be used for reports:

    1) RES_OUT_AREA              residual area created
    2) RES_IN_AREA                Area of used residual plates (without trim)
    3) RES_IN_AREATRIM Area of residuals used


6.3.2 Use the latest user input for new variant of optimization in Optimization Manager
      (#360709)


The situation before:
The user edits stockplate and optimization parameters and after the optimization the user input is
away.
Now, the programs remember the user input for every glass article and show the latest user input
for every glass article.


6.3.3 Send waste to AWB for cost calculation (#363566)


The A+W Production Manager sends the waste to the A+W Business after the user saves the
quotation and the AWBusiness calculates the cost for the item in the position automatically because
the Production Manager calls the A+W Business COM object to calculate the costs. This only works
in the Production Manager quotation mode (Offer mode).


You need the script 20160509 to insert (BW_AUFTR_OPTI and BW_ANGEB_OPTI) and update
database tables.


6.3.4 New driver scripts


We support new drivers (the script 20160502 update database tables):


    -   PerfectCut – Pattern
    -   PerfectCut - Racks
    -   Optima cutting driver



10.12.2021                      EN-INST-A+W Business Production Manager.docx                     105
Other new drivers (the script 20160201 update database tables):


    -   PDS bender
    -   PDS IG line


6.3.5 Multi selection in lists


The user can select several entries in list with mouse and keyboard:
    -   ctrl + left mouse clicks to select entry (other selected entries are remain selected)
    -   ctrl + space to select entry (other selected entries are remaining selected)
    -   ctrl + A to selected all entries. If all entries selected, the entries will be deselected
    -   shift + left mouse clicks select all entries in row between the selected rows.


This function is not implemented in the TABs Optimization Manager and Output. Here only works
the ctrl + A function.


6.3.6 Customized edge deletion


    1. Isolated glass unit


We use the cutbacks (REUCKSCHNITT1…8) of the table SYSADM.BW_AUFTR_MODELL to create edge
deletion. The user can enter the cutbacks in the AWB dialog (mouse click on spacer item [here
orange])




10.12.2021                      EN-INST-A+W Business Production Manager.docx                        106
Figure 65: Edit cutback in AWB



The user can change the cutbacks in the green box. There is a default cutback on the position
(BW_AUFTR_POS.REUCKSCHNITT) of the spacer (value yellow box). REUCKSCHNITT)(value of yellow
box).
The program uses the cutbacks of SYSADM.BW_AUFTR_MODELL. If the values are zero, we use the
cutback of the BW_AUFTR_POS.REUCKSCHNITT table. We only write a -1 record to Opt2Fa, if the
edge deletion/cutback is greater than the default cutback of the machine. You can set the default
cutback of the machine in the aggregate dialog of AWB (see below).


    -    Next possible solution to set cutback:
Otherwise, you could create a CU to add or change the cutback in the SYSADM.BW_AUFTR_MODELL
table. E.g. If you use U-Profiles, you have to add a small value to the cutbacks.


Follow settings are needed to enable the feature:


    -    You have to enable the feature on the aggregate dialog in AWB and check the orange
         marked check box:




10.12.2021                       EN-INST-A+W Business Production Manager.docx                  107
Figure 66: Enable edge deletion in AWB and set default cutback



    -    You should set the default cutback of the machine in the green marked text field.


    2. Single glass or laminated glass unit
The user can use the AW Processing 1025 edge deletion for single glass or laminated glass. He has to
add this processing on the single glass and the A+W Production Manager use these values as
cutbacks.


You have followed restrictions:
    -    We only calculate the cutback from A+W catalog
    -    All segments of the shape have to be lines (no arcs). We do not calculate the cutback for
         shapes with arc segment.


You need the DB script: 20161014a.sql.
See case #376802.


6.3.7 New columns in table PROD_OPTI_STATISTICS


Here the new columns (all decimal (28,8), not null and default is 0):


    -    OPTI_AREA          Optimized area without residual plates and with trims
    -    OPTI_COST                   Costs of OPTI_AREA
    -    NET_AREA           net area of the sheet (not of the circumscribing rectangle)
    -    NET_AREA_COST               Costs for NET_AREA
    -    NET_QUANTITY                Number of sheets
    -    INVOICE_AREA        Invoice area of the sheets from AWB (STL_QM_FAKT or
         PP_QM_FAKT columns in AWB tables)


10.12.2021                         EN-INST-A+W Business Production Manager.docx                      108
    -   INVOICE_AREA_COST          Costs of INVOICE_AREA
    -   REUSABLE_REST                    Area of residual plates
    -   REUSABLE_REST_COST Costs of REUSABLE_REST_QM
    -   WASTE_AREA              waste area (includes sheet waste, trim area of jumbo, residuals not
        used)
    -   WASTE_AREA_COST         Costs of WASTE_AREA
    -   BREAK_AREA                       area of the broken sheet (not of the circumscribing
        rectangle)
    -   BREAK_AREA_COST         Costs for BREAK_AREA
    -   BREAK_QUANTITY          Number of broken sheets


You need the DB script: 20161016a.sql.
See case #378569.


6.3.8 Save residual plates in AWB DB


If you click ‘Book Stockplates’ in the context menu of Optimization TAB, The Production Manager
saves the residues plates in the AWB DB.
In AWB you can do the following:


    -   You could edit the residual plates in the AWB residual plates management (see next
        picture). You can only change values if the residual sheet is not used by an optimization (you
        will see this if the 'in optimization' field is 0).
    -   You can change the amount and other properties (See orange box).
    -   The field ‘From Optimization’ can be negative. Then we use a residual plate that was added
        manually by a user.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                         109
Figure 67: residual plate management and edit amount of residual plate



We only save the residual plates, if the plate is greater or equals a minimal width and a minimal
height. You can edit the minimal residual plate width and height in the AWB master data of the glass
article (See orange box):




Figure 68: Edit residual plate width and height



For your information


The default values for the minimal width and height are 9999 mm to have the old behaviour, where
we do not save the residual plate.




The Production Manager writes the new residual plates in the DB, if the user Book the stockplates
via context menu in the Optimization Manager TAB.


You will see the following residuals:




10.12.2021                           EN-INST-A+W Business Production Manager.docx                110
Figure 69: Recognized residual plates

The program recognized only residual plates which are ends on the border of the plate. We will not
detect any residual plates that are in the middle of the plate where sheets are on either side of the
residual. Like here:




Figure 70: Not recognized residual plates



See new Parameter ID 22 to decrease the width and height of created residual plate.
You need the DB script: 20161005a.sql.
See case #378522.




10.12.2021                          EN-INST-A+W Business Production Manager.docx                   111
6.3.9 Marking stepped drilled holes in cutting code


We mark stepped drill holes, too. The user can only add stepped drill holes and the drill holes for
the sheets will be marked in the cutting code.


See 6.8 for implementation.


6.3.10 Print cutting labels via machine driver


     1) You have to add the machine IDs in the category 'Labels from cutting machines' in the
        Production Manager Config Tool (new parameter ID 23). Look at the orange rectangle in the
        next picture:




Figure 71: ConfigTool Settings for cutting labels via driver



     2) You have to add 2 reports to the AWB report directory. The reports are known as:
     -    LabelDat.rpt (Bottero, Macotec need only this report)




10.12.2021                            EN-INST-A+W Business Production Manager.docx                    112
    -    PrintCuttingLabels.rpt (not every machine needs this report. E.g. Turomas, Hegla need this
         report.)


    Note: Every machine could have a own PrintCuttingLabel.rpt named
    PrintCuttingLabels[AggregateId].rpt. E.g. if the machine ID is 1000, the name of the report file
    has to be PrintCuttingLabels1000.rpt.
    If we support a new machine and there is no information about this machine in this document,
    you can look for this in the Market Solutions document:
    \\jupiter\Doku_DocuWare\MarketSolutions\AUW_Configuration_cutting.docx
    It could be that you need the new Cutting Driver Batch. IF you need a new one, you have to ask
    DLA for this batch.


You get the AWB Report directory in the master data. Look at this picture and check the green box:




Figure 72: Master data report location



Now, we write some data for the cutting label printing via machine driver. We write 2 new files in
the cutting driver path:
    -    Label.dat

10.12.2021                          EN-INST-A+W Business Production Manager.docx                       113
    -   PrintCuttingLabels.pdf


We write an Opt2Bar file to the optimization save file. The machine driver needs the Opt2Bar file for
cutting label printing (barcode and optimization order of sheets).


If the user adds some sheet via PlanEdit, we write follow for the sheets to the Opt2Bar file:


    -   Order number = -2
    -   Item number = -1
    -   Barcode is an empty string


The Turomas cutting table requires both reports and generates from the PrintCuttingLabels.pdf
report a prin file (that's the binary file format of the Hermes printer).
The Hegla cutting table also requires both reports. But Hegla needs only the real pdf output and not
a prn file like Turomas.


For the Turomas cutting table, you need the following tools (see next chapter 7.3.10.1)


    -   The CAB Drvier for Hermes printer
    -   Multi File Port Monitor (mFileMon)
    -   PDF Reader/Viewer Adobe or Foxit Reader


6.3.10.1 Reports


6.3.10.1.1 LabelDat.pdf


LABEL.DAT is a text file generated by Crystal Report LABELDAT.RPT. This report generates a
section of data for each barcode. Each section starts with the following line which is needed
to identify the section [CuttingDataProviderSection][{Number of
Machine}][{Barcode}] and it ends with [EOS].




10.12.2021                       EN-INST-A+W Business Production Manager.docx                     114
Our drivers currently support the keyword CuttingDataProviderSection. New drivers
or other applications in the future will possibly support other keywords.


The section contains a list of individual parameters in the following format:


< {Name of parameter}="{Parameter Value}">

This format could be different for individual drivers, currently we have only one driver
which uses this format.


Here is an example from A+W Business Pro:


[CuttingDataProviderSection][1000][T200020630001000]

<ORDERNO="20630"> <ITEMBNO="1"> <BOMID="0"> <JOB="1004">

<OPTIMIZATION="8"> <QUANTITY="5"> <SHAPENO="0">

<COMMISSION="Kommission A"> <CUSTOMERITEM="KDPos A">

<DELIVERYDATE="30.06.2017"> <BARCODE="T200020630001000">

<PRODUCTNO="104"> <PRODUCT="Float 4 mm A+W">

<CUSTOMERNO="1070"> <CUSTOMERNAME="Becker Glasbau">

<WIDTH_CUT="1.700,00"> <HEIGHT_CUT="1.800,00">

…

[EOS]



This file can be used for every cutting code driver, maybe in future also to send additional
information to the cutting code driver. Actual (v6.3 and v6.4) it is used only for the label
print feature of the BOTTERO or Macotec cutting code driver.

6.3.10.1.2 PrintCuttingLabels.PDF


In the PrintCutting.PDF you provide real labels, one label per page and one label for each
barcode in the optimization.




10.12.2021                   EN-INST-A+W Business Production Manager.docx                    115
Figure 73: LabelDat.pdf report




Each page must have a hidden control field containing the barcode number:


         @@BARCODE={Barcode}@@



The cutting code driver splits the PDF into one page for each barcode and builds a new PDF for each
path


6.3.10.2 Configuration of Turomas cutting tables


After generate the cutting code driver with Albwir.Xoptc.Turomas.exe, execute the
additional tool TuromasLabelProcess.exe. This tool uses the same configuration file,
Turomas.config, and is working if OPT2BAR and PrintCuttingLabels.PDF exist beside the
generated cutting code.
For each pattern in the cutting code a file <CuttingCodeName>_<PatternNo>.POS and
<CuttingCodeName>_<PatternNo>.PDF will be generated. The PDF file contains the labels
from PrintCuttingLabels.PDF.


After this the generated PDF files per pattern will be convert into a PRN file. A PRN file is the
file format which is generated direct by the printer driver. In this solution the printer driver
generates his output direct into a file. The generated PRN file will be renamed into
<CuttingCodeName>_<PatternNo>.PRN and is part of the package of cutting code and .POS



10.12.2021                       EN-INST-A+W Business Production Manager.docx                   116
files. The PDF file isn’t need anymore and the files will be removed if the conversion was
done fine.


The conversion into PRN file is not so easy, you need some tools and some configurations:


    -   Hermes CAB Windows printer driver


Turomas uses CAB Printer ( (), e.g. Model Hermes+ 4L/300. Download the right printer driver and
install it on the Server where you generate cutting code. Configure the printer driver, generate a
label format with the size of the used label and set this format as default, maybe it is need to set
this as default for each windows user.
The Crystal Report PrintCuttingLabels.RPT has also to be generated and stored with this printer
driver and the same label layouts you use on the server during cutting code generation. The same
technic we use if we generate normal labels with Crystal Reports.
The name of the printer has to be configured in Turomas.config parameter <Printer>.


        <PRINTER>CAB Hermes+ 4L/300</PRINTER



    -   PDF Reader
We support ADOBE or FOXIT. One of the readers has to be installed and which is used has
to be configured in Turomas.config in the parameter <ReaderType> :1 = ADOBE, 2 = FOXIT.
Our driver opens the PDF in the reader and print them on the configured printer. The driver
also closes the PDF reader if the PRN file was generated. This can take a while so you have
to configure some timeouts in milliseconds if nothing happens in the parameter
<WaitForPdfReader> and <WaitOpenFile>.


    -   <ReaderType>1</ReaderType>
    -   <WaitForPdfReader>10000</WaitForPdfReader>
    -   <WaitOpenFile>2000</WaitOpenFile>



    -   Multi File Port Monitor
The freeware tool Multi File Port Monitor is needed (https://sourceforge.net/projects/mfilemon/).
The tool is in the AUW Turomas package in the Tools subdirectory or it can be downloaded.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                            117
Install the tool and configure a printer port for the Windows printer driver and set the output in the
driver fix to this port. If you do this, the driver doesn’t print on a physical printer, it prints the result
into a file. We can’t use the Windows standard printer port FILE, because in this function you have
to enter an output filename every time you print and with the Multi File Port Monitor you can
configure the filename.


In Devices and Printers mark a printer and open in the Printer server properties the tab Ports and
Change Port Settings.




Figure 74: Configure CAD Hermes printer for Turomas cutting table




Add a new Port from type Multi File Port Monitor. We recommend as port name PRNFILES.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                           118
Figure 75: Configure mFileMon Port for Turomas cutting table



Now, you have to set the port name in this dialog:




Figure 76: Add mFileMon Port for Turomas cutting table




10.12.2021                         EN-INST-A+W Business Production Manager.docx   119
Configure the Output path (red rectangle in next picture) and the Filename pattern (green rectangle
in next picture) for this port.




Figure 77: Settings for mFileMon



The path must be fixed, UNC path possible but variables (e.g. %APPDATA%) doesn’t work. For this,
the user needs read and write rights.
Use the following pattern for the file name: PrintCuttingLabels.%u.%c.prn. This generate a file with
user name and computer name. So it is possible to generate this cutting code on one Server from
different users.


In the next step allocate the new port to the Turomas printer. Open the Printer Properties and in
tab Ports select the new port PRNFILES.




Figure 78: Open Printer properties


10.12.2021                           EN-INST-A+W Business Production Manager.docx                   120
Figure 79: Set PRN Port at printer properties




For testing the configuration open a PDF document in your PDF reader and print the
document on this printer. After this the PRN file should be generated in the configured
output directory.


You must configure the same output path and file pattern in the Turomas.config in
parameter <TempPrinterFile> as configured in Multi File Port Monitor. The placeholder %u
and %c works in both file pattern.


         <TempPrinterFile>C:\Temp\PrintCuttingLabels.%u.%c.prn</TempPrinterFile>




6.3.10.2.1 Turomas.config

In the Turomas.config the parameter for the label print function are configure in section <Label>.
Here an Example:


   <Label>


10.12.2021                           EN-INST-A+W Business Production Manager.docx                    121
      <WaitForPdfReader>10000</WaitForPdfReader>

      <WaitOpenFile>2000</WaitOpenFile>

      <ReaderType>1</ReaderType>

      <Printer>CAB Hermes+ 4L/300</Printer>


<TempPrinterFile>C:\Temp\PrintCuttingLabels.%u.%c.prn</TempPrinterFile>

  </Label>



6.3.10.3 Configure the Bottero cutting driver


BOTTERO generates and print the Labels with his own applications, but they need several
information for the sheets in the cutting code to print them on the label. The information
we prepare in the LABEL.DAT


The driver BotLabelProcess.exe must be execute before XCBOTHPS.EXE and it search in
LABEL.DAT for packages with the following syntax:


[CuttingDataProviderSection][{Maschin ID}][{Barcode Number}]

<{Name of Parameter}="{Parameter Value}">

...

[EOS]



The Output is the file BotLabel.TXT. The cutting code driver XCBOTHPS.EXE uses this file if it
exists and inserts the information into the cutting code. The complete text between the
header line and [EOS] will be used and convert into one line. Special character like
line/page break will be removed.


6.3.11 Crystal report Runtime 13 (#399962)


We could use the Crystal Report (CR) Runtime 13 since Version 6.4. The old (CR) Runtime version
12 works, too. The old CR Runtime version will be used, if the new CR Runtime version not installed.
That’s the fallback. Check AWD case #399962.



10.12.2021                    EN-INST-A+W Business Production Manager.docx                       122
6.3.12 Notes about shape 770, 771, 771, 772


There are no FRM files for these shapes. You have to create SN files for the shape. The shapes will
be handled as shape 99 in the Production Manager program.


6.3.13 Refinements in Hotfix 898, 915, 952, 980


    -   Faster breakage loading, if you open the breakage dialog
    -   Faster job item search in wizard/standard mode (= faster job creation and less memory
        needed) (since version 915)
    -   Save the same job items in wizard mode like in standard mode. The wizard mode saves only
        scheduling item at previous version.
    -   Marking rounding corners (see Parameter 18)
    -   If the user optimizes jobs in the Optimization Manager, the program checks the items which
        will be written to PROD_JOBITEMTEMP table. If there are no items to write, the program
        cancels the optimization.
    -   If the user saves optimizations in the Optimization Manager, the program checks if their
        item in the PROD_JOBITEMTEMP table. If no item in the table, the program does not save
        the optimizations.
    -   New DB Script: 20171201a. This script contains an update for table PROD_SHAPETRIM.
        Follow shapes will be added:
        200, 201, 770, 771, 772, 773, 801, 802, 803, 804, 807, 808
    -   Faster loading of optimizations in Optimization Summary Tab (since version 950)
    -   For some database queries, capitalization is not heeded (since Version 952).
    -   We fixed a memory leak. The List Controls do not remove the added function pointers. That
        is solved and the List Control needs less memory because there is no memory leak (since
        version 980)


6.3.14 Feedback from Realtime Optimizer (RTO) to AWB to discount stockplates in AWB
       (#407260)




10.12.2021                     EN-INST-A+W Business Production Manager.docx                       123
You have a cutting table with a Remaster. Then the RTO has to write PRODBAZ files and the AWB
read the PRODBAZ files to discount the stockplates, set status from AWB orders.


6.3.14.1 AWB Configuration


You need to install the latest AWB and AWB SQL script: 20180126a.


You have to set the follow check box in AWB:




Figure 80: Set the Remaster for RTO/Cutting table



The AWB interface service have to handle the ProdBaz file from the RTO (see the Installation Docu
from the AWB Interface Service 1.12). You have to activate the XTV Workflow and enable AWB to
read ProdBaz files (see AWB Config Docu for further details 7.4).
You have to add the ProdBaz directory in this dialog (Red marked. You find this dialog in Production
settings under Master Data-> Company->Data Tab 13. Production):




10.12.2021                          EN-INST-A+W Business Production Manager.docx                  124
Figure 81: Set ProdBaz file path for RTO



You can enter the dialog, if you press ‘Settings’ (red marked) in Master Data-> Company->Data Tab
13. Production:




Figure 82: Find the RTO file path settings




6.3.14.2 RTO, AWB Pro Configuration


You have to set follow in the RTO config file (xopton.cfg)


    1) RTO writes no feedback file for residual plates at the moment. No sheet information
       (Order/Pos) will be passed to AWB for residual plates. A new flag “ResidualPlates” will
       be added to the section [FeedBackFile]. For “ResidualPlates=Y” a feedback file will
       also be written for residual plates. AWB will not find the stockplate size and has to
       ignore it. AWB will only use the “Order/Itm” information of the sheet records.
    2) You have to set the WriteSheetRecord=Y in section/partition [FeedBackFile] to write
       the sheets into the feedback file. Then we can set the state of the order in AWB.
    3) AWB Pro needs the status information ("Cutting started" and "Cutting finished") for
       each imported save file (ZWB optinumber). A new section [BusinessProFeedback] will

10.12.2021                           EN-INST-A+W Business Production Manager.docx              125
        be added to the XOPTON.CFG. With the entry “FeedbackFilePath” a path can be
        configured which is reachable for the RTO and AWB Pro. The “FeedbackFilePath” has
        to be the same like the aggregate Output Directory in AWB settings Capacity Planning
        > Aggregate > General Check next picture:




        Figure 83: Set the Remaster for RTO/Cutting table




        When the RTO starts cutting an AWB Pro optimization or the AWB Pro optimization is
        reoptimized in a tableoptimization the RTO writes an empty file (Name=AWB
        Optinumber Extension=state). Example: For optinumber=1956 the filename will be
        “1956.300” (1956=AWB Pro optinumber / 300=Production started). If the
        optimization has been completely cut the RTO will write a file “1956.700” (1956=AWB
        Pro optinumber / 700=Produced). Then the A+W Production Manager sets to the
        optimization status to 700 (=released) and releases the reserved stockplates of AWB
        Pro. The 'Book Stockplates' context menu is deactivated on the Optimization
        Summary tab in the Production Manager.
    AWB configuration:
    You need the call of the function udf_ReadFeedbackFiles() so that the exchange service
    knows where it can read the feedback files and import them into the database under A+W
    Business > Master Data > Import Customizing.
    And you need the call of udf_ProcessXTV() to process the data imported.




10.12.2021                        EN-INST-A+W Business Production Manager.docx           126
    The A+W Production Manager reads the *.700 file and sets the status of the stockplates,
    optimizations, and optimization statistics to booked.


    You can send the status finished cutting to A+W Business automatically with the A+W
    Production Manager. Please, check the ParameterID 27 at config tool.


6.3.14.3 Optimization statistics


The PROD_OPTI_STATISTICS is not correct for changed optimization by RTO. The table contains the
old optimization data from the Production Manager. The Production Manager do not update the
entries. You have to use the AWP tables xopt_optimierung and so on in this environment.


6.3.14.4 A+W Production Manager


The user could not book stockplates in the Optimization summary tab, if the Remaster setting active
on the producing machine. The entry on the content menu (Book stockplates) is deactivated. The
Context menu entry is enabled if one or more optimizations were produced on a machine without
Remaster. The Production Manager only books only the stockplates for optimization produced on a
machine without remaster.
The optimization state in PROD_OPTIMIZATION and PROD_OPTI_STATISTICS are only set to Booked,
if the optimization produced on a machine without remaster.
The A+W Production Manager reads the *.700 files and books the plates and sets the status to
booked with a background process. The user doesn't have to do anything. There is nothing to
configure on the Production Manager.
We implemented a new context menu entry in the Optimization Summary TAB. The entry bears the
name 'Update.' If the menu entry enabled, the Production Manager read one or more *.700 files
and make some database updates. If the menu entry disabled, there is no new data. The menu
entry is only shown, if there are a XOpton with a remaster.
The Production Manager shows a message in the Status Bar (where the Program and Database Info
is shown), if there are new data.


6.3.15 Fix some issues 417027, 416756, 417132, 416887


6.3.15.1 #417027: Booking stockplate error. Sheet is not placed in the cutting state



10.12.2021                    EN-INST-A+W Business Production Manager.docx                      127
If in the optimization there are sheets with different PO numbers, not all sheets will be booked in
the cutting status. Now we will book all sheets correctly.


6.3.15.2 #416756: Hardware products/articles in the order selection


If you are seeking sheets in the order selection, the tab also displays hardware products/products.
Now we do not show this item.


6.3.15.3 #417132: Bavelloni cutting machines (MTS, MTL) supports optimization numbers
         larger than 3 digits.
That was fixed at the machine driver xcbavshp.exe. The driver will be deployed by the A+W
Production Shared Folder Setup. The new driver has the version 13.0.178.1 from 23.02.18.




6.3.15.4 #416887: faster GetFRM
The GetFRM assembly is faster now. It should be 2-3 times faster. The creation of batches is faster
since the creation of batches uses the edge correction and shape detection. The GetFRM assembly
will be deployed by the A+W Production Runtime Setup.


6.3.16 Archive reports as pdf


If the batch has been optimized, we were able to save all order and optimization reports and labels
on the hard disk. The base archive folder is the AWB file attachment path from the AWB master
data (red marked in the next picture). That is the default path:




Figure 84: File attachment path at AWB master data

You can change the base archive Folder path at the Config Tool. See parameter 25.


10.12.2021                         EN-INST-A+W Business Production Manager.docx                       128
Then we add the relative path ‘\ProdMan\Archive\’ to the master data path. That’s the base path
for every batch. We add the year and month (double digit, leading zero, if necessary) to the path.
The path for one batch is:
‘File attachments path’ + ‘\ProdMan\Archive\’ + ’Year\Month\’ + ‘JobNumber’
For example:
‘File attachments path’ + ‘\ProdMan\Archive\2018\08\1234’




Figure 85: Archive reports at Production Manager

The orange marked button and context menu saves the reports to disk. You have to selected least
one batch with status optimized or higher.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                      129
The green marked context menu opens the archive folder. We opened the base folder if the user
selected more than one job or the user select no job.
If the user selects one batch with status optimized or higher, we check if there a directory with the
job number and open the directory with the job number, if it exists. Otherwise we open the base
folder.


For your information:


    -   If the reports exist on disk, we override them.
    -   Please, use the crystal reports for the optimization result and optimization pattern report
        because if you not use these reports, we use the PlanEdit print export and this export needs
        a user input for saving.
    -   Each batch report or each label has the batch number as prefix (e.g.
        2062_795_LGUProductionList.pdf).
    -   Every optimization report or label has the job number + ‘_‘ + optimization number as prefix
        (e. g. 2062_795_ListOfStockplate.pdf)




6.3.17 New Job Status at Job Status dialog


We can set a new job status ‘Produced’ at Job Status dialog.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                        130
Figure 86: Archive reports at Production Manager

You change the job status at the orange marked combo box. If you set this status, you can mark the
job as produced but the job will not be archived. The next status is ‘Released’ and then the AWB
archiving workflow works.


6.3.18 Residual plates size not correct (420104)


We calculate the residual plate size not correctly. That issue is solved with April 2018 setup/release.


6.3.19 Add supplier info


We have to execute the SQL script 20180614a to switch on the feature.


You can open a new dialog under optimization summary TAB via the context menu:




10.12.2021                         EN-INST-A+W Business Production Manager.docx                     131
Figure 87: Open supplier info dialog



The dialog shows like this:




Figure 88: supplier info dialog

You select some rows and add a text into the green marked box. Press the button red button and
the program adds the text to the last column.
Ok save the data to database.
Cancel do not save the data.


6.3.20 New filter criteria at optimization summary TAB


You can show only optimizations with job, which status is smaller than produced and released.


You have to uncheck the green marked check button (checked is the previous behavior):




10.12.2021                             EN-INST-A+W Business Production Manager.docx              132
Figure 89: Status criteria at optimization summary tab




6.3.21 Default PDF printer to show Optimization Result and Pattern report on screen
       from PlanEdit


We have changed the behavior:


    1) We try to find the maxx PDFMailer printer. If we find this PDF printer, we use this PDF
       Printer for PlanEdit reports to show on screen. We search after the printer name “maxx
       PDFMailer”.
    2) If we do not find this PDF Printer, we use another PDF printer. We use the first printer,
       which contains “PDF” in his name. That’s was the old behavior.


You should always install the maxx PDFMailer printer. Then you get no FileSave Dialog to save the
PlanEdit reports.


6.3.22 Mark macro processings


We can mark macro processing. You have to set the mark drill hole and cut-out parameter (6.8 and
ParameterID 18) because the program does not know the content of the macro. The macro could
contain drill holes and/or cut-outs.




6.3.23 Some hints for specials shapes 901 and 902


Let's take a look at the 2 shapes:


10.12.2021                          EN-INST-A+W Business Production Manager.docx                   133
Figure 90: Shape 901 and Shape 902




10.12.2021                           EN-INST-A+W Business Production Manager.docx   134
Do not use the shapes in the AWB entry. This cannot work since the shapes have more than 8
edges.


Some hints for AWP and not AWB Pro:


The shapes 901 and 902 only work with a product of the insulated glass unit (IGU). You cannot add
some steps, edge processings or other inner cut-outs, border cut-outs, corner cut-out and corner
processing. Heed the restriction of the A+W Production system (AWProduction):

    -   We have no shape recognition since we cannot detect the inner cut-out and would detect
        shape 0.
    -   We ignore steps and edge processings.
    -   No marking of drilled holes, inner cut-outs or corner processings on the cutting table
    -   This makes sense if the customer has a Bystronic cutting table and a Lenhardt IG line.
The A+W Bystronic cutting table driver can cut and delete the edges of these special forms (also
inner cut-outs). The Lenhardt line can produce the frames. It is model 91 in the Lenhardt shape
catalog.



You have to change the spacer report. We do not calculate the spacer segment length from the
inner cut-out since the shape detection detects the shape 0. We calculate the spacer only from the
rectangle/shape 0 (outer contour).



You can enter this XL_JobRelease. cfg entry:



[XL_SHAPE_CATALOG]

;#253779 implementation shape 901

ConvertSpecialShapes=Y



Then the shapes 901 and 902 will be produced as shape 0 (rectangle); otherwise as shape 98 (Lisec
free shape).



6.3.24 February Release 2019


    1) Edge correction at aggregate assignment was not correct. We have corrected this.


10.12.2021                    EN-INST-A+W Business Production Manager.docx                         135
    2) Use Crystal Reports for cutting results and cutting pattern in PO mode and do not print with
       PlanEdit or a PDF printer.
    - You need the Prodman_OptimisationResult.rpt and Prodman_OptimisationCuttingplan.rpt
       report.
    - You have to add the reports at the AWB masterdata. The OptimizationResult has the ID 826
       and the CuttingPlan has the ID 830
    3) Print archive reports at background in Job summary control. User could work further with
       the program but he cannot enter the job or optimization output control and cannot enter
       the wizard mode
    4) Background printing is used in the output tab with the same restriction at 3)


6.3.25 March release 2019


    1) Filter and search short keys


The user can press enter (instead of pressing the search button) to search data in job summary,
order search, optimization summary and job information TAB. The filter button has the short key
Ctrl+Alt+A or Ctrl+F. Ctrl+A is used by the list controls to select all entries.


    2) Obsolete script in v12.5


Do not install script with name: 20180614a at v12.5. The new column SUPPLIER_INFO only
works in v6. We made a new script for v12.5 to solve the issue: 20190307a



    3) ConfigTool is warned if the batch number range overlaps the breakage or quotation
       number ranges.


The config tool shows a warning, if



    -   Job number and breakage job number overlap. You can reduce the job
        number range to 8999. Check whether some batch numbers are in the range
        of the breakage batch number.
    -   Batch quotation and batch number overlap. You can adjust the number range
        of the quotation. Check whether some batch numbers are in the quotation
        job number range.

10.12.2021                    EN-INST-A+W Business Production Manager.docx                        136
     4) Delete block file entries




There is a new Ribbon to make some internal and environment work.




Figure 91: New ribbon TAB



The first and only entry is ‘Remove Entries’ from block file. If you press the button, you see this
dialog:




Figure 92: Delete block file entries dialog



You can set a time in days. If the block file entry older, the entry will be removed. The program
reminds the last setting of the days.



Its will be only delete entries with follow naming:

     -    Starts with prefix ‘ ;-)Shape99_’          (=nested shape from ShapeOpt)

10.12.2021                            EN-INST-A+W Business Production Manager.docx                    137
    -    The name matches OrderNumber_PositionNumber_BomId (= Blockexport from
         ProductionManager)
    -    The name matches OrderNumber_PositionNumber_BomId_AggregateID (= block
         export from AWB Production Terminal)


6.3.26 Write Muntin section in AWISO.dat for TFB Bender driver to make drilled holes for
       muntins in the spacer


Restriction:


    -    The muntins have to be below the spacer item at AWB order entry.




Figure 93: Place of muntins at AWB order entry

    -    You have to add the muntin to a spacer in muntin/georgian bar entry. We have to use the
         red marked combo box for spacer selection. The green marked button adds the
         muntin/georgian bar to the other spacers and all spacers contain the same muntin/georgian
         bar.




10.12.2021                         EN-INST-A+W Business Production Manager.docx                138
Figure 94: AWB muntin entry




    -   We only support the TFB bender driver (driver number 13) at the moment.
        13 = TFB              = XL_ISO_TFB_0
    -   You have to set the FormatVersion in the driver section at XT_AWISO.cfg file to 2.00 e. g.
    [XL_ISO_TFB_0]
    FormatVersion=2.00


6.3.27 Partial deliveries in AWB (#444661)


You need the database script 20190603a to use the function.


If a customer makes partial deliveries in AWB, the AWB deletes the entries in some database tables
(BW_AUFTR_*). The AWB sends us the job number and we marked the job as Partial delivered (new
column in PROD_JOB table PARTIALDELIVERED,. Not null, int, default is 0). The column
PARTIALDELIVERED is 0, if not partial delivered; 1 = PARTIALDELIVERED.


If the job is partial delivered, the user cannot do:
    -   any output (job and optimization)
    -   Resolve batch
    -   Resolve the optimization
    -   Edit the optimization
    -   Archive batch
    -   Aggregate assignment
    -   Show detailed job view



10.12.2021                      EN-INST-A+W Business Production Manager.docx                         139
Restrictions at Production Manager:


    -   The user has to print the job and cutting reports and labels reports and create all bender
        and cutting code before one order is partial delivered.
    -   If the user needs labels for the partial delivery order, he has to make a job with the partial
        delivered order. Then the user can print labels. The user has to release the job because of
        the achieving.


6.3.28 Selected plate as first plate in optimization (#449810)


The user can use the priority value for special selecting. If the user enters a negative value, the plate
will be used as first plate at the optimization. The user can only enter one negative priority value in
the stockplate dialog. That means only one plate could be used. The plates get a green ball (blue ball
means stockplate; yellow ball means residual plate) at second column.


6.3.29 Support of bended IGU and LGU (#450801)


We cut the correct cutting size at cutting table, if the glasses will bended.


Follow restrictions:


    -   It works only with shape 0
    -   You cannot edit the shape number and parameters with the cutting edit dialog




6.3.30 XTV Mode (#451823)


You can start the Production Manager in an XTV mode. The program starts only with the last 2 tabs
(Optimization summary and Output).




10.12.2021                      EN-INST-A+W Business Production Manager.docx                          140
Figure 95: XTV Mode



The user cannot resolve, edit, save optimizations with the context menu at optimization summary
tab. The output tab is not changed.




Figure 96: XTV mode optimization summary context menu



If the user presses ‘Detailed view’ at context menu, it opens a new window with the pattern list and
pattern picture of optimization. This dialog is modal and opens in full size. The user can select the
next the pattern with the controls Space, Arrow down, F12. If the user wants to select the previous
pattern, he has to press Shift+ Space, Shift + Arrow up or Shift + F12. The window closes, if the user
presses escape (ESC) button.




10.12.2021                       EN-INST-A+W Business Production Manager.docx                      141
Figure 97: XTV detail view windows



The Production Manager starts in XTV mode, if the user belongs to the ‘XTV’ (case sensitive) group.
You can edit the setting in the AWB. See the following figure:




Figure 98: Set group for AWB user




10.12.2021                           EN-INST-A+W Business Production Manager.docx                142
6.3.31 Changes in September 2019 release


6.3.31.1 New assemblies in Setup


The Production Manager deploy all assemblies, which are needed to run. There are new assemblies
in the setup:
    -    Get99.dll
    -    GetFRM32.dll
    -    The native logging dlls: Log4cxx.dll and AWSOA.Core.Native.dll


6.3.31.2 Faster batch creation and detailed scheduling


We load the data (glass article, capa properties, edge processing data, etc.) only one time from the
database and not every time and sometimes in for-loops. This makes batch creation and the
detailed scheduling faster.


6.3.31.3 Minimized ribbon bar




Figure 99: Minimized ribbon bar

The user can minimize or maximized the ribbon bar with the red marked button.


6.3.31.4 Rack numbers with more than 4 digits and ACLIM_BOCK_FACH in label.set


The opt2dat contains the ACLIM_BOCK_FACH at character host field. The default is 2 and means
that the last 2 digits from the rack number is the slot number at harp rack.
E. g. the ACLIM_BOCK_FACH is 2 and we use a harp rack:
Rack number 30056 means slot 56 at harp rack 30000.




10.12.2021                        EN-INST-A+W Business Production Manager.docx                    143
6.3.31.5 Tool tip with information about batch, breakage, optimization number range, etc.


If the user moves the mouse pointer over the batch or the optimization labels/text, a tool tip can be
displayed. The text of the tooltip always follows the format: 1000 – 8999 (4711).


1st number (1000): minimum job, breakage, optimization number
2nd number (8999): maximal job, breakage, optimization number
3rd number (4711): current job, breakage, optimization number




Figure 100: Tooltip about number range




6.3.32 Changes in November 2019 release


    -    ParameterID 28: Keep float glasses together at same rack if the shape is a shape 99 and an
         IGU/LAMI


    -    The Production managers calculates the correct cutting rectangles of shape 99 and show the
         right cutting rectangles at order summary tab.
    -    #453238 New formula variables 6.6

         Machine1AfterCutting
         Machine2AfterCutting
         Machine3AfterCutting
         Machine4AfterCutting

10.12.2021                        EN-INST-A+W Business Production Manager.docx                    144
        Machine5AfterCutting

What the difference to Machine1, Machine2, …, Machine5 variable:

The Production Manager has the variables Machine1, Machine2, Machine3, Machine4 and
Machine5. These variables contain the machine number of the First, Second, Third, Fourth and Fifth
processing machine after cutting. The problem is that the same machine can participate in several
processings and our goal is to identify individual and unique machines after the cutting, and we
have to ignore doubled machines for the processing sequence.


6.3.33 Barcoding - unique label identification per glass (#439200)
Now you can create barcoding for the individual idetnification of glass.


With the current process of glass manufacturing, a single barcode is used for all BOM items.


In order to work with this setting, please insert the value of the last barcode in the
Production Management Config Tool:




10.12.2021                     EN-INST-A+W Business Production Manager.docx                    145
Figure 101: Barcode number setting




The pre-set minimum value is 1000 and the value increases with each newly created
barcode. The maximum value for the barcode is 9223372036854775807. It is expected that
a barcode with 19 digits is the typical maximum. Barcodes with 20 digits up to the
maximum value are also possible, however.


Information about the parameter in the configuration is also under the settings of
PROD_PARAMETER chapter 5.9 in the new field number 29.
How is the unique label ID per glass generated?
As soon as a new job is created, the associated orders receive the START_BARCODE for the
products of the type single glass, LAMI glass, and IG, as well as the entire BOM for these
products. All of this happens in the background.


10.12.2021                           EN-INST-A+W Business Production Manager.docx       146
After the order goes into production, the labels are printed with the new single glass
barcodes. Important is that the labels are printed with one label per product.


The labels affected by this change are the following:


Labels for the optimization




Labels for the batch




Figure 102: Affected labels during the label detection




After this change, each label that is a single label per product, has the unique barcode per
glass.
6.3.34 Production racks [AW-59393]
You need the database script 20210114a to use the function.

The "AWB Barcoding" now has information about the physical rack (production rack) on which the
glass is located after booking of the label. Thus it is possible, if someone is seeking a particular glass
in production, to locate information about on which physical rack it is located.

The management of the production racks is developed as part of the "AWB Advance Barcode"
module. At the moment, "AWB Advance Barcode" consists of the unique barcode label per glass. (
T1 + "Glass Barcode" )

To define the production rack, we use the existing rack management in A+W Business. The
production racks use the same barcode pattern as the dispatch racks:


10.12.2021                           EN-INST-A+W Business Production Manager.docx                       147
GE + "rack number"



6.3.34.1 Set-up of the racks in A+W Business (rack management)
The rack management in production now allows the selection of the rack type; you can choose
between dispatch, production, and mixed racks. A mixed rack is a rack that is available both for
dispatch and production.




6.3.34.2 Completion report (Business Scanner)
After the production racks are set in rack management, you can book a glass on the scanner with a
selected rack on which first the production rack is set on the completion report dialog with the GE +
"rack number" barcode and then the glass label scanned.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                         148
6.3.34.3 Options on the rack menu (Business Scanner)
On the "Racks" menu of the scanner program, the following new options have been added to
manage production racks:

    •   Unload Rack
        This option is already available for dispatch racks and is also used for production racks.




    •   Display Rack
        This option is already available for dispatch racks. In case of production racks, however, the
        information is expanded to: sequence + order + article + customer number + width + height




    •   Search for order
        The idea is that the user can enter the order, the element, and the BOM_ID and the scanner
        returns the physical rack that matches the search criteria.

    •   Reallocate Rack
        This option is already available for dispatch racks. Sometimes, the entire content of a rack is
        shifted to another rack. With this option, two bookings must be made: on the source rack
        and on the target rack in order to update the value for the rack in the table
        "BA_GESTELLE_AUFTR".

    •   Reallocate unit
        Frequently after a mistaken booking, a single glass is shifted from one rack to another rack.
        With this option, the barcode of the individual glass, the source rack, and the target rack are
        used in order to update the rack booking in the table "BA_GESTELLE_AUFTR".




10.12.2021                     EN-INST-A+W Business Production Manager.docx                          149
6.3.34.4 Booking history
In the booking history, a new field called "Rack" is displayed, with a search field:




10.12.2021                      EN-INST-A+W Business Production Manager.docx           150
7 Uninstalling
Use the OS control panel to uninstall the software.




10.12.2021                    EN-INST-A+W Business Production Manager.docx   151
8 A+W iCut
8.1 Prerequisite
8.1.1 Software
A Windows 10 or Server 2019 installation is the prerequisite for the installation of A+W iCut.

Creating a diskset

The installation diskset can be generated with the batch GetAWiCutComplete.cmd; this way, all A+W
modules are available for a successful installation.




The Microsoft .NET Framework 3.5 has to be installed !!!
Dism /online /enable-feature /featurename:NetFx3 /All /Source:D:\sources\sxs /LimitAccess

The directory C:\sources\sxs has to be adjusted to suit the Windows installation medium.
The Windows network search and file release have to be activated; otherwise no release drive P: can
be attached.




10.12.2021                      EN-INST-A+W Business Production Manager.docx                     152
10.12.2021   EN-INST-A+W Business Production Manager.docx   153
8.1.2 Modules of the license server
The following modules play a role for A+W iCut; these have to be released in the Edition Startup on
the license server. The production modules have to be enabled in the standard edition.



 Module      Application     Edition        Name                             Price list no.   Add-on
                                                                                              module

 1           ALFAK(300)      Startup        Basic module A+W Business        235001           No

 143         ALFAK(300)      Startup        Basic module Production          235001           No
                                            Manager

 11          ALFAK(300)      Startup        EDI Import                       240011           Yes

 156         ALFAK(300)      Startup        Excel Import                     240018           Yes

 140         ALFAK(300)      Startup        Barcode Manager (EL)             240101           Yes

 52          Planedit        Standard       Planedit                                          No

 1           XOPT-Opti       Standard       XOPT-Opti                                         No

 2           XOPT            Default        XOPT                                              No

 4           XOPTS           Default        XOPT/S                                            No

 1           XOPTS           Default        A+W Shape Optimizer              240115           Yes
             SHAPENESTER

 ?                                          Machine driver




10.12.2021                    EN-INST-A+W Business Production Manager.docx                             154
8.2 Installation SQLServer Express and the database
Please perform the installation with the SQLServer 2019 Express or newer.




Select the new installation of the SQL Server. In the following, only the entries will be listed that
deviate from the suggested values.




Select a default instance.
Install the SQL Server as mixed mode installation and give the current user the administration rights
via the SQL Server



10.12.2021                    EN-INST-A+W Business Production Manager.docx                       155
Now install the SQL Server management tool; the call causes a download of the installation package.




Do the download and execute the EXE.


10.12.2021                    EN-INST-A+W Business Production Manager.docx                      156
Now you can log onto the SQL Server, either via the Windows login or the "sa" authentication.




Please install the databases for your selected language for A+W iCut.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                      157
Thus the SQL Server installation is completed and the database for A+W iCut is present.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                158
8.3 Installation of the software with the A+W Setup Launcher
8.3.1 Creating the fingerprint for the soft lock
Download the SoftlockPreparePackage.zip and unzip it.
\\jupiter.a-w.intra\Doku_DocuWare\AWEnterprise\LicenseServer\!General\FAQ_Tips_Tricks\Softlock

Start a command shell as administrator and execute the file "StartPrepare.cmd."

If there are problems, perhaps you need a newer version of the "Sentinel HASP installer." You can
download this from the manufacturer.
https://www.sentinelcloud.com/minisites/SRM/Downloads.aspx?s=&c=all&p=Sentinel+HASP&o=all&t=all&l=all




The haspdinst.exe has to be stored in the "SoftlockPreparePackage \Driver" subdirectory.
During the installation, the fingerprint file of the computer can be generated. Using this, the license
for this computer can be issued.




10.12.2021                            EN-INST-A+W Business Production Manager.docx                      159
8.3.2 Installing the Setup Launcher and license server
If you have received your license file, we can begin with the installation of the Setup Launcher and
the license server. Execute the SetupStarter.Exe.




Select the A+W License Server diskset




This places the following components on your computer.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                      160
Please enter the license file in the configruation of the license server.




10.12.2021                      EN-INST-A+W Business Production Manager.docx   161
8.4 Installation of A+W iCut software
Start the A+W Setup Launcher again




The following modules are installed by the defined diskset




10.12.2021                    EN-INST-A+W Business Production Manager.docx   162
Here, the specification is made of the user under whom the COM parts are running. This can be the
user who uses iCut or another user with appropriate rights (login authorization).




The license server is running on the PC; for a server installation, this could also be another machine.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                         163
Here, the recommended OLEDB Provider should be selected; it is also selected in the diskset.
The user has to be specified for the Exchange Windows Service; he receives the "Windows Service
Logon" authorization.




The Windows Service is installed and started. It executes the workflow.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                     164
8.5 iCut activation in script management
The activation is done in the script management by setting the edition to "iCut."




On the next start of A+W iCut, the license of the edition "Startup" is queried and the license file must
be ordered accordingly. It is important that at least the module 1 and 143 in the "Startup" edition are
released. All other modules are limited by the program or are additional modules (see also 0.)




10.12.2021                     EN-INST-A+W Business Production Manager.docx                         165
The display of the license in the license manager looks like this:




10.12.2021                      EN-INST-A+W Business Production Manager.docx   166
8.6 MDI window and the main menu
In A+W iCut there are two user groups, the standard users and the XTV users. The standard users
(operators) work in the office and can, for example, edit products, enter orders, approve batches for
the production manager, etc. The XTV users, by contrast, work on the cutting table. In the Production
Manager, there is an XTV mode and in this mode, users can only display optimization 9cutting plan)
and remove stockplates. For this reason, depending on the group to which a user belongs, the main
menu in A+W Business is displayed accordingly.




The other tool dialogs such as the "Last used" – tool are not available in A+W iCut. Furthermore, some
functions are deactivated in the edition.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                       167
8.7 Master Data
8.7.1 Customers
In the customer management, only the fields for the definition of the address are available. All others
are deactivated, just like the functions that you can call from the menu.


8.7.2 User rights
In the management of the user rights, only the programs are displayed that are available in this
edition. Adding new rights also only works for the selected programs.




10.12.2021                     EN-INST-A+W Business Production Manager.docx                        168
8.7.3 Number ranges
In the number ranges, you can specify ranges for orders and S+N file numbers. No other areas can be
edited. Furthermore, you can define the ranges only for the standard scheduling range <n.e.>.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                      169
8.7.4 Product Management
In product management, only existing products can be changed, the tabs 3 and 12 were deactivated,
there are no prices and also no technical parameters (service description).

For the following product groups, a new creation of products is permitted:


       “001 - Single glass” / “011 - Single glass”
       “002 - TG” / “018 - TG”
       “003 - LG” / “020 - LG”




8.8 Documents
8.8.1 Number manager
In the number manager, you can only copy or overwrite a number manager. Furthermore, you can
make a status change and display the currently selected document. The scale drawing can no longer
be called from the number manager in this edition.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                    170
8.8.2 Document entry
It's only possible to enter orders. Furthermore, the total tab is deactivated and there is no price
calculation in the item entry. But for the history, status change, and selection of the number manager,
all functions are deactivated. Only the first tab of the header entry is active.




In the item entry, it is not possible to select the columns in the table. You can only enter edge
processings, steps, and shapes. The creation of texts is also possible. If the item entry is ended, the
program changes back to header entry.



10.12.2021                     EN-INST-A+W Business Production Manager.docx                        171
In the item entry remain only 1=item, 2=BOM, 3=shapes and processings, and 8=texts active. Only
edges, steps are allowed as processings.


8.8.3 Form printing
The form printing can be started from the main menu or as direct printing from order entry and be
done from the number manager. It is only an order confirmation and a production paper can be
printed. The printouts are generated via Gupta Reports. Crystal Reports is not supported.


8.8.4 Archive transfer
In the transfer to the archives, it is only possible for the user to delete orders from A+W Business and
to remove flows from the production manager via defined workflow task.




No archive databases are required for A+W iCut.


8.8.5 Exchange Service
The Exchange Service and the infrastructure are not installed. The A+W Commercial 6 Exchange
Windows Service takes their place.
This Windows service executes the workflow tasks defined in A+W Business, such as the archiving of
production manager batches.



10.12.2021                     EN-INST-A+W Business Production Manager.docx                         172
For this, a formula (Company > Formulas) that calls the function udf_TransferEndOfDayProdManager(
) has to be defined at the start.




Then you change to the Customizing program (Company > Customizing) and create a new workflow
task with this formula.




10.12.2021                   EN-INST-A+W Business Production Manager.docx                     173
Now you have to specify how and when this task should be executed.




As already mentioned, the execution will be taken over by the Exchange Windows Service.

And on the tab 5.Monitor, you can verify the result of the execution.




10.12.2021                    EN-INST-A+W Business Production Manager.docx                174
8.8.5.1 Config Tool
In order to specify the Trace Level for the Exchange Windows Service, you have to use the A+W
Commercial 6 Exchange Windows Service Config Tool.
Here you select the Commercial Exchange Service and click Protocol. Then you can define the trace
and log level.




10.12.2021                   EN-INST-A+W Business Production Manager.docx                       175
8.8.6 Data back-up
This has to be done by the planning via script.




10.12.2021                     EN-INST-A+W Business Production Manager.docx   176
9 Appendix
9.1 Table of figures
Figure 1: Release server directory ........................................................................................................ 20

Figure 2: Welcome screen of the SetupLauncher ................................................................................ 22

Figure 3: Dialog Choose or create diskset ............................................................................................ 23

Figure 4: Setup directory ...................................................................................................................... 24

Figure 5: Components to be installed .................................................................................................. 25

Figure 6: Configuration Interface Service ............................................................................................. 26

Figure 7: Grant "Service Account" right ............................................................................................... 27

Figure 8: ALCIM settings configuration ................................................................................................ 27

Figure 9: A+W Business 6 Setup settings dialog ................................................................................... 28

Figure 10: Service user dialog............................................................................................................... 28

Figure 11: AWSOA Communication configuration dialog .................................................................... 29

Figure 12: AWSOA Service User dialog................................................................................................. 30

Figure 13: Service user dialog............................................................................................................... 30

Figure 14: A+W Business configuration ............................................................................................... 31

Figure 15: Start the installation ............................................................................................................ 32

Figure 16: Save the installation configuration ..................................................................................... 33

Figure 17: A+W Production Manager configuration – Database login ................................................ 34

Figure 18: A+W Production Manager configuration – ODBC-settings ................................................. 35

Figure 19: A+W Production Manager configuration – Transfer directory ........................................... 36

Figure 20: A+W Production Manager configuration– CAD-Designer-directory ................................... 37

Figure 21: A+W Production Manager configuration – BLOCK.PTH-files .............................................. 38

Figure 22: A+W Production Manager configuration– BLOCK.PTH-files – copy target ......................... 38

Figure 23: A+W Production Manager configuration – BLOCK.PTH-files standardized ........................ 39

Figure 24: A+W Production Manager configuration – General settings .............................................. 40

Figure 25: Reboot query ....................................................................................................................... 40

Figure 26: No Windows domain and use SQL Server Authentication .................................................. 41


10.12.2021                                  EN-INST-A+W Business Production Manager.docx                                                      177
Figure 27: Company master data – Documents ................................................................................... 43

Figure 28: Order master data – Status allocation ............................................................................... 44

Figure 29: Production master data – Registration points production ................................................. 45

Figure 30: B2B-master data – SN file rules ........................................................................................... 47

Figure 31: Formula search .................................................................................................................... 48

Figure 32: Workflow-task configuration – Formula ............................................................................. 49

Figure 33: Workflow task configuration – Workflow task ................................................................... 50

Figure 34: Workflow task configuration – Autom. process execution ................................................. 51

Figure 35: Formula search .................................................................................................................... 52

Figure 36: Workflow task configuration – Formula ............................................................................. 53

Figure 37: Workflow-Task configuration – Workflow task................................................................... 54

Figure 38: Workflow-Task configuration – Autom. process execution ................................................ 55

Figure 39: A+W Business bender text configuration ............................................................................ 56

Figure 40: A+W Business bender text check in order item .................................................................. 57

Figure 41: Configure XTV cutting code for Realtime Optimizer ........................................................... 59

Figure 42: Helga technical article code settings ................................................................................... 66

Figure 43: RTO batch number .............................................................................................................. 68

Figure 44: AWB Pro Partial deliveries................................................................................................... 69

Figure 45: A+W Production Manager spacer code .............................................................................. 72

Figure 46: Describes grandparents, parents, end product type or class ............................................. 79

Figure 47: Customer item and commission reference in AWB ............................................................ 80

Figure 48: ProjectNumber in AWB ....................................................................................................... 80

Figure 49: A+W Business item structure .............................................................................................. 82

Figure 50: A+W Production Manager PROD_PARAMETER table ......................................................... 83

Figure 51: A+W Production Manager Config Tool to update PROD_PARAMETER table ..................... 84

Figure 52: Additional processing text (edge processing) ..................................................................... 89

Figure 53: DR_DRUCKPUNKTE Table ID 824......................................................................................... 90

Figure 54: DR_REPORTE Table ID 824 .................................................................................................. 90


10.12.2021                                  EN-INST-A+W Business Production Manager.docx                                                    178
Figure 55: Production flag in stock definition ...................................................................................... 95

Figure 56: Default storage place flag for plates ................................................................................... 95

Figure 57: Parameter control to set the max/min options .................................................................. 96

Figure 58: Prioritization of residual plates ........................................................................................... 97

Figure 59: PreOptimizationStep.bat file ............................................................................................... 99

Figure 60: Stock ID for the booking of stockpates ............................................................................. 101

Figure 61: Registry Techsoft root directory ....................................................................................... 102

Figure 62: p:\Common directory ........................................................................................................ 103

Figure 63: xOptMult batch long path name ....................................................................................... 103

Figure 64: xOptMult batch short path name ..................................................................................... 104

Figure 65: Edit cutback in AWB .......................................................................................................... 107

Figure 66: Enable edge deletion in AWB and set default cutback ..................................................... 108

Figure 67: residual plate management and edit amount of residual plate ...................................... 110

Figure 68: Edit residual plate width and height ................................................................................. 110

Figure 69: Recognized residual plates ................................................................................................ 111

Figure 70: Not recognized residual plates .......................................................................................... 111

Figure 71: ConfigTool Settings for cutting labels via driver ............................................................... 112

Figure 72: Master data report location .............................................................................................. 113

Figure 73: LabelDat.pdf report ........................................................................................................... 116

Figure 74: Configure CAD Hermes printer for Turomas cutting table................................................ 118

Figure 75: Configure mFileMon Port for Turomas cutting table ........................................................ 119

Figure 76: Add mFileMon Port for Turomas cutting table ................................................................. 119

Figure 77: Settings for mFileMon ....................................................................................................... 120

Figure 78: Open Printer properties .................................................................................................... 120

Figure 79: Set PRN Port at printer properties .................................................................................... 121

Figure 80: Set the Remaster for RTO/Cutting table ........................................................................... 124

Figure 81: Set ProdBaz file path for RTO ............................................................................................ 125

Figure 82: Find the RTO file path settings .......................................................................................... 125


10.12.2021                                 EN-INST-A+W Business Production Manager.docx                                                  179
Figure 83: Set the Remaster for RTO/Cutting table ........................................................................... 126

Figure 84: File attachment path at AWB master data........................................................................ 128

Figure 85: Archive reports at Production Manager ........................................................................... 129

Figure 86: Archive reports at Production Manager ........................................................................... 131

Figure 87: Open supplier info dialog .................................................................................................. 132

Figure 88: supplier info dialog ............................................................................................................ 132

Figure 89: Status criteria at optimization summary tab..................................................................... 133

Figure 90: Shape 901 and Shape 902 ................................................................................................. 134

Figure 91: New ribbon TAB ................................................................................................................ 137

Figure 92: Delete block file entries dialog .......................................................................................... 137

Figure 93: Place of muntins at AWB order entry ............................................................................... 138

Figure 94: AWB muntin entry ............................................................................................................. 139

Figure 95: XTV Mode .......................................................................................................................... 141

Figure 96: XTV mode optimization summary context menu ............................................................. 141

Figure 97: XTV detail view windows ................................................................................................... 142

Figure 98: Set group for AWB user ..................................................................................................... 142

Figure 99: Minimized ribbon bar ........................................................................................................ 143

Figure 100: Tooltip about number range ........................................................................................... 144

Figure 101: Barcode number setting .................................................................................................. 146

Figure 102: Affected labels during the label detection ...................................................................... 147




10.12.2021                                  EN-INST-A+W Business Production Manager.docx                                                     180

