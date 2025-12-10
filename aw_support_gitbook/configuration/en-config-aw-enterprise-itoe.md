---
description: "EN CONFIG A+W Enterprise iTOE"
---



# EN CONFIG A+W Enterprise iTOE

         Configuration Instructions


A+W Enterprise iTOE




                                                                    english




   A+W Software GmbH   EN-CONFIG-A+W Enterprise iTOE.docx   - -INTERNAL-
                                                                    1
Change history


          Date         Author                  Remarks                              Version
          2019-02-05   Original version        Transfer from Dokuware document      1.0
                                               AWDesk #449540 – Function keys for
          2019-10-28   SVH
                                               exiting iTOE
          2021-04-14   EB                      Incorporation of all RN texts
          2021-06-23   SVH                     Background iTOE
                                               [AW-161206] – Edge processings on
          2023-10-13   SVH
                                               underglass
          2024-02-13   SVH                     [AW-172587] - Cutbacks




Content

1.   General Information                                                                   5
     1.1. Availability                                                                     5
     1.2. Reference to documentation                                                       5
          1.2.1. Enhanced release notes                                                    5
          1.2.2. Performance description                                                   5
     1.3. Background iTOE                                                                  5
2.   Installation                                                                          6
3.   Configuration                                                                        7
     3.1. A+W CAD Designer (Shape) licensing                                              7
     3.2. AWE environment variables                                                       7
          3.2.1. MODUL_ITOE                                                               7
          3.2.2. SNFILES_DIR                                                              7
          3.2.3. AWBROKE_GETFOCUS                                                         9
          3.2.4. WIN_AWBROKE (deactivate!)                                                9
          3.2.5. SN_KUNR                                                                  9
          3.2.6. GET_DEFPARAM_AWE                                                         9
4.   Master data                                                                          10
     4.1. AW processing types                                                             10
     4.2. Special iTOE market partner                                                     10
     4.3. E/A rules                                                                       10
     4.4. Shape catalog                                                                   13
5.   Operation                                                                            14
     5.1. Operation in A+W Enterprise                                                     14
          5.1.1. Starting the iTOE with file synchronization                              14
          5.1.2. Starting the TOE from the A+W Enterprise BOM                             15
          5.1.3. Message box messages                                                     15
     5.2. Operation in the A+W CAD Designer (Shapes)                                      15


A+W Software GmbH               EN-CONFIG-A+W Enterprise iTOE.docx                             2
          5.2.1. iTOE menu elements                                                         15
          5.2.2. Application of processings for IG/LAMI                                     16
          5.2.3. Edge processings view                                                      16
          5.2.4. Applying drillings to IG and LAMI                                          17
     5.3. Emergency dialog                                                                  17
6.   Functions                                                                               18
     6.1. Status of an SN item                                                               18
           6.1.1. Changing the BOM with existing SN file                                     19
           6.1.2. Entry of following items                                                   19
     6.2. Import of DXF files                                                                20
           6.2.1. DXF Import in SN                                                           20
           6.2.2. Corrections                                                                20
     6.3. Level conversion                                                                   20
     6.4. Generation of the SN file name                                                     21
     6.5. iTOE: Support of stamps                                                            21
     6.6. Individual lite cutting of LAMI rounded corners                                    21
     6.7. Transmission of generalized edge and corner cut-outs                               21
     6.8. Deco numbers for special edges                                                     23
     6.9. Number of edges in prices for shape 99                                             23
     6.10. Use of templates                                                                  24
     6.11. Special treatment of particular shapes in SN                                      24
           6.11.1. Shapes with special treatment in SN                                       24
           6.11.2. Shapes with different numbers of segments and edges                       24
           6.11.3. Full-surface coatings on shape 99                                         24
           6.11.4. OrderXml transfer for processings on free shapes                          25
           6.11.5. Full-surface coatings on shape 99                                         26
     6.12. Calculation of edge processing in a special shape (shape 99) when transferring SN
     files 26
     6.13. Free shapes                                                                       26
     6.14. Fixed products with SN files without iTOE module                                  26
     6.15. Attaching SN files during product fixing                                          27
     6.16. Import of SN files when creating stock orders of fixed products with subparts     27
     6.17. Adaptation of SN sketch in printout                                               28
     6.18. Acceptance of SN files of ordered subparts in purchase order generation and
     transmission.                                                                           29
     6.19. Extension of the iTOE exchange rules for countersunk drillings                    30
     6.20. Preventing additional synchronization manually                                    30
7.   Inheritance with an in iTOE                                                           31
     7.1. Ordered subparts with SN file                                                    31
     7.2. iTOE inheritance of the LAMI processing on the IG                                31
          7.2.1. Print indicator/procurement type of LAMI processing steps with inheritance
          function                                                                         31
          7.2.2. Problems with LAMI inheritance of edge processings on free shapes         32
8.   Text                                                                                   33
     8.1. Additional processing texts when synchronizing via iTOE with stamps               33
          8.1.1. Processings are not summarized in the text area in order entry             33
9.   Troubleshooting                                                                        34
     9.1. Logs                                                                              34


A+W Software GmbH               EN-CONFIG-A+W Enterprise iTOE.docx                                3
    9.2. There is no reaction when clicking the TOE menu elements in the SN                    34
    9.3. ISO items do not arrive complete in the SN                                            34
    9.4. Dimensions of the circumscribed rectangle for rotated shapes                          34
    9.5. Alignment of stepped drilling                                                         34
    9.6. BOM synchronization for very flat cut-outs                                            34
          9.6.1. Application of processings after shape change                                 35
          9.6.2. Improved consistency in BOM of surface processings                            35
    9.7. ITOE - takeover of the SN files for reference                                         35
    9.8. Changes to an iTOE item after saving                                                  35
    9.9. LAMI BOM are mixed up after synchronization                                           35
    9.10. Processings are missing after synchronization with file on underglass in the SN file 36
    9.11. Edge processings are missing after synchronization with file on underglass in the
    SN file                                                                                    36
    9.12. Problems with cutbacks (cutbacks/frame deductions)                                   36
10. Figures                                                                                   37
    10.1. Overview of workflow                                                                37
    10.2. Overview of data flow                                                               37
    10.3. Update of the CAD file                                                              38
    10.4. Copy/delete the CAD file                                                            38




A+W Software GmbH               EN-CONFIG-A+W Enterprise iTOE.docx                                  4
1. General Information
The integrated TOE (iTOE) is a logic for processing AWE BOMs in the A+W CAD Designer (Shapes).
Here it is possible:
    •   To generate CAD files from AWE BOMs
    •   To process AWE BOMs in the CAD program
    •   To import shape and processing information from CAD files into the AWE BOM


1.1. Availability
The functionality is made available with the version A+W Enterprise 6 and A+W CAD Designer
(Shapes) 6.


1.2. Reference to documentation
1.2.1. Enhanced release notes
The module was developed with AWDesk #202952.
The release notes were created with AWDesk #365161 (see Docu tab of the case). The
information from the release notes was taken over completely into this document.


1.2.2. Performance description
The performance description of the module is linked via the intranet (PM > Documentation)




1.3. Background iTOE
The background iTOE was implemented with ticket [ZW-57149].
Goal of the development was a synchronization of AWE BOM and SN file in the background.
For a detailed description of the flow, see the configuration document of the A+W Enterprise CAD
Service.




A+W Software GmbH               EN-CONFIG-A+W Enterprise iTOE.docx                             5
2. Installation
To use the iTOE, the following programs have to be installed and configured correctly:
    -   A+W Enterprise Frontend,
    -   A+W CAD Designer (Shapes)
    -   License client for licensing the CAD designer for use of the iTOE (see also Chapter 3.1).
Details for the installation are in the installation instructions for each product.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise iTOE.docx                               6
3. Configuration
3.1. A+W CAD Designer (Shape) licensing
An A+W CAD Designer (Shape) license is required to use the iTOE.
If there is no license, the CAD Designer will open with the following message when you start the
iTOE:




