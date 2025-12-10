---
description: "EN AWProduction DynOpt"
---



# EN AWProduction DynOpt

A+W DynOpt   N




             english
                                                                                                   Introduction




                              Introduction
                              This section of the documentation contains editorial notes.


                              Revision overview
                              Version / Date             Description

                              1.00 / 03-2016             Original version



                              Editorial
                              The editorial provides information on the following topics:
                              •   Notes on this document
                              •   Copyrights
                              •   Trademarks
                              •   Contacts

                              Notes on this document
                              This publication is written exclusively for end users of A+W DynOpt.
                              The documentation and software described therein are licensed only and must
                              be used or copied only in accordance with the terms of our license agreement.
                              The contents of the documentation are for information purposes only and are
                              subject to changes without prior notice.
                              The text and illustrations were compiled with the utmost care. In spite of this,
                              we cannot rule out all mistakes. A+W Software GmbH assumes no liability for
                              errors or omissions unless these are based on intentional or grossly negligent
                              behavior.
                              The descriptions in this documentation rely on the full version of A+W Produc-
                              tion.

                              Copyrights
                              © 2016, A+W Software GmbH, all rights reserved, including the right of reprint,
                              the production of copies and of the translation.
                              The documentation may be copied, completely or in part, saved in an archiving
                              system, or transferred in any other form only in accordance with our license
                              agreement. Transmission of the documentation is not allowed, neither elec-
                              tronically, nor mechanically, nor by recording or in any other way, without prior
                              written approval from A+W Software GmbH.

                              Trademarks
1.00 / 01-2016




                              All hardware and software names mentioned in this documentation might also
                              be registered trademarks or other property rights of third parties. Copyrights of
                              third parties must be complied with.


                 A+W DynOpt                                                                               N-3
                 Introduction




                                Contacts
                                A+W Software GmbH

                                Am Pfahlgraben 4 - 10

                                D-35415 Pohlheim

                                Germany

                                   +49 6404 2051 0

                                   +49 6404 2051 877

                                Zentrale@a-w.com

                                http://www.a-w.com
1.00 / 01-2016




                 N-4                                    A+W DynOpt
                                                                                                                                              Contents




                              Contents
                              Introduction ............................................................................................................. N-3
                                Revision overview ............................................................................................... N-3
                                Editorial ............................................................................................................... N-3

                              Tutorial                                                                                                               J-7
                              Overview ................................................................................................................. J-9
                              Dynamic Optimization ........................................................................................... J-10
                               Description of services ...................................................................................... J-11
                               Problem statement ............................................................................................ J-13
                               Optimization with A+W DynOpt ......................................................................... J-17
                                 Dynamic time line ........................................................................................... J-19
                                 Buffer system ................................................................................................. J-21
                                 Buffer reservation ........................................................................................... J-22
                               Working with Panorama .................................................................................... J-23
                              Working with A+W DynOpt ................................................................................... J-25
                               A+W DynOpt Editor ........................................................................................... J-27
                                 Prioritizing rush lites in two steps ................................................................... J-29
                                 Using A+W DynOpt Editor ............................................................................. J-33

                              Section index                                                                                                      N-35
                              Index ..................................................................................................................... N-37
1.00 / 01-2016




                 A+W DynOpt                                                                                                                           N-5
                 Contents
1.00 / 01-2016




                 N-6        A+W DynOpt
A+W DynOpt        J

             Tutorial
                 Tutorial                                                                                 Overview




                              Overview
                              This document provides information about the concept of dynamic optimiza-
                              tion. It also provides information about manual interventions with which you
                              can start and edit the optimization.
                              This tutorial offers the following information:
                              •    “Dynamic Optimization” on page J-10
                              •    “Working with A+W DynOpt” on page J-25

                              Required knowledge
                              This tutorial is directed at participants who are responsible for work prepara-
                              tion in A+W Production and who thus organize the optimal flow of production.
                              The participant must be familiar with the concept of master data and schedul-
                              ing in A+W Production.

                              Display conventions
                              Certain parts of sentences are specially marked. These have the following
                              meanings:

                              Italics                    Mark character strings describing the software
                                                         elements, e.g. the Campaign planning dialog.

                              Bold                       Marks character strings to be entered via the keyboard,
                                                         e.g.: Enter the value 0.

                              >                          The so-called breadcrumb trail marks the way to open a
                                                         dialog, e.g. Master data > Capacity Planning >
                                                         Campaign planning > Add campaign.

                              []                         Square brackets designate buttons on the dialog, e.g.:
                                                         Save the data with [OK].

                              <>                         Pointy brackets designate keys or key combinations on
                                                         the keyboard, e.g.: Use <F1> to open the online help.


                              Reader’s note
                              The contents of a training module are based on the knowledge conveyed in
                              the previous module. We therefore recommend that you do not skip any mod-
                              ules.
