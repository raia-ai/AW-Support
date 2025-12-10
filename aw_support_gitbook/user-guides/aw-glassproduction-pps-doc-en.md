---
description: "A+W Production Software Suite Overview"
---


# A+W Production Software Suite

---
## Overview

### Features
- Flexible PPS solution for complete rough and detailed scheduling for IGU, Tempered, single and laminated glass production
- Complete control of your production areas, machines and material flow
- Rough and detailed scheduling, optimization, machine assignment and control as well as creation of production papers and labels.
- Allows planning and control of even the most demanding multi-level production flows
- Sequence optimization, rack and stacking organization and optimization

### Specs
- ERP system is required
- Can be run on different SQL engines, Informix or MS SQL
- Reports: Crystal Reports
- Operating System: Microsoft Windows

## Machinery Allocation

### Features
- Automatic assignment and flexible reassignment of all related processes for production
- Base or Complex rules as machine restrictions
- Preferred routes through the factory based on selectable criteria's
- BOM Configurator to add processing's
- Integration plausibility checks

### Specs
- For plausibility checks external interfaces are needed

### Example: Machinery Allocation Editor
The following table shows an example of how machines can be managed within the system, including their type, registration point, and component ID.

| ID   | Name                        | Type                 | Registration point       | Compo |
|------|-----------------------------|----------------------|--------------------------|-------|
| 110  | Cutting Table 1             | Cutting (Zuschnitt)  | 110/Table1               | TB1   |
| 120  | Cutting Table 2             | Cutting (Zuschnitt)  | 120/Table2               | TB2   |
| 130  | LG Cutting 1                | Cutting (Zuschnitt)  | 130/Table3               | TB6   |
| 150  | Combi 1                     | Cutting (Zuschnitt)  | 150/Combi Table 1        | TB3   |
| 155  | Combi 2                     | Cutting (Zuschnitt)  | 155/Combi Table 2        | TB5   |
| 190  | Manual Cutting              | Cutting (Zuschnitt)  | 190/Manual Cutting       | TB4   |
| 210  | Goods receipt               | Other (Sonstiges)    | 210/Goods Received       |       |
| 220  | Stock                       | Other (Sonstiges)    | 220/Stock Withdrawal     |       |
| 310  | Edger Seaming               | PROCESSINGLINE       | 310/Seaming              | LISEC |
| 410  | Edger Polishing (4 sides)   | Other (Sonstiges)    | 410/Polishing            |       |
| 510  | Edger Grinding (2 sides)    | Other (Sonstiges)    | 510/Grinding             |       |
| 610  | Edger Single Special Edges  | Other (Sonstiges)    | 610/Special1             |       |
| 810  | Drilling                    | Other (Sonstiges)    | 810/Drilling             |       |
| 910  | CNC center                  | Other (Sonstiges)    | 910/CNC                  |       |
| 1010 | Surface treatment           | Other (Sonstiges)    | 1010/Surface Process     |       |
| 1210 | Screen Printing             | Other (Sonstiges)    | 1210/Screenprint         |       |
| 1310 | Toughening 1                | Other (Sonstiges)    | 1310/Fum 1               |       |
| 1320 | Toughening 2                | Other (Sonstiges)    | 1320/Fum 2               |       |
| 1410 | Heat Soak                   | Other (Sonstiges)    | 1410/Heat Soak           |       |
| 1510 | LG-Line                     | Other (Sonstiges)    | 1510/Lam 1               |       |
| 1610 | IG-Line 1                   | IG-Line (ISO-Linie)  | 1610/IG 1                | LIN1  |

## Rough Scheduling

### Features
- Creation of Jobs
- Analyse of planning relevant information for production
- Optional Rack Optimizer
- Planning of purchased parts

### Specs
- For rack optimization A+W Rack optimizer is required

## Detailed Scheduling

### Features
- Sequenced optimization
- Multiple Rack allocation in production sequence
- Multistep rack allocation possible
- Comfortable display and change possibilities

### Specs
- A+W Sequence Optimizer required

## Release Management

### Features
- Release of production related paperwork(or preview) and labels for controlling your production in the background
- Release of machine code for the production area

### Specs
- Machine Connectors for code release

### Example: Releasable Documents and Outputs
- List of supplies
- Production label
- Rack list cutting
- Rack allocation list cutting
- Shipping label
- Cutting plan
- Manual cutting list
- List of physical rack optimisation
- Work order
- LAMI sorting list
- LAMI production list
- Processing list
- IG sorting list
- Fire Protection Glass (Brandschutzglas)
- Spacer list
- Georgian bar list
- Shipping list
- PMO rack list

## Multistep Management

### Features
- Combined production organisations for the inheritance of sequence to upstream and intermediate products (TGH in IGU)
- Automatic removal of intermediate products from the overall bill of materials based on glass type approval
- Automatic holding together of different base glasses belonging to an order position

### Specs
- Definition of release parts and release processes

## Statistics/BI

### Features
- Statistical evaluations based on A+W ERP and PPS databases
- Display of key figures on a customizable graphic user interface
- Completely web-based – display the data on desktop PCs, tablets or smartphones
- Use pre-defined A+W reports and create your own reports flexibly – even without a connection to your A+W applications and their databases
- Full control over all aspects of the analysis, data and rights management