The CAD Designer (Shape) can be exited normally via the iTOE menu elements (see below for
description) after confirming the message.


In order to prevent that the iTOE is started inadvertently if the user does not have a license, the
iTOE is activated explicitly via the environment variable MODUL_ITOE.




3.2. AWE environment variables
3.2.1. MODUL_ITOE
The variable activates the use of the interactive iTOE. Without activation of this module variable,
the files assigned manually will no longer be copied and deleted order-related. The files are still
used for the display on the processing dialog, however there is no BOM synchronization and you
can also not start the iTOE in order to edit the file.


3.2.2. SNFILES_DIR
The environment variable SNFILES_DIR is defined in A+W Enterprise. The file path stored here (or
a superior path) must be connected as network drive on the Windows server. The path
specification must end with a backslash.
Both the CAD service as well as the access rights required by A+W CAD Designer (Shape) to the
path stored in SNFILES_DIR as well as all subdirectories.

A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                  7
The variable must be set generally (manr=0).
SN accesses this path if an existing CAD Designer (Shape) file should be opened (kposp.brokefile).
The CAD service and the interactive CAD access this path in order to save a SN file.


For orderXML transfer to A+W Production with attached SN files, SNFILES_DIR must match AWP
Master Data > Configuration > Rough Scheduling > (Shaping & Nesting) Data File Path since only a
relative path is transferred in the orderXML file. (see also #347756)
There, however, the registry is usually stored as basic path (SERVERDIR, Server Directory), to be
found under: HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Albat+Wirsam\Techsoft
The basic variable SNFILES_DIR controls the interplay with A+W Production and is indispensable
for use of the new iTOE. For this reason, when starting the A+W Enterprise main module, there is
now a check whether the variable SNFILES_DIR is set. The check is only done if either an A+W
Production connection (AWC_ALCIM_ANBINDUNG active) or the new iTOE (MODUL_ITOE active)
is configured.
The check tests whether the variable is not set or is empty. In this case, the message is output:
"The variable SNFILES_DIR is not configured correctly. Please inform your A+W planner."
There is no check whether the content of the variable is maintained correctly. The program then
continues, however without set SNFILES_DIR if there is work with SN files, there will be non-
specific error messages later.
Subpath for SN files

There is another environment variable SNFILES_SUBDIR = <xxx>, which includes a subpath. If it is
set, the file selection dialog opens in this subdirectory of the main directory <SNFILES_DIR>. The
variable can be set user-related.

Client-specific SNFILES_DIR configuration

The SN files (iTOE) are located in the specified subdirectories under the permanently defined SN
basepath, which is defined via the ENV switch SNFILES_DIR. These files are assigned by type of SN
files and date. From the naming conventions of the file itself, it is also not possible to assign the
files to specific clients in the internal client separation. For this reason, the evaluation of the
switches for the SN basic path is now performed for each client. For example, the assigned SN files
are located in: < SNFILES_DIR [client-related]>\TOE\<year>\<month>\<day>\<int.order number>-
<ItmNo>.SN (with active iTOE module)

Before the change, copy MANUALLY all existing SN files on the WINDOWS side into the new
directories. This ensures that the files in the old orders can be found again and that reference to
the old processes is also possible.

All possible template files (SN and DXF) must also be copied, since the client-specific directory is
now also offered for selecting files. If the SN template files were saved in the separate
subdirectories (SNFILES_SUBDIR), the files including these separate subdirectories must be copied
over (from SNFILES_DIR in general to SNFILES_DIR [client-specific]). The switch SNFILDE_SUBDIR
remains user-specific and not client-specific.

When changing clients later, all SN files are copied.



A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                  8
When creating the ENV switches for a specific client, it is essential that an assignment for client =
0 is also retained. This is then used for the fixed articles.

SNFILES_DIR should always be created per client PLUS 1x for client=0 (keep old value) If all files
have been copied, activate SNFILES_CLIENT_EXACT= ON.




3.2.3. AWBROKE_GETFOCUS
This variable does not have to be set. Starting with version 6.0, after exiting the iTOE, the A+W
Enterprise actively obtains the focus regardless of whether the variable is active. (the variable still
comes from the "old" iTOE.)
The logic that runs when retrieving the focus corresponds to the logic that ran for the "old" iTOE if
the variable was assigned the value 1.
Only if the problem occurs that after exiting the iTOE the focus on the A+W Enterprise is lost can
you try to solve the problem by setting the variables. Here, you can set the variables to the value
2 or 3 and test them. (permissible are the values 1, 2 and 3)


3.2.4. WIN_AWBROKE (deactivate!)
This is the MODULE variable of the "old TOE."
This variable must be deactivated.


3.2.5. SN_KUNR
Market partner (customer) for which the iTOE E/A rules are stored.
The variable must be set so that the E/A rules apply.


3.2.6. GET_DEFPARAM_AWE
Client reference: no
If no level for the processing is reported from iTOE (e.g. general cut-out), then the level is taken
over from the A+W Enterprise master data (help for DXF files).
See [AW-84741].




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                    9
4. Master data
4.1. AW processing types
    •   For each AW processing type, all permissible dimensioning types (mtype 0/1/2) must be
        created since the application of processings in the SN is possible with each permissible
        dimensioning type and the processing are thus also reported back with the dimensioning
        type used in the SN in the A+W Enterprise BOM.
    •   For all AW processing types used in the iTOE, restrictions in the item dimensioning and
        parameter properties "fix" and "must" must be avoided.
        Create all parameters are "variable"!


4.2. Special iTOE market partner
An iTOE market partner must be created for which the E/A rules are then stored subsequently.
This should be entered in the ENV switch SN_KUNR.


4.3. E/A rules
Under Keys->Products->S/N exchange rules, you store at least 1 exchange rule for all AW
processing types.




Thus, for example, a new processing of type 1005 (grinding) is always replaced by item 198130.
If, however, a processing is price-relevant and depends on the header item, then you should
create a detailed rule for this:




If this depth is not sufficient and if the processing items are also parameter-relevant (e.g. drilling),
then you should enter the rule more precisely:




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                  10
Thus a drilling with diameter starting at 5 mm is replaced by item 199005.
But there is another rule:




Thus the new drillings with the diameter starting at 20 mm are already depicted by item 198001.


For particular shapes, the edge processings must also be replaced by different items if there is a
circular edge. This is possible if for this edge processing, in addition to a "normal" rule, you also
store one for shape edge:




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                    11
So that this rule is also applied, in the master data for shapes, you should also mark the
appropriate edges as shape edge: (Keys->System->Shapes->Edge assignment )




There are also the special cases for corner cut-outs (A+W processing type 1300), inner cut-outs
(A+W processing type 1415), and edge cut-outs (A+W processing type 1400), which can only be
described in iTOE and cannot be mapped completely with the parameters from the A+W
processing catalog. These are reported in iTOE as A+W processing type +3 (A+W processing types
1303,1403, and 1418). For these processings, you can also create the separate E/A rules.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                          12
The decor edges come from iTOE as AW type 1090 (other edge processings) and also report the
deco number. For these, you should create a separate E/A rule per decor.




If there are several processings that come into question for the particular A+W processing type
and cannot be mapped 1:1 with existing restrictions, then you can also create several records for
the same combination, e.g. glass type + processing type + identical restrictions. For the
synchronization of the data, there is a query about an appropriate article, which can then be
selected from the smaller quantity.


If for an A+W processing type no exchange rule was stored, after each entry in the TOE there is
always a query for the appropriate item. All active articles from the master data that belong to
this A+W processing type are then available for selection.

Furthermore, starting with QR7 2021, it applies that if a processing with permanently defined
edge quality is reported from iTOE, this was not always detected clearly and a selection of the
appropriate processings was offered. For the determination of the processings, the dimension
parameter is always checked in 1st place, and then the appropriate data, e.g. for the drilling
diameter X is found. For the 2nd place test for edge quality, the processings with precisely
reported data from iTOE are searched for, but also the stored rule with non-filled edge quality
that applies "for all appropriate."
The determination is made more precise at that point. If from the 1st check for dimension
parameters several processings are determined to be appropriate and if a defined edge quality is
reported from iTOE, then there is a check whether there is a unique assignment and this
processing is adopted.
The same logic is built in for reported levels.



4.4. Shape catalog
The iTOE was developed for the A+W Shape Catalog. Other shape catalogs were not tested.
In case of a conversion to a non-A+W shape catalog, the configuration document
\\hausi\AWDCaseDoc\333\333775\Configuration PMC Catalog.docx must be heeded precisely.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                                13
5. Operation
5.1. Operation in A+W Enterprise
In the order entry, you first enter an item with the desired item and quantity.



5.1.1. Starting the iTOE with file synchronization
Takeover of shape information and processings from an SN file:
As soon as you are in the field "Quantity", you have the opportunity to attach a SN file to the item
with CTRL+E. After attaching the file, you will be asked whether you would like to synchronize the
file and BOM. If you answer the query with YES, the TOE is started and you have the opportunity
to check the content of the SN file. If you exit the TOE with "Exit" or "Exit and save file", the shape
information, dimensions and processings of the SN file are taken over into the AWE BOM.
For the synchronization of the AWE and SN BOMs, there are 3 steps:
    1. "UPDATE": Update of the changed processings, if present
    2. "DELETE": Deletion of the old processings (+ UPDATE, if necessary)
    3. "NEW": Insertion of the new processings
Here it must be noted that the processings from iTOE that are also present in the AWE BOM come
largely not as "UPDATE," but rather as "DELETE" + "NEW." Thus it is first checked whether this
combination cannot be replaced with "UPDATE." Here it is also taken into account if the
processing in AWE was not originally directly under the glass, but rather under META processings,
and it is placed accordingly under META.
The edge and corner-related processings also come from iTOE individually per edge and are first
pulled together into a processing with the appropriate edge vector.
If a free shape is reported back from iTOE, then there is no direct information about the number
of edges for this shape. This will be determined in the course of data takeover insofar as possible
from the maximum edge number or corner number.
If a processing was present in the AWE BOM, but not in the SN BOM, this processing will be
marked for deletion. If it is a standard edge processing, then the user will be asked whether it
should actually be removed. If this processing should remain, it is not deleted. If a perfect
synchronization succeeds (snstatus < 100), then this is also reported in the SN file if the file
depends on the position (snstatus < 0). The same also applies for standard stamps if it is not
present in the SN BOM. However, this can then not be taken over if a free shape was reported
from iTOE.
If the processing marked for deletion is not directly on the glass in the AWE BOM, but rather
under a META processing, then during the synchronization not just this processing, but the
complete META processing will be removed from the BOM.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                14
5.1.2. Starting the TOE from the A+W Enterprise BOM
After entry and confirmation of the dimensions, you are (usually) in the "Procurement type" field.
There, you can start the TOE with the key combination CTRL+F or ALT+F. Important for the
starting is that in the AWE the existing processings are already completed with all parameters and
thus they can be passed to the TOE. Starting at an earlier point in time, even if the dimensions of
the item are known, is not permitted.


5.1.3. Message box messages
If within the TOE there is an error in the SN, the error message is transferred by the SN to the
AWE back end and displayed there in a message box.
The message is displayed in the language in which the communicating SN was installed.




5.2. Operation in the A+W CAD Designer (Shapes)
5.2.1. iTOE menu elements
Currently, the iTOE can be quit via 4 different menu elements or function keys (AWDesk
#449540).
The hotkeys can only be used when the SN is in focus (foreground).



    •   Quit TOE <F2>
        Change to the A+W processings are taken over into the AWE BOM.

        Insofar as possible, no SN file is stored for the item. Without a corresponding file, the
        person making the entry has the greatest degree of freedom. All changes to the BOM
        (new processings, glass exchange, changes to processing parameters, shapes, muntins,
        steps or global BOM exchange) are then still permissible.


    •   Cancel TOE <F3>
        All changes made in the TOE are discarded. The AWE BOM remains in the state before
        entering the TOE.


    •   Quit TOE and save file <F4>
        Change to the A+W processings are taken over into the AWE BOM.
        In addition, the corresponding SN file is saved.


    •   Save TOE file without SL balancing <F5>
        Change to the A+W processings are NOT taken over into the AWE BOM.
        The SN file is saved with all changes made in the TOE.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                                 15
    •   Import the ERP BOM <F6>


    •   Discard file and reset from the ERP BOM <F7>



5.2.2. Application of processings for IG/LAMI
With IG or LAMI, the SN file has several resolution stages. On the top level is the header part, then
the partial products. Generally, if possible, all processings should be applied to the header part.
You can then use the Processing/BOM menu element to assign a particular subpart. This has the
advantage that the processing is also visible if a drawing of the header part (e.g. in SNLive) is
displayed. Furthermore, only these processings are synchronized with the AWE BOM.




5.2.3. Edge processings view
In the "Edge processings" view, no interior cutouts/drillings may be deleted. For this, you must
change to the "Interior contours" view.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                                16
5.2.4. Applying drillings to IG and LAMI
The drilling is applied to the header part.
If a drilling should be applied explicitly to the subparts, the drilling must be selected and then
selected in the Processing > BOM menu. Then the drillings can be selected per glass and you can
select the check mark for the parts in the appropriate box.




5.3. Emergency dialog
When the iTOE is started, the A+W Enterprise creates a dialog in the background with which the
iTOE (the started SN) can be terminated. The dialog contains as buttons exactly the same menu
items as those available in the SN menu for exiting the iTOE. The dialog is only intended for
emergencies when the SN no longer responds to clicks or keys for some reason. The emergency
dialog was built in during the development of the iTOE, because in the predecessor module
AWBroke exactly this problem could occur: The AWBroke module sometimes got stuck and ALCIB
could no longer be operated. ALCIB then had to be terminated via the Task Manager. Order data
was lost in the process. To prevent such problems in the ITOE, the emergency dialog was
implemented. It should prevent the loss of order data in the event of problems in the SN.
So far, however, no problems with the SN are known in the iTOE. The emergency dialog seems to
be obsolete.
With AWDesk #449540 the shortcuts to exit the iTOE / to return from the iTOE are now also
displayed in the emergency dialog (just like in the SN menu). However, the function keys cannot
be used if the emergency dialog is in the foreground. The function keys can only be used when the
SN is in the foreground. If the emergency dialog is in the foreground, the function keys do not
lead to the desired effect.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                             17
6. Functions
6.1. Status of an SN item
The status of an item that was processed with TOE was stored in the new field kpos.snstatus. The
SN status is displayed in the order entry in the item details next to the name of the CAD file.
Overview of possible status values
 SN status         Description
 0                 All CAD processings were taken over into the AWE BOM and no associated
                   CAD file was saved
 1                 The associated CAD file is saved at the request of the person making the entry.
                   (-> SN menu element: Exit TOE and save file)
 2                 The associated CAD file is saved because it contains information that could not
                   be returned as AWType to AWE.
 3                 The associated CAD file is saved because for a reported AWType, no
                   appropriate processing was found in the master data.
 4                 2+3
 5                 The associated CAD file is saved because status 1,2,3 or 4 was reached and in
                   addition, this is a free shape or a fixed geometry (shape dimensions may no
                   longer be changed).
 6                 This status is set if one or several generalized cut-outs (AWType 1303, 1403,
                   1418) are reported from the iTOE (status = 2) and also fixed shape dimensions
                   (status = 5).
 7                 This status is set if the associated CAD file is saved because it contains
                   information that could not be returned to AWE as AWtype. (status=2) and also
                    if one or several generalized cut-outs (AWType 1303, 1403, 1418) are
                   reported from the iTOE (status = 2).
 8                 This status is set if one or several generalized cut-outs (AWType 1303, 1403,
                   1418) are reported from the iTOE (status = 2) and also unknown shape
                   dimensions (status = 5)
 100               AWE BOM and CAD file are in a non-synchronized state. In particular free
                   shapes and shapes from SN with shape change ("cadShapeTransformation")
                   receive the status 100 after initial transfer and must be adjusted manually in
                   case of further adjustments.
 101/102           Special status for steps (step changes in the SN are not taken over into the
                   AWE)
 103               After AWE inheritance of processings by intauf. New processing are generated
                   here, which do not exist in the SN file.


For status values >= 100, it applies that:


A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                18
All additional changes to the AWE BOM are NOT taken over into the CAD file.
All additional changes to the CAD file are NOT taken over into the AWE BOM.
This means that production-relevant changes must be made explicitly in the CAD file and changes
that affect prices or texts explicitly in the AWE BOM.


6.1.1. Changing the BOM with existing SN file
For the following changes to the AWE BOM, currently there is reliance on status 100 if there is a
SN file:
    •   Exchange of glass or foils
    •   Change or new generation of steps


If an item is in SN status 1-4, the following changes can still be made without having to convert
the status to 100:
    •   Add, change, delete items without A+W processing type
    •   Change of texts
    •   Change of processing parameters
    •   Change of procurement types, print identifiers,…
    •   Dimension changes also to shapes, these are then synchronized with SN; if this
        synchronization encounters an error, this causes a change to status 100
If an item is in SN status 6,7 or 8, you:
-       can no longer change the parameters for these generalized processings in AWE;
-       can no longer change the parameters for all other processing that are reported after "2
edges" from SN;
-       can no longer change the item dimensions
-       cannot add new processings with the dimensioning "after 2 edges" in the AWE BOM. It's
best to convert to "absolute". Important for stamp!
These changes, if it is necessary, should be made directly in iTOE as correction and the data
synchronized again. This is possible according to the status < 100.


6.1.2. Entry of following items
If after an item entered via the iTOE the next item has an identical item article, then the BOM is
always taken over with all processings and only the number of the BOM is incremented. This can
make additional entry difficult since all additional processings in the following item are generally
not desired and they should be taken over from the SN file via the iTOE.
During the entry of a following item with the same header article, there will now be a CU query
whether the BOM in the original is desired. Of course this can also be disabled via customizing, so
that original BOMs are always obtained automatically.




A+W Software GmbH                  EN-CONFIG-A+W Enterprise iTOE.docx                               19
6.2. Import of DXF files
The DXF import can be used without SN license. In this case, a call of the SN in the foreground or a
synchronization of the BOMs (iTOE) is not possible.
This section describes only aspects of the DXF import that are related to the iTOE.
A detailed description of the DXF import is in the "Enterprise" configuration instructions.


6.2.1. DXF Import in SN
The import of a DXF file in SN can be done as follows:
    -   in the AWE order entry, enter an item with shape 0 and dummy dimensions
    -   start the iTOE
    -   change to the Sketch dialog and delete the existing contour
    -   change to the DXF Import view
    -   select via the Import > DXF menu
    -   select DXF file to be imported
    -   mark contour and define as shape glass
    -   exit iTOE with "Exit" menu element



6.2.2. Corrections
After DXF import the following problem occurred in SN-Live sketches: with particular BOM
configurations, it happened that after the iTOE comparison of an SN sketch with shape with an
AWE BOM, incorrect shape parameters were then displayed in the SN Live sketch. The problem
only occurred with BOMs for which several shape sets were stored in the KMODPARAM table, and
only if the SN file was not retained after the iTOE adjustment. This has been corrected in later
versions.




6.3. Level conversion
Normally, the interface (AWE front end - CAD) is responsible for converting the glass and
processing data from AWE format into CAD format and back during the transfer (e.g. processing
vector).
The transfer of the level index is an exception. The AWE index (1, 2 or 3) is transferred to the CAD
and the CAD converts the value. Returned by the CAD is the CAD index (-1, 0, 1), which is handed
off to the back end this way. The back end then converts to the AWE values.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                               20
6.4. Generation of the SN file name
The file name, which is later stored in kposp.brokefile (that is, only the relative path below
SNFILES_DIR), is composed as follows: TOE\<Year>\<Month>\<Day>\<aufnr>_<posnr>.sn
Example:
aufnr 123456, posnr 1 on 07/04/2018 => file name TOE\2018\7\4\123456_1.sn


6.5. iTOE: Support of stamps
The iTOE also supports the surface processing "Stamp". Rules can be created for this and
automatic matching is also supported for this product group.
If the stamp number from the A+W CAD Designer (Shapes) is reported, it must be used for the
referencing (E/A rules).


6.6. Individual lite cutting of LAMI rounded corners
For rounded corners on LAMI, there is now the following additional functionality in the A+W CAD
Designer Shapes:
The rounded corners can be cut on individual lites and processed on the LAMI (polished). To do
this, the rounding must be transferred from AWB/AWE only on the LAMI, when saving the SN file,
the system checks whether the cutting is possible. The cutting point is then adjusted accordingly.
This function is enabled by configuration switch
(SN.ini, section User)
LamPreferCutRoundedCornersOnParts =1 activated.
When an SN file is saved, the system checks whether the BOM for rounded corners must be
adjusted. This is the case if the file contains a LAMI or an IG with one (or more) LAMI on which
there are one (or more) rounded corners. For each rounded corner, it is examined whether it can
be cut to size on all individual lites of the LAMI depending on the radius and glass thickness of the
individual lites. There are already some configuration options in SN for this purpose. If it can be
cut to size on all lites, the BOM is adapted to the rounding so that it is inherited by the partial lites
and then also appears in the cut. The radius on the partial lite results from the recorded radius of
the rounding plus the possible addition for LAMI grinding or polishing.
The roundings are generated if the corresponding A+W standard processing is available in the SN
file. This is the case if the file was created from orderXML or if a BOM (iTOE) was made.


6.7. Transmission of generalized edge and corner cut-
   outs
You can now create exchange rules in the iTOE for the processing of the AW types corner cut-out
(1300), edge cut-out (1400) and inner cut-out (1415), which require a special production, which
are marked as "special processing" by marking them (detail dialog in the exchange rules). These
processings come from the iTOE with the special AW types 1303, 1403, 1418 and are mapped in
the interface to the generally valid processing types 1300, 1400, 1415 and additionally marked as
special processing. If at least one processing of these special types is reported from iTOE, the SN

A+W Software GmbH                  EN-CONFIG-A+W Enterprise iTOE.docx                                 21
file is kept in the item and the item receives the SN status 2, 4 or 5 (depending on additional
conditions). This enables additional comparisons of changes in both systems.
For the special corner cut-outs we recommend creating a separate article in the master, where
the processing parameters "Orientation to A" and "Orientation to B" are deactivated. For the
other two, it is optional whether they are to be represented by their own processing articles (for
example, for a different price).

Starting with alcib - 13.04.10833 and SN 13.4.2776.9000 (Released with Quality Release
(2022/02))

Generalized cut-outs: affected are processing with AW type in iTOE/SN 1303,1403, 1418. In A+W
Enterprise, these processings are bent to the "normal," saved as 1300, 1400, 1415 +
poszu.dmes10 = 999 and can be recognized this way.

These processings cannot be described correctly in A+W Enterprise and therefore not all changes
in A+W Enterprise can be reported back to A+W CAD Designer (Shape). Since customers are
becoming ever more courageous with the use of iTOE, the problems that are associated with
these processings and cannot be solved directly in A+W Enterprise are occurring more frequently.
The consequence of this is a not very meaningful error message from A+W CAD Designer (Shape)
and resetting of the item to status = 100 in A+W Enterprise, which stops all further actions with
comparison.

According to the extensive error behavior analysis, there are now new values for the field
kposp.snstatus (see also the table documentation)

    -   Status = 6 => if everything ok + generalized processings
    -   Status = 7 => old status = 2(additional info directly in SN Datei) + generalized processings
    -   Status = 8 => old status = 5 (unknown shape information) + generalized processings


If status 6,7 or 8 is determined now, you:

    -  can no longer change the parameters for these generalized processings in AWE;
    -  can no longer change the parameters for all other processing that are reported after "2
       edges" from SN;
    - can no longer change the item dimensions
    - cannot add new processings with the dimensioning "after 2 edges" in the AWE BOM. It's
       best to convert to "absolute". Important for stamp!
These changes, if it is necessary, should be made directly in iTOE as correction and the data
synchronized again. This is possible according to the status < 100.

The interception of the changes that cause errors during the comparison with iTOE was already
done in earlier versions (beginning of August 2021). The rules were too restrictive, however, so
that nearly everything was forbidden if these processings were taken over from iTOE into the
BOM. Here's the less restrictive variant.

Unfortunately, there is no 100% solution here and so there may be additional cases.

See [AW-84741].




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                                22
6.8. Deco numbers for special edges
Order entry:
Deco numbers can now be stored for special edges (AWType 1090). The deco numbers are
transferred to the production as well as to the SN/SNLive when generating sketches and SN files,
so that a corresponding deco text appears on the sketch.

The deco number is also transferred in the iTOE.

The general search for edge processing can be limited purposefully via deco number.

Master data in A+W Enterprise:
Processing steps with AW processing type=1090 should be stored in Article master-><F4> >Article
dimensions data with fixed parameter. It will not be possible to change this during order entry.

A+W CAD Designer (Shape):
In the SN.ini, the deco settings are stored in the [Decoration] section.
For the deco numbers of special edges on single lites, the ranges Deco11 to Deco27 and Deco100
to Deco131 are provided as standard [addendum of DPE: according to Wolfgang Trost, the deco
values from 100 to 131 are not available in production as of 11/15/2018]. Please note that the
deco numbers stored in the AWE have an offset of +1 to the deco variable in the SN.ini. AWE deco
number 12 therefore refers to "Deco11" in the SN.ini etc. Deco number is to be stored as a fixed
and non-modifiable parameter under article dimensioning.

For use of this function, an update of A+W Enterprise (front end, back end) and A+W Production
has to be made.


6.9. Number of edges in prices for shape 99
The old rule "Shape 99 has 4 edges" no longer applies since it was possible to enter shape 99
using the iTOE. Depending on the SN view, the iTOE always delivers up to 10 edges. At this point,
A+W Enterprise also cannot recognize whether it is about "all edges" or whether it was passed on
to AWE only because of the limitation to 10 edges. With fewer than 10 edges it is also not known
whether here for shape 99 "all" or only some edges/corners are processed. Thus, the general rule
cannot apply here that for all edges, the data has to be retrieved from price properties. For this
reason, all edges reported from iTOE are also transferred here in the AWE as price-relevant
quantities and then also calculated with e.g. 5 x width + 5 x height or 4 x width + 6 x height.
One possibility for further calculation of the 4 edges in shape 99 is to maintain the data in the
master differently. So first allow 10 edges for the number of edges. And then to set the
"remaining" edges (from the 5th) to calculation type "none".

However, this only works after activating the following configuration:

99.frm on site (insert 2 lines for $edges) or take from us. UNIX side only. $XOPTDIR/0/99.frm
        $edges
        10
FREIE_FORM_KANTENTOE = Activate ON.


A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                             23
6.10.           Use of templates
The use of templates was not previously provided in the ITOE.
Currently, templates can only be used in the AWE environment by the AWE CAD service (within
the special logic of Kermi and Glasprofi).
The selection of a template and corresponding entry of all corresponding parameters in an order
item of the order entry is not possible.
However, a template like any other SN file can be used for synchronization. For this, the template
file is added as SN file to the appropriate item (CTRL+E) and then "synchronization" is selected. In
the CAD program, the dimensions can then be adjusted and after that, the template information
taken over into the AWE BOM by exiting the TOE.


6.11.           Special treatment of particular shapes in SN
6.11.1.         Shapes with special treatment in SN
The shapes 66,67, 76 and 77 are treated specially in the SN and at the moment cannot be
processed in the TOE.


6.11.2.         Shapes with different numbers of segments and edges
The shapes 60, 61, 62, 63, 81, 74, 75, 78, 123, 124, 125, 133 are processed in A+W CAD Designer
(Shapes) with a number of segments that differs from the number of edges in A+W Enterprise.
When applying a processing with dimensioning to 2 edges in CAD Designer, these processings can
therefore no longer be compared to the SN after the import into AWE if there is an attached SN
file. The items receive a status that excludes a further comparison (status 100).
However, problematic situations can still occur.
Example:
Shape 78, drilling, dimensions for 2 edges, comes with CAD vector "1001" (dimensioned for
Segment 1 and 4) back from the SN, it becomes bearbvek "11" in AWE. BOM is compared and SN
file is (absolutely!) maintained. Status is now 100.
Now the SN file is discarded. Here you will see a warning message that the sketch was not
synchronized completely with the BOM.
If after that the SN sketch is generated from the AWE BOM, the drilling is dimensioned for
another segment than in the discarded SN file. (AWD #393874).


6.11.3.         Full-surface coatings on shape 99
When applying coatings over the entire surface, a dimensioning problem could occur in CAD.

The env variable VSGVERERBUNG_MIT_ITOE is transferred to the front end and evaluated there.



A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                               24
If the variable is active, the processings are queried in the iTOE for the SN with the method
GetProcessings() with "Mode 2" (include representative).

If the variable is not active, the processings are queried in the iTOE for the SN with the method
GetProcessings() with "Mode 0" (standard logic, do not include representative).
The changes in the back end and front end change the standard behavior in iTOE if a new front
end is delivered to a customer but an old AWE back end is still used.


6.11.4.         OrderXml transfer for processings on free shapes
Handling of more than 10 corners and edges

Since the standard shapes in the A+W shape catalog cannot have more than 10 edges, the
edge/corner vectors are limited to 10 system-wide. When entering free shapes via iTOE, however,
the processing at an edge > 10 can be reported back to AWE. These processings are transferred
"internally" to the last edge = 10 so that they can also be evaluated. The edge/corner vector
remains empty for this processing. The corner is then texted as "Corner > 10". In the processing
dialog, a "*" in the edge number indicates that there are more than 10 edges/corners.

General description of processings on free shapes (shape 99) in interplay with the CAD modules
(iTOE and AWE CAD Service) and for OrderXML transfer
The handling of processings on free shapes is difficult in A+W Enterprise since the number of
corners/edges of the shape is not known. Depending on the processing flow, situations may arise
in which it is no longer possible to display the processing parameters correctly in AWE. Even when
the file is transferred to production (OrderXML file), the parameters cannot be specified correctly.
When a Shape 99 is transferred to production with SN file, production must therefore always be
based on the SN file, never on the transferred BOM.
In principle, processings for a shape 99 can only be recorded in the AWE with regard to the
circumscribed rectangle, since - as already mentioned - the number of edges/corners is not
known. Entering edge or corner processing at a specific edge/corner therefore makes no sense. It
is also not useful to use a dimension type other than "Absolute".
Another problem resulting from the unknown edge/corner number is the conversion of the AWE
edge/corner vector into the edge and corner numbers passed in the OrderXML file. For historical
reasons, the edge vector (poszu.bearbvek) stored in the AWE contains the edges/corners
clockwise and also only a maximum of 10 edges/corners. The production and CAD systems expect
the edge/corner numbering to be counterclockwise. If now the number of corners / edges in the
free shape is not known, the correct production / CAD edge / corner can no longer be determined
from the AWE vector.

Example:

An SN file with shape 99 with 11 edges/corners is attached to an AWE item and synchronized. The
SN files contains rounded corners on the corners 1, 2, and 11.
Here is an overview of the current handling of the processing vectors:designation CAD vector
conversion in AWE vector (maximum 10 places) transfer in the OrderXML file
Rounded corner on corner 1 10000000000 1000000000 corner 1 because can be assigned clearly
(corner 1 always remains corner1)
Rounded corner on corner 2 01000000000 0000000000 corner "all" since the corner has been lost
in AWE vector and the scheduling would fail if no corner would be specified.
Rounded corner on corner 11 00000000001 0100000000 corner "all" because the corner in the
AWE vector cannot be converted to the production corner (11), because the information how

A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                                 25
many corners the free shape has is not available in the AWE.
If no corner was specified, the import would fail.


6.11.5.          Full-surface coatings on shape 99
When applying coatings over the entire surface, a dimensioning problem could occur in CAD. Here
the env variable VSGVERERBUNG_MIT_ITOE is transferred to the front end and evaluated.
If the variable is active, the processings are queried in the iTOE for the SN with the method
GetProcessings() with "Mode 2" (include representative).
If the variable is not active, the processings are queried in the iTOE for the SN with the method
GetProcessings() with "Mode 0" (standard logic, do not include representative).
The changes in the back end and front end change the standard behavior in iTOE if a new front
end is delivered to a customer but an old AWE back end is still used.




6.12.   Calculation of edge processing in a special
   shape (shape 99) when transferring SN files
When importing edge processing steps from an SN file, a solution was first suggested to set the
number of edges for shape 99 via the FRM file and in the master to 10, because up to 10 edges
can be reported from the iTOE. However, this solution has led to the problems with the normal
AWE entry for the special shapes, since this is only possible in the AWE by dimensioning a
rectangle. For this reason the first solution was abandoned. Shape 99 should continue to be in the
FRM file with number of edges 4 and edge assignment in the master should again only be done
for 4 edges or it should be removed completely. The price-relevant data for the edges, which are
transferred from SN file, are regulated in AWE via the article dimensioning (default number), if it
is reported from TOE that the respective edge processing is present on all edges.

When exchanging an edge processing in the AWE BOM after synchronization with an SN file that
is saved, it could happen that the current edge processing was missing in the SN file. The problem
has been eliminated. A current AWE front end has to be installed.


6.13.            Free shapes
Communication of A+W Enterprise and A+W CAD Designer (Shape) was reworked with regard to
iTOE processing of free shapes.


6.14.  Fixed products with SN files without iTOE
   module
In version AWE6 there is the possibility in AWE to attach SN files to fixed products. However, this
functionality was only intended for users of the iTOE module. Now it has been extended for the
other users as well.
If an SN file (kpos.brokefile) was assigned during fixing (directly in the field via F9. Not via scripts),
it is saved under <ARTIKELBILD_PFAD>\SN\<artnr>.SN (art no of the fixed product). This file is


A+W Software GmbH                  EN-CONFIG-A+W Enterprise iTOE.docx                                   26
located here as part of the master data and is never deleted unless the existing fixed product is
overfixed with a new file. If the file <SNFILES_DIR>\FIXPROD\artnr.SN already exists, which means
that orders for the product have already been entered, this file will also be overwritten.
If the product is now entered in an order, the SN file <ARTIKELBILD_PFAD>\SN\artnr .SN is
automatically copied to <SNFILES_DIR>\FIXPROD\artnr.SN (if it is not yet there) and the name
"FIXPROD\<artnr>.SN" is also written to kpos.brokefile. This file is also not deleted if the file
assignment is then removed in the item with CtrlF9.
This logic can be activated via the ENV switch. For existing fixed elements, a subsequent
maintenance is first necessary: You should manually assign the corresponding file to each product
via Master->Fixed Products via F9 in the field and then overfix under the same number.

Configuration: FIXPROD_WITHSN = ON


6.15.           Attaching SN files during product fixing
With the appropriate configuration, it is also possible to add a separate SN file to the fixed
products (Article master -> Finished products -> Article fixing). A separate internal number is
assigned to the temporarily created file. You enter data in the same way as you enter items in a
sales order (order/quotation). If the selected item is marked for product fixing (<Shift+F8>), the
file is stored in a separate directory under the product number directly after the new product
number has been assigned (subdivision SN in the $ARTIKELBILD_PFAD). The file with the
temporary number is then deleted. The dimensioned product receives the flag artikel.prodbemass
= 3 in the master, so that it can be recognized later when external EDI is set up. During order
entry, the SN file of the product (<Produktnummer.sn>) is transferred to the current item with the
name <aufnr>_<posnr>.sn. All fixed products with an attached SN file are given the status 100
(can no longer be synchronized), because only in this case is it useful to get the file. All other
changes must be made separately in iTOE and AWE. This must also be taken into account when
over fixing.
Even if the item is selected for fixing in order/quotation entry, the procedure described above
applies except that the item file is deleted.
The transfer of the fixed elements via external EDI is not part of this development and can only be
developed separately after the respective interface has been clarified.

Configuration: Please check that it is possible to create the directory <$ARTIKELBILD_PFAD>/SN
and that you have the rights to write the files.
ENV switch FIXPROD_WITHSN = ON


6.16.     Import of SN files when creating stock orders
   of fixed products with subparts
The SN transfer logic has also been extended for stock fill orders. The settings described in case
#440332 must also be set up for the stock fill orders. If a filling order is now generated via the
warehouse, the article master is used to check whether an SN file is available and this is moved
via FTP into the iTOE folder structure ($DFUE_SNFILES_DIR\TOE\<YYYY>\<MMM>\<DD>\) with a
new name.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                              27
6.17.           Adaptation of SN sketch in printout
This development is intended to create the possibility of suppressing certain processings during
output of a sketch in the printout.
The control takes place via print flag within the order BOM.
The print service calls the sketch interface with an additional indicator. If the sketches are to be
created for a work order or a copy of a work order, the Production indicator is transferred,
otherwise Sales. Creation of the sketches is taken over by the corresponding sketch module.
If the print service requests an SN sketch for an item, a special logic runs if the env variable
SNLIVE_EVAL_PRINTFLAG is active. The print flag (AUFSTRUKT.DRUCKKZ) is checked for each AW
type processing of the BOM and a decision is made whether the processing appears on the SN
sketch based on the current form type and the setting of the print flag:

    •   Print flag "N" => Processing is not printed

    •   Print flag "Y" => Processing is printed

    •   Print flag "P" => Processing is printed, if the form type is "Production paper".

    •   Print flag "V" => Processing is printed, if the form type is "Sales paper".

Restrictions to be observed

    1. The SN sketch that the user sees in the order entry is not the same that appears on the
       printout. In the SN sketch of the order entry, all edits are still displayed, independent of
       the print flag. Exception: An SN file is attached to the item. In this case, the SN sketch in
       the order entry shows the image that also appears on the printout.
    2. If an SN file is assigned to an item, the person who drew the SN file is responsible for
       ensuring that the print sketch is in the correct form, i.e. the print sketch only contains the
       processings that the recipient of the print sketch is to see. In this case, the print program
       does not influence the print sketch.
    3. When the iTOE is used, the same applies as in point 2: When using the iTOE to attach an
       SN sketch to an item, the user operating the iTOE is responsible for ensuring that the print
       sketch contains only the processings that the recipient of the print sketch should see. In
       this case, the print program does not influence the print sketch.
The only form that has a production character is the work order, which has form type 27. In
addition, there are form types 31, 132, 142, 927, which are used as work order copies. These are
treated as form type = 27.

Configuration: SNLIVE_EVAL_PRINTFLAG.

If the variable is active, the print indicator for the processings is evaluated in the print service
when the SNLIVE sketch is generated. Depending on the form to be printed, the system decides
which processings appear on the sketch. The variable does not influence the display of the SNLIVE
sketch in the front end. Here all processings of the AWType catalog always appear on the sketch,
independent of the print indicator.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                   28
6.18.   Acceptance of SN files of ordered subparts in
   purchase order generation and transmission.
The developments from cases #430912 and #437924 are a prerequisite for the new logic of taking
over SN files of ordered subparts in purchase order generation and transmission.
As developed with the above mentioned cases, this development also concerns the ordered lower
part insulating glasses. Since it is not possible to attach SN files to sub-parts, a logic was
developed which checks whether an SN file exists in the master data of the ordered sub-part
insulating glass. If this is the case, then this SN file is attached to the order when the order is
generated and is also transferred when the order is transferred.

PO creation:
Site a)

    •     The system checks whether the item article in the purchase order (BOM sub-parts of the
          order) is a fixed article (article.prodbemass = 3).
    •     If it is a fixed item, the system checks whether there is an SN file in the item master data
          for this item. This is done by checking whether an SN file (article number.sn e.g.
          "4711.sn") exists in the path $DFUE_ARTIKELBILD_PFAD\SN\.
    •     If an SN file exists for the respective article, this file is copied from the current path to the
          TOE SN file path ($DFUE_SNFILES_DIR\TOE\<YYY>\<MM><DD>\) and renamed to match
          the order (<aufnr>_<posnr>.sn e.g. "27001_1.sn").
    •     The database field kposp.brokefile is then updated with the SN file and its subdirectories
          (e.g. "TOE/2019/4/10/4711"), and the database field kposp.snstatus is set to 100.

PO transfer:
Site a)

    •     First, the file name is determined from the database (kposp.brokefile).
    •     Then the packet is created with the SN file and transferred to site b.
Site b)

    •     The transferred package with SN file is unpacked.
    •     The order is created.
    •     The sent SN files are renamed with the new number range of site b (<ordno>_<itmno>.sn
          e.g. "52001_1.sn").
    •     The new SN file name is updated in the database (kposp.brokefile).

    •  Finally, the renamed SN file is moved to the TOE-SN file directory of site b
       ($DFUE_SNFILES_DIR\TOE\<YYYY>\<MM>\<DD>\).
