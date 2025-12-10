---
description: "EN AWProduction PMO 2.00"
---



# EN AWProduction PMO 2.00

Packing Optimization          I




                            english




                A+W Production
                                                                                                             Introduction




                                        Introduction
                                        In this part of the documentation you can find editorial notices.


                                        Revision Overview
                                        Packing Optimization       Description
                                        Version / Date

                                        2.00 / 01-2023             Free edit mode added.

                                        1.02 / 01-2017             Product and company names adjusted

                                        1.01 / 07-2013             Layout adapted to CI 2013.

                                        1.00 / 03-2007             Original version.



                                        Editorial
                                        The editorial contains the following themes:
                                        •   Notes on this document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contact

                                        Notes on this document
                                        This document is intended only for end users of A+W Production.
                                        The documentation and software described are licenses that must be used or
                                        copied only in accordance with the conditions of our license agreement. The
                                        contents of the documentation are only informative and is subject to changes
                                        without prior notice. The text and illustrations were compiled with the utmost
                                        care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be
                                        held liable for errors or inaccuracies, unless they can be attributed to wilful or
                                        grossly negligent action.
                                        The descriptions in this document are based on the full installation of A+W
                                        Production.

                                        Copyrights
                                        © 2023, Product and company names adjusted., any right, also the right of re-
                                        print, the production of copies and of the translation, is reserved. The docu-
                                        mentation must be copied, completely or in part, saved, or transferred only in
                                        accordance with our license agreement. Transmission of the documentation is
                                        not allowed, neither electronically, nor mechanically, nor by recording or in any
2.00 / 01-2023




                                        other way, without Product and company names adjusted. prior approval in
                                        writing.




                 A+W Production Packing Optimization                                                                   I-3
                 Introduction




                                Trademarks
                                Any designation of hardware and software being mentioned in the documen-
                                tation can also be registered trademarks or other commercial rights of third
                                parties being protected by law. Rights of third parties being protected by law
                                are to be observed insofar.

                                Contact
                                A+W Software GmbH
                                Am Pfahlgraben 4-10
                                D-35415 Pohlheim
                                   +49 6404 2051-0
                                   +49 6404 2051-877
                                Zentrale@a-w.com
                                http://www.a-w.com
2.00 / 01-2023




                 I-4                                                  A+W Production Packing Optimization
                                                                                                                                                        Contents




                                        Contents
                                        Introduction .............................................................................................................. I-3
                                          Revision Overview ................................................................................................ I-3
                                          Editorial ................................................................................................................ I-3
                                        Contents .................................................................................................................. I-5

                                        Tutorial                                                                                                                I-1
                                        The Basic Idea ......................................................................................................... I-3
                                        General .................................................................................................................... I-4
                                        Master Data ............................................................................................................. I-7
                                          Optimization Rules (*.RUL file) ............................................................................. I-7
                                          Settings (*.VAL file) .............................................................................................. I-7
                                            Parameters ....................................................................................................... I-8
                                        Views ..................................................................................................................... I-13
                                          Packing Group View ........................................................................................... I-13
                                            Restrictions ..................................................................................................... I-14
                                        View Optimization .................................................................................................. I-17
                                          Views .................................................................................................................. I-18
                                            3D view ........................................................................................................... I-18
                                            Top View ......................................................................................................... I-19
                                            Detailed View .................................................................................................. I-20
                                          Modes ................................................................................................................. I-25
                                            Full Screen Mode ............................................................................................ I-25
                                            Editing Mode ................................................................................................... I-26
                                            Expert Mode .................................................................................................... I-27
                                            Free Edit Mode ............................................................................................... I-28
                                          Clip List ............................................................................................................... I-32

                                        Software Reference                                                                                                   I-57
                                        Menus .................................................................................................................... I-59
                                         Rules .................................................................................................................. I-61
                                         Values ................................................................................................................ I-63
                                         Packing Groups .................................................................................................. I-66
                                         Packing Group View ........................................................................................... I-69
                                           Totals .............................................................................................................. I-70
                                           Filter function .................................................................................................. I-70
                                           Hotkeys ........................................................................................................... I-70
                                           Context Menu for Tagged Entries ................................................................... I-71
                                         PackView ............................................................................................................ I-73
                                         Menu Line ........................................................................................................... I-74
                                         Icons ................................................................................................................... I-78
                                         Views .................................................................................................................. I-81
                                         Change Rack Description ................................................................................... I-81
                                         New Rack Properties .......................................................................................... I-82
                                         Change Box Properties ...................................................................................... I-84
                                         Unit Properties .................................................................................................... I-85
                                         Info Line at the Bottom of the Screen ................................................................. I-86

                                        Section Index                                                                                                        I-89
                                        Index Packing Optimization ................................................................................... I-91
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                                                              I-5
                 Contents
2.00 / 01-2023




                 I-6        A+W Production Packing Optimization
Packing Optimization         I

                        Tutorial




                A+W Production
                 Tutorial                                                                                 The Basic Idea




                                        The Basic Idea
                                        Packing optimization saves tedious resorting as well as the temporary stock.
                                        It adapts the entire production process to Direct packing and to the optimum
                                        use of the racks and boxes.
                                        In a production without packing optimization (PMO), all units produced are put
                                        into a temporary stock. After that, the units have to be packed onto transport
                                        racks which requires time-consuming sorting. Mostly, the units in the tempo-
                                        rary stock are not available in the sequence required for the transport rack. It
                                        may also be the case that the transport rack has to be loaded according to the
                                        customer's instructions, or you have to stick to a certain route or unloading se-
                                        quence.
                                        The task of the packing optimization is to distribute the corresponding order
                                        items onto racks, taking into account all defined conditions, that as little trans-
                                        port space as possible is needed and the customer's requirements regarding
                                        the rack load are fulfilled. The scheduling strategy is defined by the packing
                                        rules. Apart from information on the physical properties such as height, width,
                                        and weight, these include customized parameters for the racks to be used
                                        such as the number of stacks that can be loaded next to or on top of each oth-
                                        er.
                                        Packing optimization splits orders into groups that are going to be packed to-
                                        gether (packing groups), e.g. same delivery date, same route, same shipping
                                        address.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                   I-3
                 General                                                                             Tutorial




                           General
                           This chapter describes the structure of the packing optimization (PMO) and
                           how it basically works. The master data of the packing optimization are com-
                           plex and its proper implementation requires specialist knowledge.
                           Packing optimization includes two definition areas which have to be handled
                           separately:
                           •   The physical conditions (rules), that must be kept at dispatch (weight, ar-
                               rangement of stacks, distances, etc.)
                           •   Order treatment (grouping, sorting, loaded on special racks, etc.) required
                               by the customer.
                           For the customer, the focus mostly lies on the unloading sequence of the
                           transport racks. The more rigid the restrictions for this sequence, the less free-
                           dom is left for the packing optimization when planning the racks. The planning
                           density is apt to become worse as a result.
                           A frequent requirement is to unload units together. All units of the same order
                           shall be unloaded together for example. Or all units of an item shall be unload-
                           ed in a row. It is not even sure that units to be unloaded together are even
                           close to another on the racks. It may well be that the units have been put into
                           different stacks or even different racks. The optimization always makes sure
                           that no other units have to be unloaded before you get at the units that shall
                           be unloaded together. The more freedom is given to the optimization, the bet-
                           ter the planning density on the racks, and the less racks will be needed.
                           A packing group can be split into sets (corresponding to the orders). This
                           means that the items of a set can be unloaded without having to unload other
                           items first. The set may be distributed to different stacks or racks. The unload-
                           ing sequence of the sets can be defined by the packing optimization, or can be
                           set. You can also plan the sets so that the unloading sequence is random.
                           Stacks on the rack have to have a tree structure, e.g. starting with a big stack,
                           followed by maximally two stacks in front of which can, again, be maximally
                           two stacks. From the top, this looks like that (the back of the rack is shown in
                           grey):




                                                      Back of the rack

                           Fig. I-1     Rack load, top view
2.00 / 01-2023




                           Another option is to structure individual stacks by means of matrices. In a ma-
                           trix structure, several units can be set next to another and on top of each other.
                           You need to consider the following properties:

                 I-4                                               A+W Production Packing Optimization
                 Tutorial                                                                                    General




                                        •   All units of a row, except of the top row, must have identical height.
                                        •   All units of a row must have identical thickness.
                                        •   The total thickness of every row must fall below or must equal the total
                                            width of the bottom row.
                                        •   The thickness of every row must fall below or must equal the width of the
                                            bottom row.
                                        •   Every row is centred on top of the bottom row.
                                        This is why units can be set next to another and on top of each other in one
                                        stack. The units can belong to one or several order items. From the front, a
                                        single stack may look like this:




                                                              (1/2)               (2/2)




                                                    (1/1)               (2/1)             (3/1)



                                        Fig. I-2       Matrix load, stack seen from the front


                                        The top stacks are always put in the middle of the stacks below.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                              I-5
                 General                                                                             Tutorial




                           With matrices, you can put a bigger stack in front of two smaller ones (no tree
                           structure).




                                                       Back of the rack

                           Fig. I-3     Matrix load, top view


                           Units of an item are basically kept together if possible. If an item does not fit
                           onto one rack because of the maximum weight or rack depth, it will be split.
2.00 / 01-2023




                 I-6                                               A+W Production Packing Optimization
                 Tutorial                                                                                     Master Data




                                        Master Data
                                        The user will see two types of master data when working with the packing op-
                                        timization:
                                        •   Optimization Rules (*.RUL file): *.RUL files contain general settings, infor-
                                            mation concerning physical racks and corresponding loading rules. These
                                            can be defined by customer or order.
                                        •   Settings (*.VAL file): *.VAL files allow customer specific settings for the op-
                                            timization rules.
                                        *.RUL- and *.VAL files can be selected. Slight modifications such as the
                                        maximum rack load can be performed by the user for a certain packing group.

                                            Other Master Data
                                            Apart from that, there are rack rules, loading rules, and rule allocations. The
                                            rules are defined by A+W Software GmbH together with the user. If you
                                            want to change your packing optimization, please contact A+W Software
                                            GmbH to avoid undesired results!


                                        Optimization Rules (*.RUL file)
                                        *.RUL files contain the rack rules. The rack rules describe the maximum load
                                        a rack can take, and the loading conditions. This applies to racks (A rack, L
                                        rack) as well as to boxes (standard or individual sizes).
                                         Software Reference, “Rules” on page I-61



                                        Settings (*.VAL file)
                                        *.VAL files include the allocations of customized packing parameters (*.VAL
                                        files) and rack rules. Theoretically, every *.RUL file can have its own *.VAL file;
                                        please remember that this will increase the maintenance work.
                                         Software Reference, “Values” on page I-63
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                   I-7
                 Master Data                                                                          Tutorial




                               Parameters
                               Packing optimization uses different parameters for defining the rack loads. Be-
                               low please find descriptions of the most frequently used parameters. The pa-
                               rameters you are using may differ from those due to your individual
                               requirements.

                               Parameter name: Compile sets in stacks.
                               Description: Defines how sets shall be compiled in stacks (e.g. orders).
                               Valid entries:
                               •   0-No, free optimization
                               •   1-Mono,
                               •   2-Multi,
                               •   3-Peripheral
                               Mono:
                               The mono mode means that each set can be unloaded without having to move
                               units of another set. All sets can be unloaded in any sequence. This is why
                               each stack includes just one set.




                                                     Set 2                        Set 1



                                                  Set 1                            Set 2




                               Fig. I-4     Rack 1




                                                Set 2                             Set 3



                                                Set 3                                Set 3




                               Fig. I-5     Rack 2
