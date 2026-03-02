---
description: "EN-FUNC-AW_Capacity_Planner"
---


# A+W Functional Description: A+W Capacity Planner

---
## Content

1.  **Notes on this document**
    -   2.1. Trademarks
    -   2.2. Copyrights
    -   2.3. Disclaimer of liability
2.  **Performance Description**
    -   3.1. Data
    -   3.2. Description
    -   3.3. Prerequisites
    -   3.4. List of functions
        -   3.4.1. General
        -   3.4.2. Scheduling
        -   3.4.3. Transition times
        -   3.4.4. Calculation and management of processing times
        -   3.4.5. Cost calculation
        -   3.4.6. Reservation of machine capacities
        -   3.4.7. Campaign planning
        -   3.4.8. Managing shifts and shift plans
        -   3.4.9. Reassignment
        -   3.4.10. Production Monitor
        -   3.4.11. Booking/completion report
        -   3.4.12. Error handling/reworking
    -   3.5. Limitations
        -   3.5.1. General
        -   3.5.2. Scheduling
        -   3.5.3. Calculation and management of processing times
        -   3.5.4. Managing shifts and shift plans
        -   3.5.5. Production Monitor
        -   3.5.6. Cost calculation
        -   3.5.7. Reservation of machine capacities
        -   3.5.8. Campaign planning
        -   3.5.9. Reassignment
    -   3.6. Notes
        -   3.6.1. Setting up new capacity planning
        -   3.6.2. Additional notes and detailed information
3.  **Contact Address**

## Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### Copyrights

© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## Performance Description

### Data

| Field | Value |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220007, 221007, 222007, 226007, 223007, 224007, 227007, 225007 |
| **Module** | A+W Capacity Planner |
| **Brief description** | The module serves to schedule the existing production capacities at the cutting line, directly balancing them against the capacities already reserved for the orders on hand. |
| **Available** | |

### Description

The A+W Capacity Planner handles the planning and control of existing production capacities thanks to direct and ongoing comparison with the capacities reserved for the orders on hand. This permits to detect bottlenecks early on, and to amend the planning results where necessary.

Based on the parts chains included in the order data, for each element of the BOM, taking into consideration the delivery and inward goods dates, the production and processing dates and associated costs are determined and reported back to the ERP system. Here the A+W Capacity Planner also checks whether a requested dispatch/delivery date can be adhered to, and also under which basic conditions (e.g. machine availabilities, transition times, route dates) the earliest possible alternative date is possible if necessary.

A graphic capacity monitor - as new, central A+W Production control station - supports the checking of the utilization of machines and allows quick intervention in case of capacity bottlenecks, overruns, and work backlogs. In connection with the A+W Barcode Manager (article number 220010) and/or A+W Production Terminal (article number 220012), the production progress is booked and displayed graphically.

A simple and intelligent rescheduling helps you with required manual intervention into current production planning and to reschedule individual work processes on alternative machines or another shift due to machine maintenance.

### Prerequisites

- A+W Production (ALCIM) (article numbers 220001 and 220002)
- Set-up and correct master data (e.g. processing sequences, machine master data)
- The transfer from and reporting to the ERP system must be configured correctly.
- Parameters and switches in the machine assignment and capacity planning areas must be set up correctly and configured.

### List of functions

#### General

- In the course of capacitive scheduling, the system calculates various alternative results (transition times, machines, times, costs) and automatically selects the best/most efficient result. The final results are saved in the database and can then be visualized.
- Scheduling is done item by item and must be successful per item. If an order item cannot be scheduled successfully, then the whole order is not scheduled (imported).

#### Scheduling

- There is backward scheduling - starting from the defined requested delivery date in the ERP system.
- For the scheduling, the following are considered: shifts created, available capacities and times, defined bottlenecks, processing time per machine/tool, transition times between machines/tools, defined campaigns and reservations.
- The capacity planning is done in the course of scheduling, as a date optimization process (using alternative possibilities and their weighting).
    - The overall scheduling runs in iterations while testing and considering several additive basic conditions. Here, in addition to the capacity planning, the following are checked/executed: item and processing master data, machine assignment, shape geometry. Therefore, the capacity planning cannot be regarded in isolation.
    - Should a scheduling iteration not be successful, alternative possibilities (for example, alternative tools, alternative transition times) are checked and an alternative calculation is performed.
    - If the overall scheduling is not successful, an appropriate notice/error message is output. The user can then react to the error/problem to the extent of the technical possibilities and feasibility using an appropriate reworking dialog.
    - The number of scheduling iterations per order item can be configured.