1.00 / 01-2016




                 A+W DynOpt                                                                                   J-9
                 Dynamic Optimization                                                                       Tutorial




                                        Dynamic Optimization
                                        The tutorial about the A+W DynOpt module focuses on the optimization of the
                                        production flow from planning of the lots to the finished product.
                                        This chapter provides information on the following subjects:
                                        •   “Description of services” on page J-11
                                        •   “Problem statement” on page J-13
                                        •   “Optimization with A+W DynOpt” on page J-17
                                        •   “Working with Panorama” on page J-23
1.00 / 01-2016




                 J-10                                                                                  A+W DynOpt
                 Tutorial                                                                          Dynamic Optimization




                                         Description of services
                                         There is significant savings potential during flat glass processing if you opti-
                                         mize the usage of stock plates during cutting.
                                         •   With the innovative optimization algorithm and intelligent and state-of-the-
                                             art stock connection, it is possible to place and cut different types of glass
                                             in alternation.
                                         •   With the use of an intermediate buffer, it is possible to optimize, cut, and
                                             sort the contents of the intermediate buffer dynamically.
                                         •   The activation of cutting tables with optimized cutting patterns directly from
                                             the optimization also speeds up the work process.
                                         A+W DynOpt is a complex system network of various hardware and software
                                         components:
                                         •   Cutting table(s)
                                         •   Stock and residual plate stock
                                         •   Intermediate buffer and sorting system
                                         •   A+W Production for work preparation
                                         •   A+W Realtime Optimizer for online optimization on the table
                                         •   Panorama and A+W Production Cockpit for overall control and visualiza-
                                             tion of the system.
1.00 / 01-2016




                 Fig. J-1   Production view in A+W Production Cockpit



                 A+W DynOpt                                                                                           J-11
                 Dynamic Optimization                                                                               Tutorial




                                          Cut planning with A+W DynOpt
                                          If the production batches are enabled in A+W Production, they can be import-
                                          ed into A+W DynOpt. The batches are enabled for import in the A+W DynOpt
                                          Editor and imported by the A+W Realtime Optimizer module. This is how these
                                          batches are incorporated into the dynamic optimization.
                                          These imported and enabled batches are checked constantly. Here the
                                          A+W DynOpt batches are suspended completely and re-optimized dynamical-
                                          ly taking into account different aspects, e.g. to better combine the same glass
                                          types or bring forward lites with a higher priority. The cut patterns calculated
                                          are visualized by A+W DynOpt per cutting table.




                 Fig. J-2   Visualization of the cutting patterns in A+W DynOpt


                                          The lites cut are placed in an intermediate buffer from which they are then re-
                                          moved in the original sequence. This procedure offers the following benefits:
                                          •   A continuous stream of glass flows in the correct production sequence.
                                          •   The best possible yield results are achieved.
                                          If you are working with a residual plate stock, suitable residual plates can be
                                          used instead of relying on stock plates. In addition to a good optimization result
                                          per cutting table, this procedure increases real yield and you can significantly
                                          reduce the residual sheet stock.
1.00 / 01-2016




                                           “Real yield” on page J-18




                 J-12                                                                                        A+W DynOpt
                 Tutorial                                                                 Dynamic Optimization




                              Problem statement
                              Operations in the glass business are currently being confronted with new chal-
                              lenges: Customers are demanding an extremely wide variety, very short deliv-
                              ery times, and quick deliveries. Added to this is a large number of rush orders.
                              At the same time, the delivery quantities per customer and route are sinking.
                              The consequences of this situation are:
                              •   The lot sizes are getting smaller and production must constantly be re-
                                  planned.
                              •   Greater flexibility in production requires the following problem solutions:
                                  – More residual glass must be managed for the optimization of cutting.
                                  – Increased effort for handling of the lites.
                                  – Due to the smaller lot sizes from detailed planning, the room for play in
                                     the optimization for cutting is smaller.
                                     This affects current yield as well as real cutting, for which the yield is re-
                                     garded across the year. This real yield specifies the total quantity/area
                                     of unusable glass.
                                  – Overall, this results in a yield that is up to 10% lower.
                              A+W DynOpt reacts to these requirements with a flexible solution.