2.00 / 01-2023




                 I-8                                                  A+W Production Packing Optimization
                 Tutorial                                                                                Master Data




                                        Multi:
                                        The multi mode is similar to the mono mode but each set can be mixed with
                                        other sets on maximally one stack. In a mixed stack, every set forms a block
                                        (separated from the other sets).




                                                                Set 2                     Set 1



                                                         Set 1                            Set 2




                                        Fig. I-6       Rack 1




                                                          Set 2                           Set 3



                                                         Set 3                            Set 3




                                        Fig. I-7       Rack 2


                                        Peripheral:
                                        In peripheral mode, you can unload each set without moving units from other
                                        sets. The unloading sequence is fixed however (either by PMO or by the user).
                                        This is why there may be more than one set per stack.




                                                                                          Set 1
                                                                Set 2

                                                                                          Set 2
                                                         Set 1



                                        Fig. I-8       Rack 1
2.00 / 01-2023




                 A+W Production Packing Optimization                                                              I-9
                 Master Data                                                                        Tutorial




                                               Set 2                            Set 2

                                                                                Set 3
                                              Set 3

                                                                                Set 2


                               Fig. I-9    Rack 2


                               Free:
                               In the free mode, sets and items cannot be unloaded together. The orders are
                               mixed to gain the highest packing density.




                                                                                 Set 1
                                                    Set 2

                                                                                 Set 2
                                              Set 1



                               Fig. I-10   Rack 1




                                                                                Set 2
                                               Set 2

                                                                                Set 3
                                              Set 3

                                                                                Set 2


                               Fig. I-11   Rack 2
2.00 / 01-2023




                 I-10                                               A+W Production Packing Optimization
                 Tutorial                                                                                   Master Data




                                        Parameter name: Sets consist of.
                                        Description: This entry defines how the sets are formed. Sets can be formed
                                        by order, by reference, or by route.
                                        Valid entries:
                                        •   1=Order,
                                        •   2=Reference,
                                        •   3=Route

                                        Parameter name: Keep sets together on the racks?
                                        Description: This entry defines if and if so, how the sets shall be kept together
                                        on the racks. 0 means that the sets will not be kept together on the racks. 1
                                        says that the sets are kept together in a rack and 2, that they can be put onto
                                        maximally two racks.
                                        Valid entries:
                                        •   0=no,
                                        •   1=one rack,
                                        •   2=two racks

                                        Parameter name: Sorted unloading of sets?
                                        Description: Defines if and if so, how the sets shall be unloaded. The default
                                        setting is 0, i.e. the sets will not be sorted.
                                        Valid entries:
                                        •   0=no,
                                        •   1=Sets ascend. ++,
                                        •   2=Set descend. --

                                        Parameter name: Maximum weight for all rack types
                                        Description: This entry defines the maximum weight of all rack types of this
                                        packing group in kg.

                                        Parameter name: Maximum number of stacks on top of each other
                                        (default=1)
                                        Defines how many stacks can be put on top of each other. The default setting
                                        is 1 which means that no stack can be put on top of another. The highest pos-
                                        sible number of stacks that can be put on top of each other is 5.

                                        Parameter name: Maximum offset left/right (default: 100 mm)
                                        Description: This entry marks the maximum rack offset. This entry applies to
                                        both sides. The default setting is 100. This means that the offset on the right
                                        and on the left is 100 mm. The highest possible entry is 1000 (1000 mm).
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                I-11
                 Master Data                                                                              Tutorial




                               Parameter name: Maximum aspect ratio for vertical lites (de-
                               fault=3.0)
                               Description: Defines the minimum relation of long/short side starting from
                               which the lites have to be stacked horizontally. Example: Entry 2 means that
                               the lite 2500/1000 will be stacked horizontally and the lite 1500/1000 vertically.
                               The default setting is 3. The highest possible entry is 5. 1 means that all lites
                               have to be turned onto their longer side.

                               Parameter name: Max. aspect ratio for stacking vertical lites (de-
                               fault=2.0)
                               Description: This is the maximum aspect ratio for stacking a unit, i.e. for setting
                               one unit on top of another. This parameter is only effective if it is smaller than
                               the parameter Maximum aspect ratio for vertical lites.
2.00 / 01-2023




                 I-12                                                   A+W Production Packing Optimization
                 Tutorial                                                                                        Views




                                        Views
                                        The packing optimization has its own view which shows the packing groups
                                        you have created.


                                        Packing Group View
                                        You can open the Packing Group View via menu View > Packing Group View
                                        or by using the icon.




                                        Fig. I-12            Packing view icon


                                            A        B




                                                                                                                   C




                                                                                                                   D




                                                         F      E
                                        A Tab                                     D Hot keys
                                        B Column                                  E Totals
                                        C Table header                            F Filter function
                                        Fig. I-13            Packing Group View


                                        The Packing Group View shows the existing packing groups. Packing groups
                                        can be created in the context menu of the following views:
                                        •       Orders
                                        •       Processings
                                        •       Details
                                        The Tabs allow to roughly organize the Packing group view. The Tabs are split
2.00 / 01-2023




                                        into Table columns. You can also define Filters to restrict the view in certain
                                        cases. Example: The column Rack allows to filter by individual rack groups. A
                                        variety of filter functions allows to adapt the view to your requirements.


                 A+W Production Packing Optimization                                                              I-13
                 Views                                                                                                       Tutorial




                                                  For information on the filters and the total, please refer to section Rough
                                                  scheduling.
                                                  The hot keys can vary from view to view. They depend on the functions avail-
                                                  able in the individual view. Buttons are activated by tagging an entry. For one
                                                  or more tagged entries, the Packing Group View gives quick access to:
                                                  •    Create Batch: Opens the dialog Create Batch
                                                  •    Glass Types: Opens the dialog Glass Type Display
                                                  •    Details: Opens the dialog Detailed Display


                                                  Restrictions
                                                  The context menu of the packing group view allows to edit packing groups, i.e.
                                                  you can move, delete, or change the packing groups. The individual functions
                                                  depend on the status of the packing group however. It is therefore impossible
                                                  to delete a packing group after detailed scheduling because detailed schedul-
                                                  ing is based on the results of the packing group.
                                                  The following table shows which packing groups can be edited, and in which
                                                  status.


                 Status     Explanation                 Change     Move PG      Delete      Optimize     View           Reset
                                                        PG                      PG                       optimization   optimization

                 50         Released for                Yes / No1) Yes / No1)   Yes / No1) Yes           No             Yes
                            optimization

                 75         is currently optimized      No         No           No          No           No             No
                            in background

                 80         Optimization failed         Yes        Yes          Yes         Yes          No             Yes

                 100        optimized                   Yes / No   Yes / No     Yes / No    Yes          Yes            Yes

                 >100       Detailed scheduled          No         No           No          No           Yes            No

                 Tab. I-1        Packing group status
                                                  1)
                                                    Fields reading yes/no have either been released for optimization or have
                                                  been optimized already. The user will be asked if he wants to change anything.


                                                   How to create packing groups
                                                  Packing groups are created in just the same way in all views (orders, process-
                                                  ing, etc.). This is why we are going to describe the procedure just once, in con-
                                                  nection with the view Orders.
                                                  1 Open the view Orders either by means of menu View > Orders or with the
                                                    corresponding icon.
                                                  2 Choose the order(s) that shall form a packing group.
                                                  3 Open the context menu and select Form packing group
2.00 / 01-2023




                                                  4 The dialog Packing groups appears.




                 I-14                                                                      A+W Production Packing Optimization
                 Tutorial                                                                                          Views




                                        5 Enter the name of the main packing group in field Main packing group.
                                            Software Reference, “Packing Main Group” on page I-66
                                        6 Enter the name of the packing group in field Packing group.
                                            Software Reference, “Packing Group” on page I-67
                                        7 Select the required rule from combo box Packing rule.
                                            Software Reference, “Packing Mean Rule” on page I-67
                                        8 Enter another name for the packing group in field Description.
                                            Software Reference, “Description” on page I-67
                                        9 Enable or disable the checkbox Exclude items from optimization.
                                            Software Reference, “Exclude items from optimization” on page I-67
                                        10 Enable or disable the checkbox Combine several production lines.
                                            Software Reference, “Pack multiple production lines together” on page I-67
                                        11 Change the VAL settings if required.
                                        12 Press [Ok].
                                        13 The selected order(s) will be removed from the Orders view. You will find it/
                                           them in the just created main packing group in view Rack.


                                         How to optimize a packing group
                                        1 Open the Rack via either via menu View > Rack or by the corresponding
                                          icon.
                                        2 Choose the packing group(s) you want to optimize.
                                        3 Open the context menu and select Optimize PG.
                                        4 Optimization starts.


                                         How to change the parameters of an existing packing group
                                        1 Open the Rack via either via menu View > Rack or by the corresponding
                                          icon.
                                        2 Choose the packing group(s) you want to change.
                                        3 Open the context menu and select PG management > Change parameters.
                                        4 This opens the dialog Packing groups. Your changes will affect the fields
                                           •   Packing rules
                                           •   Description
                                           •   Exclude items from optimization
                                           •   Pack several production lines together
                                           •   VAL.
                                        5 Select the required rule from combo box Packing rule.
2.00 / 01-2023




                                            Software Reference, “Packing Mean Rule” on page I-67




                 A+W Production Packing Optimization                                                                 I-15
                 Views                                                                     Tutorial




                         More information on the packing group view
                          Software Reference, “Packing Group View” on page I-69
2.00 / 01-2023




                 I-16                                          A+W Production Packing Optimization
                 Tutorial                                                                                      View Optimization




                                             View Optimization
                                             After running the packing optimization, you can display the results in a three-
                                             dimensional view. Results in this case means: Where will the units be posi-
                                             tioned on the transport rack? You can also repack the optimized racks by
                                             means of just a few mouse clicks. The software for visualizing the packing re-
                                             sult is called PackView.


                             A   B   C                                 D




                 I




                                                                                                                      E




                                         H
                                                                  G             F
                 A Menu line                 D Top view                             G Total weight in kg (front and back)
                 B Icons                     E Detailed unit view                   H Extension of total load on the current rack
                 C 3D view                   F Distribution of weight on the left     side: Width , Height , Depth 
                                               and right rack side                  I Expert mode, Setting wheels for close-up
                                                                                      view
                 Fig. I-14       PackView


                                             PackView automatically starts after an optimization has been run successfully.
2.00 / 01-2023




                                             More information on visualization
                                              Software Reference, “PackView” on page I-73



                 A+W Production Packing Optimization                                                                          I-17
                 View Optimization                                                                            Tutorial




                                     Views
                                     PackView offers the following views:
                                     •   3D view
                                     •   Top view
                                     •   Detailed view
                                     The view you are currently in will be edged in yellow. Individual units can be
                                     selected by means of the mouse. When you select a unit from the 3D view, it
                                     will be shown in red in both the top and detailed view. No matter what view you
                                     are in, the selected unit will be marked red in all other views as well.


                                     3D view


                                     A




                                                                                          B




                                                                                          C


                                     A Current side of rack                 C Bottom left corner (reference point for
                                     B Selected unit                          the back)

                                     Fig. I-15    3D view


                                     The 3D view gives a three-dimensional view of both sides of the rack. The red
                                     number in the top left corner shows which rack side is being displayed.