Configuration:

The prerequisite for using the new logic is an FTP server on the Windows computer and a working
FTP connection for user: alcibnet.

Environment variables:



A+W Software GmbH                   EN-CONFIG-A+W Enterprise iTOE.docx                                   29
    •   IB_MIT_SN_DATEIEN must be set to "ON" so that the SN files are also transferred in the
        order transmission. The variable must be enabled both in sending and in receiving client.
    •   DFUE_SNFILES_DIR the Windows path of the iTOE SN files must be entered. The variable
        must be enabled both in sending and in receiving client. Notation <server>!<relative or
        absolute directory>
    •   DFUE_ARTIKELBILD_PFAD the Windows path for the article pictures must be entered.
        Notation <server>!<relative or absolute directory>

FTP scripts
The following scripts are required for this logic on the Unix machine:

    •   ftp_lsdirpc_sd: Creates a list of files in an existing Windows directory.
    •   ftp_mdirpc_sd: Creates a Windows directory.

    •   ftp_topc_sd: Transfer file from Unix to Windows machine.

    •   ftp_frompc_sd: Transfer file from Windows to Unix system.


6.19.   Extension of the iTOE exchange rules for
   countersunk drillings
For countersunk drillings, one of the most important dimensions is parameter 5. However, the
iTOE specific exchange rules were only provided for the first three parameters. For this reason, it
was not possible to distinguish between one-sided and two-sided countersunk drillings. With this
extension, a countersunk drilling on both sides can now be defined by maintaining parameters 2
and 5. Important is also that for the countersunk drilling, you mark every 3rd diameter for testing;
this should also be the case for one-sided countersunk drillings. The exchange rule for iTOE has
been extended and refined so that the decisive parameters for evaluation can now be stored. The
evaluation has also been extended accordingly.