### Specs
- Third party Software is needed

# A+W Production Add-ons

This section details the various add-on modules available for the A+W Production suite, which provide enhanced and specialized functionalities.

**Available Add-ons:**
- A+W Capacity Planner
- A+W Production Multisite PO Tracking
- A+W Breakage Manager
- A+W Shape Optimizer
- A+W Sequence Optimizer
- A+W Realtime Optimizer
- A+W Production Terminal
- A+W DynOpt
- A+W Defect Optimizer
- A+W Residual Stock Manager
- A+W Continuous Cutting
- A+W Furnace Optimizer
- A+W Rack Optimizer
- A+W Barcode Manager
- A+W Smart Factory
- Machine Connectors
- A+W Breakout Display
- A+W Info Terminal

---

## A+W Capacity Planner (Add-on)

### Features
- Calculation and display of free capacities and machine utilization
- Calculation and reporting of production dates and costs
- Automatic rescheduling of delivery dates in case of insufficient capacities during dispatch
- Automatic load distribution on machines based on work processes
- Graphic display of production progress (using PDC bookings via A+W Barcode Manager or A+W Production Terminal)

### Specs
- A+W Barcode Manager required

## A+W Production Multisite PO Tracking (Add-on)

### Features
- Tracking control of external items inside a company group without printing new labels

### Specs
- A+W Barcoding Manager
- Different number areas for barcodes

## A+W Breakage Manager (Add-on)

### Features
- Ability to report rejects from our different products and addons
- Individual treatment for BOM

### Specs
- A+W Barcode Manager required

## A+W Shape Optimizer (Add-on)

### Features
- Cut minimization due to combination of shapes in a circumscribed rectangle
- Adherence to the defined production sequence
- Cost reduction due to optimal space usage of patterns on stock sheets
- Environment-friendly – Reduction of waste
- Easy break-out integrated

### Specs
- A+W Production required
- A+W Sequence Optimizer required

## A+W Sequence Optimizer (Add-on)

### Features
- Optimizes in the required sequence, no manual glass sorting
- Saves space on the A-Racks by using the full space of the rack and more than one stack
- Multithread optimization with more than 19 different optimization algorithms

## A+W Realtime Optimizer (Add-on)

### Features
- Continuous material flow between cutting and downstream processes
- Consideration of the production sequence arising from fine planning
- Residual sheet reduction due to filling up with rush order sheets or breakage or with sheets from a freely-selectable follow-up optimization
- Dynamic optimization of any* breakage
- Online control of the cutting tables and breakage displays

### Specs
- PPS Solution
- * Barcode Manager and Breakage Manager required

## A+W Breakout Display (Add-on)

### Features
- Display of cutting patterns and information for the cutting operator
- Handling of Breakages, and breakage reasons during cutting
- Online communication with hardware, like push buttons or pedals, or Machines.

### Specs
- PPS Solution with A+W Real Time Optimizer
- Barcode Manager and Breakage Manager required for Breakages

## A+W Production Terminal (Add-on)
The A+W Production Terminal is a series of specialized interfaces for different stages of production.

### A+W Production Terminal – IG In
#### Features
- Visualization of lite structures
- Display of CAD drawings and file attachments
- Adjustment of the user interface
- Machine Connector integration increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal – IG Assembly
#### Features
- Visualization of lite structures
- Display of CAD drawings and file attachments
- Adjustment of the user interface
- Machine Connector integration increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal – IG Out
#### Features
- Visualization of lite structures
- Display of CAD drawings and file attachments
- Adjustment of the user interface
- Machine Connector integration increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal - Processing
#### Features
- Visualization of lite structures
- Display of CAD drawings and processes with assignment
- Adjustment of the user interface
- Increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal - Tempering
#### Features
- Visualization of lite structures on furnace bed
- Display of CAD drawings including stamps and processings
- Adjustment of the user interface
- Increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal - Batch
#### Features
- Visualization of lite structures
- Display of CAD drawings
- Adjustment of the user interface
- Increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal – LAM In
#### Features
- Visualization of lite structures
- Display of CAD drawings
- Adjustment of the user interface
- Increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

### A+W Production Terminal – LAM Assembly
#### Features
- Visualization of lite structures
- Display of CAD drawings
- Adjustment of the user interface
- Increasing process reliability
- Fewer production papers
- Increased productivity
#### Specs
- A+W Barcode Manager needed

## A+W Info Terminal (Add-on)

### Features
- Visualization of lite structures
- Display of CAD drawings
- Adjustment of the user interface
- Increasing process reliability
- Fewer production papers
- Increased productivity

### Specs
- A+W Barcode Manager needed
- No bookings possible

## A+W Dynopt (Add-on)

### Features
- Improved efficiency of the cutting lines with continues glass flow
- No limits on the size of production lots (from individual sheets on through to daily production)
- For use with Harp Racks (mixed with A-racks) instead of a physical sorting system
- Preparation time from cutting to production is reduced to a minimum
- Linking of batches and reducing residue plates.

### Specs
- A+W Real Time Optimizer