2.00 / 01-2023




                 I-18                                                       A+W Production Packing Optimization
                 Tutorial                                                                             View Optimization




                                        You can change the rack side in the following ways:
                                        •   In menu View open Switch side view.
                                        •   Use the <space bar> on the keyboard.
                                        •   Use the icon.




                                            Fig. I-16      Change rack side


                                        You can display a rack from several angles. PackView calls these angles Cam-
                                        era positions. The above illustration (Tutorial, “3D view” on page I-18) shows
                                        the so-called Camera start position. The 3D view will be opened from this cam-
                                        era position as a standard. You can use one of the following options to go to
                                        the next camera position:
                                        •   In menu View open Next camera position or Previous camera position.
                                        •   Enable the number block by pressing the key <Num> on the keyboard.
                                            Press the key <+> or <->.
                                        •   Use the icon.

                                                                   Next camera position.

                                                                   Previous camera position.

                                            Fig. I-17      Change camera position


                                        The 3D view allows to move units by means of the Copy function. This means:
                                        tag a unit, copy it, move it to the required position and insert it. Units can be
                                        turned on the spot after copying.


                                        Top View

                                        A


                                                                                                       B




                                        A Bottom left corner (reference point)      B Selected unit
2.00 / 01-2023




                                        Fig. I-18       Top view




                 A+W Production Packing Optimization                                                                I-19
                 View Optimization                                                                                 Tutorial




                                     The top view shows the rack from above. The red unit is the currently selected
                                     one.
                                     In the top view and in the 3D view, units can be moved or turned by means of
                                     the Copy function.


                                     Detailed View
                                     The detailed offers a table showing how the order items are positioned on the
                                     racks. The first unit on the list is the one that stands at the back of the rack.
                                     The last unit on the list comes first on the rack, i.e. the table is sorted in loading
                                     sequence.


                                                                                                                        A
                                                                                                                        B




                                     A Table header                             B Column
                                     Fig. I-19     Detailed view
2.00 / 01-2023




                 I-20                                                          A+W Production Packing Optimization
                 Tutorial                                                                                  View Optimization




                                        The table header offers the columns:
                                        •   Rack#, consists of
                                            – Side
                                            – Stack
                                        •   Rack description, consists of
                                            – Quantity
                                            – Row
                                        •   Rack ID, consists of
                                            – Surface [sqm]
                                            – Vert. stacks
                                        •   Type, consists of
                                            – Weight [kg]
                                            – Quantity
                                        •   Group, consists of
                                            – Order No.
                                        •   Size [mm], consists of
                                            – Item No.
                                            – Size [mm]
                                            – Weight [kg]
                                            – Production line

                                        Description of table header and columns

                                        Rack# Shows the actual rack for packing optimization and all racks for the
                                        packing optimization. Example: 1/3 means that the packing group consists of
                                        three racks of this rack type the first of which is displayed. The actual rack#/
                                        total number appears at the top of the window header.

                                        Side Shows the currently displayed rack side. Valid options:
                                        • 1: The following units are placed on the 1. rack side
                                        • 2: The following units are placed on the 2. rack side

                                        Stack This field is directly related to the field Side and shows the stack that
                                        contains the unit displayed in this line. If the field reads 1, the unit is in the first
                                        stack on this side of the rack. If the field reads 2, the unit is in the second stack
                                        on this side of the rack. The number of stacks depends on the rack size and
                                        unit size. A rack can hold more stacks if the units are very small and less
                                        stacks if the units are large.
                                        Example:
                                        This side of the rack holds two stacks.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                       I-21
                 View Optimization                                                                             Tutorial




                                     The tagged unit is the first row (at the back of the rack) of the first (seen from
                                     the reference point!) stack:




                                     Fig. I-20    1st stack, 1st row


                                     The next picture shows the first row (at the back of the rack) of the second
                                     (seen from the reference point!) stack:




                                     Fig. I-21    2nd stack, 1st row
2.00 / 01-2023




                                     In front of the second stack there are other rows. The next picture shows the
                                     second row of the first stack:


                 I-22                                                        A+W Production Packing Optimization
                 Tutorial                                                                         View Optimization




                                        Fig. I-22      1st stack, 2nd row


                                        The next picture shows a unit in the second row of the second stack:




                                        Fig. I-23      2nd stack, 2nd row


                                        Rack description The contents of this field is loaded from PMO master data
                                        and shows the rack name defined there.
2.00 / 01-2023




                                         Software Reference, “Packing Main Group” on page I-66




                 A+W Production Packing Optimization                                                           I-23
                 View Optimization                                                                         Tutorial




                                     Quantity This field shows how many individual units this side of the rack
                                     holds at present.
                                      Tutorial, “Side” on page I-21

                                     Row This field shows the number of stacks in front of each other. At the back
                                     of the rack for example, there is a big stack followed by two smaller stacks.

                                     Rack ID Shows the ID of the rack that is currently displayed. This number
                                     matches the number left of the slash in field Rack#.
                                      Tutorial, “Rack#” on page I-21

                                     Surface [sqm] Shows the total square metres of the units this side of the rack
                                     holds.
                                      Tutorial, “Side” on page I-21

                                     Vert. stacks Shows the number of stacks set on top each other.

                                     Type Shows the rack type. Valid options:
                                     • A = A Rack
                                     • L = L Rack
                                     • Box = Case

                                     Weight [kg] This field shows the total glass weight (in kilogramme) on this
                                     side of the rack.
                                      Tutorial, “Side” on page I-21

                                     Quantity This field shows the number of units this item consists, and the ac-
                                     tual unit. Example: 1/2 means that the item consists of two units one of which
                                     is shown in this line.

                                     P group Shows the main packing group and the packing group. The contents
                                     of this field are loaded from dialog Packing groups, fields Main packing group
                                     and Packing group.
                                      Software Reference, “Packing Main Group” on page I-66
                                      Software Reference, “Packing Group” on page I-67

                                     Order No. Shows the customer's order number imported from the order pro-
                                     cessing system.

                                     Item No. This field refers to field Order no. and shows the corresponding item
                                     number for this order number.

                                     Size [mm] Shows the size of the current item in mm.

                                     Weight [kg] Shows the weight of the current item in kg.

                                     Production line Defines the production line on which the corresponding item
                                     shall be produced. The data are loaded from machinery allocation.
2.00 / 01-2023




                                      Software Reference, “Work Process” on page G-111




                 I-24                                                      A+W Production Packing Optimization
                 Tutorial                                                                              View Optimization




                                        For special requirements, you can configure the number and contents of the
                                        columns displayed. For more information, please contact A+W Software
                                        GmbH.


                                        Modes
                                        PackView offers three different modes. The available tools depend on the ac-
                                        tual mode.
                                        •   Full Screen Mode
                                        •   Editing Mode
                                        •   Expert Mode


                                        Full Screen Mode
                                        PackView starts out in full screen mode. You can tag a lite by clicking on a unit
                                        in the 3D view or in the top view, or by selecting an item from the detailed view.
                                        The selected unit is shown in red in both the 3D view and in the top view. In
                                        the detailed view, the selected unit is edged in red.




                                        Fig. I-24      Full screen mode


                                        The full screen mode gives access to the various camera positions. Press the
                                        corresponding button to move the rack by 45° in the defined in the 3D view.
                                        This allows you to look at the rack from various angles, e.g. to be able to as-
                                        sess the free space left on the rack.

                                            Mode
                                            The mode you are currently in (full screen/edit) appears at the end of the
                                            header in square brackets. Example: [Full screen].
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                 I-25
                 View Optimization                                                                             Tutorial




                                     Editing Mode
                                     PackView start in full screen mode. The editing mode is accessible via menu
                                     Edit > Edit,
                                     or by hard key <F3>
                                     or by means of the icon



                                     Fig. I-25      Icon 'editing on/off'


                                     You can tag a lite by clicking on a unit in the 3D view or in the top view, or by
                                     selecting an item from the detailed view. The selected unit is shown in green
                                     in both the 3D view and the top view. In the detailed view, it is edged in green.
                                     PackView automatically selects partial stacks that can actually be moved. If
                                     you select a unit in the middle of a stack, PackView automatically tags all units
                                     in front of it.




                                     Fig. I-26      Editing mode


                                     The editing mode gives access to the various camera positions. Press the cor-
                                     responding button to move the rack 45° in the defined direction in the 3D view.
                                     This allows you to look at the rack from different angles, e.g. to assess the free
                                     space left on the rack. Apart from that, you can move individual units or entire
                                     stacks on the rack, or align them with the left or right edge.

                                        Mode
                                        The mode you are currently in is shown at the end of the header in square
                                        brackets. Example: [Edit].
2.00 / 01-2023




                 I-26                                                        A+W Production Packing Optimization
                 Tutorial                                                                           View Optimization




                                        Expert Mode
                                        PackView starts in normal mode. The expert mode is accessible via menu
                                        View > Expert mode on/off,
                                        or by the icon



                                        Fig. I-27      Icon Expert mode on/off


                                        You can switch on the expert mode in both the full screen and editing mode.




                                        Fig. I-28      Expert mode


                                        Apart from the functions described in connection with the full screen and edit-
                                        ing mode, the expert mode allows to zoom the rack or rotate it around the X or
                                        Y axis.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                              I-27
                 View Optimization                                                                                Tutorial




                                                          To zoom, place the cursor on the
                                                          middle of the wheel, press the left
                                                          mouse key, and keep pressing it. By
                                                          moving the wheel to the top, you can
                                                          reduce the rack. By moving the wheel
                                                          to the bottom, you can enlarge the
                                                          rack.
                                                          To rotate around the Y axis, place the
                                                          cursor on the middle of the wheel,
                                                          press the left mouse key, and keep
                                                          pressing it. By moving the wheel to the
                                                          right, you can turn the rack to the right.
                                                          By moving the wheel to the left, you
                                                          can turn the rack to the left.
                                                          To rotate around the X axis, place the
                                                          cursor on the middle of the wheel,
                                                          press the left mouse key, and keep
                                                          pressing it. By moving the wheel to the
                                                          top, you can tilt the rack upwards. By
                                                          moving the wheel to the bottom, you
                                                          can tilt the rack downwards.
                                     Fig. I-29


                                     The expert mode also allows to rotate the rack freely. Free rotation is enabled
                                     in menu
                                     View > Free rotation
                                     or by the icon



                                     Fig. I-30     Icon free rotation


                                     The cursor changes in the following way:




                                     Fig. I-31     Cursor for free rotation


                                     Position the cursor on the rack, press the left mouse key, and keep pressing
                                     it. You can now turn the rack to the left or to the right, or tilt it upwards or down-
                                     wards. Press the mouse wheel to move the rack to the left or to the right.


                                     Free Edit Mode
                                     This mode allows you to reorganize lites on a rack without considering physi-
2.00 / 01-2023




                                     cal limitations. You can, for example, select any lite and perform advanced
                                     movements and actions with the selected lites. For example, it is possible to
                                     move lites forward or backward within a stack. This means, you get more pos-



                 I-28                                                          A+W Production Packing Optimization
                 Tutorial                                                                             View Optimization




                                        sibilities in the Free Edit mode, but on the other hand you are responsible for
                                        a wrong or impossible placement.
                                        With the key combination <Ctrl> + <left mouse button>, any units can also be
                                        selected in the middle of the stack. Without the <Ctrl> key pressed, the princi-
                                        ple of selection remains unchanged.




                                        Fig. I-32      <Ctrl> + left mouse button


                                        The Enter key can be used to create a so-called Locator (a group of units that
                                        can be manipulated together) instead of pressing <Ctrl> + <C>.
                                        Pressing the Enter key again exits the Locator status and the placement of the
                                        units are confirmed instead of pressing <Ctrl> + <V>for the same operation.
                                        If the lites taken from the stack(s) are not grouped, a virtual Locator is created
                                        (shown indented from the rack) and the rest of the lites are consolidated on the
                                        rack. This means, all gaps are removed and the remaining lites are automati-
                                        cally moved to each other. You must then manually select the new location for
                                        the Locator to continue editing.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                 I-29
                 View Optimization                                                                             Tutorial




                                     Fig. I-33    New position of the lite


                                     With the Up/Down arrow keys, the lites can be moved forward or backward on
                                     the rack. Moving backwards/forwards through several lites is only possible if
                                     the lites form a block lying next to each other (they have the same Z and Y co-
                                     ordinates and the same thickness).




                                     The Alt key can be used to force the alignment of the lites to take place in re-
                                     lation to the rack. If the Alt key is not pressed, the alignment works as before
                                     (according to the unit below).
                                     New possibility to rotate the lites. In normal mode, lites can only be rotated if
                                     they form a block. It should be noted, however, that the lites may be incorrectly
                                     placed after rotation.
                                     An automatic validity check is carried out when the edit mode is switched off.
                                     All lites that interfere with other lites or violate other rules are marked with a
                                     color defined as ShowReasonMaterial in PackView.ini. We recommend setting
                                     at least the transparency to a lower value for better clarity.