1.00 / 01-2016




                 A+W DynOpt                                                                                  J-13
                 Dynamic Optimization                                                                                       Tutorial




                                    Standard optimization                                         A+W DynOpt

                  Cutting          Fixed production sequence                       Cutting         "chaotic"
                                   Type by type per lot                                            dynamic

                            Temporary storage                                                Dynamic buffer
                               Manual re-sorting                                                 Automatic sorting out in
                                                                                                 production sequence

                                  Production                                                        Production
                                  line 1              Rack                                          line 1

                                  Production                                                        Production
                                  line 2              Rack                                          line 2




                                                               Shipping                                          Shipping


                 Fig. J-3        Optimization methods


                                                This graphic presents a simplified comparison of optimization using a standard
                                                method and with A+W DynOpt. Both approaches will be described in more de-
                                                tail below.

                                                Standard optimization
                                                With the previous solution approach, all areas of production were optimized
                                                one after another. Under the current conditions, following optimized produc-
                                                tion, great work is required in shipping, which people try to eliminate with a lot
                                                of manual labor. For because of the wide range of variants and short reaction
                                                times, the lites get jammed up on the racks. This requires close attention from
                                                the workers in shipping and increased work when assigning the lites to the or-
                                                ders.
                                                With this fixed work organization, the work preparation attempts to find appro-
                                                priate lot sizes. Exceptional cases, such as broken lites and rush orders, are
                                                very expensive since these must generally be cut by hand.
                                                However, efficient production must be controlled so that the processing steps
                                                are run through seamlessly for each lite –on through to direct packaging,
                                                where the finished lites are packaged directly without temporary storage and
                                                can be loaded onto the truck. Direct packaging thus has an enormous influ-
                                                ence on the entire production.
1.00 / 01-2016




                 J-14                                                                                                 A+W DynOpt
                 Tutorial                                                                 Dynamic Optimization




                              Lot size conflicts
                              The lot size conflict is well-known in the glass industry. The flexibility and yield
                              must be sounded out via the lot size.




                                          Fl
                                            ex
                                                ib
                                                  ilit
                                                      y
                                           d
                                           el
                                         Yi




                                                           Lot size


                              Fig. J-4          Lot size conflict


                              In this graphic you can see that the yield sinks with greater flexibility. With a
                              very high yield, flexibility approaches zero.
1.00 / 01-2016




                 A+W DynOpt                                                                                  J-15
                 Dynamic Optimization                                                                           Tutorial




                                         At the same time, due to the wide range of variants, there are organizational
                                         problems in cutting:
                                         •   The cut lites must be stored somewhere temporarily. The dynamic buffers
                                             after cutting are thus more important than before.
                                         •   The residual plates must be managed.




                 Fig. J-5   Example: Wide range of variants and quantities processed


                                         The question of lot size conflict and residual plates must be checked constant-
                                         ly – production requires a dynamic solution that reacts constantly to current
                                         events.
1.00 / 01-2016




                 J-16                                                                                    A+W DynOpt
                 Tutorial                                                                       Dynamic Optimization




                              Optimization with A+W DynOpt
                              In order to be able to work completely automatically and dynamically, A+W
                              DynOpt poses requirements of the hardware:
                              •   A buffer and a sorter are used on the cutting table.
                              •   The cutting tables must offer the greatest possible flexibility, e.g. with sev-
                                  eral cutting heads.
                              A+W DynOpt is configured in each case for the hardware used so that the buf-
                              fer is always sufficiently filled. Because cutting is faster than the lines, there is
                              room at this workstation for interruptions, e.g. if the stock must be entered be-
                              cause of a glass delivery.
                              A+W DynOpt is a close-range optimization, that is, the optimization always re-
                              lates to the current situation on the cutting table. Here current events are con-
                              sidered, e.g. broken lites and rush orders. A+W DynOpt Always regards the
                              future supply of batches and lots and automatically optimizes anew.
                               “Dynamic time line” on page J-19

                              Optimization of the batches
                              The optimization and production are organized in batches and lots:
                              •   A batch is the quantity of glass that should be regarded as a group and put
                                  into production. It can include different types of glass.
                              •   A lot is a sub-quantity of a batch. A lot combines the lites that are produced
                                  at the same time under the same production conditions on the same ma-
                                  chine.
                              One lot is generated for each glass type on each table. The sequence of the
                              individual plates within the batch is determined according to the best possible
                              flow. Thus different types of glass are placed on the tables.

                                  Example

                                  A batch contains the glass types float 4 mm and float 5 mm.
                                  They follow one another directly and should be cut on table 1.
                                  From the sequence float 4 - float 5 - float 4, the following lots arise:
                                  Lot 1 - float 4 - part 4
                                  Lot 2 - float 5 - part 1
                                  Lot 1 - float 4 - part 2


                              The detailed and rough planning of A+W Production provides the basis for the
                              optimization with A+W DynOpt. Here the batches planned in detail are sus-
                              pended and recalculated. The detailed planning also considers the storage
                              spaces for the cut lites. This planning is retained in A+W DynOpt.
                              The production batches are only regarded as binding if they serve the produc-
                              tion flow. The final production batches therefore are created only after cutting