6.20.  Preventing                            additional                  synchronization
   manually
Set SN status = 100 manually with Ctrl+A in the field "SN file".
After the data takeover from the iTOE, sometimes it is necessary to restrict additional changes to
the AWE BOM and no longer to synchronize them with the SN file.
For this case, it is possible in all items with SN file and a free mode for synchronizing the data (SN
status < 100) to set the mode = 100 manually with Ctrl+A in the "SN file" field and thus to prevent
the synchronization.
Setting of SN status = 100 is done after a corresponding CU query was confirmed.
Caution: This action cannot be undone.
See PF [AW-152766].



A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                30
7. Inheritance with an in iTOE
7.1. Ordered subparts with SN file
If an order item contains an ordered subpart and a SN file was attached to the item, then this item
is also taken over into the order item (subpart). The SN file still contains the glass structure of the
entire order item and not just of the ordered item.
From this it follows that in the SN file (through inheritance from the header part), processings can
be contained on the ordered glass (e.g. drillings) that should not be made.
If an order item contains an ordered subpart and a SN file was attached to the item, then this file
is also taken over into the order item for the subpart. The SN file still contains the glass structure
of the entire order item and not just of the ordered item. From this it follows that in the SN file
(through inheritance from the header part), processings can be contained on the ordered glass
(e.g. drillings) that should not be made. When printing out the order via the A+W Enterprise Print
Service, the CAD sketch is also printed according to the attached SN file.