2.00 / 01-2023




                 I-30                                                        A+W Production Packing Optimization
                 Tutorial                                                   View Optimization




                                        Fig. I-34      Lower transparency
2.00 / 01-2023




                 A+W Production Packing Optimization                                    I-31
                 View Optimization                                                                           Tutorial




                                     Clip List
                                     If you cut out one or more units, these will be automatically transferred to the
                                     clip list.
                                     Example: Tag a unit in the editing mode.




                                     Fig. I-35    Clip List


                                     Now press the button for cutting the unit



                                     Fig. I-36    Button for cutting the unit


                                     PackView shows the rack without the unit as you have cut it out. The detailed
                                     view shows the contents of the clip list; in this case, the cut unit:
2.00 / 01-2023




                 I-32                                                           A+W Production Packing Optimization
                 Tutorial                                                                              View Optimization




                                        Fig. I-37      Clip list


                                        Use the button Clip list to switch between clip list and rack load in the detailed
                                        view.
                                        You can change the sorting of the fields marked by a - in the detailed view. If
                                        you point the cursor on such a field and press the left mouse key, the symbol
                                        will change from - to . This means that this field is sorted in ascending order.
                                        Press the left mouse key again to change the symbol from  to . This means
                                        that the field is sorted in descending order. Press the right mouse key to switch
                                        off the sorting.
                                        You can click on several columns. These will be sorted acc. to the column you
                                        have clicked on first, then by the next, etc. The number shows this hierarchy.


                                         How to select the next/previous rack for display
                                        Packing optimization will usually load several racks. When the optimization
                                        has been successful, PackView automatically starts with the first rack. To dis-
                                        play the other racks, proceed as follows:
                                        1 Select menu View > Show next rack, use the corresponding icon or the
                                          keys <PgUp> or <PgDn>.
                                            Software Reference, “Show Next Rack” on page I-77
                                            Software Reference, “Show Previous Rack” on page I-77
                                           This way, you can display rack after rack.


                                         How to select any rack for display
2.00 / 01-2023




                                        Packing optimization usually loads several racks. After successful optimiza-
                                        tion, PackView automatically starts with the first rack. To display another rack,
                                        proceed as follows:



                 A+W Production Packing Optimization                                                                 I-33
                 View Optimization                                                                         Tutorial




                                     1 Select menu View > Select rack for display …, use the corresponding icon
                                       or the keys <PgUp> or <PgDn>.
                                         Software Reference, “Select Rack for View …” on page I-77
                                     2 The Input dialog appears. Field Enter rack ID allows to enter the rack num-
                                       ber.
                                     3 Press [OK] to display the corresponding rack.


                                      How to move one or a couple of units
                                     1 Enable the processing mode in menu Edit > Edit via hard key <F3> or by
                                       using the icon.
                                         Software Reference, “Toggle edition on/off” on page I-78
                                     2 Tag the unit(s) you want to move. The unit(s) is/are edged in green. Other
                                       units which will have to be moved as well will also be edged in green. You
                                       select add more units or deselect them by mouse-clicks.




                                        Fig. I-38    Tag unit


                                     3 Copy the unit(s) either in menu Edit > Copy, via the icon or by means of the
                                       keyboard (<Ctrl>+<C>).
                                         Software Reference, “Copy” on page I-78
2.00 / 01-2023




                 I-34                                                        A+W Production Packing Optimization
                 Tutorial                                                                           View Optimization




                                           The entire unit is shown in green.




                                           Fig. I-39    Copy unit


                                        4 Move the unit to the required place using the arrow key, or by means of the
                                          icon.
                                            Software Reference, “Move to the left” on page I-79
                                            Software Reference, “Move to the right” on page I-79




                                           Fig. I-40    Move unit


                                        5 When you have positioned the unit, fix it either using menu Edit > Insert or
2.00 / 01-2023




                                          by means of the icon.
                                            Software Reference, “Paste” on page I-78




                 A+W Production Packing Optimization                                                             I-35
                 View Optimization                                                                          Tutorial




                                        Fig. I-41    Insert unit


                                      How to move a whole stack
                                     1 Enable the processing mode in menu Edit > Edit, via hard key <F3> or by
                                       means of the icon
                                         Software Reference, “Toggle edition on/off” on page I-78
                                     2 Tag the unit in the stack is closest to the back of the rack, which you want
                                       to move. The unit and all units in front of it will be edged in green.
                                        You can deselect units by just another click.
2.00 / 01-2023




                 I-36                                                        A+W Production Packing Optimization
                 Tutorial                                                                           View Optimization




                                           Click next to the rack to deselect all tagged units.




                                           Fig. I-42    Tag stack


                                        3 Copy the stack either in menu Edit > Copy or by means of the icon
                                            Software Reference, “Copy” on page I-78
                                           The whole stack is shown in green. All tagged units will be removed from
                                           the detailed view.




                                           Fig. I-43    Copy stack


                                        4 Move the stack to the desired position using the arrow keys or the icon
2.00 / 01-2023




                                            Software Reference, “Move to the left” on page I-79
                                            Software Reference, “Move to the right” on page I-79



                 A+W Production Packing Optimization                                                            I-37
                 View Optimization                                                                          Tutorial




                                        Fig. I-44    Move stack


                                     5 When the stack has reached its new position, you can insert it either using
                                       menu Edit > Insert or by means of the icon.
                                         Software Reference, “Paste” on page I-78




                                        Fig. I-45    Insert stack


                                      How to use the clip list
                                        If you want to position many units, e.g. from different stacks, on the other
                                        side of the rack or even on another rack, the clip list might come in handy.
                                        You can even sort the sequence of units by size, order number, etc. to set
                                        up the new stack according to your requirements.
2.00 / 01-2023




                 I-38                                                       A+W Production Packing Optimization
                 Tutorial                                                                               View Optimization




                                        1 Enable the processing mode in menu Edit > Edit via hard key <F3> or by
                                          using the icon.
                                            Software Reference, “Toggle edition on/off” on page I-78
                                        2 Tag the unit(s) you want to move. The unit(s) will be edged in green.




                                           Fig. I-46    Tag unit
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                I-39
                 View Optimization                                                                              Tutorial




                                     3 Cut out the unit(s)/stacks either using menu Edit > Cut or by means of the
                                       icon.
                                         Software Reference, “Cut” on page I-78




                                        Fig. I-47     Cut unit


                                        The unit(s)/stack will be removed from both the 3D view and the top view.
                                        The detailed view automatically shows the contents of the clip list. Use
                                        menu View > show clip list or click on the corresponding icon to switch from
                                        detailed view to clip list and back. You can cut out more units to fill the clip
                                        list.




                                        Fig. I-48     Show/hide clip list
2.00 / 01-2023




                                     4 Go to the required rack side or rack.




                 I-40                                                         A+W Production Packing Optimization
                 Tutorial                                                                                 View Optimization




                                           Fig. I-49      Other rack side or other rack


                                        5 Use menu View > Show clip list or the corresponding icon to display the
                                          contents of the clip list. If there are several units in the clip list, you can sort
                                          them by various criteria. For more information, please see
                                            Tutorial, “Clip List” on page I-32




                                           Fig. I-50      Show clip list


                                        6 Now click on the icon [Insert]
                                            Software Reference, “Paste” on page I-78
                                           The cursor changes into crosshairs
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                     I-41
                 View Optimization                                                                              Tutorial




                                        Fig. I-51     Insert unit


                                     7 Move the crosshairs to the place where the unit(s)/stack shall be inserted.




                                        Fig. I-52     Position crosshairs


                                     8 Press the left mouse key. The unit(s)/stack will be inserted if possible. If
                                       there are several units/stacks in the temporary stacker, you can put them
                                       onto a stack by pressing <Ctrl>+<C> several times.
                                        If the unit(s)/stack cannot be inserted in the required position, this will look
                                        as follows:
2.00 / 01-2023




                 I-42                                                         A+W Production Packing Optimization
                 Tutorial                                                                                 View Optimization




                                           Fig. I-53     Position crosshairs


                                           This means that the unit(s)/stack appears in the required place for a short
                                           time - in orange - before it vanishes again. Reasons for non-positioning can
                                           be: The unit(s)/stack is too thick and would fall off the rack, or the centre of
                                           gravity is too far right and the unit(s)/stack would fall off the rack, etc.
                                           If it is possible to insert the unit(s)/stack in the required position, this will be
                                           done when you press the left mouse key.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                      I-43
                 View Optimization                                                                             Tutorial




                                        The clip list in the detailed view will be emptied at the same time, i.e. there
                                        are no unit(s)/stack left in the clip list.




                                        Fig. I-54    Insert unit


                                      How to deal with several stacks in the clip list
                                        You can use the clip list if you want to move several stacks to the other side
                                        of the rack or onto another rack altogether. You can sort the sequence of
                                        units by size, order number etc. In the following example, we are going to
                                        move three stacks from different rack sides to the clip list and reposition
                                        them on an empty side of the rack.
                                     1 Enable the processing mode in menu Edit > Edit via hard key <F3> or by
                                       using the icon.
                                         Software Reference, “Toggle edition on/off” on page I-78
2.00 / 01-2023




                 I-44                                                        A+W Production Packing Optimization
                 Tutorial                                                                           View Optimization




                                        2 Tag the last unit (seen from the front) of the first stack you want to move.
                                          All units in front of the tagged one will be edged in green.




                                           Fig. I-55    Tag stack


                                        3 Cut out the stack either using menu Edit > Cut, or by means of the icon.
                                            Software Reference, “Cut” on page I-78




                                           Fig. I-56    Cut stack


                                           The stack will vanish from both the 3D view and the top view. The detailed
2.00 / 01-2023




                                           view automatically shows the contents of the clip list. You can use menu
                                           View > Show clip list or click on the corresponding icon to switch between
                                           detailed view and clip list.


                 A+W Production Packing Optimization                                                              I-45
                 View Optimization                                                                  Tutorial




                                     Go to the next rack to tag the second stack.




                                     Fig. I-57   Tag stack
2.00 / 01-2023




                 I-46                                                   A+W Production Packing Optimization
                 Tutorial                                                                              View Optimization




                                        4 Now move the stack to the clip list.




                                           Fig. I-58    Cut stack


                                           The units of the stack that were the last to be added to the clip list are high-
                                           lighted in blue. Moreover, the packing optimization suggests the new sort-
                                           ing of units.
                                        5 Go to the next rack to tag further stacks.




                                           Fig. I-59    Tag stack
2.00 / 01-2023




                                        6 Now move the stacks to the clip list.




                 A+W Production Packing Optimization                                                                  I-47
                 View Optimization                                                                          Tutorial




                                        Fig. I-60     Cut stack


                                     7 Go to the required rack side or rack on which the stacks from the clip list
                                       shall be positioned.




                                        Fig. I-61     Other rack side or other rack


                                        The icon () in section Height shows that the units are currently sorted by