1.00 / 01-2016




                              – which solves the lot size conflict to a significant degree.




                 A+W DynOpt                                                                                    J-17
                 Dynamic Optimization                                                                             Tutorial




                                        If A+W DynOpt suspends the batches from the detailed planning, the program
                                        retains the sequence for a batch. This means that the lites are transferred from
                                        the buffer to cutting to the storage spaces planned by detailed planning. The
                                        lites are thus still organized for the subsequent processes after cutting. The li-
                                        tes are removed from the buffer as they are required in subsequent processes.
                                        The empty slots can then be filled anew.
                                        Therefore A+W DynOpt stands between the processes and communicates
                                        with A+W Production, the database, all A+W Production terminals, and all con-
                                        nected components, e.g. cutting tables, buffers, sorting systems, residual
                                        plate buffers. A+W DynOpt handles the control and communication with all
                                        participating software and hardware systems, monitors state data, and reports
                                        relevant results and events, e.g. breakage.
                                        The “Panorama” handles the mapping of the machine model.
                                         “Working with Panorama” on page J-23

                                        Triggers for re-optimization
                                        A+W DynOpt can suspend the not-yet-transmitted plates and re-optimize
                                        them, e.g.:
                                        •   Broken lites are in the breakage pool.
                                        •   The batch sequence is changed due to manual interventions or defined pri-
                                            orities.
                                        •   New batches have been imported.
                                        Normally, this suspension is always done after a plate change. After that, the
                                        newly-available total quantity of lites is optimized.

                                        Real yield
                                        For the optimization, A+W DynOpt orients itself according to the true yield.
                                        This is not just the optimization of the cutting, but an optimization that makes
                                        the entire production more profitable.
                                        This approach refers not just to individual yield optimizations, but keeps an eye
                                        on the entire work day, how many stock plates have gone into production, and
                                        how many residuals were created in the process. In addition, A+W DynOpt
                                        considers and reduces the effort for handling the lites – thus also reducing the
                                        share of broken lites and scratches.
                                        Thanks to this comprehensive view, individual steps by A+W DynOpt may at
                                        first not appear conclusive. However: A+W DynOpt allows advancing to a de-
                                        gree of optimization that you would not achieve with customary planning. Ex-
                                        isting or new residual lites are used better and with higher priority for cutting.
                                        The more yield and fewer residual plates, the higher the material utilization
                                        and the lower the material costs.
1.00 / 01-2016




                 J-18                                                                                      A+W DynOpt
                 Tutorial                                                                                Dynamic Optimization




                                             Dynamic time line
                                             In A+W DynOpt the clusters form an endless time line on which the lites are
                                             arranged and planned. A cluster is generally the quantity of a slot cart. The op-
                                             timization works through this time line down to cutting. The lites that are need-
                                             ed earlier in production are sorted into the time line earlier and thus have a
                                             higher priority. Gaps are filled with the later lites in order to get a good yield.


                      Output                                                                                    Input




                                                                                                                t


                                     A               B       C        D                 E           F

                 A Dynamic buffer for cut lites                        D Optimized clusters (table 2)
                 B Cut clusters (table 1)                              E Clusters can be optimized further (“re-optimized”)
                 C Cutting                                             F Clusters are not yet optimized (filler lites)
                 Fig. J-6      Cluster on the time line for dynamic optimization


                                             This figure shows the optimized batches that batch through cutting and are
                                             placed into the buffer. The batches planned in detail form the start for the pro-
                                             gram. The cut lites that are output from the dynamic buffer form the output.
                                             The red line indicates cutting:
                                             •    The clusters to the left of the red line (light blue) are already cut and are
                                                  placed in the buffer.
                                             •    The clusters to the right of the red line are not yet cut and are broken down
                                                  into three priorities:
                                                  – The dark blue clusters are completely optimized and are cut next with
                                                      high priority.
                                                  – The yellow clusters are not yet completely optimized and can still be