7.2. iTOE inheritance of the LAMI processing on the IG
If the processings are inherited via the iTOE (from bottom to top), the relationships between the
price-relevant LAMI processing on the LAMI itself and the production-relevant LAMI processings
on the individual lites in the BOM are noted. If this is LAMI in IG, then for the subsequent change
of the BOM on the IG level, all tuples of the BOM are renumbered. Here, the existing dependency
of the inherited LAMI processing is not considered. Since earlier the inheritance was always
updated by the background process intauf, this had no disadvantages. For the inheritance via the
iTOE, however, the inheritance takes effect right away and is no longer updated, and thus the
establishment of the dependencies is very important. This has now also been implemented.


7.2.1. Print indicator/procurement type of LAMI processing steps
    with inheritance function
If inheritance via iTOE is active, the processing is taken over as reported by iTOE. The connection
of the representative processing steps (processing steps on the LAMI article for pricing) is still
maintained and the "inherited" processing steps are marked with an asterisk. No changes
(parameters) may be made for these processing steps. All processing parameters must therefore
be carried out on the processings of the LAMI BOM level and are then adopted in all
corresponding "inherited" processing steps. The parameters can be changed via the general
processing parameter dialog or from the processing parameter dialog in the BOM. However,
changing the parameters in the BOM directly ("Processing parameters (short)") is not permitted.
The control of inherited processing steps by the background process intauf was deactivated for
the new inheritance logic (in case of inheritance by AWE, all inherited processing steps from
intauf are always deleted and re-inserted). To keep the new tuple numbering, the deletion had to
be reorganized. If it is now necessary to delete a processing at LAMI level and the corresponding
processing is also available at individual lite level, it must first be deleted manually. Only then the
representative processing can be deleted.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                                 31
7.2.2. Problems with LAMI inheritance of edge processings on free
    shapes