- Initially, there is a check in the course of capacity planning whether the requested delivery date defined in the order can be adhered to.
    - If this date cannot be adhered to, the system can calculate an alternative date (considering the route/dispatch dates from the ERP system) and either report/propose or take over automatically (depending on the system configuration).
    - Confirmation of the requested delivery date or a newly-calculated delivery date is reported to the ERP system.

#### Transition times

- For the scheduling, transition times between different machines/tools can be defined. Three priorities can be used for transition times (normal, rush, and minimal). Furthermore, particular transitions can be forbidden (e.g. in order to depict that different machines cannot be reached without internal transport). Generally the use of the different transition times is controlled by appropriate order priorities.
    - Transition times can be specified in hours/minutes or shifts.
    - If allowed by the order priority or user control, the schedule optimization considers the shorter transition times insofar as this can calculate a work plan. Here, shorter transition times are preferred for early processing processes (e.g. cutting and seaming in one shift instead of tempering and packaging in one shift).
    - There is no complete switching from one transition priority to another, but rather an assessment of the entire BOM for minimal deviation from the optimal production throughput.
    - It is possible to specify a maximum value for transition times. Thus the system can calculate up to this maximum value within the flexible tolerances arising this way and consider possible alternatives, earlier dates in the calculation (e.g. for campaigns).
    - Possible/required buffer times at the end of the processing/process chain, e.g. for remake production, can be defined permanently (as set up "buffer processing") or reached automatically with the input of flexible transition times (maximum values).
- Orders that were transferred from the ERP system with high priority (identifiers in the Order.xml file, rush orders, e.g.) are scheduled automatically with a higher priority. The faster transition times are used insofar as they are useful for solution-finding.

#### Calculation and management of processing times

- There is a calculation of processing times. For this, simple and/or complex formulas can be stored for the calculation in 2 different editors.
    - "Simple" expressions can be formulated in a graphic editor. The graphic editor is recommended for expressions with 2-3 dependencies (e.g. glass thickness, length of an edge to be processed)
    - More complex expression can be formulated in a free, SQL-based editor. The SQL-based editor is recommended for complex expressions with 3 or more dependencies (e.g. shapes, shape edges, drill hole diameters).

#### Cost calculation

- For the cost calculation, wage costs, machine costs, and other costs can be defined. The total costs arise from the total of these three cost records.
- Determined total costs are reported to the ERP system.

#### Reservation of machine capacities

- It is possible to work with two different reservation methods – reservation orders and / or reservation of bottleneck machines.
    - Reservation orders must be entered as such in the ERP system and transmitted accordingly.
    - Reservation orders reserve appropriate capacities (times) on all machines/tools required for the production.
    - Reservation orders must be released for production by the ERP system before they can be planned and produced.
    - Reservations on bottleneck machines can only be created individually and are temporally limited.
    - Reservations on bottleneck machines can either be created for specific customers or projects.
    - For the management of reservations on bottleneck machines, there is an editor available for the user.
    - Created reservations on bottleneck machines are displayed graphically in the Production Monitor. A context dialog offers detail information about reservations created.
    - The user is informed about periods elapsed on/for reservations on bottleneck machines.

#### Campaign planning

- It is possible for individual processing processes to create campaign dates (individual dates or dates that recur weekly for a particular time period), insofar as the processing has been defined as campaign processing. In the scheduling, only these defined campaign dates are taken into account. All other shifts and dates are invalid for this processing.

#### Managing shifts and shift plans

- Various shift plans can be defined.
    - There is a shift plan editor available for long-term planning.
    - Short-term changes and additions with respect to the shift plans can be undertaken flexibly in the Production Monitor.
    - Various shift times (beginning and end) can be defined, as well as a duration for which a shift plan is created.
    - It is possible to activate/permit scheduling of shifts only for rush orders.