1.00 / 01-2016




                                                      filled up with fill lites (green).
                                                  – The green clusters are not yet optimized. With a new optimization of the
                                                      yellow clusters, they can be used as fill mass.


                 A+W DynOpt                                                                                                   J-19
                 Dynamic Optimization                                                                              Tutorial




                                        If the lites of a cluster are cut, they are placed in the buffer and A+W DynOpt
                                        executes a new optimization. Some lites from the next cluster will already be
                                        cut, because it was taken as fill mass for the previous cluster. The rest of the
                                        current cluster will be cut.
                                        The goal of the optimization is that every production line is always replenished.
                                        Therefore, there must be as much flow out of the buffer as possible. Important
                                        here is that an individual time line is formed for each output. A+W DynOpt tries
                                        to use these as evenly as possible.
                                        The principle goes like this: The next cutting of a plate must create as high a
                                        flow out of the buffer as possible. This is only achieved if lite and counterlite
                                        for IGU or LSG are in the buffer. Here, in the next step cutting plans are creat-
                                        ed and in the second step these cutting plans are optimized so that the lites
                                        that belong together for IGU/LSG production are available at the same time.
                                         “Buffer system” on page J-21


                                          A



                                          B

                                          C




                                          D



                                        A Newly-optimized batches                C Cut lites in the buffer
                                        B Special glass, waiting for cutting     D Cutting plans
                                        Fig. J-7      Optimized batches and buffer reservation


                                        In this figure you can see that spaces are held free for special glass if it is re-
                                        quired, e.g. for IGU production. The optimization must consider that these lites
                                        are not cut so late that the IGU line can no longer be operated.
                                         “Buffer reservation” on page J-22
                                        A+W DynOpt also uses residual plates when optimizing. Thus, in comparison
                                        to customary production, it is possible to achieve significant material savings.
                                        Reported broken lites are automatically taken up into the optimization, so that
                                        as quick a remake as possible can be guaranteed. Each new optimization is
                                        linked to triggers, e.g. a specified state or a particular number of broken lites.
                                        In addition, all batches that have not yet been transferred to cutting are com-
                                        pletely suspended and re-optimized.
                                         “Optimization of the batches” on page J-17
1.00 / 01-2016




                                         “Dynamic time line” on page J-19




                 J-20                                                                                        A+W DynOpt
                 Tutorial                                                               Dynamic Optimization




                              Buffer system
                              Production with A+W DynOpt only makes sense with a suitable buffer. This re-
                              quires a buffer system in which lites are stored temporarily in sufficient quan-
                              tities and can be output to the lines at the right time. Thus the buffer also
                              ensures production on the lines if cutting stops.
                              A+W DynOpt is specially configured to the customer-side hardware. This also
                              applies for already-existing buffers. A+W DynOpt represents the logical buffer
                              in that is plans the lites that belong together. The physical reservation of the
                              buffer is specified by the manufacturer of the buffer. A+W DynOpt is always
                              adjusted so that it exploits the existing buffer optimally.
                              A+W DynOpt interacts with the buffer system and exchanges data. Here,
                              among other things, the reservation of the slots is configured so that it is ad-
                              justed locally to the production. Lites that are determined for an IGU line are
                              also stored near the IGU line.
                              In addition, the quantities of individual slots in the buffer can be locked. Slots
                              can also be locked completely by the manufacturers, e.g. if they are damaged
                              and cannot be used.
1.00 / 01-2016




                 A+W DynOpt                                                                                J-21
                 Dynamic Optimization                                                                                      Tutorial




                                               Buffer reservation
                                               In the buffer, there is a distinction between the logical and physical reservation
                                               of the buffer.
                                               •   The logical reservation specifies how lites must be kept together in slots.
                                                   This is the planning specification for the machine manufacturer.
                                               •   With the physical reservation, the slots are assigned as the logical reserva-
                                                   tion permits or requires this. The cut lites always batch according to the
                                                   specifications of the logical reservation in the slots.
                                               The cutting plans are only transferred to cutting if the space for the lites in the
                                               buffer is guaranteed.
                                               The Cutting overview dialog displays the reservation of the buffer.




                                A      B                                   C         D               E
                 A Status of the marked slot                               C Green: filled slot
                 B Marked slot                                             D Lites physically on hand (blue)
                                                                           E Gray: reserved slots for lites that are expected
                 Fig. J-8     Buffer overview in A+W Production


                                               Under the slots, the status of each slot is displayed:
                                               •   White: the slot is completely free.
                                               •   Gray: the slot is reserved.
                                               •   Dark green: the slot is reserved, but the lites are not yet ready for transport
                                                   out.
                                               •   Light green: the slot is reserved and the lites are ready for transport out.
