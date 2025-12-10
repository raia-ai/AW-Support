---
description: "EN-FUNC-AW_Production_Terminal"
---


# A+W Production Terminal Functional Description

**A+W - Software for Glass**

---

---
## Contents
1.  **Contents**
2.  **Notes on this Document**
    *   2.1. Trademarks
    *   2.2. Copyrights
    *   2.3. Disclaimer of liability
3.  **Performance Description**
    *   3.1. Data
    *   3.2. Description
    *   3.3. Prerequisites
    *   3.4. List of functions
        *   3.4.1. Terminal Edit
        *   3.4.2. Terminal Order
        *   3.4.3. Terminal Processing
        *   3.4.4. Terminal TG-In
        *   3.4.5. Terminal TG-Out
        *   3.4.6. Terminal LG-In
        *   3.4.7. Terminal LG-Assembly
        *   3.4.8. Terminal IG-In
        *   3.4.9. Terminal IG-Assembly
        *   3.4.10. Terminal IG-Out
        *   3.4.11. Terminal Manual Cutting
        *   3.4.12. Terminal Georgian Bars
        *   3.4.13. Terminal Info
        *   3.4.14. Terminal Bender
        *   3.4.15. Terminal Cut to Rack
    *   3.5. Limitations
    *   3.6. Notes
4.  **Contact Address**

---

## Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### Copyrights

© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

---

## Performance Description

### Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220012 |
| **Module** | A+W Production Terminal |
| **Brief description** | Control and display program in production |
| **Available** | Starting with A+W Production v6 |

### Description

A+W Production Terminal handles production control at various points in the production flow. Since different information and functions are required at different stations in production, there are a multitude of versions for the individual process steps. The basic functions of A+W Production Terminal include the display of information about the lites to be produced, the booking of lites at registration point or rack, breakage entry, and label printing. Other standard functions are the logging in and out of employees, the booking of machine states (operation, fault, pause), and the possible entry of batch information, which is written to the database during production of the lites.

In the A+W Production Terminals Order, Processing, TG-In, LG-In, and IG-In it is possible to load work in progress into the display. In these terminals, an overview of the work planned on the individual machine is possible with a dialog.

In all A+W Production Terminals except for Terminal Edit, it is possible to display the CAD drawing for the selected lite.

### Prerequisites

The requirement for the use of A+W Production Terminal is the formation of production batches with A+W Production. The booking service A+W Production Booking must be installed.

### List of functions

The functions of the individual terminals will be described here.

#### Terminal Edit

With Terminal Edit, it is possible to reschedule lites, racks or registration points. The display offers an overview of which racks and lites are at the selected registration point and which lites are on the racks. Rebookings of lites to rack, lites to registration point, and rack to registration point are possible. Furthermore, bookings of states to lites, racks, and registration points are possible, for example, breakage on lite or state delivered on rack or registration point truck.

A dialog offers information about delivered racks, the customer assignment of the delivered rack can be edited.

#### Terminal Order

The Terminal Order handles the booking of lites to a selected registration point. Terminal Order is not assigned to any station in production; instead, it can be used everywhere where a larger number of lites must be booked. A batch or an order number can be entered to select the lites. When filling the display, all lites are displayed that have an incomplete processing at the selected registration point. The CAD drawing and a list of processings are displayed for the selected lite.

The lites to be booked are marked in the list and the quantity to be produced is entered. The selected lites are rebooked with produce. A breakage report can be made for the selected lites.

Terminal Order is the only terminal that supports quantity PDC.

#### Terminal Processing

Terminal Processing is on processing machines, for example drills or grinding machines. The display is filled by reading a lite bar code. Alternatively, the display can also be filled by selecting a lot for this machine. Data from the lite read is displayed, dimensions, the CAD drawing, and a list of already-booked and still-open processings.

During production, the processing is booked on the machine and the lite is booked to the outgoing registration point. Generally a driver for processing the lite is also called. Several drivers can be configured, the driver to be called can be selected with a combo box.

To be clarified is whether there is a driver that can be called by Terminal Processing for the machine to be activated. Normally it is assumed that there is a CAD drawing for the lite to be processed.

