---
description: "A+W Breakage Manager - Functional Description"
---


# A+W Functional Description: A+W Breakage Manager

*A+W - Software for Glass*

---

---
## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2021, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220013 |
| **Module** | A+W Breakage Manager |
| **Brief description** | Module for entering, tracing, and adding breakage to the production organization |
| **Available** | From A+W Production 6 |

### 3.2. Description

The A+W Breakage Manager is a system-wide module for the entry, tracing and steering of reported broken lites into the production organization.

Broken lites can be entered via scanner, A+W Production Terminals, the breakage screen in cutting or through manual entry into the system. The current state of such remakes can be observed via views in A+W Production.
The A+W Breakage Manager now offers different possibilities for steering these broken lites back into production (see function list).
Advantages: breakage handling is integrated completely into A+W Production. There is no more handing around manual notices and making manual entries in cutting or at other points. Mistaken production due to potentially incorrect entries is thus avoided. Furthermore, the status of a remake in the system can be checked at any time and breakage statistics can be compiled according to cause, location and glass type.

### 3.3. Requirements

In order to be able to use the full functional scope of the A+W Breakage Manager, in addition to the appropriate hardware, you must have the following software modules:

- A+W Production (core module)
- A+W Barcode Manager (for the entry and tracing of remakes)
- A+W Realtime Optimizer (for automatic recutting)

### 3.4. List of functions

The A+W Breakage Manager consists functionally of 3 parts:

- Reject entry
- Reproduction
- Reject tracing and evaluation (reporting)

#### 3.4.1. Reject entry

Rejects are entered with state bookings. First the type of state is determined, which determines what should happen with the lite subsequently. Such states can be entered via scanner, A+W Production Terminals, the breakage screen in cutting or through manual entry into the system. Via the selected state, both the quality of the reject as well as the type of reproduction can be determined. The following state types are distinguished:

- **Defect:** is used, for example, if no reproduction is required because the defect can be eliminated (polishing out of a scratch). This state is only saved for the glass until the glass is booked again.
- **Cancellation:** with this state, you mark a lite as canceled (only for the production; not commercially!). With this state you are trying to avoid having the lite produced further.
- **No automatic recutting:** this state type ensures that all processings on the lite are reset (that is, they must be repeated). However, no automatic recutting is initiated.
- **Automatic recutting:** this state type ensures that the lite is recut automatically and that all processings must be repeated. So that with a reject booking of an assembled product (LG or IG) the components included can be recut automatically, it is absolutely necessary that you have previously booked the components as "assembled" with the A+W Production Terminal.
- **Rough scheduling remakes:** for complex processings it can be necessary to not recut the rejected lites directly, but rather to re-plan them completely. The "Rough scheduling remakes" type therefore generates a new item in the order pool as a copy of the original item. That is, the new item initially receives the processing dates of the original item. An automatic calculation of new processing dates by the capacity planning would not be very helpful here since the reproduction would otherwise be done much too late. The new item is marked as such in the A+W Production views and it can be rescheduled (new processing dates, new production run, new optimization, etc.)
- **Part break:** the type "Part break" is used if an assembled product (e.g. insulated glass) is not completely broken, but rather some of it can be reused. In a separate editor, the user can determine for each part of the BOM in the assembled part how it should be handled. For parts that can be reused, you can determine the location where you have stored the part until it is needed again later in production. For the defective parts, you can determine which type of reproduction should be done (automatic recutting, rough scheduling of remakes). Furthermore, it is also possible to repeat particular processings (e.g. a coating or screen printing must be washed off and reapplied). In order to use the part breakage sensibly, it is necessary that the individual components have been booked previously as "assembled" by the A+W Production Terminals.

#### 3.4.2. Reproduction

The reproduction of the broken lites can be done in different ways.

- **Automatic recutting:** these lites can be used both in the detailed scheduling as well as in the A+W Realtime Optimizer. In the detailed scheduling, they will simply be optimized with "normal" lites. In the A+W Realtime Optimizer they can be used in table optimizations (individual optimizations in cutting) or re-optimizations (filling up of the residual lite).
- **Rough scheduling remakes:** here the new item will be rescheduled with respect to processing dates, rough scheduling (batch formation) and detailed scheduling (optimization) and directed into production in new batches.

#### 3.4.3. Reject tracing and evaluations

- For all state types except "Defect" the last production state of the lite in the database is saved, so that statistical evaluations can be created via breakage location, breakage reason, glass type, etc.
- The current state of the broken lites can be displayed in the views of A+W Production.
- There is a standard report available where the breakage reason (cause), breakage location and glass type (value) can be evaluated in order to take appropriate measures to avoid breaks.
- With each breakage report, a recutting label or other papers that are helpful for reproduction can be generated automatically.
- An e-mail sending of such papers (reports) is also possible.

### 3.5. Restrictions

Not included in the A+W Breakage Manger are:
- The design of recutting labels or other papers (service in the project on request)
- The breakage of ordered glass is initially only handled in A+W Production. An automatic reordering in the ERP system is only done in A+W Enterprise starting with Version 5.4. The status type "rough scheduling remake" is compulsory. In older versions or in A+W Business, the A+W Breakage Manager only supports this process manually with papers/e-mails.
- The automatic reproduction is only supported for glass (automatic recutting). For the reproduction of frames, foils or other components, the A+W Production Terminals can assist you with appropriate displays.

### 3.6. Notes
(This section is empty in the source document.)

## 4. Contact Address

A+W Software GmbH  
Siemensstraße 3  
35463 Fernwald  
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com  
Internet: http://www.a-w.com/