1.00 / 01-2016




                                               Missing lites generate gaps in the time line. The buffer gets ever fuller because
                                               production waits for the lites. If the buffer becomes too full for optimal yield, it
                                               can become absolutely necessary to produce a particular lite. In this case, it


                 J-22                                                                                               A+W DynOpt
                 Tutorial                                                                 Dynamic Optimization




                              must be considered that the yield is not optimal, however production does not
                              come to a standstill.
                              If there are no more gaps in the time line, the buffer gets emptier. Thus the pos-
                              sibilities for optimization and yield increase again.


                              Working with Panorama
                              The Panorama handles the mapping of the machine model and communica-
                              tion with the machines. This is the central machine control and communication
                              component of A+W DynOpt.
                              The result of the optimization is written to the database and forms a so-called
                              step. These steps are read in by the A+W Realtime Optimizer, which then gen-
                              erates the data for Panorama. Panorama uses this data to control the system.

                              Residual plates
                              Panorama reports residual plates from the residual plate buffer to the A+W Re-
                              altime Optimizer. It queries the residual plate buffer via Panorama to see if this
                              plate can be stored. If so, the data is adjusted by the A+W Realtime Optimizer
                              and transferred to Panorama.

                              Buffer system
                              Panorama manages the buffer system logically and checks whether additional
                              cutting codes may be transferred. If all lites of the plate fit into the buffer sys-
                              tem, the cutting code is generated and transferred to the machine. According
                              to the specifications of the A+W DynOpt core and the optimization, Panorama
                              also controls which lites may be placed together in a buffer slot.

                              Rejects
                              Panorama receives item and breakage reports about the entire system from
                              the machine. Rejects that arise during transport in are remade automatically.
                              Essentially Panorama always tries to update the rejects so that the unit can
                              still be placed complete at the output. For this, A+W DynOpt has the following
                              modes for how plates with rejects can be prioritized:
                              •   The plates are sorted based on the next required normal lites at the output.
                                  Here plates that consist only of rejects are placed at the end of the se-
                                  quence.
                              •   The plates are sorted based on the next required normal lites at the output.
                                  Here plates that consist only of rejects are placed at the beginning of the
                                  sequence.
                              •   If based on the buffer reservation it is possible, all plates with rejects are
                                  placed at the beginning of the sequence. If, due to the buffer load, A+W
                                  DynOpt cannot accept such a sequence, units must be completed as
                                  quickly as possible in order to reduce the buffer load.
1.00 / 01-2016




                 A+W DynOpt                                                                                 J-23
                 Dynamic Optimization                                                                          Tutorial




                                        Special lites
                                        Lites that do not come from the optimization can be fed directly to the output,
                                        e.g. Purchased lites or hand cutting. If necessary, these lites can also be fed
                                        via an individual input.

                                        Production sequences
                                        For the production batches transferred, Panorama manages production se-
                                        quences with the information about units, lites, sequence, and status of a
                                        batch.
                                        Based on this information and the sequence of the sequences, Panorama
                                        commissions lites for transport out into an outlet. Panorama also receives item
                                        and breakage reports on the outgoing transport line.
1.00 / 01-2016




                 J-24                                                                                    A+W DynOpt
                 Tutorial                                                          Working with A+W DynOpt




                              Working with A+W DynOpt
                              A+W DynOpt requires only an employee with a comprehensive view of pro-
                              duction. This employee can initiate changes in the production flow and A+W
                              DynOpt executes the changes for the best possible performance.
                              The program channels the imported batches independently from input to out-
                              put as long as enough batches are imported and no interventions, e.g. due to
                              rush or broken sheets, are required.
                              The sequence of the batches can be changed with A+W DynOpt. For exam-
                              ple, lots can be pulled from the IGU line if this is necessary. The employee then
                              requests the lot in question on the screen and A+W DynOpt reorganizes the
                              lot.
                              The change is made with the maximum possible advantages and disadvantag-
                              es at this time. The consequences of the change, e.g. a batch pushed up, is
                              visible directly on the screen.
                              The employee must be able to assess the consequences of his interventions.
                              A+W DynOpt offers tools with which the employee can maintain an overview
                              and assess his decisions:
                              •   The A+W DynOpt Editor
                              •   Tab XOPT-ON Dynamics of A+W Realtime Optimizer
                              •   Cutting overview of A+W Realtime Optimizer
                              •   A+W Production Cockpit With configurable dialogs
                                  This control desk with various indicators created individually for a
                                  A+W DynOpt project is an optional add-on module that is not described
                                  here. As a central control desk, it displays the state of the overall system,
                                  e.g. glass flows and bottlenecks, output, buffer reservations, etc.
1.00 / 01-2016




                 A+W DynOpt                                                                               J-25
                 Working with A+W DynOpt                                                                            Tutorial




                            A
                                           B         C




                 A The A+W DynOpt Editor             B XOPT-ON Dynamics                 C Cutting overview

                 Fig. J-9       Program dialogs for working with A+W DynOpt


                                             The user must interpret the indicators and dialogs. Thus A+W DynOpt be-
                                             comes visible and the employee knows what the current status of production
                                             is.

                                                Example: effective work with A+W DynOpt

                                                The shift manager sees which glass types in what quantities the
                                                orders include. He recognizes that, for example, only three more lites
                                                must be cut from 8 mm LSG, but in the later course of orders, 2
                                                additional lites of the same type will follow.
                                                Therefore, the appropriate order with these lites must be imported
                                                into A+W DynOpt so that the program detects these lites of the same
                                                type and pulls the cutting of the lites of the same type together.
                                                For this, enough batches must have been imported so that A+W
                                                DynOpt can plan with maximum yield. If there are too few batches in
                                                the system, the program can only plan with a little data and the yield
                                                is reduced.