2.00 / 01-2023




                                        height, in descending order. For more information on sorting, please see
                                         Tutorial, “Clip List” on page I-32




                 I-48                                                          A+W Production Packing Optimization
                 Tutorial                                                                           View Optimization




                                        8 As you want to sort the units by Width, we need to change the sorting first.
                                          Position the cursor on the icon () in section Height and press the right
                                          mouse key. The icon will change to -. Now click the left mouse key on - in
                                          section Width. 1 appears and the sorting changes.




                                           Fig. I-62    Change sorting


                                        9 Insert the two widest units first. The red frame shows the unit you have se-
                                          lected for inserting. Now click on the icon [Insert]
                                            Software Reference, “Paste” on page I-78
                                           The cursor changes into crosshairs. Move the crosshairs to the place
                                           where you want to insert the unit and press the left mouse key. The unit is
                                           inserted and will be removed from the temporary stacker.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                             I-49
                 View Optimization                                                                         Tutorial




                                     At the same time, the next unit from the clip list is marked for positioning
                                     (red frame).




                                     Fig. I-63    Insert unit


                                     You can use the arrow keys to align the unit. Click on the icon [Copy]; the
                                     color of the unit will change to green.




                                     Fig. I-64    Copy unit
2.00 / 01-2023




                                     Now use the icon [Move to left] to move the unit to the left side of the rack.
                                     When the unit has reached its destination, click on the icon [Insert] to posi-
                                     tion it.


                 I-50                                                    A+W Production Packing Optimization
                 Tutorial                                                                             View Optimization




                                           Fig. I-65    Copy unit


                                           Position the next unit in the same way. First press the icon [Copy] to change
                                           the cursor into crosshairs. As the unit has the same size as the one you
                                           have moved before, the packing optimization will put this unit right in front
                                           of the other, i.e. moving it will not be necessary.

                                           Keyboard
                                           <Ctrl>+<V> inserts the next unit from the clip list in front of the one you
                                           have inserted before.
2.00 / 01-2023




                                           Fig. I-66    Insert unit




                 A+W Production Packing Optimization                                                                I-51
                 View Optimization                                                                          Tutorial




                                     10 Now change the sorting from width to height, in descending order.




                                        Fig. I-67   Sort by height, descending
2.00 / 01-2023




                 I-52                                                      A+W Production Packing Optimization
                 Tutorial                                                                              View Optimization




                                        11 Now insert the unit that is now the top one. Click on the button [Insert] to
                                           position the unit in the middle.




                                           Fig. I-68    Insert unit


                                           Use the icons [Copy], [Move to left]/[Align left] and [Insert] to move the unit
                                           to the left edge.




                                           Fig. I-69    Move unit to the left
2.00 / 01-2023




                                        12 When you press the icon [Insert] to insert the next unit, the crosshairs will
                                           appear again. This is because the packing optimization does not know
                                           whether you want to insert the unit in front of 1 or 2.


                 A+W Production Packing Optimization                                                                 I-53
                 View Optimization                                                                               Tutorial




                                                      1   2




                                        Fig. I-70     Move unit to the left


                                     13 Insert the unit in front of 1.




                                                          2




                                        Fig. I-71     Insert unit


                                     14 As you can see, the unit is edged in green in Abb. I-71 on page I-54. It is
                                        therefore still active. Use the icon [Insert] or <Ctrl>+<V> to position the next
                                        unit in front of it. This way, you can position the units until there is no space
                                        left on the rack. The unit that would practically fall off the rack, is briefly
2.00 / 01-2023




                                        shown in orange color on the rack, but will not be positioned on it.




                 I-54                                                         A+W Production Packing Optimization
                 Tutorial                                                                           View Optimization




                                           Fig. I-72    Insert unit


                                        15 If you press the icon [Insert], the cursor changes into crosshairs and you
                                           can start to search a place for the next unit. You can proceed in this way
                                           until all units from the clip list have been put into the rack.


                                        More information on PackView
                                         Tutorial, “View Optimization” on page I-17
                                         Software Reference, “PackView” on page I-73
2.00 / 01-2023




                 A+W Production Packing Optimization                                                              I-55
                 View Optimization                               Tutorial
2.00 / 01-2023




                 I-56                A+W Production Packing Optimization
Packing Optimization             I

                 Software Reference




                A+W Production
                 Software Reference                                                                                    Menus




                                                Menus
                                                The following table shows the dialogs and functions available in menu Master
                                                data.


                 Menu Entry                                     Dialog/Function

                 PMO                   Rules                     Chapter “Rules”on page I-61

                                       Values                    Chapter “Values”on page I-63

                 Tab. I-2       Dialogs in menu Maser data

                                                The following table shows the dialogs and functions offered by the context
                                                menu of the views Orders, Processing, and Details.


                 Menu Entry                                     Dialog/Function

                 Context menu          Create packing group      Chapter “Packing Groups”on page I-66

                 Tab. I-3       List of dialogs accessible through the context menu

                                                The following table shows the dialogs and functions in the context menu of the
                                                view Packing group.


                 Menu Entry                                     Dialog/Function

                 Context menu          Move packing group        Chapter “Move Packing Group”on page I-71

                                       Optimize packing          Chapter “Optimize Packing Group”on page I-71
                                       group

                                       Optimize packing          Chapter “Optimize Packing Group in Back-
                                       group in background        ground”on page I-72

                                       Packing group man-        Chapter “Packing Group Management”on
                                       agement                    page I-72

                                       Display packing group     Software Reference, “PackView” on page I-73

                 Tab. I-4       List of dialogs accessible through the context menu
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                     I-59
                 Menus                                                                                 Software Reference




                                            The table below shows the dialogs and functions in menu View.


                 Menu Entry                                  Dialog/Function

                 Packing group                                Chapter “Packing Group View”on page I-69
                 view

                 Tab. I-5     List of dialogs in menu View

                                            Instructions on how to open individual dialogs are provided again in the follow-
                                            ing dialog descriptions. If there are several ways of opening a dialog, these are
                                            specified as well.
2.00 / 01-2023




                 I-60                                                               A+W Production Packing Optimization
                 Software Reference                                                                                 Menus




                                        Rules
                                        Master Data > PMO > Rules




                                        Fig. I-73      PMO, Rules


                                        This dialog serves to enter new optimization rules or change existing ones.
                                        Technical info: Database table: PMO_MASTER_RULES

                                        Description of Button

                                        Load .RUL files Press this button to load the *.RUL files from the corre-
                                        sponding directory. If *.RUL files are already displayed, the system will remind
                                        you that all current records will be lost. This is the right procedure for enabling
                                        *.RUL files.

                                        Description of Columns

                                        .RUL file This column shows the name of the currently loaded *.RUL files.

                                        Name Shows the name of the *.RUL file.

                                        VAL_FILE This column shows the allocation of *.VAL and *.RUL files, i.e. the
                                        value file belonging to the rule file.

                                        Description of Fields

                                        .RUL file Enter the name of the .RUL file. Button […] opens the dialog Open
                                        where you can select a .RUL if you do not know its name.
                                        Technical info: Compulsory field, alpha-numeric, 9-digit, database field: FILE
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                  I-61
                 Menus                                                               Software Reference




                         Name Enter the name of the *.RUL file.
                         Technical info: Compulsory field, alpha-numeric, 40-digit, database field:
                         NAME

                         Description Enter a description of the *.RUL file.
                         Technical info: Input optional, alpha-numeric, 160-digit, database field: DE-
                         SCRIPTION

                         .VAL file Shows the .VAL file belonging to the .RUL file. Button […] opens the
                         dialog Open where you can select a .VAL file if you do not know its name or if
                         you want to assign another .VAL file to a .RUL file.
                         Technical info: Compulsory field, alpha-numeric, database field: VAL_FILE


                         More information on rules
                          Tutorial, “Optimization Rules (*.RUL file)” on page I-7
2.00 / 01-2023




                 I-62                                              A+W Production Packing Optimization
                 Software Reference                                                                                Menus




                                        Values
                                        Master Data > PMO > Values




                                        Fig. I-74      PMO, Values


                                        Enter the customized values or change existing entries.
                                        Technical info: Database table: PMO_MASTER_VALUES

                                        Description of Buttons

                                        Load .VAL Files Use this button to load the *.VAL files (rule) from the corre-
                                        sponding directory. If *.VAL files are already displayed, the system will remind
                                        you that all currently displayed records will be lost. This is the right procedure
                                        for enabling *.VAL files.

                                        Description of Columns

                                        .VAL File This column shows the name of the currently loaded *.VAL files.

                                        Parameter This column shows the packing parameter of the *.VAL file. This
                                        value stems from the field Packing mean parameter ID.
                                         Software Reference, “Packing Mean Parameter ID” on page I-64

                                        Description Shows the name of the *.VAL file. This value stems from the field
                                        Name.
                                         Software Reference, “Name” on page I-64

                                        Minimum Value Shows the minimum value for this parameter. This value
2.00 / 01-2023




                                        comes from field Minimum value.
                                         Software Reference, “Minimum Value” on page I-65




                 A+W Production Packing Optimization                                                                 I-63
                 Menus                                                             Software Reference




                         Maximum Value Shows the maximum value for this parameter. This value is
                         taken from field Maximum value.
                          Software Reference, “Maximum Value” on page I-65

                         Value Type Shows the value type of this parameter. This value comes from
                         field Value type.
                          Software Reference, “Maximum Value” on page I-65

                         Description of Fields

                         .VAL File This field shows the *.VAL file. Button […] opens the dialog Open
                         where you can select a *.VAL file if you do not know its name or if you want to
                         change a .VAL file.
                         Technical info: Compulsory field, alpha-numeric, database field: FILE

                         Packing Mean Parameter ID Enter e.g. the number of the parameter the val-
                         ue of which you want to enter or change. There are nine packing parameters:
                         Packing parameter 1: Keep sets together in stacks (0-no, 1-mono, 2-multi, 3-
                         peripheral). For details, please refer to Functional Principles.
                          Tutorial, “Parameters” on page I-8
                         Packing parameter 2: Sets consist of (1-order, 2-reference, 3-route).
                         Packing parameter 3: Keep sets together on racks? (0-no, 1-one rack, 2-two
                         racks)
                         Packing parameter 4: Sorted unloading of sets? =0-no, 1-in ascending order
                         ++, 2-in descending order --)
                         Packing parameter 5: Maximum weight for all rack types.
                         Packing parameter 6: Maximum number of stacks on top of another (de-
                         fault=1)
                         Packing parameter 7: Maximum offset left/right (default: 100 mm)
                         Packing parameter 8: Maximum aspect ratio for vertical lites (default=3.0)
                         Packing parameter 9: Max. aspect ratio for vertical lites at stacking (de-
                         fault=2.0)
                         For details, please refer to Functional Principles.

                         Name Enter the name of the *.VAL file.
                         Technical info: Compulsory field, alpha-numeric, 40-digit, database field:
                         NAME

                         Description Enter a description of the *.VAL file.
                         Technical info: Input optional, alpha-numeric, 160-digit, database field: DE-
                         SCRIPTION
2.00 / 01-2023




                 I-64                                           A+W Production Packing Optimization
                 Software Reference                                                                             Menus




                                        Minimum Value Enter the minimum value for the current parameter.
                                        Technical info: Compulsory field, numerical, 50-digit, database field: VAL-
                                        UE_MIN

                                        Maximum Value Enter the maximum value for this parameter.
                                        Technical info: Compulsory field, numerical, 50-digit, database field: VALUE_-
                                        MAX


                                        More information on settings
                                         Tutorial, “Settings (*.VAL file)” on page I-7