#### Terminal TG-In

Terminal TG-In is at the furnace intake and assists with the assignment of the furnace bed. The filling of the display is done by reading the lite bar codes when placing on the furnace bed. The scanned lites are booked to the furnace bed and appear on the display. On a separate window, the furnace bed is depicted graphically with its assignment. With action bar codes or with mouse and keyboard, it is possible to position lites differently on the furnace bed. If the furnace bed is completely assigned, the furnace bed is booked to the registration point furnace and it appears on the display of the downstream Terminal TG-Out.

#### Terminal TG-Out

Terminal TG-Out is at the furnace outlet. The furnace bed produced at the inlet is displayed here. On the main window there is a list of the lites, on an additional window a graphic display of the furnace bed. For storage of the lites, an outgoing rack is reported and the lites on the furnace bed are booked to the rack. If all lites of the furnace bed have been stored, the next furnace bed produced is displayed.

#### Terminal LG-In

Terminal LG-In is at the inlet to the LSG line. The selection of the units to be produced can either be done by batch and lot (analogous to Terminal IG-In) or order-by-order or by scanning individual subparts.

For the next unit, the dimensions, the CAD drawing, and the product structure with position of coating and structure are displayed.

With production, the unit appears on the display of the downstream Terminal LG-Assembly.

The unit can be skipped and subparts can be reported broken after selecting a breakage reason.

#### Terminal LG-Assembly

Terminal LG-Assembly is in the cleanroom. The units produced by the upstream Terminal LG-In are displayed in their production sequence. For the next unit, the dimensions, the CAD drawing, and the product structure with position of coating and structure and the required films are displayed. The display appears already if the first subpart has been produced on Terminal LG-In in order to display the information about the films in the cleanroom as early as possible.

With production, the assembly of the unit is booked and the LSG is booked into the autoclave. If an autoclave is fully loaded, the next autoclave can be selected. Subparts can be reported broken.

#### Terminal IG-In

Terminal IG-In is at the inlet to the insulated glass line. All insulated glass lots to be produced on this line are displayed here. A batch and a lot can be selected and the units to be produced are displayed in their planned production sequence. For the next unit, the dimensions, the CAD drawing, and the product structure with position of coating and structure are displayed.

With production, the unit appears at the inlet of the downstream Terminal IG-Assembly and it appears on the display there.

If subparts to be set up are not available, the unit can be skipped. One or several subparts can be reported broken after selecting a breakage reason. Activation of the machine is possible from IG-In. Here, there are two different variants:

*   **Single IG line activation (MachineConnector B)**, which includes the file generation for release and optionally a copying of the file in the IG-In into a directory for the line. The selection of the batch and the record must be done manually on the line.

*   **IG line activation via TCP/IP communication (MachineConnector C)**. The driver file generation is done in the course of the A+W Production release. The A+W Production Terminal IG-In copies the file, if necessary to a directory for the line. The selection of the batch and the record within the batch of the IG line is done via a TCP/IP message from the A+W Production Terminal. This means that the line synchronizes itself on the units loaded in the A+W Production Terminal IG-In. This saves the user the manual selection on the IG line, which especially for reproduction, where you have to jump back and forth between batches, results in many fewer manual operations. The switching in the IG-In takes place automatically lite by lite via the TCP/IP communication via the infeed message in the washing machine. Through TCP/IP communication, the previously required double operation on the terminal and IG line is reduced to a minimum.

#### Terminal IG-Assembly

Terminal IG-Assembly is on the insulated glass line behind the washing machine and in front of the station for setting the frame. The units produced by the upstream Terminal IG-In are displayed here in their actual production sequence. As in Terminal IG-In, the dimensions, CAD drawing, and product structure for the next unit are displayed with position of coating and structure.

With production, the assembly of the unit is booked and the IGU appears on the display of the downstream Terminal IG-Out. Subparts can be reported broken.

#### Terminal IG-Out