Work-around in AWE:

There are two different problems. In the case of the SN file 2122311017.SN, there is an error in
creating a rounded corner in the SN file. The rounded corner has to be inserted in the geometry.
After the correction of the SN file, the BOM synchronization should work here.

The cause of the endless loop for SN file 212231014.SN is that for the file in question, from the
CAD, the edge processing for each edge or each segment of the free shape is not reported back (-
> getProcessingDetails()). On the one hand, there are edges/segments for which no edge
processing is reported; on the other hand, there are edges/segments for which the edge
processing is reported back for only one of the LAMI lites, even though the processing exists on
both LAMI lites according to the SN file. In some cases, the reference processing (-> for the LAMI
inheritance logic) is not reported back.

Now an env variable is made available that prevents the endless loop. If this correction logic
works, an appropriate message is output in the foreground:"No reference was found for at least
one inherited processing. The A+W Enterprise BOM absolutely must be checked." The AWE BOM
has to be adjusted if necessary.
So that the message is output in German, the fx_texte/messages have to be up-to-date:
fxtexte and messages at least from 10/01/2020

If the correction logic takes hold, a message is also written to the toeneu log with the notice that
an endless loop should be prevented.

ITOE_MISSINGREF_SETPROCREFZERO
If the variable is active, the reference for an inherited processing is set to 0
in the iTOE for LAMI inheritance if in the data that is reported from the CAD, no reference record
is found. This way, an endless loop
is prevented. However, the cause of the problem is incorrect data from the CAD. The AWE BOM
therefore has to be checked after the synchronization. Under some circumstances, missing
processings have to be added. For this, the
user receives the message 37894.
AWDesk #461339, PF52045