2.00 / 01-2023




                 A+W Production Packing Optimization                                                              I-65
                 Menus                                                                Software Reference




                         Packing Groups
                         Orders > Context menu > Packing groups
                         Processing view > Context menu > Form packing groups
                         Detailed view > Context menu > Form packing groups
                         Packing group view > Context menu > Manage PG > Change parameters




                         Fig. I-75    Packing groups


                         This dialog is used to define the settings for forming the packing group. You
                         can also change the settings for existing packing groups. Settings can be
                         changed until the packing group is optimised.
                         Technical info: Database table: PMO_GROUPS

                         Description of Fields and Buttons

                         Packing Main Group You can select an existing main packing group from
                         the combo box (e.g. to add details) or enter a new one. To enter a new packing
                         group, fill in the corresponding text. A main packing group can be e.g. a pro-
                         duction shift or a day's production. If you load the dialog for an existing packing
                         group, you will not be able to change the entries in this field.
                         Technical info: Compulsory field, alpha-numeric, 20-digit, database field:
                         PMO_MASTERGROUP
2.00 / 01-2023




                 I-66                                             A+W Production Packing Optimization
                 Software Reference                                                                                 Menus




                                        Packing Group This field is a packing group within the main packing group.
                                        You can select an existing packing group from the combo box, or enter a new
                                        one. To enter a new packing group, fill in the field. A packing group within the
                                        production shift could be a production step or within a day's production, a cer-
                                        tain route number. If you have loaded the dialog for an existing packing group,
                                        you cannot change the entries in this field.
                                        Technical info: Compulsory field, alpha-numeric, 20-digit, database field:
                                        PMO_GROUP

                                        Packing Mean Rule When you create a new packing group, this field is pre-
                                        set with not selected at first. Open the combo box and assign the required
                                        packing rule to the packing group. If you access an existing packing group, this
                                        field shows the packing rule assigned to the main packing group. Packing
                                        rules are defined in dialog Rules.
                                         Software Reference, “Rules” on page I-61
                                        Technical info: Compulsory field, alpha-numeric, 20-digit, database field:
                                        RUL_FILE

                                        Description Allows to enter a description of the packing group.
                                        Technical info: Input optional, alpha-numeric, 80-digit, database field:
                                        GROUP_INFO

                                        Exclude items from optimization If you enable this checkbox, the items se-
                                        lected in the rack group view will not be optimised for racks. They will go to the
                                        green box. This makes sense e.g. if you know already prior to packing optimi-
                                        zation that the lites of an item are too big to fit on any rack.
                                        Technical info: Input optional, database field: KEEP_SET_TOGETHER

                                        Pack multiple production lines together If you have got several production
                                        lines, you can use this checkbox to compile packing groups without consider-
                                        ing the production lines. PMO usually plans the racks so that the units can be
                                        loaded irrespective of the individual production lines.
                                        Technical info: Input optional, database field: LINE_PACK_TOGETHER

                                        Description of Columns

                                        Value In this column you can change the values from the VAL file once (for
                                        this optimization). Double-click on the field to open and edit it or press [F2]. En-
                                        ter the required value and leave the field using the <Return> key. You can
                                        change the values of all lines of the table.
                                         Software Reference, “Minimum Value” on page I-65

                                        Description This column shows the name of the *.VAL file. This value comes
                                        from the field Name.
                                         Software Reference, “Description” on page I-64

                                        Value Type Shows the value type of this parameter. This value comes from
                                        field Value type.
2.00 / 01-2023




                                         Software Reference, “Maximum Value” on page I-65




                 A+W Production Packing Optimization                                                                   I-67
                 Menus                                                               Software Reference




                         More information on packing groups
                          Tutorial, “Optimization Rules (*.RUL file)” on page I-7
                          Tutorial, “Settings (*.VAL file)” on page I-7
2.00 / 01-2023




                 I-68                                              A+W Production Packing Optimization
                 Software Reference                                                                        Menus




                                        Packing Group View
                                        You can open the Packing group view via menu View > Packing group view or
                                        by using the icon.




                                        Fig. I-76            Packing view icon



                                            A        B




                                                                                                                    C




                                                         E      D
                                        A Tab                                    D Totals
                                        B Column                                 E Filter function
                                        C Table header
                                        Fig. I-77            Rack Group View


                                        The Packing group view shows the existing packing groups. Packing groups
                                        can be created in the context menu of the following views:
                                        •       Orders
                                        •       Processings
                                        •       Details
2.00 / 01-2023




                 A+W Production Packing Optimization                                                         I-69
                 Menus                                                                 Software Reference




                         Contents and sorting of the Packing group view are defined in the context
                         menus. The Packing group view offers three different context menus. The po-
                         sition of the cursor defines the context menu to be opened:
                         •   Move the cursor to Tabs and open the context menu to configure the tabs.
                         •   Move the cursor to the table header to open the context menu to configure
                             the table header.
                         •   Tab an entry in the Packing group view to open the context menu for editing
                             the tagged entry.
                              Software Reference, “Context Menu for Tagged Entries” on page I-71


                         Totals
                         You can use the totals line to get an idea of the number of tagged entries. Like
                         in Tabs and the Table header, the total can be configured individually. For de-
                         tails, please refer to section Rough scheduling.


                         Filter function
                         The filter function serves to filter the current view by individual criteria such as
                         customer name, production date, or product type. For details, please refer to
                         section Rough scheduling.


                         Hotkeys
                         The bottom right section of the Packing group view offers the hotkeys de-
                         scribed below. These give quick access to the corresponding functions.
                         Please note that you have to tag one or more records to execute this function.
                         The buttons are inactive if no record is tagged! You can also access the indi-
                         vidual functions by menu entries.




                         Fig. I-78     Create batch button (F6)


                         If you have tagged a record in the Packing group view and press this button,
                         the Job creation dialog appears.




                         Fig. I-79     Glass types button (F7)


                         Tag a record in the Packing group view and press this button to open the Glass
                         type view for the corresponding record.
2.00 / 01-2023




                         Fig. I-80     Details button (F8)



                 I-70                                             A+W Production Packing Optimization
                 Software Reference                                                                          Menus




                                        Tag a record in the Packing group view and press this button to open the De-
                                        tailed view for the corresponding record.


                                        More information on the pack group view
                                         Software Reference, “Packing Group View” on page I-69
                                         Operation, “Packing Groups” on page I-39


                                        Context Menu for Tagged Entries
                                        View > Packing groups > Tag record > right mouse key > Context menu




                                        Fig. I-81      Context menu for tagged records


                                        The context menu for a tagged record offers the following options:
                                        •   “Move Packing Group” on page I-71
                                        •   “Optimize Packing Group” on page I-71
                                        •   “Optimize Packing Group in Background” on page I-72
                                        •   “Packing Group Management” on page I-72
                                            – “Change Parameter” on page I-72
                                            – “Reset Optimization” on page I-72
                                            – “Delete Packing Group” on page I-72
                                        •   “View Packing Group” on page I-72
                                        •   “Items” on page I-72
                                        •   “Parts” on page I-72
                                        •   “Glass Types” on page I-72
                                        •   “Processings” on page I-72
                                        •   “Details” on page I-72
                                        •   “Search Order” on page I-72
                                        Menu Items

                                        Move Packing Group This menu item serves to open for a tagged record the
                                        view Packing groups. This allows to move one or more selected packing
                                        group(s).
                                         Software Reference, “Packing Groups” on page I-66

                                        Optimize Packing Group Use this menu item to start the optimization for the
2.00 / 01-2023




                                        selected packing group(s).




                 A+W Production Packing Optimization                                                           I-71
                 Menus                                                               Software Reference




                         Optimize Packing Group in Background Use this menu item to start opti-
                         mization in the background. If AlcimServer is installed, the optimization can
                         also be run on the server. If you do not use this menu to start the optimization,
                         it will run as a so-called foreground process on your terminal.

                         Packing Group Management This menu item has three sub-menus:
                         • Change parameter
                           “Change Parameter” on page I-72
                         • Reset optimization
                           “Reset Optimization” on page I-72
                         • Delete packing group
                           “Delete Packing Group” on page I-72.

                         Change Parameter Use this menu to open for a tagged record the view
                         Packing groups. There you can assign another packing rule to the selected
                         packing group and change the name of the packing group. The fields Main
                         packing group and Packing group can no longer be changed.
                          Software Reference, “Packing Mean Rule” on page I-67

                         Reset Optimization You can use this menu item to reset an existing optimi-
                         zation. This function cannot be used for all packing groups however; it de-
                         pends on the status of the corresponding packing group. Deletion will cause
                         the resolution of this PG, i.e. orders will not be deleted.
                          Tutorial, “Restrictions” on page I-14

                         Delete Packing Group This menu item serves to delete the selected packing
                         group(s). This function cannot be used for all packing groups however; it de-
                         pends on the status of the corresponding packing group. Order items will not
                         be deleted; only the packing group allocation.
                          Tutorial, “Restrictions” on page I-14

                         View Packing Group If you open this menu item for a tagged record, you can
                         view the suggested packing of the transport rack in PackView.
                          Tutorial, “View Optimization” on page I-17

                         Items Use this menu item to open - for a tagged record - the view Items.

                         Parts Use this menu to open the Element view for a tagged record.

                         Glass Types Use this menu to open the Glass type view for a tagged record.

                         Processings This menu item opens - for a tagged record - the view Process-
                         ing.

                         Details This menu opens the Detailed view for the tagged record.

                         Search Order Use this menu item to open the dialog Search orders.
2.00 / 01-2023




                         More information on the pack group view
                          Tutorial, “Packing Group View” on page I-13
                          Operation, “Packing Groups” on page I-39



                 I-72                                              A+W Production Packing Optimization
                 Software Reference                                                                                      Menus




                                               PackView
                                               PackView automatically starts after an optimization has been run successfully.



                               A   B   C                                    D




                      I




                                                                                                                         E




                                           H
                                                                       G            F


                 A Menu line                           D Top view                          G Weight distribution in kg (front and
                 B Icons                               E Detailed unit view                  back)
                 C 3D view                             F Weight distribution in %          H Extension of total load on the
                                                                                             current rack side: Width , Height
                                                                                             , Depth 
                                                                                           I Expert mode, Setting wheels for
                                                                                             close-up view
                 Fig. I-82     PackView


                                               PackView shows the results of packing optimization. Various tools (camera po-
                                               sitions, views, etc.) allow to display racks in various ways. You will find more
                                               details below.
2.00 / 01-2023




                                               The program consists of:
                                               •   Menu Line (A)


                 A+W Production Packing Optimization                                                                         I-73
                 Menus                                                                Software Reference




                         •   Icons (B)
                         •   Views (C, D, E)
                         •   Info Line at the Bottom of the Screen (F, G, H)


                         Menu Line

                         Fig. I-83      Menu line


                         Menu File offers the sub-menus:
                         •   Open
                         •   Close
                         •   AutoSave
                         •   Print Setup
                         •   Print Preview
                         •   Print …
                         •   Exit
                         For details please refer to the table below. The functions of most of the menus
                         can also be executed via icons. To avoid double descriptions, the functions will
                         be explained in the section dealing with icons. Whenever this is the case, the
                         table will mention a reference in field Description.

                         Icon        Menu Entry              Description

                                     Open                    This menu is used to open saved or exported
                                                             files. Such files have the extension out and the
                                                             files are saved in directory PackView.

                                     Close                   This menu is used to close the current view.
                                                             Then, the view is empty. PackView remains
                                                             open.

                                     AutoSave                This menu is used to save an intermediate
                                                             result. This way it is always possible to return or
                                                             to load a saved intermediate result. The files are
                                                             saved under the name AutoSave.out. To save
                                                             several intermediate results, it is necessary to
                                                             rename the files.

                                     Print Setup             This menu is used to open the dialog Print
                                                             setup. Here you configure the printout.

                                     Print Preview           This menu is used to display a print preview,
                                                             before you start the pint.

                                     Print …                 This menu is used to start the printout directly.
