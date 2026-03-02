---
description: "A+W Harp Rack Planner Functional Specification"
---


# A+W Harp Rack Planner
---
## A+W Functional Specification

## 1. Contents

1.  **Contents**
2.  **Notes on this Document**
    2.1. Trademarks
    2.2. Copyrights
    2.3. Exclusion of liability
3.  **Performance Description**
    3.1. Data
    3.2. Description
    3.3. Requirements
    3.4. List of functions
    3.5. Limitations
    3.6. Notes
4.  **Contact Address**

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### 2.3. Exclusion of liability

A+W Software GmbH assumes no liability for data errors that rely on basic principles of the standard functions made available by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All adjustments, expansions, database queries, reports, analyses, and interface expansions that were created individually for our customers and/or machines and software partners as well as all costs and efforts associated with these were borne by the client (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary in order to ensure that the adjustments/expansions commissioned that were undertaken/developed for a version will also work perfectly and be used in the subsequent version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220008 |
| **Module** | A+W Harp Rack Planner |
| **Brief description** | The A+W Harp Rack Planner calculates the center of gravity within the framework of detailed scheduling of harp racks. |
| **Available** | Starting with A+W Production 2016 |

### 3.2. Description

The **A+W Harp Rack Planner** serves to allow the symmetrical loading of harp racks. With this loading variant, maximum weights, empty weights, length specifications, centers of gravity, and the permissible deviations of a harp rack are considered.

The module is integrated within the detailed scheduling and can be activated accordingly via the configuration. Based on the stored master data for a harp rack, the individual lites are stored symmetrically in the slots. Here, attention is paid that the harp rack's center of gravity is always in the middle (± the permissible deviation). If this restriction should be violated sometime despite free slots, a new harp rack is filled. The lites of the first harp rack are then pushed far enough to the middle that symmetry is achieved.

### 3.3. Requirements

- A+W Production (article number 220001 and 220002)
- Set-up and correct master data (storage space master or more precisely: harp racks)
- The symmetrical loading must be activated using the appropriate parameters.

### 3.4. List of functions

- When loading a harp rack, the system heeds its permissible center of gravity range and checks adherence to this after each lite loaded. For this it is constantly calculated how many slots must remain empty so that the symmetry can be achieved. It is important to note that the system does not undertake any resorting of the individual lites and units since the sequence is specified during production.
- The loading is always from one side or from the first slot. If the maximum weight of the harp rack is reached or if, for example, the first lites are so heavy that the number of slots is reached (arises from: calculated free slots + occupied slots), the lites will be shifted according to the minimum center of gravity and a new harp rack will be filled according to the same principle for the remaining lites.

### 3.5. Limitations

The loading of a harp rack is done according to a static principle, that is, that intermediate partial loadings and subsequent moving of the harp rack are not considered. Furthermore, the loading sequence calculated by the detailed scheduling is decisive, so that when unloading the harp rack, the balance is changed. Concretely this means that the desired stability can only be given at the moment of the complete loading, a moving of harp racks onto which not all lites are loaded or from which lites have already been unloaded can result in instabilities that are not covered by this module.

However, a certain "dynamic loading variant" can be achieved, for example, for a harp rack with 4 rollers calculating only 3 rollers as load carriers (e.g. also recommendation from HEGLA). Thus during intermediate movement, the risk of tipping is minimized.

The loading algorithm will not calculate an absolute balance (center of gravity precisely in the middle => 0.5) since in practice this is influenced by many parameters (imprecise lite weights, etc.). The balance in the depth of a harp rack is also not considered.

Therefore, the system cannot be a guarantee of an always fully-balanced loading. The specialized employee also bears some responsibility.

### 3.6. Notes

So that shaped lites can also be calculated with the exact weight, it is important that the corresponding ERP system transmits this information on order transfer.

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0
E-mail: info@a-w.com
Internet: http://www.a-w.com/
