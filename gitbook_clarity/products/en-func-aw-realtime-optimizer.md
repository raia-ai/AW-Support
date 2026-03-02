---
description: "EN FUNC A+W Realtime Optimizer"
---



# EN FUNC A+W Realtime Optimizer

     Functional Description


A+W Realtime Optimizer




                              english
1. Content
Notes on this Document
This documentation and the software described in it are only licensed and may only be used and
copied pursuant to this license. The contents of the documentation are for information purposes
only and are subject to changes without prior notice. The text and illustrations were compiled with
the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be
held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent
action.


1.1. Trademarks
All hardware and software names mentioned in this documentation may also be registered
trademarks or other industrial property rights held by third parties. Copyrights of third parties must
be complied with.


1.2. Copyrights
© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in an
archiving system, or transferred in any other form only in accordance with our license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


1.3. Disclaimer of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This also includes possibly
necessary long-term costs and expenses for amending and extending subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH                EN-FUNC-A+W Realtime Optimizer.docx                                3
2. Performance Description
2.1. Data
 Product                 A+W Production and others
 Module number           220016 – A+W Realtime Optimizer

                         230080-230083, 220080-220083, 220980-220983 –
                         A+W Realtime Optimizer (EL)

                         230116, 220903 – A+W Realtime Optimizer (Stand-Alone)
 Module                  A+W Realtime Optimizer
 Brief description       A+W Realtime Optimizer is a control station for the
                         improvement of yield and the cutting process.
 Available               Starting with A+W Production v5


2.2. Description
The A+W Realtime Optimizer is used primarily for control of the cutting process in production. In
addition to cutting table control, the A+W Realtime Optimizer offers the possibility of visualizing
the pattern to be broken on the cutting table using the Realtime Optimizer – Breakout Display and
reporting any breaks in the sheets back to the system.
During the cutting process, the A+W Realtime Optimizer offers various possibilities for feeding
rejects back into the production process through optimization. Similarly, it is possible to fill up
residual sheets with sheets of the next lot to be cut by re-optimizing the residual sheet.
If there is a residual stock, the A+W Realtime Optimizer can store residual sheets and use them
again, either through optimization or by substituting a residual sheet. Several optimizations created
in A+W Production can be combined and, using table-specific optimization restrictions, they can be
re-optimized.
It is possible to edit optimizations with the manual cutting plan editor or to create a cutting plan
completely manually. Progress of the production process can be booked precisely to the sheet in
the PDC. Labels can be printed stock lite by stock lite. If the hardware requirements for a defect
optimization are fulfilled, defects on the stock plate can be visualized with activated defect
optimization in the A+W Realtime Optimizer – Breakout Display. If optimization in the optimization
mode is available in the defects, there is an attempt while adhering to the storage location
sequence to place the sheets around the defect location.


2.3. Prerequisites
The standard A+W Realtime Optimizer requires an installed A+W Production module. The stand-
alone version of the A+W Realtime Optimizer can be operated without A+W Production. Only an
A+W Production database is needed.


A+W Software GmbH               EN-FUNC-A+W Realtime Optimizer.docx                                4
2.4. List of functions
2.4.1. General
BDE bookings
The following PDC functionalities are available:
    •   State bookings of the machine status for each configured cutting table.
    •   Booking of individual sheets on a registration point.
    •   Generation of breakage remakes in case of booking to a breakage registration point.
    •   A+W Serial Manager (series PDC). The series PDC is only possible for installations with the
        standard Panorama cut. In the DynOpt environment, no orders with quantity PDC can be
        processed since for the quantity PDC no unique lite bar code is assigned. Similarly,
        processing is not possible if a Panorama shape that deviates from the standard is stored,
        which executes a precise-to-the-lite identification via the bar code. Essentially, before using
        the A+W Realtime Optimizer for series PDC, you must consult A+W Development.
    •   Logging people in and out
        Several people can be logged in on each table.
        As soon as people can log in, it is absolutely necessary that all people logged in be logged
        out before the A+W Realtime Optimizer can be closed.
        It can be configured that a login is absolutely necessary so that the cutting function can be
        executed. The functions table optimization, edit in the manual cutting plan editor, entry of
        rush lites, entry of broken lites, and entry of manual plans are not affected by this and
        proceed now as before without logged-in user.
DC bookings require the A+W Barcode Manager module (article number 220010).
Batch identification
It is possible to book a batch identification for the cut lites. This batch identification is saved in the
system and can be determined in research cases. There are two variants here:
    •   The operator can enter a batch identification manually, This ID is used for all cut stock plates
        of the same type (item + dimensions) until the operator enters a new ID.
    •   Booking of external batch information for individual lies. In this mode, the A+W Realtime
        Optimizer receives the batch information from the connected cutting table. The table
        manufacturer must support this functionality. The availability must be clarified in advance
        with A+W.