Terminal IG-Out is at the outlet of the insulated glass line. The units produced by the upstream Terminal IG-Assembly are displayed here. The dimensions, CAD drawing, and data important for dispatch such as customer and delivery location are displayed for the next unit to be stored. To store the unit, a rack is reported through scanner reading or manual input. The units are assigned to various packaging groups; for example, the grouping can be done by customer.

During production, the next unit can be booked to the outgoing rack reported. The unit can be reported broken after selecting a breakage reason.

**LoadRacks Dialog**

In A+W Production Terminal IG-Out, a second screen can be incorporated, one that displays from which logical A-racks lites are already present in the sorting system and via which the transport out of a rack can be requested. The dialog appears as a second screen on a separate monitor and can remain permanently open during usage.

The lites present in the sorting system are displayed per stack, there is one line per stack. The display is sorted according to job-rack stack; the sorting cannot be changed. Although the display is precise to the stack, the transport out is only done rack-wise. If the user selects a stack, all other stacks of this rack are automatically selected as well. Racks can be selected and requested, for which all or only some of the lites are present in the sorting system.

Analogous to the filters in A+W Production Terminal Jobs, with a combo box, the display can be filtered according to the various outputs, for example, for "All tables," "Table 1," and "Table 2." In contrast to A+W Production Terminal Jobs, however, here no SQL expression is saved as a filter; instead, only the registration point number of the table, for example "110" or "120." If the selection in the combo box changes, only the racks are displayed that correspond to the selected table.

This dialog can only be used if a panorama has already been installed at the customer's, one that serves a sorting system. This sorting system must have an A-rack wall. The panorama must be in a position to react to the message GetRequestableRacks(). This must be clarified project-specifically.

#### Terminal Manual Cutting

The Terminal Manual Cutting is generally found on a manual cutting table and displays all released batches and lots for this table. It can be installed on any table that does not have its own activation.

After a batch or a lot has been selected, the associated items are displayed on the Release dialog including the model display and the CAD drawing.

The label printing for the corresponding lite can be started directly. After selection of a breakage reason, the lite can be reported broken.

#### Terminal Georgian Bars

With the Terminal Georgian Bars, the Georgian bar patterns to be produced are displayed on the monitor.

If a batch or lot has been selected, the corresponding Georgian bar patterns are displayed on the Release dialog and their production can be reported finished.

Printing for the corresponding Georgian bar pattern can be started directly. After selection of a breakage reason, the Georgian bar can be reported broken.

#### Terminal Info

The A+W Info Terminal only provides information about orders or individual lites in production. As compared to A+W Production Terminal, there is no opportunity to make bookings in the PDC or to generate CNC code.

Apart from detailed information on the workload at hand, lite structures, furnace loads, CAD sketches, production texts, documents, and the customer's own sketches can be displayed for the corresponding order items. Furthermore, it is possible to output reports and labels from the A+W Info Terminal on a printer that can be selected.

#### Terminal Bender

The frames to be produced with the Terminal Bender are displayed on the monitor. If a batch or lot has been selected, the corresponding frame patterns are displayed on the Release dialog. After selection of a breakage reason, the frame can be reported broken.

#### Terminal Cut to Rack

The Terminal Cut to Rack is behind cutting. One or several racks are selected and the Release dialog is opened. A physical rack is then assigned to the quantity selected.

After selection of a breakage reason, the lite can also be reported broken here.

### Limitations

Quantity PDC is only supported by Terminal Order.

If Production Terminal is running on a terminal server, there are limitations for the use of serial scanners and buttons. With the use of thin clients, it may not be possible to use serial devices under some circumstances. For each thin client, it must be clarified whether serial scanners and buttons can be used with this device.

The activation of machines is possible on the terminals for IGU production and in Terminal Processing. Especially in combination with DynOpt, there are solutions that are not standard and in any case make for greater set-up effort and additional development work.

The IG line activation via TCP/IP communication is only possible with lite-by-lite switching in the IG-In.

### Notes
*(This section is intentionally blank in the source document.)*

---

## Contact Address

**A+W Software GmbH**

Siemensstraße 3  
35463 Fernwald  
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com  
Internet: http://www.a-w.com/