- It is possible to deactivate or delete shifts flexibly.
- It is possible to flexibly create new shifts individually.
- It is possible to define a shift (for a tool) as bottleneck shift.
    - Here, the limits defined for a bottleneck apply (e.g. overload)
- It is possible to define a tool (machine) as bottleneck.
    - Here, the limits defined for a bottleneck apply (e.g. overload)
- It is possible to shorten or lengthen shift times.

#### Reassignment

- There is a graphic rescheduling editor available. Here it is possible to shift complete orders or an individual processing to another date and/or to another machine (must be defined as alternative tool)(rescheduling).
- Various modes can be rescheduled for the rescheduling:
    - **Reschedule complete parts list:** The complete parts list to which the processing belongs is rescheduled.
    - **Only marked processing:** Only the marked processing is rescheduled.
    - **Marked and all following processings:** The marked and all following processings of the sheet are rescheduled.
    - **Marked and all previous processings:** The marked and all previous processings of the sheet are rescheduled.
    - **Unconditional date assignment for marked processing:** The marked processing is assigned the selected date on the selected machine. There is no plausibility check, machine capacities are not considered here.
- The rescheduling of the delivery/dispatch date is protected and only happens if the dispatch process should be selected manually, explicitly and be the goal of the rescheduling.
- It is possible to protect individual processing dates against rescheduling. This protection can also be lifted again.
- Inward goods dates for ordered glass will be considered. Depending on the configuration, individual users can be permitted to work around this check during rescheduling.
- Depending on the configuration, individual users can be permitted to shift the delivery date by a maximum number of days that can be specified during rescheduling. This can also be regarded as automatic rescheduling.

#### Production Monitor

- With active A+W Production capacity planning, the Production Monitor provides a new, central graphic control station for the work preparation, control, and monitoring.
    - It is possible to begin the process of rough scheduling from here.
    - It is possible to filter for individual orders/reservation orders.
    - It is possible to filter for individual machines/machine areas.
    - It is possible to change individual elements and emphases (for example, colors, display of backlogs).
    - It is possible to switch the processing times/output of on individual machines (or globally for all machines) between hours/minutes, area, and weight. Here, attention must be paid to correct settings and a correct interpretation of the values displayed.
- It is possible to change the displayed/calculated processing time and thus the appropriate capacitive machine utilization for a selected shift (processing) using a factor. A complete recalculation of all processing times of a BOM (parts chain) is possible via a new scheduling.

#### Booking/completion report

- With the A+W Barcode Manager (article number 220010) and/or A+W Production Terminal (article number 220012), it is possible to report processing processes as completed.
    - Based on the bookings, the booked and free capacities are displayed in color in the Production Monitor and updated accordingly.
    - If production should be done earlier (and booked accordingly) than calculated/scheduled by the capacity planning, then the capacities - in the future - will be released again.
    - Released capacities are considered in the course of new order scheduling.

#### Error handling/reworking

- It is possible to react to error/problems in the course of capacitive scheduling. Various strategies/selection possibilities are available to the user for this on a separate dialog - the so-called "Manual reworking":
    - **Repeat Data Import.** With this option, the order data is scheduled again and unchanged. This can be helpful if master data entries were flawed/were missing and were corrected accordingly.
    - **Force scheduling.** With this option, the scheduling is forced. Here the capacity limits of bottleneck tools are not considered.
    - **Ignore scheduling.** With this option, the scheduling is forced and the order is scheduled using the minimum transition times. Most scheduling rules are overridden here (e.g. adherence to campaign dates, capacity limits).
    - **Delete incorrect orders.** With this option, the orders in question are deleted from A+W Production. Correction of the data in the ERP system and another data transmission to A+W Production are necessary.
    - **Confirm determined delivery date.** This causes the takeover of the dispatch/delivery date newly calculated by the capacity planning as well as the appropriate reporting to the ERP system (only possible together with A+W Enterprise as ERP system).

### Limitations

#### General

- Changes to capacity master data only become effective in the course of rescheduling (for newly-scheduled orders/quotations/reservation orders).
    - For the active saving and takeover of these changes, a restart of the scheduling service (Items4Alcim) is recommended.
- It is not possible to have various capacity results (dates, costs, times) calculated for an order/quotation/reservation order and then select a result. The system automatically selects the best/most efficient (most time- and cost-effective) result.