Requires the PDC bookings functionality
Editing with manual cutting plan editor
An optimization to be cut can be edited with the manual cutting plan editor before transfer to the
cutting table. During cutting, the residual sheet can be changed with the manual cutting plan editor
before the cutting code is transmitted to the cutting table. The residual sheet from an optimization
can be suspended. The lites of the residual sheet are inserted into a sheet pool and can be optimized
again in a table optimization. After creation of a table optimization, the cutting pattern for the
newly-created optimization are displayed in the A+W Realtime Optimizer – Breakout Display. It is
not possible to change the optimization. During the linking process, the linked pattern can be


A+W Software GmbH                 EN-FUNC-A+W Realtime Optimizer.docx                                   5
displayed in the A+W Realtime Optimizer – Breakout Display. Changing the pattern is not possible.
For this functionality, the manual cutting plan editor module is not required.
Entry of rejects
Rejects can be entered after the fact by entering order and item. Alternatively, rejects can be
entered elsewhere via bar code or A+W Production Terminal. These rejects are used in total at the
points described.
The A+W Breakage Manager is required for reject handling.
Entry of rush lites
Rush lites can be entered and are then available to the different optimization modes. Rush lites do
not receive a valid order number and they have no bar code. Due to the lacking bar code, no PDC
functionalities are available. If breakage remakes are generated by PDC bookings, remake
generation for rush lites is not possible.
Entry of manual plans
It is possible to create a manual cutting plan with the manual cutting plan editor and to cut using
the cutting process. The cutting plan receives a batch number from the range of the table
optimization (15000 .. 19999). No information for the individual lites on the plan is stored in the
database. The plan can only be cut and visualized on the breakage table. No additional
functionalities are available.
Prints labels
Labels can be printed during cutting sheet by sheet for the pattern to be cut. If the printing is done
via Crystal Report, a runtime license for Crystal Report is required.
Defect optimization with the A+W Defect Optimizer
With the appropriate hardware prerequisites, defect optimization with the A+W Defect Optimizer
offers 2 operating modes:
    •   Defects on the stock sheet are only visualized. In the A+W Realtime Optimizer – Breakout
        Display, defects are displayed on the stock sheet. The user must decide whether he would
        like to report the lites broken or not. The position of the lites on the stock sheet is not
        changed.
    •   The sheets on the stock sheet are re-placed retaining the storage space sequence,
        whereby if possible, no sheets are placed on the defects on the stock sheet. If this is not
        possible, there is an attempt to place as small a sheet as possible on the defective area. In
        the A+W Realtime Optimizer – Breakout Display, defects are displayed on the stock sheet.
        In addition, lites on relevant defect locations are marked with a yellow cross in the
        display. Now the user can decide whether he would like to report the lites broken or not.
The complete functional specifications of the A+W Defect Optimizer are listed in a separate
document.
Storage reporting
In case of an upstream A+W ERP System, the cut stock dimensions can be reported to the ERP stock
and booked there via an interface. The interface informs both about the stock dimensions used as
well as about the order items found there.




A+W Software GmbH                EN-FUNC-A+W Realtime Optimizer.docx                                6
Re-optimization
Using the re-optimization, rejects can be optimized to the last pattern. There are 2 optimization
modes available:
    •   In "separate" mode, the lites on the residual sheet remain unchanged. The rejects are
        optimized and inserted onto the stock plate after the last cross cut. Additional patterns
        can be created.
    •   In the "mix" mode, the lites on the residual sheet are suspended, the breakage quantity is
        added and re-optimized. Here the sequence on the suspended lites is retained on the
        storage space. Thanks to the optimization, additional patterns can arise.
Quick optimization
Quick optimization allows a re-optimization during the cutting process. Patterns of an optimization
for which no cutting code has been transmitted to the cutting table can be suspended and re-
optimized with any existing rejects or rush lites. The rejects are optimized with priority 0 and are
thus found on the first patterns of the re-optimization. The re-optimization includes a batch number
from the range of the table optimization (15000 .. 19999). The new optimization is inserted into the
pattern sequence in the original position in the cutting process.
Residual stock activation
Various machine manufacturers sell automatic residual stock systems. There, residual plates can be
stored automatically and removed automatically for use. The A+W Realtime Optimizer includes an
interface to these residual stock systems. The activation and functionality of the residual stock
depends on the manufacturer and must be clarified in advance with A+W. In addition, the A+W
Connector B is required. The interface to the residual stock in the A+W Realtime Optimizer includes
the following functionalities:
    •   Storage of the residuals of a stock sheet
    •   Use of a residual stock sheet for manual plan creation
    •   Substitution for the residual plate of a sheet from the residual stock without re-
        optimization
    •   Use of up to 9 residual stock plates in a table optimization
    •   Use of residual stock plates in re-optimization for newly-created patterns
    •   Use of residual stock plates in quick optimization
    •   Use of residual stock plates in follow-up optimization during linking
In principle it is also possible to manage a manual residual stock, details must be agreed upon with
A+W Development before use.
Cutting code creation
For cutting code creation, depending on the cutting table used, an additional A+W cutting code
generator module may be required.