It is recommended that you set the env variable only temporarily at the moment in order to be
able to schedule individual orders where precisely this problem occurs during the BOM
synchronization. Since ET is currently not there, I have inserted the correction logic to the best of
my knowledge. However, it is possible that with the adjustment, I have created side effects that
could create other problems. That's why my correction logic should only be applied for selected
orders. The generated AWE BOMs must be checked precisely later on.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                               32
8. Text
8.1. Additional processing texts when synchronizing
   via iTOE with stamps
The additional texts for which processings in the master (artvermasspr.ztxt) applies as processing
parameter in A+W Enterprise, which however are not a component of the processing parameters
in SN, are completed with the takeover of the new processings after synchronizing from the A+W
Enterprise master data. For stamps, however, there is a special solution that you check whether
the output BOMs already have a stamp. This then causes the implementation of the new stamp
on the UPDATE mode. Here, all data from the iTOE is taken over. Here, however, the additional
texts for processings were lost. This program behavior has been corrected.


8.1.1. Processings are not summarized in the text area in order entry
With the conversion of the processings to A+W processing types, it became necessary to enter
these individually for some processings (e.g. drilling, edge cut-out). The texting logic has also been
adapted for the affected processings so that they are not texted individually. The processing
"Rounded Corner" remained definable even after the conversion via a vector and no summary of
the texts was activated. However, if the input is done via iTOE, identical rounded corners are
always reported individually to AWE. They are then also transferred individually for each corner.
For this reason, the combination of identical texts and the incrementing of the text components
$A1 and $AP is now also implemented for processings of type A+W rounded corner.




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                               33
9. Troubleshooting
9.1. Logs
See also "EN-CONFIG-A+W Enterprise System" section "Special things to note in the iTOE
research"