1.00 / 01-2016




                 J-26                                                                                        A+W DynOpt
                 Tutorial                                                                       Working with A+W DynOpt




                                          A+W DynOpt Editor
                                          A+W DynOpt works independently in the background, however the input data
                                          must be made available manually. The A+W DynOpt Editor dialog is available
                                          for this; use it to reach all additional dialogs.
                                          With the editor, you specify the work quantity to A+W DynOpt. With the se-
                                          quence of the imported batches, you specify their priority for processing.


                                 A                                     B                          C




                 D




                 E
                 F




                 A Batches from A+W Production                       D Details about the selected lites
                 B Batches transferred to A+W DynOpt                 E Setting for display on the time line
                 C XOPT-ON dynamic batches                           F Dynamic time line
                 Fig. J-10   The A+W DynOpt Editor


                                          On the top portion of the dialog, you import and prioritize batches. On the lower
                                          portion of the dialog, you see the dynamic time line and the status of each
                                          batch.
1.00 / 01-2016




                 A+W DynOpt                                                                                           J-27
                 Working with A+W DynOpt                                                                         Tutorial




                                       Status colors for the batches on the dynamic time line:
                                       •   Green: Lites of the batch are not yet optimized. Status 0.
                                       •   Yellow: at least one lite of the cluster has been optimized. Status 100.
                                       •   Blue: all lites of the cluster have been optimized. Status 200.
                                           If there are no more changes and there is no new optimization, the lites are
                                           cut this way.
                                       •   Light blue: the entire cluster has been cut.

                                       Sequence of the work
                                       With the following work, you can monitor the dynamic optimization:
                                       •   Import batches into A+W DynOpt.
                                       •   Get an overview:
                                           – Dynamic time line on the A+W DynOpt-Editor dialog
                                           – Configured dialogs in A+W Production Cockpit
                                           – XOPT-ON Dynamics tab
                                       •   Send cutting codes to the cutting tables on Cutting overview.

                                       Importing batches
                                       Import enough batches that A+W DynOpt can plan optimally and the dynamic
                                       time line does not batch empty.

                                       Prioritizing batches
                                       On the Edit batch sequence dialog, you change the prioritization of the batch-
                                       es. Critical for the prioritization is the answer to the question: Which lites have
                                       to be finished first?
                                       Here the speed of the cutting tables and the glass types play a role, e.g. can
                                       float be cut more quickly than LSG. A+W DynOpt automatically reaches further
                                       into the future for the LSG cutting. The planner must only be aware that he dis-
                                       tributes the share of batches with LST somewhat across the prioritization.
                                       The LSG gets a jump on the cutting so that both glass types land in the buffer
                                       at the right time and are available on the lines for further processing.

                                       Rejects
                                       Rejects are channeled automatically by A+W DynOpt as soon as they are re-
                                       ported by a scanner to a A+W Production terminal or other programs.
1.00 / 01-2016




                 J-28                                                                                     A+W DynOpt
                 Tutorial                                                          Working with A+W DynOpt




                              Prioritizing rush lites in two steps
                              If you would like to channel rush lites quickly through production, prioritize the
                              lites on the Edit batch sequence dialog in two steps.
                              You should only change the batch sequence within the same status, that is,
                              drag a batch with a green status up to a maximum of the top of the batches
                              marked in green. If you shift a batch over status limits, this change affects the
                              entire process.
                              A+W DynOpt can decline a prioritization under some circumstances if it would
                              cause problems in cutting or in the buffer.
                              The prioritization of batches cannot be executed as long as an optimization is
                              running.




                              Fig. J-11     Editing batch sequence


                              On this dialog you edit the sequence of the batches.
                              Status colors of the batches on the Edit batch sequence dialog:
                              •   Green: no cluster of the batch can flow out of the buffer.
                              •   Yellow: at least one cluster of the batch can flow out of the buffer.
                              •   Red: all lites of the batch can flow out of the buffer or are already flowing
                                  out.