A+W Software GmbH               EN-FUNC-A+W Realtime Optimizer.docx                                 7
Cutting table activation
The cutting table activation is manufacturer-dependent in offline and for most cutting table
manufacturers possible in online mode. In online mode, the cutting table and the A+W Realtime
Optimizer communicate with one another in alternation. Here, it is frequently necessary to
purchase a module from the table manufacturer. In addition, it can be necessary for a table
manufacturer's technician to be on-site for start-up. In which mode a table can be activated must
be clarified in advance with A+W.
Table optimization
The table optimization offers the possibility to combine up to 99 optimizations that were created
with A+W Production and to re-optimize them. It is possible to mix the A+W Production
Optimizations during optimization to improve cutting. Similarly, optimizations can be re-optimized
in a large optimization. The sequence of the original optimizations in the new table optimization
can be selected at will. The "mix" and "separate" modes can be combined in a table optimization.
The storage space sequence on A racks is not changed during the re-optimization. Optionally, the
table optimization can use rejects, rush sheets, and sheets from suspended residual sheets in
addition to the original sheets. The use of filler lites to fill up gaps or to fill up the residual sheet is
possible. The table optimization is always created for a cutting table with its optimization
restrictions. For which table the optimization is created can be selected before setting the
optimization. It is possible to use hand cutting lots for which no A+W Production optimization was
created in table optimizations.
Linking
Linking serves to prevent residual sheets. The residual plate is filled up with lites of a follow-up
optimization. With active re-optimization, first there is a re-optimization and then the residual
sheet is linked. There are 2 optimization modes available:
    •     In "separate" mode, the lites on the residual sheet remain unchanged. The lites of the
          follow-up optimization are placed on the residual plate by the optimization after the last
          cross cut.
    •     In the "mix" mode, the lites on the residual sheet are suspended and the quantity of lites
          from the follow-up optimization with priority 0 are added. If not all suspended lites are
          placed on the residual sheet, the link optimization is discarded.
Visualization with A+W Realtime Optimizer – Breakout Display
During the cutting process, the current breakage pattern of the pattern is displayed with the storage
space information for the lites. During the process, lites that have been broken can be marked in
the display and are fed back into the system as recut lites.
For this functionality, the A+W Realtime Optimizer module is required. In the Entry Solution (A+W
Realtime Optimizer (EL)), the A+W Realtime Optimizer – Breakout Display is already included for
breakage pattern display.




A+W Software GmbH                  EN-FUNC-A+W Realtime Optimizer.docx                                    8
2.4.2. Function list A+W Realtime Optimizer Stand-alone
Import function
The import function offers the opportunity to import A+W Save files into an A+W Production
database.
The database tables are filled from the content of the Opt2 files. If there is a correctly-written
Opt2bar.dat in the Save files, a bar code precise-to-the-sheet can be taken over from the superior
system. The content of the A+W Save files must satisfy certain minimum requirements. Information
about the glass type and thickness must be present. Whether an import is possible without
problems must be clarified in advance, preferably with a sample file, with A+W.


2.4.3. A+W Realtime Optimizer (EL)
Operation with A+W Production
For operation in the A+W Production environment, the functionalities listed below are available
without limitation as in the A+W Realtime Optimizer.
Stand-alone operation without A+W Production
In stand-alone operation, the limitation described under A+W Realtime Optimizer Standalone
apply.
Article            Name                   Functions
230080, 220080,    A+W Realtime           BDE bookings
220980             Optimizer (EL)
                                          Batch identification
                                          Editing with manual cutting plan editor
                                          Storage reporting
                                          Cutting code creation
                                          Cutting table activation
                                          Visualization with A+W Realtime Optimizer –
                                          Breakout Display (without breakage reporting)
230081, 220081,    A+W Realtime           Entry of rejects
220981             Optimizer (EL) -
                                          Entry of rush lites
                   Basic Optimizer
                                          Re-optimization
                                          Table optimization
230082, 220082,    A+W Realtime
220982             Optimizer (EL) -       Linking of optimizations, quick optimization
                   Advanced Optimizer
230083, 220083,    A+W Realtime           Recommended: Basic optimization module
220983             Optimizer (EL) -
                                          Residual stock activation
                   Remaster
                                          Additional module required: A+W Connector B




A+W Software GmbH              EN-FUNC-A+W Realtime Optimizer.docx                              9
2.5. Restrictions
2.5.1. General
The functionalities described are only available without limitations with the use of the 'Panorama'-
supported new cutting dialog.


2.5.2. A+W Realtime Optimizer Stand-alone
    •   A+W Production and the A+W Realtime Optimizer Standalone may not use a joint database
        since otherwise required data is deleted by A+W Production.
    •   No PDC functionality is supported.
    •   Filler orders are only possible in the form of rush lites.


2.5.3. A+W Realtime Optimizer (EL)
In stand-alone operation without A+W Production, the limitations described under A+W Realtime
Optimizer Standalone apply.




A+W Software GmbH                EN-FUNC-A+W Realtime Optimizer.docx                             10
3. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Realtime Optimizer.docx   11