9.2. There is no reaction when clicking the TOE menu
   elements in the SN
Check registration of the SN or re-do the registration.
To do this, open a console with Admin rights, change to the path of the SN installation (generally
C:\Program Files (x86)\A+W\Techsoft\SN) and issue the following command:
SN -regserver


9.3. ISO items do not arrive complete in the SN
If in the CAD designer only one lite appears for an IG item, the BOM should be checked: if the
frame/spacer is a metapart, the lite does not arrive completely in SN.


9.4. Dimensions of the circumscribed rectangle for
   rotated shapes
When using the iTOE, the correct dimensions of the circumscribed rectangle were not
transferred to the AWE for rotated shapes. Up to now, the dimensions of the absolute
rectangle were taken over and not the dimensions of the rectangle with respect to the
base edge of the rotated shape. The problem has been eliminated.


9.5. Alignment of stepped drilling
Stepped drillings were not always aligned in the ITOE. This has now been corrected.
During the transfer of the stepped drilling from SN to the AWE an exception occurred
and a message about an "Unspecified Error" was displayed. This problem was also
solved by an adjustment in the AWE front end.


9.6. BOM synchronization for very flat cut-outs
Very narrow cut-outs may not have been correctly reported back to iTOE. This has now
been corrected.



A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                              34
9.6.1. Application of processings after shape change
In the course of the integrated TOE in AWE, the user can manipulate the shape in the A+W CAD
Designer (Shapes) so that the shape number changes. Then the edge numbers stored in the CAD
no longer fit the current shape. This could mean that with the subsequent application of
processings, the incorrect edges were referenced in AWE. The behavior has now been corrected,
the edges are identified with respect to the current shape information.


9.6.2. Improved consistency in BOM of surface processings
The case concerns SN files without a BOM (glass structure) to which a BOM is assigned. (especially
in the iTOE). In the case of surface processings, post-processing of the BOM for processings is
necessary, since no BOM-specific information can yet be stored in the output file.
The behavior has now been improved: If no BOM has been explicitly attached, the system
behaves as if the processings were attached to the header, the level as originally stored in the
value window. In the case of single lites, no reworking of the BOM is usually necessary. In the case
of IG/LAMI, adjustments must be made if the processings are to be applied to the parts. If you
store a BOM for a surface processing, this current status is now also displayed in the value
window. The transfer of the BOM to AWE now takes this into account correctly.


9.7. ITOE - takeover of the SN files for reference
If an order or quotation with reference to an existing process was entered with SN files, now the
SN files are copied and not taken over as reference.


9.8. Changes to an iTOE item after saving
In correction mode, old processing IDs were not transferred to iTOE and could therefore no longer
be found in the assigned file. This program behavior has been corrected.
Furthermore, you cannot discard the order in correction mode if the file assigned during entry
was deleted in at least one item.


9.9. LAMI BOM are mixed up after synchronization
By adding simple edge processings to a processed multiple LAMI via a separately generated SN
file, the existing edge processings on the LAMI header level were removed. As a result, the
original information supplied to iTOE about the position of the individual glasses has also
changed, resulting in an incorrect composition of the bill of material. This program behavior has
been corrected.
In addition, it was specified that no deviating processings are to be stored as an exchange that
differ in the dimension type or the dimension corner. This restriction also allows an optimization
of the communication between iTOE and AWE. If successively transmitted processings for the
same element also have the same parameters (diameter, radius, level, cut-out dimensions, etc.),
the first processing found (article number from the iTOE exchange rule) is noted and also used for
the next one.




A+W Software GmbH                EN-CONFIG-A+W Enterprise iTOE.docx                              35
9.10.     Processings are missing after synchronization
   with file on underglass in the SN file
The effect is caused for LAMI by an update of the processing in the SN, that is, the call of
ModifyProcessing() with "proc mode 0" if a processing changes due to the assignment of the AWE
article. This happens, for example, if a corner cut-off in the SN file does not include edgework, but
the synchronized AWE article has edgework.
The solution is to supply the processing in the SN with the correct parameters, here the
edgework.
See PF [AW-107312].




9.11.   Edge processings are missing after
   synchronization with file on underglass in the SN file
The handling of edge processings on free shapes has been improved. This affects the manual
attachment in the A+W CAD Designer. Frequently, the user selects the "Select all" menu option.
Here, however, with segment chains with smooth transitions, this creates more processings than
necessary. This makes processing further down the line slower and more complicated. Now, when
attaching, an analysis of the segment chains is undertaken and only the minimally required
number of processings is generated.
The second improvement is in the communication with order entry. Edge processings on free
shapes are now summarized by the CAD before they are reported back. This especially simplifies
the exchange of processings (e.g., grinding for arissing).
Set the switches in the SN.ini:
[User]
MergeEdgeWorkingOnFreeShape = 1


See also PF [AW-138062] and [AW-161206].




9.12.   Problems with cutbacks (cutbacks/frame
   deductions)
The SN reports the cutbacks as processings back to AWE.
This circumstance created follow-up problems (deletion of the cutbacks in the SN file).
The handling of cutbacks in the iTOW is (status as of 2/13/2024) not completely integrated.
See PF [AW-172587].




A+W Software GmbH                 EN-CONFIG-A+W Enterprise iTOE.docx                              36
10. Figures
10.1.       Overview of workflow




10.2.       Overview of data flow




A+W Software GmbH   EN-CONFIG-A+W Enterprise iTOE.docx   37
10.3.       Update of the CAD file




10.4.       Copy/delete the CAD file




A+W Software GmbH    EN-CONFIG-A+W Enterprise iTOE.docx   38