2.00 / 01-2023




                                     Exit                    This menu is used to close the program
                                                             PackView.

                         Tab. I-6       File menu



                 I-74                                           A+W Production Packing Optimization
                 Software Reference                                                                                Menus




                                        If you have been editing racks, PackView allows to save the result. You have
                                        to confirm (sticking to the suggested file name) this if you want to use the
                                        amended rack load.

                                        Menu Edit offers the sub-menus:
                                        •   Editing F3
                                        •   Edit Rack Description …
                                        •   Insert New Rack …
                                        •   Change Box Properties …
                                        •   Undo
                                        •   Repeat
                                        •   Copy
                                        •   Cut
                                        •   Paste
                                        •   Move to the Green-box
                                        •   Rotate Unit CW
                                        •   Rotate Unit CCW
                                        •   Move Unit to the Right
                                        •   Move Unit to the Left
                                        •   Precise Movement
                                        •   Align
                                        For details please refer to the table below. The functions of most of the menus
                                        can also be executed via icons. To avoid double descriptions, the functions will
                                        be explained in the section dealing with icons. Whenever this is the case, the
                                        table will mention a reference in field Description.

                                        Icon       Menu Entry                Explanation

                                                   Editing F3                Use this menu to enable or disable Editing. You
                                                                             can also use the respective icon.
                                                                              Software Reference, “Icons” on page I-78

                                                   Edit Rack Description …   Use this menu to open the dialog Change Rack
                                                                             Name
                                                                              Software Reference, “Change Rack Descrip-
                                                                               tion” on page I-81

                                                   Insert New Rack …         Use this menu to open the dialog New Rack
                                                                             Properties
                                                                              Software Reference, “New Rack Properties”
                                                                               on page I-82

                                                   Change Box Properties … Use this menu to open the dialog Change box
                                                                           properties …
                                                                              Software Reference, “Change Box Proper-
                                                                               ties” on page I-84
2.00 / 01-2023




                                        Tab. I-7       Menu Edit



                 A+W Production Packing Optimization                                                                  I-75
                 Menus                                                              Software Reference




                         Icon       Menu Entry               Explanation

                                    Undo                      Software Reference, “Icons” on page I-78


                                    Repeat                    Software Reference, “Icons” on page I-78


                                    Copy                      Software Reference, “Icons” on page I-78


                                    Cut                       Software Reference, “Icons” on page I-78


                                    Paste                     Software Reference, “Icons” on page I-78


                                    Move to the Green-box     Software Reference, “Icons” on page I-78


                                    Rotate Unit CW            Software Reference, “Icons” on page I-78


                                    Rotate Unit CCW           Software Reference, “Icons” on page I-78


                                    Move Unit to the Right    Software Reference, “Icons” on page I-78


                                    Move Unit to the Left     Software Reference, “Icons” on page I-78


                                    Precise Movement         Use this menu to move the unit on the rack by
                                                             1,0 mm into the desired direction.

                                    Align                     Software Reference, “Icons” on page I-78




                         Tab. I-7         Menu Edit

                         Menu View offers the sub-menus:
                         •   3D View
                         •   Top View
                         •   Detail View
                         •   View Clip List
                         •   Show Next Rack
                         •   Show Previous Rack
                         •   Select Rack for View …
                         •   Next Camera Position
                         •   Previous Camera Position
                         •   Home Camera Position
2.00 / 01-2023




                         •   Switch Side View
                         •   Enable Expert Mode
                         •   Free Rotation


                 I-76                                           A+W Production Packing Optimization
                 Software Reference                                                                               Menus




                                        •   Show No-move Reason
                                        •   Measuring Tool
                                        •   Unit Properties
                                        For details please refer to the table below. The functions of most of the menus
                                        can also be executed via icons. To avoid double descriptions, the functions will
                                        be explained in the section dealing with icons. Whenever this is the case, the
                                        table will mention a reference in field Description.

                                        Icon       Menu Entry                 Explanation

                                                   3D View                     Software Reference, “Icons” on page I-78


                                                   Top View                    Software Reference, “Icons” on page I-78


                                                   Edge View                   Software Reference, “Icons” on page I-78


                                                   Detail View                 Software Reference, “Icons” on page I-78


                                                   View Clip List              Software Reference, “Icons” on page I-78


                                                   Show Next Rack              Software Reference, “Icons” on page I-78


                                                   Show Previous Rack          Software Reference, “Icons” on page I-78


                                                   Select Rack for View …      Software Reference, “Icons” on page I-78


                                                   Next Camera Position        Software Reference, “Icons” on page I-78


                                                   Previous Camera Position    Software Reference, “Icons” on page I-78


                                                   Home Camera Position        Software Reference, “Icons” on page I-78


                                                   Switch Side View            Software Reference, “Icons” on page I-78


                                                   Enable Expert Mode          Software Reference, “Icons” on page I-78


                                                   Free Rotation               Software Reference, “Icons” on page I-78


                                                   Show No-move Reason  Software Reference, “Icons” on page I-78

                                                   Measuring Tool              Software Reference, “Icons” on page I-78


                                                   Unit Properties             Software Reference, “Icons” on page I-78
2.00 / 01-2023




                                        Tab. I-8       Menu Edit




                 A+W Production Packing Optimization                                                                I-77
                 Menus                                                                    Software Reference




                         Icons


                         Fig. I-84      Icons


                         The table below describes the icons. The functions of most of the icons can
                         also be executed through menu entries.
                          Software Reference, “Menu Line” on page I-74

                         Description of Icons

                                Open source file         Use this icon to open a packing optimization.

                                Select rack for view     Use this icon to open the dialog Input.

                                Switch side view         Use this icon to display the different side views.
                                                         This icon can only be used in the 3D view.
                                Show previous rack       If the packing group includes several racks, you
                                                         can use this icon to display the previous rack.
                                Show next rack           If the packing group includes several racks, you
                                                         can use this icon to display the next rack.
                                Home camera position     The home camera position is the default setting of
                                                         the camera.
                                Previous camera          Use this icon the move the rack by 45° in counter-
                                position                 clockwise direction. After rotating the rack
                                                         completely, the rack side changes.
                                Next camera position     Use this icon the move the rack by 45° in
                                                         clockwise direction. After rotating the rack
                                                         completely, the rack side changes
                                Toggle edition on/off    Use this icon to toggle edition on/off. This is e. g.
                                                         necessary to change the rack description.
                                Undo                     Undo the last action. Can be used repeatedly to
                                                         undo earlier actions.
                                Redo                     Redo the last undone action. Can be used
                                                         repeatedly to redo previous actions.
                                Copy                     Tag the selected unit.

                                Cut                      Remove the selected unit and transfer it to the clip
                                                         list.
                                Paste                    Insert the content of clip list.

                                Move to the green-box  Remove the selected unit and transfer it to the
                                                       green-box.
                                Precise movement on/offThis icon is only active if a unit has been selected.
                                                       Then, you can move the selected unit to the left or
                                                       to the right desired position. Afterwards click on
                                                       the icon Paste to insert the unit at this position.
2.00 / 01-2023




                         Fig. I-85      Icons




                 I-78                                              A+W Production Packing Optimization
                 Software Reference                                                                                        Menus




                                               Move to the left         This icon is only active if you are in the expert
                                                                        mode and a unit has been selected. Then, you
                                                                        can move the selected unit to the left or to the
                                                                        right desired position. Afterwards click on the icon
                                                                        Paste to insert the unit at this position. To move
                                                                        the unit use either the arrow keys or the mouse. If
                                                                        you use the arrow keys the unit is moved to the
                                                                        left side by 10mm per click.
                                               Move to the right        This icon is only active if you are in the expert
                                                                        mode and a unit has been selected. Then, you
                                                                        can move the selected unit to the left or to the
                                                                        right desired position. Afterwards click on the icon
                                                                        Paste to insert the unit at this position. To move
                                                                        the unit use either the arrow keys or the mouse. If
                                                                        you use the arrow keys the unit is moved to the
                                                                        right side by 10mm per click.
                                               Rotate unit in clockwise This icon is only active if you are in the expert
                                               direction                mode and a unit has been selected. Then, it is
                                                                        possible to rotate a selected unit by 90 degrees in
                                                                        clockwise direction. Afterwards click on the icon
                                                                        Paste to insert the unit at this position.
                                               Rotate unit in counter- This icon is only active if you are in the expert
                                               clockwise direction      mode and a unit has been selected. Then, it is
                                                                        possible to rotate a selected unit by 90 degrees in
                                                                        counter-clockwise direction. Afterwards click on
                                                                        the icon Paste to insert the unit at this position.
                                               Align to the left        This icon is only active if you are in the expert
                                                                        mode and a unit has been selected. Then, it is
                                                                        possible to align the selected unit to the left.
                                                                        Afterwards click on the icon Paste to insert the
                                                                        unit at this position.
                                               Align to the center      This icon is only active if you are in the expert
                                                                        mode and a unit has been selected. Then, it is
                                                                        possible to align the selected unit to the center.
                                                                        Afterwards click on the icon Paste to insert the
                                                                        unit at this position
                                               Align to the right       This icon is only active if you are in the expert
                                                                        mode and a unit has been selected. Then, it is
                                                                        possible to align the selected unit to the right.
                                                                        Afterwards click on the icon Paste to insert the
                                                                        unit at this position
                                               Expert mode              Toggles the expert mode on/off.

                                               Free rotation            Toggles the free rotation on/off. This icon is
                                                                        directly connected to the icon for the expert mode.
                                                                        It is only active if the expert mode is on. After
                                                                        pressing the icon the mouse pointer changes and
                                                                        you can rotate the rack freely. If the free rotation is
                                                                        enabled, the icon is highlighted grey and the
                                                                        mouse pointer changes to:
                                                                            . With a push you can put the rack into a
                                                                        continuous rotation. To stop the rotation click on
2.00 / 01-2023




                                                                            .
                                        Fig. I-85      Icons




                 A+W Production Packing Optimization                                                                         I-79
                 Menus                                                             Software Reference




                                Dimension tool    Toggle the dimension tool on/off. After pressing
                                                  the icon the mouse pointer changes and you can
                                                  measure different distances. The results are
                                                  displayed at the bottom of the screen. If the
                                                  dimension tool is enabled, the icon is highlighted
                                                  grey and the mouse pointer changes to:


                                Unit properties   Show or hide the unit properties. Use this icon to
                                                  open the dialog Unit Properties.
                                                   Software Reference, “Unit Properties” on
                                                       page I-85
                                3D view           Toggle the 3D view on/off. Use this icon to enable
                                                  or disable the 3D view. If the 3D view is enabled,
                                                  the icon is highlighted grey.
                                Top view          Toggle the top view on/off. Use this icon to enable
                                                  or disable the top view. If the top view is enabled,
                                                  the icon is highlighted grey.
                                Edge view         Toggle the edge view on/off. Use this icon to
                                                  enable or disable the top view. If the top view is
                                                  enabled, the icon is highlighted grey.
                                Detail view       Toggle the detail view on/off. Use this icon to
                                                  enable or disable the detail view. If the detail view
                                                  is enabled, the icon is highlighted grey. The detail
                                                  view and the clip list can be displayed
                                                  simultaneously.
                                Clip list         Switch the detail view between rack load and clip
                                                  list. After copying units to the clip list, you can
                                                  display the clip list content. The clip list and the
                                                  detail view can be displayed simultaneously.
                         Fig. I-85      Icons