#### Scheduling

- It is not possible to perform forward scheduling.
- A transition scheduling process (grid) cannot be switched manually.
- Calculated production start dates are not considered automatically for the batch formation (in the course of rough scheduling).
    - Here it is recommended to insert additional information columns into the displays that display the production start dates and processing dates calculated by the capacity planning.
    - The calculated earliest production date If all parts chains included in a batch should be selected/confirmed as production start date for the batch formation.
- If in the course of rough scheduling another, different production start date should be selected as the earliest production start date calculated by the capacity planning, this has no effect on the capacity planning and corresponding dates.
- It is not possible to display reasons for/causes of a scheduling result in order to trace the calculation of the capacity planning, for example.

#### Calculation and management of processing times

- Changes to processing times (master data) have no effect on already-scheduled orders.
    - Should it be necessary, it is recommended that you reschedule or check an individual processing time again using the Production Monitor (context menu -> Check factor again).

#### Managing shifts and shift plans

- It is not possible to define pauses within shifts. Here a shift grid must be defined in which there are pauses between the shifts.
- If in ongoing operation there is a change of shift plans or properties (e.g. deletion of shifts or change from 2- to 3-shift operation), then dates and/or times for orders/individual processing processes are not automatically aligned with the changes.

#### Production Monitor

- If production should be done earlier and booked accordingly with A+W Barcode Manager (article number 220010) and/or A+W Production Terminal (article number 220006 and 220007) than calculated/scheduled by the capacity planning, then the capacities - in the future - will be released again. The graphic display of the planned processing is not updated (remains graphically in the future, but is displayed as produced/processed).
- Reservation orders are not displayed graphically (distinguished from normal orders).
- Campaigns are not displayed graphically (distinguished from normal shifts).
- It is not possible to display transition times graphically.

#### Cost calculation

- In A+W Production it is not possible to manually change/override the production costs calculated for an order (after scheduling has been done).
    - Here, a change of the master data and a subsequent rescheduling may be necessary.
- It is not possible to define different cost records for different days and/or times.

#### Reservation of machine capacities

Created reservations on bottleneck tools are only considered for the scheduling of normal orders, not for reservation orders.

#### Campaign planning

Campaign planning is based on work processes. Machine-dependent campaigns can be depicted in that machine-specific work processes are created.

#### Reassignment

There is no automatic rescheduling of already-scheduled orders/processings (for example, in the course of changes to shifts and transition times).

### Notes

#### Setting up new capacity planning

- The set-up is normally done in the course of a customer project or update. For this, a detailed conversation is initiated, in which the customer (e.g. Production Manager and employees who handle work preparation) and the A+W consultant analyze the basic conditions and real requirements together. Subsequently, this result is mapped in the course of the technical basic conditions in shifts, transition times, and processing times.
- In a new project, a database with a set of defined and described shifts and formulas for processing times can be made available to the customer. This guarantees that a) production using the defined standards is possible quickly and easily and b) these standards will continue to function in the course of update and patches.
- The capacity planning has significant effects on the production organization and machine management and can therefore result in significant added costs. Therefore, it is recommended that you familiarize yourself intensively with the possibilities and displays of A+W Production Capacity Planning. Furthermore, it is recommended that in case of changes in the processing and/or machine master data area, you always contact A+W Support.
- In practice, there are various strategies for optimal capacity planning and management; these depend heavily on the company in question, the machines, and the products to be produced. Therefore, there is no automatic scheduling and shift management.
- The A+W standard database, which we offer customers in the course of a new project and we recommend that they use, includes a pre-defined set of capacity master master data (e.g. shifts and formulas for processing times). These were set up by experienced A+W consultants based on many years' experience.

#### Additional notes and detailed information

- For detailed descriptions of exact operation methods and workflows in the course of capacity planning, please see the A+W Production Capacity Planning manual and the help.
- For detailed questions before you have purchased product(s), please contact A+W Sales or, in the course of cooperation, A+W Support.

## Contact Address

**A+W Software GmbH**

Siemensstraße 3  
35463 Fernwald  
Germany

**Tel.** +49 641 96620-0  
**E-mail:** info@a-w.com  
**Internet:** http://www.a-w.com/