1.00 / 01-2016




                 A+W DynOpt                                                                                J-29
                 Working with A+W DynOpt                                                                                     Tutorial




                                                First step
                                                In the first step, you shift the rush lites to the desired position before cutting on
                                                the Edit batch sequence dialog.
                                                You can drag the batch to the top of the status to which it belongs, that is, a
                                                batch marked green to the top of the batches marked green.


                        Output                                                                                      Input




                                                                                                                    t


                                        A               B         C                  D

                 A Dynamic buffer for cut lites                                  C Cutting
                 B Cut clusters (table 1)                                        D Rush lite
                 Fig. J-12       Prioritization of the rush lites, step 1


                                                The batch is then displayed in the appropriate place on the time line. The batch
                                                is now handled with high priority. At the same time it is ensured that the best
                                                possible optimization is guaranteed by A+W DynOpt. If you were to place a
                                                batch right at the start, A+W DynOpt would no longer have the opportunity to
                                                optimize as well as possible. In addition, the flow could stop.
1.00 / 01-2016




                 J-30                                                                                                   A+W DynOpt
                 Tutorial                                                                             Working with A+W DynOpt




                                                Second step
                                                In the second step, you shift the rush lites cut to the desired position after cut-
                                                ting on the Edit batch sequence dialog.
                                                If the batch is cut, it is marked in red. In the second step of the prioritization,
                                                you can drag the batches marked in red to the top. Thus the lites are the next
                                                ones taken from the buffer and channeled into the lines.


                       Output                                                                                     Input




                                                                                                                  t


                                       A                    B C                     D

                 A Cut rush lites in the buffer                                 C Cutting
                 B Cut rush lite
                 Fig. J-13      Prioritized rush lite


                                                The batch is then displayed as cut on the time line and shifted into the buffer.
1.00 / 01-2016




                 A+W DynOpt                                                                                                   J-31
                 Working with A+W DynOpt                                                                      Tutorial




                                       Tracing the result




                                       Fig. J-14    A+W Production Cockpit, batch overview


                                       You get the most effective display of batches and individual lites on the Batch
                                       overview tab in A+W Production Cockpit. This way, you can trace where the
                                       lites are and change their prioritization.
1.00 / 01-2016




                 J-32                                                                                   A+W DynOpt
                 Tutorial                                                                    Working with A+W DynOpt




                                          Using A+W DynOpt Editor
                                          In this tutorial, you will learn how to import batches into A+W DynOpt and
                                          change the priority of the batches.
                                          On these topics, please see the following instructions:
                                          •   “How to import batches into A+W DynOpt” on page J-33
                                          •   “How to change the priority of a batch” on page J-34


                                           How to import batches into A+W DynOpt
                                          1 Open the A+W DynOpt Editor dialog.




                 Fig. J-15   Importing batches


                                          2 On the Released batches list, mark the batches that you want to import into
                                            A+W DynOpt.
                                          3 Click the [Right arrow] button.
                                              The batches are imported into the XOPT-ON dynamic batches list and thus
                                              into A+W DynOpt.
                                          4 Click [OK] to close the dialog.
1.00 / 01-2016




                 A+W DynOpt                                                                                       J-33
                 Working with A+W DynOpt                                                                     Tutorial




                                        How to change the priority of a batch
                                       1 Open the A+W DynOpt Editor dialog.
                                       2 Click the [Batch sequence] button.




                                           Fig. J-16   Editing batch sequence


                                       3 Mark the batches whose priority like to change.
                                       4 Click the [Up arrow] or [Down arrow] button to increase or decrease the pri-
                                         ority of the batches.
                                       5 Click [OK] to close the dialog.
1.00 / 01-2016




                 J-34                                                                                 A+W DynOpt
A+W DynOpt            N

             Section index
                 Section index                                                 Index




                 Index
                 B                              S
                 Batches                        Standard optimization   J-14
                 – Importing J-28
                 – Optimization J-17            T
                 – Prioritizing J-28            Time line J-19
                 Buffer                         Triggering J-18
                 – Reservation J-22
                 – System J-21
                                                Y
                                                Yield   J-15
                 C
                 Cutting
                 – Overview       J-25

                 D
                 DynOpt Editor J-25, J-27
                 – Importing batches J-28
                 – Prioritizing J-28
                 – Rejects J-28
                 – Rush lites J-29
                 – Sequence J-28
                 – Using J-33

                 F
                 Flexibility   J-15

                 I
                 Input    J-19

                 L
                 Lot sizes
                 – Conflict      J-15

                 O
                 Output    J-19

                 P
                 Panorama J-23
                 Production sequences    J-24

                 R
                 Rejects
                 – DynOpt J-28
                 – Panorama J-23
1.00 / 01-2016




                 Re-optimization J-18
                 Residual plates J-23
                 Rush lites J-29


                 A+W DynOpt                                                    N-37
                 Index   Section index
1.00 / 01-2016




                 N-38    A+W DynOpt