2.00 / 01-2023




                 I-80                                       A+W Production Packing Optimization
                 Software Reference                                                                           Menus




                                        Views
                                        PackView offers the following views:
                                        •   3D view
                                        •   Top view
                                        •   Detail view
                                        For details on views, please refer to Functional Principles.
                                         Tutorial, “Views” on page I-18



                                        Change Rack Description
                                        PackView > Editing on > Menu Edit > Change rack description …




                                        Fig. I-86      Change rack description


                                        This dialog is used to change the rack name. You can use only the fields that
                                        are necessary for changing the rack name. You cannot access any other fields
                                        at that point.
                                        Technical info: Database table: PMO_RACKS

                                        Description of Fields

                                        Group The combo box is preset with the entry -Current- and cannot be
                                        changed. The combo box below shows the rack name. You can click on this
                                        field to override the name. When you leave the dialog by [OK], the name will
                                        be changed in the table.

                                            Customized settings
                                            Depending on the installation (settings for your company) the combo box
                                            Group allows to choose the required rack group and within this group, the
                                            corresponding rack. This is always the case if you have a large number of
                                            racks or boxes to choose from. This behavior will be configured by A+W
                                            Software GmbH.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                             I-81
                 Menus                                                           Software Reference




                         New Rack Properties
                         PackView > Editing on > Menu Edit > Add new rack …




                         Fig. I-87   New rack properties


                         You can use this dialog to add a new rack.
                         Technical info: Database table: PMO_RACKS
                         Description of Fields in Section Sizes

                         Width Enter the width (in mm) of the rack you want to add.
                         Technical info: Compulsory field, numeric, database field: WIDTH

                         Height Enter the height (in mm) of the rack you want to add.
                         Technical info: Compulsory input, numeric, database field: HEIGHT

                         Depth Enter the depth (in mm) of the rack you want to add.
                         Technical info: Compulsory field, numerical, database field: DEPTH
2.00 / 01-2023




                 I-82                                         A+W Production Packing Optimization
                 Software Reference                                                                             Menus




                                        Description of the Field in Section Add Before Rackl#

                                        Combo box The combo box shows the number of racks in the corresponding
                                        packing group. This means that if a packing group consists of five racks, the
                                        combo box shows the numbers 1, 2, 3, 4 and 5. This way you can define in
                                        front of which of these five racks you want to add the new rack.
                                        Description of Fields in Section Type

                                        1 side (type L) Enable this radio button if the rack to be added is an L rack.

                                        2 sides (type A) Enable this radio button if you want to add an A rack.

                                        Box Enable this radio button if the rack you want to add is a tailored-to-size
                                        box.

                                        Description of Fields in Section Description ID

                                        Group The combo box is preset with the entry -Current- and cannot be
                                        changed. The combo box below shows the rack name. You can click on this
                                        field to override the name. When you leave the dialog by [OK], the name will
                                        be changed in the table.

                                           Customized settings
                                           Depending on the installation (settings made for your company) you can
                                           choose the required rack group from combo box Group and within the
                                           group, the corresponding rack. This makes sense if you have a large num-
                                           ber of racks or boxes to choose from. This behavior will be configured by
                                           A+W Software GmbH.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                              I-83
                 Menus                                                             Software Reference




                         Change Box Properties
                         PackView > Editing on > Menu Edit > Change box properties …




                         Fig. I-88    New rack properties


                         Menu Change box properties … is active only if the selected rack is a box. You
                         can change the properties of the box in this case.
                         Technical info: Database table: PMO_RACKS
                         Description of Fields in Section Oversize Dimensions

                         Width Oversize Enter the width (in mm) by which the box shall exceed the
                         load. This leaves space for fillers to secure the box load.

                         Height Oversize Enter the height (in mm) by which the box shall exceed the
                         load. This leaves space for fillers to secure the box load.

                         Depth Oversize Enter the depth (in mm) by which the box shall exceed the
                         load. This leaves space for fillers to secure the box load.

                         Description of Fields in Section Description ID

                         Group The combo box is preset with the entry -Current- and cannot be
                         changed. The combo box below shows the rack name. You can click on this
                         field to override the name. When you leave the dialog by [OK], the name will
                         be changed in the table.

                            Customized settings
                            Depending on the installation (settings made for your company) you can
                            choose the required rack group from combo box Group and within the
                            group, the corresponding rack. This makes sense if you have a large num-
                            ber of racks or boxes to choose from. This behavior will be configured by
                            A+W Software GmbH.
2.00 / 01-2023




                         More information on Change box properties
                          Tutorial, “View Optimization” on page I-17




                 I-84                                             A+W Production Packing Optimization
                 Software Reference                                                                               Menus




                                        Unit Properties
                                        PackView > Menu View > Unit properties




                                        Fig. I-89       Properties of reference units


                                        This dialog offers information on the selected lite. The following values will be
                                        described:
                                        •   Batch/Sequence: Shows the determined lot number after detailed schedul-
                                            ing as well as the sequence of the unit within the lot.
                                        •   Order/Item: Shows the order and item number of the order. Example:
                                            639478/20 means: Order-No.: 639478 and Line Item No.: 20.
                                        •   Width x Height x Depth: Shows the width, the height, and the thickness of
                                            the unit in mm.
                                        •   Weight: Shows the weight of the unit in kg.
                                        •   Position (X, Y, Z): Shows the position of the unit on the rack.
                                            Example:




                                            Fig. I-90      Dialog: SQL analysis


                                            The coordinates of the tagged unit are: 822.00, 51.00, 471.00. This means
                                            that its position on the X axis is 822 mm (from the reference point), 51 mm
                                            from the back of the rack, 471 mm high.
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                I-85
                 Menus                                                                 Software Reference




                         Info Line at the Bottom of the Screen

                                      A                           B            C

                         Fig. I-91     Info line at the bottom of the screen


                         The info line at the bottom of the screen provides information on the sizes and
                         weight of the corresponding rack side. The info line keeps you posted regard-
                         ing sizes and weight of the currently displayed rack side. The display will
                         change if you go to the other side of the rack.
                         The info line is split into three sections:
                         •   Section A
                         •   Section B
                         •   Section C

                         Section A
                         Section A shows the spread of the units per rack side.



                         Fig. I-92     Spread


                         For the image above, this means: The rack is loaded with units up to a length
                         of 1136 mm, a height of 1270 mm, and a depth of 168 mm.

                             Spread
                             The spread is the total spread per rack side, i.e. even gaps and fillers will
                             be included and displayed.

                         This section shows values only if the dimensioning tool is inactive. If the di-
                         mensioning tool is active, this section remains empty until the measuring result
                         appears.
                         There are three ways of enabling the dimensioning tool:


                         •   Via menu: View > Measuring tool.

                         •   By pressing the function key F4.

                         •   By using the icon.
                          Software Reference, “Icons” on page I-78

                         Tab. I-9
2.00 / 01-2023




                 I-86                                                 A+W Production Packing Optimization
                 Software Reference                                                                                 Menus




                                        Section B
                                        Section B shows the weight distribution in kg, per rack and per side.



                                        Fig. I-93      Weight in kg


                                        For the image above, this means: The total rack weight is 383 kg. The values
                                        in brackets show the weight per rack side, i.e. 183 kg for side 1 and 200 kg for
                                        side 2.

                                        Section C
                                        Section C shows the load distribution in % for the right and left side of the rack.



                                        Fig. I-94      Weight in %


                                        For the image above, this means: 51 % of the load are on the left and 49 % on
                                        the right. The percentage also considers the weight of units on the outside as
                                        compared with units on the inside. This may result in distinctive differences in
                                        the load distribution (such as 30 % vs. 70 %).
2.00 / 01-2023




                 A+W Production Packing Optimization                                                                  I-87
                 Menus                    Software Reference
2.00 / 01-2023




                 I-88    A+W Production Packing Optimization
Packing Optimization              I

                       Section Index




                A+W Production
                 Section Index                                                     Index Packing Optimization




                 Index Packing Optimization
                 A                                      – Add rack   I-82
                 Add box
                 – Added depth I-84                     I
                 – Added height I-84                    Icon
                 – Added width I-84                     – Pool view I-13, I-69
                 Add rack                               Icons
                 – Depth I-82                           – PackView I-78
                 – Height I-82                          Item no.
                 – Width I-82, I-83                     – Detailed view I-24
                 Added depth
                 – Add box I-84
                                                        M
                 Added height
                                                        Main packing group         I-66
                 – Add box I-84
                 Added width
                 – Add box I-84                         O
                                                        Order no.
                                                        – Detailed view     I-24
                 C
                 Change rack name
                 – PackView I-81, I-83, I-84            P
                                                        P group
                                                        – Detailed view I-24
                 D
                                                        Packing group I-67
                 Depth
                                                        Packing groups
                 – Add rack I-82
                                                        – Description I-67
                 Detailed view
                                                        – Exclude items from optimisation I-67
                 – Item no. I-24
                                                        – Main packing group I-66
                 – Order no. I-24
                                                        – Pack production lines together I-67
                 – P group I-24
                                                        – Packing group I-67
                 – Production line I-24
                                                        – Packing rule I-67
                 – Quantity I-24
                                                        Packing rule I-67
                 – Rack ID I-24
                                                        PackView
                 – Rack name I-23
                                                        – AutoSave I-74
                 – Rack# I-21
                                                        – Change rack name I-81, I-83, I-84
                 – Row I-24
                                                        – Close file I-74
                 – Side I-21
                                                        – Exit I-74
                 – Size I-24
                                                        – Icons I-78
                 – Stack I-21
                                                        – Menu I-74, I-86
                 – Surface I-24
                                                        – Open file I-74
                 – Type I-24
                                                        – Print I-74
                 – Vert. stack I-24
                                                        – Print preview I-74
                 – Weight I-24
                                                        – Printer setup I-74
                                                        Pool view
                 F                                      – Filter function I-70
                 Filter function                        – Hotkey I-70
                 – Pool view I-70                       – Total I-70
                 Free Edit Mode I-28                    Production line
2.00 / 01-2023




                                                        – Detailed view I-24
                 H
                 Height


                 A+W Production Packmitteloptimierung                                                   I-91
                 Index Packing Optimization                                                Section Index




                 Q                                        – Detailed view I-24
                 Quantity                                 Width
                 – Detailed view   I-24                   – Add rack I-82, I-83

                 R
                 Rack ID
                 – Detailed view I-24
                 Rack name
                 – Detailed view I-23
                 Rack#
                 – Detailed view I-21
                 Row
                 – Detailed view I-24
                 Rules
                 – .Load .RUL file I-61
                 – .Name of .RUL file I-62
                 – .RUL file I-61
                 – Description of the .RUL file   I-62

                 S
                 Side
                 – Detailed view   I-21
                 Size
                 – Detailed view   I-24
                 Stack
                 – Detailed view   I-21
                 Surface
                 – Detailed view   I-24

                 T
                 Total
                 – Pool view I-70
                 Type
                 – Detailed view I-24

                 V
                 Values I-63
                 – .VAL file I-64
                 – Description of the .VAL file I-64
                 – Load .VAL file I-63
                 – Maximum value of .VAL file I-65
                 – Minimum value of .VAL file I-65
                 – Name of .VAL file I-64
                 – Packing parameter number I-64
                 Vert. stack
                 – Detailed view I-24
                 Views
                 – Context menu for tagged entries I-71
2.00 / 01-2023




                 W
                 Weight


                 I-92                                              A+W Production Packmitteloptimierung

