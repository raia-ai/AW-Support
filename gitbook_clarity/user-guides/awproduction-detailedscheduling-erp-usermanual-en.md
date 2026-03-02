---
description: "EN_UM_AWProduction_4"
---


# Tutorial

---
## Racks and Stacking Modes

### Exercise 2: Define a harp rack

Define a rack for harp racks.

**The task**

*   **Rack type**: Harp rack
*   **Number of slots**: 99
*   **Max. number of harp racks**: 50

**Exercise 2: Solution**

The result of this exercise looks like that:

[Image: Fig. D-21 - Rack settings interface for a Harp Rack (Fächerwagen) showing fields for Slot Number Total (99), Width, Two Slots/Number, Max. No. of Harp Racks (50), etc.]

**Fig. D-21 Rack**

*   **Harp Racks**
*   **Harp Rack (Fächerwagen)**
    *   Slot Number Total: 99
    *   Width: 200 mm
    *   Two Slots/Number: Start = 0
    *   Slot Number Digits: 234
    *   Max. No. of Harp Racks: 50
    *   Check Quantity (Cutting): 0: Harp Rack
    *   Maximum Load (kg): 0
    *   Empty Weight (kg): 0
    *   Distance First/Last Slot from Axis: 0 mm
    *   Max. Deviation Center of Gravity fr. Middle (%): 0.00

### Exercise 3: Define a fixed rack

Define a fixed rack.

**The task**

*   **Rack type**: Fixed rack
*   **Stacking depth**: 1000 mm
*   **Width**: 2000 mm
*   **Max. number of fixed racks**: 99

### Exercise 3: Solution

The result of this exercise looks like that:

[Image: Fig. D-22 - Fixed rack settings interface showing fields for Stacking Depth, Width, and Max. No. of Fixed Racks.]

**Fig. D-22 Fixed rack**

*   **Fixed Racks**
*   **Fix rack (FAP)**
    *   Stacking Depth: 1000 mm
    *   Width: 2000 mm
    *   Max. No. of Fixed Racks: 99
    *   Check Quantity (Cutting)
    *   Maximum Weight (kgs): 0

**Additional information:**
*   ⇨ Tutorial, "Racks (storage locations)" on page D-262
*   ⇨ Software Reference, "Racks" on page D-394

## Optimization Modes

This subject area introduces the optimizations and tells you how to use them in A+W Production.

This subject area includes the following training sessions:
*   Overview
*   Different Optimization Modes

### Overview

**Objectives**
*   Knowing and understanding the different optimization modes.
*   Circumstances in which the individual modes are used.
*   Knowing and understanding the appropriate settings in A+W Production.

**Benefit**
Only knowing and understanding the different optimization modes will enable you to adapt A+W Production detailed scheduling to your production so that it will operate effectively and in a time-saving manner.

**Definitions**

*   **Unit**: A unit consists of two or more lites of glass which belong together because they are going to be assembled later, e.g. into IG or laminated glass.
*   **Group**: The group includes a quantity. It groups units according to certain criteria like customer number and order number.
*   **Super group**: Super groups unite different groups. This way, three groups which belong together can be treated by a set of similar rules for example. Example: Sorting onto racks because all three groups (e.g. orders) belong to the same customer or the same project.

> **Note**
> **Choosing the optimization**: When you select an optimization, you have to compromise between the optimum result (minimum waste) and the optimum production sequence with regards to assembly.

### Different Optimization Modes

When choosing the optimization you will always have to find a compromise between the best optimization result (low waste) and the best production sequence with regard to assembly.

A+W Production uses the optimization modes:
*   6.2
*   6.1
*   5.2
*   5.1
*   Free optimization

#### Optimization Mode 6.2 - Fixed Sequence

This optimization mode works with a strict sequence. Nothing can be changed; the lites are produced in a totally strict sequence. This is the sequence in which they are released for optimization.
*   The sequence of groups is fixed.
*   The sequence of lites within a group is fixed.

> **Alternating optimization items for items with unequal lites**
> Items with two or more lites of a glass type that have different geometries can be set down like normal pairs, that is, on a common stack and alternating (Lite1, Lite3, Lite1, Lite3, etc.). The desired behavior is only used for A racks for which the 6.2 mode (=fixed sequence) is set.
>
> A combination of shapes is only possible for these lites with the A+W Shape Optimizer, no longer via the detailed scheduling-internal combination of shapes!

**Under which circumstances can this mode be used?**
*   You are using A racks for optimization.
*   You have got a strict production and delivery plan.
*   You produce either by customer or glass type.
*   Your yield is (usually) poor - the result is not the main criterion however but the production in strict sequence (e.g. aligning the entire production to the truck's unloading sequence for a special customer project).
*   You have to make sure that the big lites are cut and stacked first, or you will need an additional rack for resorting.
*   You will usually need a fixed number of racks (number of groups = almost the number of physical racks).
*   You can directly optimize in production or packing sequence.

The following illustration symbolizes the effects of this mode:

[Image: A triangle diagram with vertices labeled Sequence, Yield, and Flexibility. For Mode 6.2, the emphasis is heavily on 'Sequence'.]

**Settings in A+W Production**
Optimizing in this mode requires the following settings:
Master data > Detailed scheduling > Organization > tab Production sequence > Select rack > Settings

[Image: Fig. D-23 - The Rack Settings dialog showing "Planned Optimization Mode" set to 6/2.]

**Additional information:**
*   ⇨ Tutorial, "Racks (storage locations)" on page D-262
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### Optimization Mode 6.1 - Keep Customers Together

The sequence of groups is fixed in this optimization mode, e.g. by size. The different groups can be rearranged to improve the result. A typical criterion for this would be:
*   Route | Customer

This way, the items of a customer will be produced together; you cannot define however the lites of which customer are going to be produced first.
*   The sequence of groups can be changed (X).
*   The sequence of lites within a group is fixed.

**Under which circumstances will this mode be used?**
*   You are using A racks for optimization.
*   You have got a strict production and delivery plan.
*   You produce either by customer or glass type.
*   Your yield is relatively poor (better than in mode 6.2 however) - the yield is not the main criterion however.
*   You have to make sure that the big lites are cut and stacked first, or you will need an additional rack for resorting.
*   You will usually need a fixed number of racks (number of groups = almost the number of physical racks).
*   You can directly optimize in production or packing sequence.

The following illustration symbolizes the effects of this mode:

[Image: A triangle diagram with vertices labeled Sequence, Yield, and Flexibility. For Mode 6.1, the emphasis is between 'Sequence' and 'Yield'.]

**Settings in A+W Production**
Optimizing in this mode requires the following settings:
Master data > Detailed scheduling > Organization > tab Production sequence > Select rack > Settings

[Image: Fig. D-24 - The Rack Settings dialog showing "Planned Optimization Mode" set to 6/1.]

**Additional information:**
*   ⇨ Tutorial, "Racks (storage locations)" on page D-262
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### Optimization Mode 5.2 - Standard

This optimization mode is the standard mode for detailed scheduling. The grouping and sorting key only includes the group number. This means that every item of the group has its own item number by which it can be clearly identified. This is why the elements within the groups have no fixed sequence but can be optimized freely.
*   The sequence of groups is fixed.
*   The sequence of lites within a group can be changed. Only units (e.g. for IG) will be kept together (X).

**Under which circumstances will this mode be used?**
*   If mode 5.1 is not being used.
*   If the two properties ORDER NUMBER and ITEM NUMBER are not used together in combined grouping/sorting codes.

The following illustration symbolizes the effects of this mode:

[Image: A triangle diagram with vertices labeled Sequence, Yield, and Flexibility. For Mode 5.2, the emphasis is between 'Sequence' and 'Flexibility'.]

**Settings in A+W Production**
Optimizing in this mode requires the following settings:
Master data > Detailed scheduling > Organization > tab Production sequence > Select rack > Settings

[Image: Fig. D-25 - The Rack Settings dialog showing "Planned Optimization Mode" set to 5/2.]

**Additional information:**
*   ⇨ Tutorial, "Racks (storage locations)" on page D-262
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### Optimization Mode 5.1 - IG on Harp Racks or Many A Racks

The grouping and sorting key only includes the group number. This means that every item of the group has its own item number by which it can be clearly identified. This is why the elements within the groups have no fixed sequence but can be optimized freely. This is identical with optimization mode 5.2 so far.
*   The sequence of groups can be changed (X).
*   The sequence of lites within a group can be changed.
*   Only units (e.g. for IG) will be kept together (X).

**Under which circumstances will this mode be used?**
*   You are using harp racks for optimization and you need additional A racks.
*   Your yield will be good.
*   You will have to do a lot of sorting before delivery - this requires a large number of physical racks.

The following illustration symbolizes the effects of this mode:

[Image: A triangle diagram with vertices labeled Sequence, Yield, and Flexibility. For Mode 5.1, the emphasis is between 'Yield' and 'Flexibility'.]

**Settings in A+W Production**
Optimizing in this mode requires the following settings:
Master data > Detailed scheduling > Organization > tab Production sequence > Select rack > Settings

[Image: Fig. D-26 - The Rack Settings dialog showing "Planned Optimization Mode" set to 5/1.]

**Additional information:**
*   ⇨ Tutorial, "Racks (storage locations)" on page D-262
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### Optimization Mode Free Optimization - Lites on Harp Racks

Free optimization is the standard optimization for lites on harp racks. As for manual cutting, different glass types/thicknesses can be put onto a rack (different stacks of glass) when the free optimization is used.
*   Everything is free

**Under which circumstances will this mode be used?**
*   You are using harp racks for optimization (and you need additional A racks for special glass types, e.g. for large lites).
*   Your yield will be excellent - waste is the most important parameter.
*   You will have to do a lot of sorting - this requires a large number of physical racks.

The following illustration symbolizes the effects of this mode:

[Image: A triangle diagram with vertices labeled Sequence, Yield, and Flexibility. For Free Optimization, the emphasis is heavily on 'Yield'.]

**Settings in A+W Production**
Optimizing in this mode requires the following settings:
Master data > Detailed scheduling > Organization > tab Production sequence > Select rack > Settings

[Image: Fig. D-27 - The Rack Settings dialog showing "Optimization mode Free Optimization".]

As you can see there is a correlation between Grouping and Sorting, Result and the Number of racks. The more restrictive your Grouping and Sorting, the more restrictions you will have with regard to optimization and results.
Grouping and Sorting are not the only important factors for rack allocation and production organization. The handling of lites of different sizes, glass types, shapes, etc. is as important as putting the lites onto racks.

#### Double Optimization

Free optimization allows to run a double optimization which means that different glass types can be optimized with an identical cutting plan.

> The advantage of this kind of optimization is that although free optimization is used, the lites of a unit can be stored systematically. The lites of a double optimization can be stored on a rack together with other double or free optimizations.
> **Double optimization**
> Double optimization can be used only for racks with Unit mode.

### Demos and Exercises

This section shows you how the optimization works.

**Complex exercise: Compare different detailed scheduling results together with the trainer:**

The optimization process is presented and explained.

The following dialog is explained from this point of view:
*   Dialog Detailed scheduling for batch

**Step 1: Enter test orders**
Together with the trainer, enter two test orders which include different product structures. The number of items should be 20-100 units each. You should at least enter an IG unit with toughened glass plus single float glass lites and single toughened lites (spread over several items and orders). There should be shapes, large lites, and smaller lites.

Schedule the orders. Use these two test orders plus possibly existing test/training orders in the system to create a batch (or several batches, depending on the number of test orders).

Enter the batch(es) in detailed scheduling. On tab 2 (rack load), check the result of the rack allocation in detailed scheduling. Click on the Optimization button and check the results on the cutting plan in A+W Plan Editor. What do you notice? Which data do you recognize and how can you read the rack allocation on the cutting plan? Discuss the results with the trainer.

**Step 2: Change the organization**
Close Plan Editor, select on tab 5 (Organization) another master organization and run the rack allocation again. To do this, press the Repeat button. Return to tab 2 (rack allocation). Compare the results with the first rack allocation. What are the differences? Discuss the results with the trainer.

**Step 3: Optimize the batch again**
Optimize the batch again and open the cutting plan (Plan Editor). What are the differences? Discuss the results with the trainer.
Go to tab 5 and change the master organization again by choosing your own organization (the one you have previously defined together with the trainer). Compare the results.

Change the settings for Grouping and Sorting and the Stacking mode. Check the new results of rack allocation and the optimization/the cutting plan. What are the differences? Discuss the results with the trainer.

**Step 4: Extend the organization**
Extend your own organization, e.g. by an additional glass type, or separate large shapes from small shapes.
Repeat step 3 as many times as necessary, with different settings, and compare the results each time.

## Organizations

This subject area introduces the different organization types and shows you how to use them for A+W Production.

This subject area includes the following training sessions:
*   Organization Types
*   Production Sequence
*   A+W Standard Organizations
*   Rack Organization

### Organization Types

**Objectives**
*   Knowing and understanding organization types.
*   Understanding the effects of the organizations.
*   Being able to set up organizations.

**Benefit**
For correct batch planning, you have to understand the different types of organizations. Only then will you be able to assess the effects on the actual production processes, and plan them in advance.

**Definitions**
*   **Organization**: An organization is just a set of rules to handle production.
*   **Organization group**: An organization group is a structural element of an organization for detailed definition of rules and conditions, e.g. for different glass types (toughened, laminated, IG) or for distinguishing the treatment of rectangles and shapes for a glass type (IG).

> **Note**
> *   **Different organizations**: Depending on the company's structure, different organizations can be defined.
> *   **Organization groups/rack types**: An organization consists of one or more organization groups which again consist of one or more rack types.
> *   **Production sequence**: The production sequence within an organization is defined by the sequence of organization groups.

### General

A+W Production offers so-called Organizations for the correct and efficient scheduling of batches. An organization is a set of technical rules for handling the production processes (with regard to production processes, process chains and rack management). Depending on the company's structure, any number of organizations (toughened glass organization, IG organization, processing organization, etc.) can be defined. The individual organizations organize the racks for the production steps (IG line, furnace, etc.).

### Tree Structure

To create the required production sequence, A+W Production assigns a so-called master organization to every batch. A master organization is a set of organizations, consisting of one or more organizations. Several master organizations can be defined for a company. In this case, detailed scheduling will assign to the batch the master organization that comes closest to the product mix.

A master organization must contain just one standard organization (application). Of all other organization types, a master organization must contain just one. An organization consists of one or more organization groups which again consists of one or more rack types. Also, you can define the required production sequence for the organization groups and rack types.

**Master organization**
*   Organization 1
*   Organization 2
    *   Organization group 1
    *   Organization group 2
        *   Rack type 1
            *   Condition 1
        *   Rack type 2
            *   Condition 2
    *   Organization group 3

[Image: Fig. D-28 - A practical example of a master organization tree structure in the A+W software interface.]

### Master organization

Each master organization contains a standard application organization. Moreover, application and production organizations can be created for every lot type.

When an element shall be allocated to an organization, detailed scheduling first checks whether there is a production organization for the batch type in question (in this case, 300). If no production organization is found, detailed scheduling will search for a standard production organization. In our example, there is none. This means that no production organization will be allocated. Next, detailed scheduling searches for the application organization allocated to this batch type. If none if found, the element will get the standard application organization. The required application organization (300) is available and will be allocated to the element.

[Image: Fig. D-29 and Fig. D-30 - Diagram showing the logic of allocating an element to an organization based on its batch type.]

*   **A** Master organization
*   **B** Standard application organization (blue)
*   **C** Productions organization (yellow) for batch type 700
*   **D** Application organization (blue) for batch type 700
*   **E** Element, batch type 300 or 700

A production and an application organization are found for the element of lot type 700. It will be allocated to two different organizations, with different rack types (application and production rack).

You can of course define a standard production organization to be allocated to all elements for which no standard production organization is found that matches the batch type. In contrast to the application organization, you do not need to define in the production organization a buffer rack for elements that do not fulfil the conditions of another rack of this organization. If no suitable rack is found for an element in the production organization, the production organization allocation will be simply ignored. This means that to allocate production organizations to certain batch types, a buffer rack should be defined in the organization to prevent that the allocation of individual elements is ignored.

The corresponding settings are made in the **Organization** dialog:
`Master data > Detailed scheduling > Organization`

[Image: Fig. D-31 - The Master organization settings dialog.]

#### How to set up a master organization

1.  Go to `Master data > Detailed scheduling > Organization`.
2.  Press the **[New]** button. The dialog Master organization appears.
3.  Enter the name for this master organization in field **Name of master organization**.
4.  Tick or untick the checkbox **XOPT - stack together**.
5.  Tick or untick the checkbox **Quick organization**.
6.  In combo box **Production groups**, select the required group.
7.  Select the required series in combo box **Pseudo series**.
8.  For pseudo series, enter a minimum quantity in field **Minimum quantity**.
9.  If your system has been extended or adjusted by means of a special script you can select this script in field **Used script**.
10. The **Filler** button can be used for selecting defined filler conditions.
11. Edit the field **Quasi elements**. To view all existing quasi elements, use button **[...]**.
12. Tick or untick the checkbox **Use filler**. If the checkbox is ticked, the fields **Start of filler** and **End of filler** must be edited!
13. Tick or untick the checkbox **Use residue plates**. If the checkbox is ticked, the fields **Start of residue plate** and **End of residue plate** must be edited!
14. Tick or untick the checkbox **Double optimizations together**.
15. Tick or untick the checkbox **Use breakage**. If the checkbox is ticked, the fields **Start of breakage** and **End of breakage** must be edited!
16. Press **OK**. The new master organization automatically appears in the organization dialog.

#### How to add an existing, new organization to a master organization

1.  Go to `Master data > Detailed scheduling > Organization`. Tab **Master organization** shows all existing master organizations.
2.  Select the master organization to which you want to add a new organization.
3.  The bottom right window shows all existing organizations. Select the organization to add to the master organization.
4.  Press the **[New]** button. The new organization is shown below the master organization.

#### How to set up a new organization

1.  Go to `Master data > Detailed scheduling > Organization`.
2.  Open the tab **Production sequence**.
    [Image: The Orga-Dialog showing the Production Sequence tab.]
3.  Press the **[New]** button. The new organization is shown below the last organization. This will be called `unknown / ...` at first.
4.  Select this organization and use the button **[Settings]**. The dialog organization appears.
    [Image: The Organization settings dialog.]
5.  In field **Name of organization type**, change the name from `unknown` to a characteristic name.
6.  In combo box **Type**, select the required organization type.
7.  Tick the appropriate checkbox in section **Stacking mode**.
8.  If applicable, edit the fields in section **Do not split ... if rack load is over**.
9.  Press **[OK]** to close the dialog.

#### How to add a new organization group to an organization

1.  Go to `Master data > Detailed scheduling > Organization`.
2.  Open the tab **Production sequence**.
3.  Select the organization to which a new organization group shall be added, then press the button **[New]**. The new organization group appears below the selected organization; it is called `noname`.
4.  Select the organization group called `noname` then press button **[Settings]**. The dialog organization groups appears.
5.  In field **Name**, enter a characteristic name for this Organization group.
6.  Select the required group from combo box **Group formation**.
7.  Tick or untick the checkbox **Sorting of groups**.
8.  Select the required sorting from combo box **Sorting of groups**.
9.  Press **[OK]** to close the dialog.

**Additional information**
*   ⇨ Tutorial, "Organizations" on page D-316
*   ⇨ Software Reference, "Organization" on page D-379
*   ⇨ Software Reference, "Organization Groups" on page D-381

#### How to define the grouping and sorting for a rack

1.  Go to `Master data > Detailed scheduling > Organization`.
2.  Open the tab **Production sequence**.
3.  Select the organization group for which a rack shall be defined, then press button **[New]**. The system automatically creates a rack called `unknown`.
4.  Select the rack called `unknown` then press button **[Settings]**. The dialog **Rack settings** appears.
    [Image: The Rack Settings dialog.]
5.  In field **Name**, replace `unknown` by a characteristic name for this rack.
6.  In combo box **Group formation**, define the rules for creating groups (e.g. by customer number and order number).
7.  Tick or untick the checkbox **Sorting of groups**.
8.  In combo box **Group stacking mode**, define the stacking mode for the groups, per stack.
9.  Go to combo box **Optimization behavior** and define whether the sequence of groups shall be sorted or unsorted (super groups) or if nothing shall be sorted (sequence of groups unsorted and sheets within the groups unsorted).
10. Tick or untick the checkbox **Buffer rack** (this is where all the lites go which are not allocated by means of rules to special racks). Each organization should include at least one buffer rack.
11. If this rack is an application rack, make the following settings in tab **Application**:
    *   Edit the fields **From To**.
    *   Tick the appropriate checkbox in section **Stacking mode**.
    *   Tick or untick the checkbox **Cycle optimization**.
    *   Edit the field **Max. number of groups**.
    *   Edit the field **Cycle size**.
    *   Tick the appropriate checkbox in section **Rack type**.
12. If this rack is a production rack, make the following settings in tab **Production**:
    *   Edit the fields **From To**.
    *   Tick or untick the checkbox **Create production racks**.
    *   Edit the field **Max. number of groups**.
    *   Tick the appropriate checkbox in section **Rack type**.
13. Press **[OK]** to close the dialog.

### Reject Organization

This reject organization is used to put breakage onto racks according to freely definable criteria. Based on the programmed, internal conditions, the reject organization automatically checks the properties of the broken lite (i.e. float). Like all other organizations, reject organizations are defined in the organization dialog.

### Sequence of Checks

Within an organization, racks are created for which conditions are defined. These conditions define the allocation of a lite to a certain rack. The sequence of rack types normally starts with the most restrictive conditions, using the checking sequence of the rack types as a filter for the lites.

[Image: Fig. D-32 - A diagram showing a part being checked against conditions for Rack type 1, then Rack type 2, and so on, down to Rack type 5.]

Special cases will be checked first. It is therefore possible to allocate the condition `Shape` to the rack that comes first in the checking sequence. All shapes would be allocated to this rack type. With the condition `Small lites`, the second rack type would get all lites up to a defined size, etc. The further down in the check sequence a rack type is, the weaker the conditions.

If no rack type is found for an element in an application organization, it will be allocated to the buffer rack. A buffer rack either has no conditions at all, and thus stands at the end of the checking sequence, or the code **Buffer rack** is set (we recommend defining a buffer rack for every organization group by default, no matter if a production or organization application organization is used. You should also set the code for the buffer rack by default).

Each organization group must have maximally one buffer rack; for application organizations, it is mandatory.

#### How to change the sequence of checks

1.  Go to `Master data > Detailed scheduling > Organization`.
2.  Open tab **Sequence of checks**.
3.  In section **organizations**, select the organization for which you want to change the sequence of checks.
4.  In section **Racks**, choose the rack the sequence of which shall be changed.
5.  Shift the sequence of checks for the tagged rack by means of the buttons **[Start]**, **[Up]**, **[Down]** or **[End]** until the rack has reached the required position.

[Image: The Orga-Dialog showing the Test Sequence tab where the order of racks can be changed.]

### Organization Type and Lot Type

Each element and processing has its own element type or processing type (basic glass, toughened glass, etc.), and its supply type (ordered, cutting, etc.). Depending on these two properties, the element or processing is allocated to a certain batch type. This way, elements with different processing types can be allocated to the same batch type, to be treated together, e.g. at rack allocation.

Apart from that, each organization has a certain organization type which defines the elements to be allocated to the organization. Ideally, definition and filters are based on differences and similarities:
*   Shapes?, Rectangles?
*   Height?, Weight?
*   ...

Production batches are created at cutting for different element types and different glass types.

#### Application and Production Organizations

Apart from the organization type, organizations are distinguished by their being used in production organizations and application organizations. Application organizations must be created while production organizations can be created additionally. Each element gets an application organization anyway, plus an additional production organization if required.

An application rack will always be defined for a utilization organization. A production rack can be defined additionally.

For production organizations, only production racks can be defined. In the application organization, the conditions for distributing the lites to application and production racks are the same. Allocating a product for the same processing step to both an application and a production organization allows to distribute the lites to application and production racks according to different conditions. The lites on the application racks for instance can be sorted by size, and can be distributed after production (e.g. for toughened glass, after the furnace) to production racks depending on whether they will be used for IG, or will be shipped.

If a production organization is allocated to an element for a certain processing, the groups and sorting on the application organization/racks will be ignored. After processing, the element will be put onto racks depending on the groups and sorting of the production rack (production organization).

**Additional information**
*   ⇨ Software Reference, "Production" on page D-379

#### Global Settings

The global settings are connected with the values selected in the dialogs and fields mentioned below:
*   **Dialog organization groups:**
    *   Fields: **Formation of groups, sorting within groups.**
*   **Dialog Rack settings:**
    *   Fields: **Formation of groups, sorting within groups.**

When you select in the above dialogs the value **None** for the corresponding fields, the global settings will be used.

> **Default settings**
> These entries should be made to avoid error messages at the start of A+W Production.

**Additional information**
*   ⇨ Software Reference, "Default Settings" on page D-387
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383
*   ⇨ Tutorial, “A+W Standard Organizations" on page D-333

### Demos and Exercises

Open the master data of detailed scheduling. Check out with the trainer already predefined in Orgas. Analyze the structure (tree structure, different racks, allocation of conditions). What do you notice?
Discuss the structure with your trainer.

### Production Sequence

**Objectives**
*   Knowing and understanding the production sequence.
*   Understanding the effects of the production sequence.

**Benefit**
Due to your knowledge of the possible settings in organization groups with regard to grouping and sorting, you can define the actual production sequence of batches and individual lites, and change it flexibly at any time.

**Definitions**
*   **Grouping key**: The grouping key for an organization group allows defining the production sequence without fixing a grouping/sorting for the racks.

> **Note**
> *   **No grouping**: If no grouping is defined for the organization group, the production sequence depends on the sequence of racks within the organization group.
> *   **Including grouping**: If for instance, the organization group is grouped by customer, the production sequence is no longer defined by the sequence of rack types within the organization group. The main criterion is the element property `CustDrNr`.

### General

The production sequence within an organization is defined by the sequence of organization groups. This again is defined by the sequence of rack types. The sequence within the rack types is defined by group and sorting keys.

To avoid having to define the same sorting for each rack type within an organization group, you can define the sorting per organization group. This is passed on to the rack types included in the organization group, and can be completed if necessary.

The same applies to the group that can be defined for the organization group. This is also passed on to the rack types, and can be completed if required. However, the grouping of an organization group has a major impact on the production sequence. If the organization group is grouped by `Route` for instance, the production sequence is no longer defined simply by the sequence of rack types within the organization group. The main criterion is the element property `Route`. This means that all elements of Route A will be produced first, followed by the elements of Route B, etc. For a given route, however, the sequence of rack types within the organization group is decisive. An exception however is if on a rack type within the organization group, the sequence of groups is random. If the optimization could put them in a random sequence, the grouping defined for this organization group could no longer determine the sequence of groups. In this case, the sequence is defined by the sequence of rack types; the grouping of the organization group will be passed on to the rack types involved.

### Grouping Key for Organization Groups

The grouping key defined for an organization group has a major influence on the production sequence. It allows to define the production sequence without fixing a grouping/sorting for the racks.

#### No grouping

If no grouping is defined for the organization group, the production sequence depends on the sequence of racks within the organization group (e.g. small lites, muntins, etc.).

[Image: Fig. D-33 - Diagram showing a production sequence flowing through different racks within one organization group.]

#### Including Grouping

If for instance, the organization group is grouped by customer, the production sequence is no longer defined by the sequence of rack types within the organization group. The main criterion is the element property `Customer`. In this example, this would mean that first, all lites for customer A will be produced, then for customer B, etc. For the customer itself, the production sequence depends on the sequence of racks within the organization group.

Within the groups, the element sequence is free, i.e. there are no restrictions regarding the optimization (XOPTS 5.2).

[Image: Fig. D-34 - Diagram showing production sequence grouped by Customer A and Customer B, each flowing through Rack type A and Rack type B.]

> **Defining the production sequence by means of the grouping key**
> To define the production sequence by means of the grouping key for the organization group, you must not set "sort by order and item number" for the racks. If this is done, optimization mode 6.1 will be used for optimization, and the grouping key for the organization group will be ignored.

### A+W Standard Organizations

**Objectives**
*   Knowing and understanding different standard organizations.
*   Being able to understand the corresponding settings in A+W Production.

**Benefit**
The advantage of standard organizations is that they have been defined before and can be used right away. This saves time and minimizes the risk of set-up errors.

**Definitions**
*   **Standard organization**: Organizations predefined by A+W.

> **Note**
> **In case of changes**: we recommend to copy the required standard organization and change the copied version. This way, the original version is still available and the risk of errors is kept low.

### Rack Organization

A+W Production offers a number of standard organizations for glass production. Every organization uses special sorting and grouping criteria for the lites, and will optimize production according to the individual requirements.

The table below gives an overview of the available organizations and their features. The sequence ranges from production-oriented, up to dispatch-oriented organization.

| Name | Description |
| --- | --- |
| **A Racks AIR** | This organization will be useful for benders with very strict AIR restrictions, which have no buffer to pre-produce and sort the spacers. This organization does not consider dispatch requirements. |
| **A Racks** | This organization provides a moderately dispatch-organized production sequence by customer and order, but is restricted as to the number of racks that can be used before the line. The degree of dispatch organization can be controlled by the global settings for classification and sorting. With this organization, repacking will be called for after IG production. |
| **A Racks Dispatch** | This organization offers a dispatch-oriented production sequence; several A racks will be used alternately before the line. The organization needs racks before and behind the line, and produces the lites in packing sequence. Racks for the individual customers have to be provided after the line. |
| **Harp racks** | Structure and rack allocation of this organization are similar to the A rack organization but mainly uses harp racks; this will generally improve the yield. Big and small units as well as series will be put onto A racks. |
| **Filled harp racks** | Unlike the A rack organization, the lites are produced in dispatch sequence. Even if the harp rack organization handles one rack after the other in front of the line, the required glass types can be put onto harp rack, in dispatch sequence. This organization makes sure that there are no half-filled harp racks; it sorts all harp racks in production sequence. The harp racks will be handled first, followed by the A racks containing the specialities. |

#### A Racks AIR

This organization is useful for IG producers using benders with very strict AIR restrictions, which have no buffer to pre-produce and sort the spacers.

The organization `A racks AIR` sorts the production sequence by AIR, taking the units from A racks in front of the line in consecutive order.
*   This organization does not consider dispatch requirements.
*   Only A racks will be used (200 mm in depth and 2000 mm in width).
*   The stacking mode is **Unit** (lites of a unit being put onto the same rack, on different stacks).

**Production sequence**
The production sequence is created from the following, optimized rack groups (in production sequence):
*   Common IG lites
*   IG shapes
*   IG lites with muntins
*   IG shapes with muntins
*   Stepped IG
*   Triple IG

Each of these groups consists of five air rack groups, to be produced one after the other. The AIR groups are separated by adjustable threshold values:
*   **AIR group 1** > AIR threshold 1
*   **AIR group 2** > AIR threshold 2
*   **AIR group 3** > AIR threshold 3
*   **AIR group 4** > AIR threshold 4
*   **AIR group 5**

The threshold values are preset (see below) and can be adjusted:
*   AIR threshold 1 = 10 mm
*   AIR threshold 2 = 12 mm
*   AIR threshold 3 = 16 mm
*   AIR threshold 4 = 18 mm

Each AIR rack group includes the following racks, in production sequence (small to big because the lites need to be repacked after the line):
*   Series (series flag set or quantity ≥ 10)
*   Small units, condition *small unit*, default setting:
    *   short edge < 300 or
    *   long edge < 500)
*   Common units
*   Large units, condition *large unit*, default setting:
    *   long edge > 2100 or
    *   short edge > 1600)

The production sequence on each rack is grouped by customer and order. The sequence of items within the order is free (freedom of optimization). With the exception of serial racks, a rack may accommodate several customers and orders. Series will be stacked separately, per item.

There are buffer racks for the lites which do not match any of the above rack groups; these racks will not be optimized however. There are:
*   Toughened glass lites
*   Laminated glass lites
*   Non-allocated lites

**Optimization**
This organization can be optimized by XOPTS mode **5/1** or higher. This depends on the amount of sorting the IG producer is willing to invest, and on the optimization result.
The stricter the restrictions for an A rack, the higher the waste that is likely to occur.
The drawbacks of this organization are that on the one hand, it might use very many racks while on the other hand, much sorting will be required after production.

**Number ranges**
The organization will allocate the lites to the racks. The following racks and number areas have been defined for this purpose:

**Tab. D-2: Number ranges for production organization A racks spacers**
| Organization group | Rack | Number range from | to |
| --- | --- | --- | --- |
| Buffer | Buffer | 10000 | 10999 |
| Toughened - processed | processed - series | 8951 | 8999 |
| Toughened - processed | processed - large lites | 8921 | 8950 |
| TG - processed | processed - small lites | 8901 | 8920 |
| TG - processed | processed | 8501 | 8899 |
| TG - arrissed | Arrissed - large lites | 8421 | 8450 |
| TG - arrissed | Arrissed - small lites | 8401 | 8420 |
| TG - arrissed | Arrissed | 8001 | 8399 |
| TG - arrissed | Arrissed series | 8451 | 8499 |
| Single annealed | large lites | 7921 | 7950 |
| Single annealed | small lites | 7901 | 7920 |
| Single glass | Single | 7501 | 7899 |
| Single glass | Series | 7951 | 7999 |
| Single glass - bevelled | bevelled - series | 7451 | 7499 |
| Single glass - bevelled | bevelled - large lites | 7421 | 7450 |
| Single glass - bevelled | bevelled - small lites | 7401 | 7420 |
| Single glass - bevelled | Single - bevelled | 7001 | 7399 |
| IG triple | IG triple - large units | 6921 | 6950 |
| IG triple | IG triple | 6001 | 6899 |
| IG triple | IG triple - small units | 6901 | 6920 |
| IG triple | IG triple - series | 6951 | 6999 |
| IG - shape-muntins - airsz1 | IG-1 - shp-mun - small | 1311 | 1320 |
| IG - shape-muntins - airsz1 | IG-1 - shp-mun - series | 1351 | 1399 |
| IG - shape-muntins - airsz1 | IG-1 - shp-mun | 1901 | 1950 |
| IG - shape-muntins - airsz1 | IG-1 - shp-mun - large | 1321 | 1350 |
| IG - shape-muntins - airsz2 | IG-2 - shp-mun - large | 2321 | 2350 |
| IG - shape muntins - airsz2 | IG-2 - shp-mun - small | 2311 | 2320 |
| IG - shape-muntins - airsz2 | IG-2 - shp-mun - series | 2351 | 2399 |
| IG - shape-muntins - airsz2 | IG-2 - shp-mun | 2901 | 2950 |
| IG - shape-muntins - airsz3 | IG-3 - shp-mun - large | 3321 | 3350 |
| IG - shape-muntins - airsz3 | IG-3 - shp-mun | 3901 | 3950 |
| IG - shape-muntins - airsz3 | IG-3 - shp-mun - small | 3311 | 3320 |
| IG - shape-muntins - airsz3 | IG-3 - shp-mun - series | 3351 | 3399 |
| IG - shape-muntins - airsz4 | IG-4 - shp-mun - series | 4351 | 4399 |
| IG - shape-muntins - airsz4 | IG-4 - shp-mun | 4901 | 4950 |
| IG - shape-muntins - airsz4 | IG-4 - shp-mun - small | 4311 | 4320 |
| IG - shape-muntins - airsz4 | IG-4 - shp-mun - large | 4321 | 4350 |
| IG - shape-muntins - airsz5 | IG-5 - shp-mun - series | 5351 | 5399 |
| IG - shape-muntins - airsz5 | IG-5 - shp-mun - small | 5311 | 5320 |
| IG - shape-muntins - airsz5 | IG-5 - shp-mun | 5901 | 5950 |
| IG - shape-muntins - airsz5 | IG-5 - shp-mun - large | 5321 | 5350 |
| IG - shapes - airsz1 | IG-1 - shapes - unsealed | 1241 | 1250 |
| IG - shapes - airsz1 | IG-1 - shapes | 1701 | 1799 |
| IG - shapes - airsz1 | IG-1 - shapes - small units | 1211 | 1220 |
| IG - shapes - airsz1 | IG-1 - shapes - large units | 1221 | 1240 |
| IG - shapes - airsz1 | IG-1 - shapes - series | 1251 | 1299 |
| IG - shapes - airsz2 | IG-2 - shapes - small units | 2211 | 2220 |
| IG - shapes - airsz2 | IG-2 - shapes - series | 2251 | 2299 |
| IG - shapes - airsz2 | IG-2 - shapes | 2701 | 2799 |
| IG - shapes - airsz2 | IG-2 - shapes - large units | 2221 | 2240 |
| IG - shapes - airsz2 | IG-2 - shapes - unsealed | 2241 | 2250 |
| IG - shapes - airsz3 | IG-3 - shapes - large units | 3221 | 3240 |
| IG - shapes - airsz3 | IG-3 - shapes - unsealed | 3241 | 3250 |
| IG - shapes - airsz3 | IG-3 - shapes - small units | 3211 | 3220 |
| IG - shapes - airsz3 | IG-3 - shapes - series | 3251 | 3299 |
| IG - shapes - airsz3 | IG-3 - shapes | 3701 | 3710 |
| IG - shapes - airsz4 | IG-4 - shapes | 4701 | 4799 |
| IG - shapes - airsz4 | IG-4 - shapes - large units | 4221 | 4240 |
| IG - shapes - airsz4 | IG-4 - shapes - unsealed | 4241 | 4250 |
| IG - shapes - airsz4 | IG-4 - shapes - series | 4251 | 4299 |
| IG - shapes - airsz4 | IG-4 - shapes - small units | 4211 | 4220 |
| IG - shapes - airsz5 | IG-5 - shapes - series | 5251 | 5299 |
| IG - shapes - airsz5 | IG-5 - shapes - unsealed | 5241 | 5250 |
| IG - shapes - airsz5 | IG-5 - Shapes - large units | 5221 | 5240 |
| IG - shapes - airsz5 | IG-5 - shapes - small units | 5211 | 5220 |
| IG - shapes - airsz5 | IG-5 - shapes | 5701 | 5799 |
| IG - muntins - airsz1 | IG-1 - muntins - series | 1451 | 1499 |
| IG - muntins - airsz1 | IG-1 - muntins - small | 1411 | 1420 |
| IG - muntins - airsz1 | IG-1 - muntins | 1801 | 1899 |
| IG - muntins - airsz1 | IG-1 - muntins - large | 1421 | 1450 |
| IG - muntins - airsz2 | IG-2 - muntins - small | 2411 | 2420 |
| IG - muntins - airsz2 | IG-2 - muntins - large | 2421 | 2450 |
| IG - muntins - airsz2 | IG-2 - muntins | 2801 | 2899 |
| IG - muntins - airsz2 | IG-2 - muntins - series | 2451 | 2499 |
| IG - muntins - airsz3 | IG-3 - muntins - large | 3421 | 3450 |
| IG - muntins - airsz3 | IG-3 - muntins - small | 3411 | 3420 |
| IG - muntins - airsz3 | IG-3 - muntins - series | 3451 | 3499 |
| IG - muntins - airsz3 | IG-2 - muntins | 3801 | 3899 |
| IG - muntins - airsz4 | IG-4 - muntins - small | 4411 | 4420 |
| IG - muntins - airsz4 | IG-4 - muntins - series | 4451 | 4499 |
| IG - muntins - airsz4 | IG-4 - muntins | 4801 | 4899 |
| IG - muntins - airsz4 | IG-4 - muntins - large | 4421 | 4450 |
| IG - muntins - airsz5 | IG-5 - muntins | 5801 | 5899 |
| IG - muntins - airsz5 | IG-5 - muntins - large | 5421 | 5450 |
| IG - muntins - airsz5 | IG-5 - muntins - series | 5451 | 5499 |
| IG - muntins - airsz5 | IG-5 - muntins - small | 5411 | 5420 |
| IG - stepped - airsz1 | IG-1 - stepped | 1951 | 1999 |
| IG - stepped - airsz1 | IG -1 - stepped - large units | 1521 | 1550 |
| IG - stepped - airsz1 | IG -1 - stepped - small units | 1511 | 1520 |
| IG - stepped - airsz1 | IG-1 - stepped - series | 1551 | 1599 |
| IG - stepped - airsz2 | IG-2 - stepped | 2951 | 2999 |
| IG - stepped - airsz2 | IG -2 - stepped - large units | 2521 | 2550 |
| IG - stepped - airsz2 | IG -2 - stepped - series | 2551 | 2599 |
| IG - stepped - airsz2 | IG -2 - stepped - small units | 2511 | 2520 |
| IG - stepped - airsz3 | IG -3 - stepped - small units | 3511 | 3520 |
| IG - stepped - airsz3 | IG-3 - stepped | 3951 | 3999 |
| IG - stepped - airsz3 | IG -3 - stepped - large units | 3521 | 3550 |
| IG - stepped - airsz3 | IG-3 - stepped - series | 3551 | 3599 |
| IG - stepped - airsz4 | IG-4 - stepped | 4951 | 4999 |
| IG - stepped - airsz4 | IG-4 - stepped - series | 4551 | 4599 |
| IG - stepped - airsz4 | IG -4 - stepped - large units | 4521 | 4550 |
| IG - stepped - airsz4 | IG -4 - stepped - small units | 4511 | 4520 |
| IG - stepped - airsz5 | IG-5 - stepped | 5951 | 5999 |
| IG - stepped - airsz5 | IG -5 - stepped - large units | 5521 | 5550 |
| IG - stepped - airsz5 | IG -5 - stepped - small units | 5511 | 5520 |
| IG - stepped - airsz5 | IG-5 - stepped - series | 5551 | 5599 |
| IG-airsz1 | IG-1 small units | 1111 | 1120 |
| IG-airsz1 | IG-1 | 1601 | 1699 |
| IG-airsz1 | IG-1 - large units | 1121 | 1150 |
| IG-airsz1 | IG-1 - series | 1151 | 1199 |
| IG-airsz2 | IG-2 - large units | 2121 | 2150 |
| IG-airsz2 | IG-2 - small units | 2111 | 2120 |
| IG-airsz2 | IG-2 | 2601 | 2699 |
| IG-airsz2 | IG-2 - series | 2151 | 2199 |
| IG-airsz3 | IG-3 | 3601 | 3699 |
| IG-airsz3 | IG-3- small units | 3111 | 3120 |
| IG-airsz3 | IG-3 - series | 3151 | 3199 |
| IG-airsz3 | IG-3 - large units | 3121 | 3150 |
| IG-airsz4 | IG-4 - small units | 4111 | 4120 |
| IG-airsz4 | IG-4 | 4601 | 4699 |
| IG-airsz4 | IG-4 - large units | 4121 | 4150 |
| IG-airsz4 | IG-4 - series | 4151 | 4199 |
| IG-airsz5 | IG-5 - large units | 5121 | 5150 |
| IG-airsz5 | IG-5 - small units | 5111 | 5120 |
| IG-airsz5 | IG-5 - series | 5151 | 5199 |
| IG-airsz5 | IG-5 | 5601 | 5699 |
| LAMI | LAMI - large lites | 9921 | 9950 |
| LAMI | LAMI - series | 9951 | 9990 |
| LAMI | LAMI | 9001 | 9899 |
| LAMI | LAMI - small lites | 9901 | 9920 |

The organization **A racks AIR** uses units for optimization. It is easy to handle but causes more sorting work after the line, plus you will need more space for racks.

[Image: Photo of a glass production line with A-racks.]

**Settings in A+W Production**
The following dialogs show the appropriate settings in A+W Production for **IG-AIRSZ1**.

**Settings for the organization group:**

[Image: Fig. D-35 - The Organization Groups settings dialog showing settings for IG (ISO) high volumes.]

**Rack settings:**

[Image: Fig. D-36 - The Rack settings dialog for IG high volumes.]

**Additional information**
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### IG A racks

The A rack organization supplies a moderately dispatch-oriented production sequence by customer and order. The only restriction is that just a few racks can be used in front of the line. The degree of dispatch organization can be controlled by the global settings for classification and sorting.

With this organization, repacking will be called for after IG production.
*   Only A racks will be used (200 mm in depth and 2000 mm in width).
*   The stacking mode is "unit".

**Production sequence**
The production sequence consists of the following rack groups (in production sequence):
*   Common IG lites
*   IG shapes
*   IG shapes with muntins
*   IG lites with muntins
*   Stepped IG
*   Triple IG

These rack groups are split into (in production sequence):
*   Series (series flag set or quantity ≥ 10)
*   Small units, condition *small unit*, default setting:
    *   short edge < 300 or
    *   long edge < 500)
*   Common units
*   Large units, condition *large unit*, default setting:
    *   long edge > 2100 or
    *   short edge > 1600)

Because repacking is required after the line, the sequence runs from small to large.

Lites that do not fit one of the above rack groups; will be stacked on buffer racks which will not be optimized, however. There are:
*   Toughened glass lites
*   Laminated glass lites
*   Non-allocated lites

**Grouping and sorting**
Grouping and sorting of the lites on each rack depends on the general settings for grouping and sorting.
With the exception of serial racks, most of the A racks will accommodate several customers and orders. Series will be stacked separately, per item.

**Default**
The global sorting parameters are set as follows:
*   Grouping = customer+order
*   Sorting = none

This means that customer orders will be kept together on the above racks (e.g. common IG - small units). This requires that combinations of different glass types are united in front of the line (i.e. taken from different racks). The sequence of items within the order is free (freedom of optimization).

**Changing the setting**
If there is only little space in front of the line, the global settings can be changed:
*   Grouping = article+customer+order
*   Sorting = none

The additional product code makes sure that on the racks, one glass combination will be processed after the other. As a result, only the individual glass combinations will be produced in dispatch order. The product mix thus determines the degree of dispatch-orientation.

**Optimization**
This organization can be optimized by XOPTS mode **5/1** or higher. This depends on the amount of sorting the IG producer is willing to invest, and on the optimization result.
The stricter the restrictions for an A rack, the higher the waste that is likely to occur.

**Number ranges**
The organization will allocate the lites to the racks. The following racks and number areas have been defined for this purpose:

**Tab. D-3: Number ranges for production organization A racks**
| Organization group | Storage location | Number range from | to |
| --- | --- | --- | --- |
| Buffer | Buffer | 10000 | 10999 |
| TG - processed | processed | 8501 | 8899 |
| TG - processed | processed - small lites | 8901 | 8920 |
| TG - processed | processed - large lites | 8921 | 8950 |
| TG - processed | processed - series | 8951 | 8999 |
| TG - arrissed | arrissed | 8001 | 8399 |
| TG - arrissed | arrissed - large lites | 8421 | 8450 |
| TG - arrissed | arrissed - series | 8451 | 8499 |
| TG - arrissed | arrissed - small lites | 8401 | 8420 |
| Single glass | Series | 7951 | 7999 |
| Single glass | Single | 7501 | 7899 |
| Single glass | large lites | 7921 | 7950 |
| Single glass | small lites | 7901 | 7920 |
| Single annealed - bevelled | bevelled - small lites | 7401 | 7420 |
| Single annealed - bevelled | bevelled - large lites | 7421 | 7450 |
| Single annealed - bevelled | bevelled - series | 7451 | 7499 |
| Single annealed - bevelled | Single - bevelled | 7001 | 7399 |
| IG | IG | 1001 | 1899 |
| IG | IG - small units | 1901 | 1920 |
| IG | IG - series | 1951 | 1999 |
| IG | IG - large units | 1921 | 1950 |
| IG triple | IG triple | 6001 | 6899 |
| IG - triple | IG - triple - small units | 6901 | 6920 |
| IG - triple | IG - triple - series | 6951 | 6999 |
| IG - triple | IG - triple - large units | 6921 | 6950 |
| IG - shapes | IG - shapes - series | 2951 | 2999 |
| IG - shapes | IG - shapes - small units | 2901 | 2920 |
| IG - shapes | IG shapes | 2001 | 2899 |
| IG - shapes | IG - shapes - large units | 2921 | 2940 |
| IG - shapes | IG - shapes - unsealed | 2941 | 2950 |
| IG - shapes - muntins | IG - shapes - muntins - series | 3951 | 3999 |
| IG - shapes - muntins | IG - shapes - muntins - small | 3901 | 3920 |
| IG - shapes - muntins | IG - shapes - muntins | 3001 | 3899 |
| IG - shapes - muntins | IG - shapes - muntins - large | 3921 | 3950 |
| IG - muntins | IG - muntins - small units | 4901 | 4920 |
| IG - muntins | IG - muntins | 4001 | 4899 |
| IG - muntins | IG - muntins - large units | 4921 | 4950 |
| IG - muntins | IG - muntins - series | 4951 | 4999 |
| IG - stepped | IG - stepped - small units | 5901 | 5920 |
| IG - stepped | IG - stepped | 5001 | 5899 |
| IG - stepped | IG - stepped - large units | 5921 | 5950 |
| IG - stepped | IG - stepped - series | 5951 | 5999 |
| LAMI | LAMI - series | 9951 | 9990 |
| LAMI | LAMI - large lites | 9921 | 9950 |
| LAMI | LAMI | 9001 | 9899 |
| Laminated glass | LAMI - small lites | 9901 | 9920 |

The A rack organization optimizes in a more dispatch-oriented way. Less sorting is required at the end of the line which is why less space for racks is needed.

[Image: Photo of a glass production line.]

**Settings in A+W Production**
The following dialogs show the appropriate settings in A+W Production for **IG - small units**

**Settings for the organization group:**

[Image: Fig. D-37 - The Organization Groups settings dialog.]

**Rack settings:**

[Image: Fig. D-38 - The Rack settings dialog for IG small units.]

**Additional information**
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### A Racks Dispatch

The A rack dispatch organization produces a dispatch-oriented production sequence; several A racks will be used alternately before the line.

The arrangement of the rack groups is based on size categories which are sorted by customer. The target is to achieve a production sequence which runs from large to small (taking into account certain deviations in size); inside each category, the customer orders are kept together, to be sorted onto transport racks at the end of the line.

The organization needs racks before and behind the line, and produces the lites in packing sequence. Racks for the individual customers have to be provided after the line.
*   Only A racks will be used (200 mm in depth and 2000 mm in width).
*   The stacking mode is **Glass**.

**Size Categories**
To classify lites by size, this organization uses two threshold values (S1 and S2 in the chart).

[Image: Fig. D-39 - A graph showing size categories based on short edge (A) and long edge (B) with thresholds S1 and S2.]

Since the organization will always search for and check the short edge, only the section below the diagonal (see graph) is important. The size categories are:
*   **Size category 1**: short edge > Si_threshold_2
*   **Size category 2**:
    *   short edge >= Si_threshold_1 and
    *   long edge <= Si_threshold_2
*   **Size category 3**:
    *   short edge >= Si_threshold_1 and
    *   long edge <= Si_threshold_1
*   **Size category 4**:
    *   short edge < Si_threshold_1 and
    *   long edge > Si_threshold_2
*   **Size category 5**:
    *   short edge < Si_threshold_1 and
    *   long edge >= Si_threshold_1
*   **Size category 6**:
    *   short edge < Si_threshold_1 and
    *   long edge < Si_threshold_1

**Production sequence**
The rack groups are defined according to this size scheme; the production sequence is created after the pattern 1 ' 2 ' 3 ' 4 ' 5 ' 6, i.e. from large to small. Sorting within these categories:
*   **IG size 1**
    *   Series
    *   Common IG
    *   IG specialities (step, shape, triple, muntins)
*   **IG size 2**
    *   Series
    *   Common IG
    *   Stepped IG
    *   Triple IG
    *   IG shapes
    *   IG lites with muntins
*   **IG size 3**
    *   Like size 2
*   **IG size 4**
    *   Like size 2
*   **IG size 5**
    *   Like size 2
*   **IG size 6**
    *   Series
    *   Common IG
    *   IG specialities (step, shape, triple, muntins)

For the largest and smallest lites, all specialities will be united.

**Grouping and sorting**
The rack group (size) is classified by:
`Customer + Article + MuntinCode + Shape + Steps`

Lites for a certain customer usually have to be taken alternately from the racks of a size category. The (product) number makes sure that identical glass structures are kept in production sequence (usually, same rack).
Otherwise, steps range before shapes, and shapes before muntins. Series are stacked separately, per item, but will be added to the production sequence. All other A racks hold several customer orders.

**Number ranges**
The organization will allocate the lites to the racks. The following racks and number areas have been defined for this purpose:

**Tab. D-4: Number ranges for production organization A racks dispatch**
| Organization group | Storage location | Number range from | to |
| --- | --- | --- | --- |
| Buffer | Buffer | 10000 | 10999 |
| TG - processed | processed - large lites | 8921 | 8950 |
| TG - processed | processed - small lites | 8901 | 8920 |
| TG - processed | processed | 8501 | 8899 |
| TG - processed | processed - series | 8951 | 8999 |
| TG - arrissed | arrissed - large lites | 8421 | 8450 |
| TG - arrissed | arrissed | 8001 | 8399 |
| TG - arrissed | arrissed - small lites | 8401 | 8420 |
| TG - arrissed | arrissed - series | 8451 | 8499 |
| Single glass | small lites | 7901 | 7920 |
| Single glass | large lites | 7921 | 7950 |
| Single glass | Single | 7501 | 7899 |
| Single glass | Series | 7951 | 7999 |
| Single glass - bevelled | bevelled - small lites | 7401 | 7420 |
| Single glass - bevelled | Single - bevelled | 7001 | 7399 |
| Single glass - bevelled | bevelled - large lites | 7421 | 7450 |
| Single glass - bevelled | bevelled - series | 7451 | 7499 |
| IG size 1 | Common IG size 1 | 1001 | 1499 |
| IG size 1 | Special IG size 1 | 1801 | 1899 |
| IG size 1 | IG - series - size 1 | 1951 | 1999 |
| IG size 2 | IG - series - size 2 | 2951 | 2999 |
| IG size 2 | Common IG size 2 | 2001 | 2499 |
| IG size 2 | IG muntins size 2 | 2601 | 2699 |
| IG size 2 | IG shapes size 2 | 2501 | 2599 |
| IG size 2 | Triple IG sizecat 2 | 2701 | 2799 |
| IG size 2 | IG stepped size 2 | 2801 | 2899 |
| IG size 3 | Common IG size 3 | 3001 | 3499 |
| IG size 3 | IG stepped size 3 | 3801 | 3899 |
| IG size 3 | Triple IG SizeCat 3 | 3701 | 3799 |
| IG size 3 | IG shapes size 3 | 3501 | 3599 |
| IG size 3 | IG - series - size 3 | 3951 | 3999 |
| IG size 3 | IG muntins size 3 | 3601 | 3699 |
| IG size 4 | IG muntins size 4 | 4601 | 4699 |
| IG size 4 | Common IG size 4 | 4001 | 4499 |
| IG size 4 | IG stepped size 4 | 4801 | 4899 |
| IG size 4 | Triple IG sizecat 4 | 4701 | 4799 |
| IG Size 4 | IG shapes size 4 | 4501 | 4599 |
| IG Size 4 | IG-series - size 4 | 4951 | 4999 |
| IG size 5 | Common IG size 5 | 5001 | 5499 |
| IG size 5 | IG - series - size 5 | 5951 | 5999 |
| IG size 5 | Triple IG sizecat 5 | 5701 | 5799 |
| IG size 5 | IG shapes size 5 | 5501 | 5599 |
| IG size 5 | IG muntins size 5 | 5601 | 5699 |
| IG size 5 | IG stepped size 5 | 5801 | 5899 |
| IG size 6 | IG - series - size 6 | 6951 | 6999 |
| IG size 6 | Common IG size 6 | 6001 | 6499 |
| IG size 6 | Special IG size 6 | 6801 | 6899 |
| LAMI | LAMI | 9001 | 9899 |
| LAMI | LAMI - small lites | 9901 | 9920 |
| LAMI | LAMI - large lites | 9921 | 9950 |
| LAMI | LAMI - series | 9951 | 9990 |

The organization **A racks dispatch** optimizes directly with regard to packing and shipping. This will require more racks at the end of the line (per customer/order) but the stacking logic for the lites is simpler.

[Image: Photo of a glass production line.]

**Settings in A+W Production**
The following dialogs show the appropriate settings in A+W Production for **IG series size category 1**.

**Settings for the organization group:**

[Image: Fig. D-40 - The Organization Groups settings dialog.]

**Rack settings:**

[Image: Fig. D-41 - The Rack settings dialog.]

**Additional information**
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### Harp Racks, no filling up

Structure and rack allocation of the harp rack organization is similar to the A rack organization only that harp racks will be used chiefly.
This produces a much better yield. Big and small units as well as series will be put onto A racks.
Compared with an A rack organization, an important difference is the dispatch-oriented production sequence. Even if the harp rack organization handles one rack after the other in front of the line, the required glass types can be put onto harp rack, in dispatch sequence.

**Production sequence**
Rack groups used (in production sequence):
*   Common IG lites
*   IG shapes
*   IG shapes with muntins
*   IG lites with muntins
*   Stepped IG
*   Triple IG

To make direct packing possible in part, the rack groups range from large to small (in production sequence):
*   Series: A rack, (series flag set or quantity >= 10)
*   Large units: A rack, condition *large unit*, default setting:
    *   long edge > 2100 or
    *   short edge > 1600)
*   Common units: harp racks
*   Small units: A rack, condition *small unit*, default setting:
    *   short edge < 300 or
    *   long edge < 500)

**Grouping and sorting**
Harp racks have 60 individually numbered slots. The lites on the harp racks are sorted by `Customer+order+item` while the A racks are sorted by `Customer+order`.
Lites belonging to the same product structure, will be set onto the harp rack next to another. Manually cut lites and ancillaries have to be added.
In any of the rack groups (in production sequence) there may be harp racks which only contain a small number of lites at the end. For the rack group `Shaped bars` for example there is a rack with just two units if the production batch does not include more shaped bars. This effect is avoided in the `Filled harp racks` organization.

**Optimization**
Batches which include only lites for harp racks will be optimized as free optimizations (XOPT). If an optimization includes A rack lites, sequenced optimization will be used. The lites on the harp racks will be optimized without restrictions; the effect is the same as for free optimization.

> **Harp racks not filled!**
> It is important for this organization that harp racks are not filled.
> This means that the harp racks will not be used to the best effect. Some of the slots may remain empty as the items will not be split. If an order item does not fit into the remaining slots of the harp rack, a new harp rack number will be allocated!
> The sorting on the harp rack is determined by the classification (or sorting), depending on the rack organization.

**Number ranges**
The organization will allocate the lites to the racks. The following racks and number areas have been defined for this purpose:

**Tab. D-5: Number ranges for production organization harp racks, no filling up**
| Organization group | Storage location | Number range from | to |
| --- | --- | --- | --- |
| Buffer | Buffer | 10000 | 10999 |
| TG - processed | processed - large lites | 8921 | 8950 |
| TG - processed | processed - small lites | 8901 | 8920 |
| TG - processed | processed | 8500 | 8899 |
| TG - processed | processed - series | 8951 | 8999 |
| TG - arrissed | arrissed - series | 8451 | 8499 |
| TG - arrissed | arrissed - large lites | 8421 | 8450 |
| TG - arrissed | arrissed - small lites | 8401 | 8420 |
| TG - arrissed | Arrissed | 8000 | 8399 |
| Single glass | Series | 7951 | 7999 |
| Single glass | small lites | 7901 | 7920 |
| Single glass | Single | 7500 | 7899 |
| Single glass | large lites | 7921 | 7950 |
| Single glass - bevelled | bevelled - large lites | 7421 | 7450 |
| Single glass - bevelled | bevelled - small lites | 7401 | 7420 |
| Single glass - bevelled | Single - bevelled | 7000 | 7399 |
| Single glass - bevelled | bevelled series | 7451 | 7499 |
| IG | IG | 100 | 1899 |
| IG | IG - small units | 1901 | 1920 |
| IG | IG - large units | 1921 | 1950 |
| IG | IG - series | 1951 | 1999 |
| IG - triple | IG - triple | 6000 | 6899 |
| IG - triple | IG - triple - large units | 6921 | 6950 |
| IG - triple | IG - triple - series | 6951 | 6999 |
| IG - triple | IG - triple - small units | 6901 | 6920 |
| IG - shapes | IG - shapes - small units | 2901 | 2920 |
| IG - shapes | IG - shapes | 2000 | 2899 |
| IG - shapes | IG - shapes - large units | 2921 | 2940 |
| IG - shapes | IG - shapes - series | 2951 | 2999 |
| IG - shapes | IG - shapes - unsealed | 2941 | 2950 |
| IG - shapes - muntins | IG - shapes - muntins - large | 3921 | 3950 |
| IG - shapes - muntins | IG - shapes - muntins | 3000 | 3899 |
| IG - shapes - muntins | IG - shapes - muntins - small | 3901 | 3920 |
| IG - shapes - muntins | IG - shapes - muntins - series | 3951 | 3999 |
| IG - muntins | IG - muntins - series | 4951 | 4999 |
| IG - muntins | IG - muntins - large units | 4921 | 4950 |
| IG - muntins | IG - muntins - small units | 4901 | 4920 |
| IG - muntins | IG - muntins | 4000 | 4899 |
| IG - stepped | IG - stepped - small units | 5901 | 5920 |
| IG - stepped | IG - stepped - large units | 5921 | 5950 |
| IG - stepped | IG - stepped - series | 5951 | 5999 |
| IG - stepped | IG - stepped | 5000 | 5899 |
| LAMI | LAMI - series | 9951 | 9990 |
| LAMI | LAMI - large lites | 9921 | 9950 |
| LAMI | LAMI - small lites | 9901 | 9920 |
| LAMI | LAMI | 9000 | 9899 |

The **Harp rack** organization optimizes dispatch-oriented; its structure and rack allocation is similar to the A rack organization; the difference is that harp racks will be used as the main racks.

[Image: Photo of a glass production line.]

**Settings in A+W Production**
The following dialogs show the appropriate settings in A+W Production for **IG shapes**.

**Settings for the organization group:**

[Image: Fig. D-42 - The Organization Groups settings dialog for IG Shapes.]

**Rack settings:**

[Image: Fig. D-43 - The Rack settings dialog for IG-shapes.]

**Additional information**
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383

#### Filled harp racks

The **Filled harp racks** organization makes sure that there are no half-filled harp racks; it sorts all harp racks in production sequence. The harp racks will be handled first, followed by the A racks containing the specialties.

**Production sequence**
Rack groups used (in production sequence):

| Rack Group | Rack Type |
| --- | --- |
| Common IG (sorted by product type) | Harp racks |
| IG large, small, series | A Racks |
| IG shapes - large, small, series | A Racks |
| IG shapes/muntins - large, small, series | A Racks |
| IG muntins - large, small, series | A Racks |
| Stepped IG - large, small, series | A Racks |
| Triple IG, large, small, series | A Racks |

Apart from slots kept free for adding purchased glass and manually cut glass, the harp racks are filled without gaps and will contain all common-size lites, including muntins, shapes, etc.
Large and small units as well as series are removed to be produced at the end.

**Grouping and sorting**
Series will be stacked separately, per item. All other A racks are grouped by `Customer+order`, with several orders per rack; the item sequence is free.
This organization is internally sorted by product features. The sequence of lites on the harp racks and thus, the production sequence, can be overridden by defining a general classification and sorting.
*   Grouping = none
*   Sorting = none

This general setting sorts the lites on the harp racks by the following product characteristics:
Shapes, shaped muntins, muntins, steps, triple IG, and common IG.
These will be stacked and produced together.

The following setting will keep customer orders together, notwithstanding the product characteristics:
*   Grouping = customer+order
*   Sorting = none

Shapes, muntins, and triple IG will change depending on the order mixture; the orders are classified by product characteristics.
Harp racks have 60 individually numbered slots.
The stacking mode is **Unit** - lites belonging to the same product structure will be put next to another on the harp racks. Manually cut lites and ancillaries have to be added.

**Optimization**
This organization is usually based on the sequence - see organization **Harp racks, no filling up** - but in this case, the harp racks will be filled completely even if an order item is split.

**Number ranges**
The organization will allocate the lites to the racks. The following racks and number areas have been defined for this purpose:

**Tab. D-7: Number ranges for production organization Filled harp racks**
| Organization group | Storage location | Number range from | to |
| --- | --- | --- | --- |
| Buffer | Buffer | 10000 | 10999 |
| TG - processed | processed - series | 8951 | 8999 |
| TG - processed | processed - large lites | 8921 | 8950 |
| TG - processed | processed - small lites | 8901 | 8920 |
| TG - processed | processed | 8500 | 8899 |
| TG - arrissed | arrissed - large lites | 8421 | 8450 |
| TG - arrissed | arrissed - small lites | 8401 | 8420 |
| TG - arrissed | arrissed | 8000 | 8399 |
| TG - arrissed | arrissed - series | 8451 | 8499 |
| Single glass | Single | 7500 | 7899 |
| Single glass | Series | 7951 | 7999 |
| Single glass | large lites | 7921 | 7950 |
| Single glass | small lites | 7901 | 7920 |
| Single glass - bevelled | bevelled - series | 7451 | 7499 |
| Single glass - bevelled | bevelled - large lites | 7421 | 7450 |
| Single glass - bevelled | bevelled - small lites | 7401 | 7420 |
| Single glass - bevelled | Single - bevelled | 7000 | 7399 |
| Harp rack - filled | Harp rack - all | 11000 | 50999 |
| IG | IG - small units | 1901 | 1920 |
| IG | IG - series | 1951 | 1999 |
| IG | IG - large units | 1921 | 1950 |
| IG - triple | IG - triple - small units | 6901 | 6920 |
| IG - triple | IG - triple - large units | 6921 | 6950 |
| IG - triple | IG - triple - series | 6951 | 6999 |
| IG - shapes | IG - shapes - large units | 2921 | 2940 |
| IG - shapes | IG - shapes - small units | 2901 | 2920 |
| IG - shapes | IG - shapes - series | 2951 | 2999 |
| IG - shapes | IG - shapes - unsealed | 2941 | 2950 |
| IG - shapes - muntins | IG - shapes - muntins - large | 3921 | 3950 |
| IG - shapes - muntins | IG - shapes - muntins - series | 3951 | 3999 |
| IG - shapes - muntins | IG - shapes - muntins - small | 3901 | 3920 |
| IG - muntins | IG - muntins - small units | 4901 | 4920 |
| IG - muntins | IG - muntins - series | 4951 | 4999 |
| IG - muntins | IG - muntins - large units | 4921 | 4950 |
| IG - stepped | IG - stepped - series | 5951 | 5999 |
| IG - stepped | IG - stepped - small units | 5901 | 5920 |
| IG - stepped | IG - stepped - large units | 5921 | 5950 |
| LAMI | LAMI - large lites | 9921 | 9950 |
| LAMI | LAMI - series | 9951 | 9990 |
| LAMI | LAMI | 9000 | 9899 |
| LAMI | LAMI - small lites | 9901 | 9920 |

The organization **Filled harp racks** optimizes the lites production-oriented, according to the product properties, onto harp racks and A racks. You will need more racks but production is rather dispatch-oriented as the lites are grouped by customer and order number.

[Image: Photo of a glass production line.]

**Settings in A+W Production**
The following dialogs show the appropriate settings in A+W Production for **Triple IG, large units**.

**Settings for the organization group:**

[Image: Fig. D-44 - The Organization Groups settings dialog for Triple IG.]

**Rack settings:**

[Image: Fig. D-45 - The Rack settings dialog for Triple IG - large units.]

**Additional information**
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383

### Demos and Exercises

This session shows you how to define an organization in A+W Production.

**Trainer demo: Explaining master data**
The master data of A+W Production are presented and explained.
The following dialog is explained from this point of view:
*   Dialog Organization including the tabs
    *   Master organization
    *   Production sequence
    *   Sequence of checks

**Exercise 1: Define a master organization**
Set up a master organization according to the following specifications.

**The task**
Enter a test order and schedule it together with the trainer to see the effects. The test order has to fulfill the following general conditions:
*   Name of the organization: New training organization.
*   Production groups: by customer number+order number
*   Name of the organization type: New training
*   Type of the organization type: Standard
*   Stacking mode: Unit
*   Name of the organization group: Buffer rack
*   Rack settings: A rack, super group formation: +customer number+order number, no sorting within the groups, complete groups are stacked together, optimization behavior 5.1, stacking mode unit.

**Exercise 1: Solution**
The individual steps for this task are performed in the following dialogs:
*   Organization dialog
*   Master organization dialog
*   Dialog Rack settings

#### Define a master organization

1.  Open the Organization dialog in `Master data > Detailed scheduling`.
2.  Press the **[New]** button. The dialog Master organization appears.
3.  In field **Name of master organization**, enter `New training organization`.
4.  Open the combo box **Production groups** and select `+Customer number-Order number`.
5.  Press **[OK]**. The dialog closes and you will find yourself back in the Organization dialog.
6.  The new organization appears on the list.

#### Define the production sequence

1.  Open the tab **Production sequence**.
2.  Press the **[New]** button. The entry `unknown/standard` is added.
3.  Press the **[Settings]** button. The Organization dialog appears.
4.  Go to the field **Name of organization type** and enter `New training`.
5.  In section **Stacking mode**, tick **Unit**.
6.  Press **[OK]**. The dialog closes and you will find yourself back on tab **Production sequence**.

#### Define the organization group

1.  Select the just created organization type `New training` and press button **[New]**. The entry `noname` is added.
2.  Press the **[Settings]** button. The dialog organization groups appears.
3.  Go to field **Name** and enter `Buffer rack`.
4.  In section **Group formation**, choose `Customer number`.
5.  Tick the checkbox **Sorting of groups**.
6.  Press **[OK]**. The dialog closes and you will find yourself back on tab **Production sequence**.

#### Define a rack

1.  Select the just defined organization group `Buffer rack` and press **[New]**. The entry `unknown` is added.
2.  Press the **[Settings]** button. The dialog **Rack settings** appears.
3.  Go to field **Name** and enter `A rack`.
4.  In section **Group formation**, select `+Customer number+Order number`.
5.  Go to combo box **Sorting of groups** and select **None**.
6.  In section **Stacking mode groups**, select **Complete groups together** and in section **Optimization behavior**, **5.1**.
7.  Tick the checkbox **Buffer rack**.

**Additional information**
*   ⇨ Software Reference, "Organization" on page D-379
*   ⇨ Software Reference, "Organization Groups" on page D-381
*   ⇨ Software Reference, "Workstation Settings" on page D-383

---

# Software Reference

This section provides information on the following subjects:
*   ⇨ Overview
*   ⇨ Organizations
*   ⇨ Grouping and Sorting
*   ⇨ Racks
*   ⇨ Lots
*   ⇨ Detailed Scheduling of Batches

## Overview

*   **Overview**: D-367
*   **Organizations**: D-369
    *   Master Organization Tab: D-369
    *   Production Sequence Tab: D-371
    *   Test Sequence Tab: D-372
    *   Master Organization: D-375
    *   Organization: D-379
    *   Organization Groups: D-381
    *   Workstation Settings: D-383
    *   Default Settings: D-387
*   **Grouping and Sorting**: D-388
    *   Grouping/Sorting Dialog: D-388
    *   Editor - Grouping Tab: D-389
    *   Editor - Sorting Tab: D-391
    *   Additional Sorting Tab: D-392
    *   Defining an Additional Sorting: D-393
*   **Racks**: D-394
    *   Racks: D-394
*   **Lots**: D-399
    *   Lot Types and Processings: D-399
    *   Lot Types Tab: D-399
    *   Processings Tab: D-401
    *   Implicit Processing Tab: D-404
*   **Detailed Scheduling of Batches**: D-406
    *   Detailed Scheduling for Batch...: D-406
    *   Glass Types Tab: D-407
    *   Rack Load Tab: D-410
    *   Results Tab: D-415
    *   Specials Tab: D-417
    *   Nested Shapes Tab: D-417
    *   Filler Orders Tab: D-419
    *   Residue Plates Tab: D-421
    *   Rejects Tab: D-422
    *   Rush orders tab: D-424
    *   Thickness Tab: D-425
    *   Free Optimization Tab: D-427
    *   Partial Quantities Tab: D-428
    *   Organization Tab: D-430
    *   Organization Options Tab: D-432
    *   Options Tab: D-434
    *   Stockplate Selection Tab: D-436
    *   Change minimum number of A racks: D-437
    *   Sequence of Tables: D-438

Open menu `Master data > Detailed scheduling`

Menu **Detailed Scheduling** offers the following items:
*   **Presettings**: You will need this menu if no settings have been made with regard to organization, grouping and sorting in the organization, or regarding the sorting on the rack.
    *   ⇨ "Default Settings" on page D-387
*   **Organization**: This menu is used for setting up the organizations. You can define the production sequence and the sequence of checks.
    *   ⇨ Software Reference, "Master Organization Tab" on page D-369
    *   ⇨ Software Reference, “Production Sequence Tab" on page D-371
    *   ⇨ Software Reference, "Test Sequence Tab" on page D-372
*   **Grouping**: This menu item serves to define the grouping and sorting.
    *   ⇨ Software Reference, "Grouping/Sorting Dialog" on page D-388
*   **Racks**: This menu is used for rack definition.
    *   ⇨ Software Reference, "Racks" on page D-394
*   **Processing**: This menu can be used to define new processing steps or change existing ones.
*   **Lot types**: This menu allows defining lot types and allocating processing steps.
    *   ⇨ Software Reference, "Lot Types and Processings" on page D-399

> **Dialogs are accessible from different points**
> Please note that there are various ways of opening functions and dialogs. These instructions will describe the corresponding dialogs just once.
> Instructions on how to open individual dialogs are provided again in the following dialog descriptions. If there are several ways of opening a dialog, these are specified as well.

## Organizations

`Master data > Detailed scheduling > Organization`

This dialog is used for entering or changing master organizations, organizations, or organization groups. Settings regarding the production sequence and the sequence of checks can be made as well. For detailed information, please see the explanations on the individual tabs.

The dialog is split into the following tabs:
*   "Master Organization Tab” on page D-369
*   "Production Sequence Tab" on page D-371
*   "Test Sequence Tab" on page D-372
*   "Default Settings" on page D-387

### Master Organization Tab

`Master data > Detailed scheduling > Organization`

[Image: Fig. D-46 - The Organization dialog, showing the Master organization tab.]

Tab **Master organization** is used for defining new master organizations or change existing ones. These master organizations will be allocated to batches in detailed scheduling. The left window shows all existing master organizations in a tree structure. Click on the plus sign to open a master organization and view the organization allocated to this master organization. The right window shows all existing organizations.

The symbols in the right window mean:
*   `S` (blue): Standard organization / Application
*   `S` (red): Standard organization / Production
*   `X` (red): Non-Standard organization / Production
*   `X` (blue): Non-Standard organization / Application

[Image: Fig. D-47 - An explanation of organization symbols.]

**Description of buttons**

*   **New**: Use this button to open the dialog **Master organization** which allows defining a new master organization. To define a new master organization you have to select the first entry in the tree structure in the left window, `Master organization`.
*   **Deletion**: Use this button to delete the master organization selected in the left window. The selected organization will be deleted.
    > **Deletion without security check**
    > If you have deleted something by mistake, leave the Organization dialog via button [Abort]. Next time you open it, the data will still be there.
*   **Settings**: Use this button to open the **Master organization** dialog for the master organization selected in the left window.

**More information on the tab Master organization**
*   ⇨ Tutorial, "Master organization" on page D-319
*   ⇨ Overview, "Buttons" on page A-90

### Production Sequence Tab

`Master data > Detailed scheduling > Organization > Production sequence tab`

[Image: Fig. D-48 - The Organization dialog, showing the Production sequence tab.]

Production sequence tab shows the sequence of the organization groups within the organization.

**Description of buttons**

*   **Condition**: This button is active only for organization groups and racks because conditions can be defined only for those. If you use this button after selecting an organization group, dialog **Select conditions** opens. Define a condition for the organization group. If you use this button after selecting a rack, dialog **Select conditions** opens as well. Define a condition for the rack. The condition for a rack is marked by a `?`.
*   **New**: Use to button to define a new organization, a new organization group, or a new rack. This depends on which entry has been selected. If you select `Organization` and use button **[New]**, a new organization (e.g. `Machine allocation IG large`) will be added below the last organization type. This new organization is called `unknown` at first. Select this new organization and use the button **[Settings]**. Dialog **Organization** appears in which you can make the required settings for this organization.
    When you select an organization and press button **[New]**, a new organization group will be added at the end of the selected organization. The new organization group is called `noname` at first. Select this new organization group and use the button **[Settings]**. Dialog **Organization group** appears in which you can make the required settings for this organization group.
    When you select an organization group and press button **[New]**, a new rack will be added at the end of the selected organization group. This new rack is called `unknown` at first. Select this rack and use the button **[Settings]**. Dialog **Workstation settings** appears in which you can make the required settings for this rack.
*   **Cut**: Use this button to cut out the selected record and move it to the clipboard. It can then be added to another organization by using the button **[Insert]**. Should you have cut the wrong record by mistake, the program will want to know whether the changes shall be ignored when you leave the dialog. If you confirm this question by **[Yes]**, the cut-out record will be there next time you open the organization.
*   **Copy**: Use this button to transfer the selected record to the clipboard. It can then be added to another organization by using the button **[Insert]**.
*   **Add**: Use this button to insert the copied or cut-out record from the clipboard.
*   **Delete**: Use this button to delete the selected record. If the record you want to delete is still used by an A+W Production process, a security check appears. Should you have deleted the wrong record by mistake, the system will want to know whether the changes shall be ignored when you leave the dialog. If you confirm this by **[Yes]**, the deleted record will be available next time you open it.
*   **Settings**: Use this button to open the dialog for the selected entry.
    *   Software Reference, “Organization” on page D-379
    *   Software Reference, "Organization Groups" on page D-381
    *   Software Reference, “Workstation Settings" on page D-383
    *   Formula Editor, "Select conditions" on page F-734
    *   Formula Editor: Software Reference, "Select conditions" on page F-734
*   **Export orga**: Use this button to export the selected organization.

**More information on the production sequence**
*   ⇨ Tutorial, “Production Sequence" on page D-330
*   ⇨ Overview, "Buttons" on page A-90

### Test Sequence Tab

`Master data > Detailed scheduling > Organization > Test sequence tab`

[Image: Fig. D-49 - The Organization dialog, showing the test sequence tab.]

This dialog shows the sequence of tests for an organization. This means that this tab is used to define the sequence in which the program checks whether a lite is allocated to the appropriate rack (the names of the racks are followed by the defined conditions). This way, they implicitly define the sequence in which the conditions are checked. On a rack, all allocated conditions - maximally 7 per rack - are linked by an AND-operation.

The right window shows the racks belonging to the organization selected in the left window. `*` in front of the name marks the buffer rack of this organization (which should always be found at the end of the list). Double-click on the rack you want to mark as a buffer rack. Please remember that there can be only one buffer rack per organization. This means that if there is already a buffer rack for an organization and you double-click on another rack to mark it as such, the first buffer rack becomes a normal rack again (without `*`).

The racks show the sequence (in descending order) in which the lites are allocated to certain racks. Depending on the set sequence of checks, a lite will be transferred from rack to rack until it meets a rack the condition of which it fulfils. It will be allocated to this rack. The columns **from** and **to** mark the range of numbers for the racks. Click on the required column to edit the range of numbers by means of this dialog.

**Description of buttons**

*   **Start**: Use this button to move the selected lite to first place.
*   **Up**: Use this button to move the selected lite one line up.
*   **Down**: Use this button to move the selected lite one line down.
*   **End**: Use this button to move the selected lite to last place.

**More information on the sequence of checks**
*   ⇨ Tutorial, "Sequence of Checks" on page D-324
*   ⇨ Overview, "Buttons" on page A-90

### Master Organization

`Master data > Detailed scheduling > Organization > Master organization tab> [New]`
`Master data > Detailed scheduling > Organization > Master organization tab > Select master organization > [Settings]`

[Image: Fig. D-50 - The Define master organization dialog.]

Dialog **Master organization** allows defining a new master organization, or changing the settings for an existing master organization. Master organizations are defined in two steps. First, define the master organization and the appropriate settings, then define the organizations that shall form the master organization. Further details are available in the corresponding fields.

**Technical info**: database table: `FEIN_MASTERORGA`

**Description of fields**

*   **Name of the master organization**: Enter the name of the master organization. The name of the master organization will appear in all views in connection with the organization.
    *   **Technical info**: Compulsory field, alpha-numeric, 32-digit, database field: `NAME`
*   **Stack XOPT together**: Detailed scheduling allows to remove certain lites from the optimizations, and optimize them via XOPT.
    *   ✅ Despite different glass types and thicknesses, XOPT optimizations are stacked on an A rack together.
    *   ⬜ Free optimizations are put separately onto A racks.
    *   **Technical info**: database field: `TOGETHER`
*   **Combo box**: This checkbox defines the master organization type:
    *   **Standard**: The usual master orga is used.
    *   **Quick organization**: A quick organization will be run without showing the detailed scheduling views. If batches contain cut lites which undergo a quick master organization, these will be treated like manual cutting.
    *   **Phys. rack load**: The system automatically creates a sensible load of physical racks and considers the rules and conditions (weight, size, etc.). Therefore, the Stack Optimizer will be started.
    *   **Technical info**: database field: `QUICKORGA`
*   **Creation of pairs not permitted**: This checkbox is used for triple IG. The units mainly consists of an uncoated and two coated lites; the first and third lite being coated. The coating faces the airspace so that one of the two lites would have to be turned before entering the line. To turn the lite after cutting, before loading it onto the rack, detailed scheduling shall therefore put the lites onto different stacks. To put the two stacks into an identical sequence, optimization in *fixed sequence* is required for this number range.
    *   ✅ Pairs must not be created.
    *   ⬜ Pairs can be created.
    *   **Technical info**: database field: `PAIRFORBIDDEN`
*   **Maximum number of storage locations in optimization**: In this field you can specify how many stacks may be used simultaneously by the optimization.
*   **Production groups**: The combo box shows all entries made on tab **Groupings** in dialog **Grouping/Sorting**. If you select one of the groupings in this field, detailed scheduling will create production groups according to this value (as a pre-setting which can be changed later by means of the organization settings and in detailed scheduling (optimization)). The selected values refer to the basic elements of the batch.
    *   **Technical info**: database field: `ID_GROUP`
*   **Pseudo series**: Items with identical structures can be combined in **Pseudo series** in detailed scheduling. The values in this combo box are taken from tab **Grouping** in dialog **Grouping/Sorting**. From this combo box, select the values to be applied to the pseudo series. Usually, single lites (individual items consisting of one lite each) must only be temporarily stored/put onto fixed racks, e.g. to wait for remakes. By means of pseudo series, identical items (single lites) can be combined in a series which can be put together on fixed rack as an exception from the rule. Pseudo series have another meaning. A series (quantity >100, but this can be defined by the customer) can pass through different production processes - different paths, different treatment. By means of pseudo series, single items can be marked as "series" and can be treated as such (the series flag will also be assigned internally).
    *   **Technical info**: database field: `ID_PSEUDOGROUP`
*   **Min. quantity**: This field refers to field **Pseudo series** and defines the minimum quantity for the creation of pseudo series. If the values lies below, no pseudo series will be formed.
    *   **Technical info**: database field: `PSEUDOSCHWELLE`
*   **Release**: At the release of the batch scheduled by this master organization, the displayed script (`*.bas` / `*.bat` file) will be used. Use button **[Release]** to open the dialog **Select script**. This dialog contains all scripts defined in the program. The scripts will be saved in the A+W Production directory in a separate file (file name: Scripts).
    *   **Technical info**: database field: `SKRIPT`
*   **Filler**: This field serves for optimizing lites that are thicker than ordered by the customer. These lites can be used as so-called **Fillers**. Prerequisite is that the lites will become part of an IG unit. Apart from that, the IG unit must fulfil the condition shown in this field. Use button **[Filler]** to open the formula editor. Select the required formula. When you close the dialog, the name of the formula appears in the field behind the button.
    *   **Technical info**: database field: `ID_FILLERCONDITION`
*   **Pseudo parts**: This field allows defining pseudo parts. Pseudo parts adopt the batch creation and rack information from their sub-elements and do not only depend on the batch type of the elements and processing steps. By defining a condition for the master organization you can specify the elements of the batch type for which this is permitted. Use the button **[Pseudo parts]** to open the formula editor. Select the required formula. When you close the dialog, the name of the formula appears in the field behind the button.
    *   **Technical info**: database field: `ID_QUASICONDITION`

**Bottom section**
This section deals with the use of special elements (fillers, residue plates, rejects, and rush orders). First tag the special element on the list, then assign the rack number on the right.

*   **Use filler**: This field refers to existing filler orders. Detailed scheduling can use filler orders only if this checkbox is active in the selected master organization.
    *   ✅ In the cutting area, the fillers are put onto any racks the number range of which is defined by **Start Filler** and **End Filler**. Each item is allocated to just one rack number.
    *   ⬜ No fillers will be used.
    *   **Technical info**: database field: `USEFUELLER`
*   **Start of filler**: This field refers to the range of rack numbers for the filler orders used. Enter the smallest rack number on which filler orders can be put.
    *   **Technical info**: database field: `FUELLERSTART`
*   **End of filler**: This field refers to the range of rack numbers for the filler orders used. Enter the highest rack number on which filler orders can be put.
    *   **Technical info**: database field: `FUELLERENDE`
*   **Use residue plates**: This field refers to lites which belonged to resolved residue plates of previous detailed scheduling jobs.
    *   ✅ The selected master organization uses residue plates. In the cutting area, the residue plates will be put onto any rack the number range of which is defined by **Start residue plate** and **End residue plate**. Every item is allocated just one rack number.
    *   ⬜ No residue plates will be used.
    *   **Technical info**: database field: `USERESTBLATT`
*   **Start of residue plate**: This field refers to the range of rack numbers for the residue plates used. Enter the smallest rack number on which residue plates can be put.
    *   **Technical info**: database field: `RESTBLATTSTART`
*   **End of residue plate**: This field refers to the range of rack numbers for the residue plates used. Enter the highest rack number on which residue plates can be put.
    *   **Technical info**: database field: `RESTBLATTENDE`
*   **Use rejects**: This field refers to existing breakage.
    *   ✅ The selected master organization uses existing breakage. In the cutting area, the broken lites will be put onto any racks the number range of which is defined by **Start of breakage** and **End of breakage**. Every item is allocated just one rack number.
    *   ⬜ No rejects will be used.
    *   **Technical info**: database field: `USEBRUCH`
*   **Start of rejects**: This field refers to the range of rack numbers for the rejects used. Enter the smallest rack number on which reject can be put.
    *   **Technical info**: database field: `BRUCHSTART`
*   **End of rejects**: This field refers to the range of rack numbers for the rejects used. Enter the highest rack number on which reject can be put.
    *   **Technical info**: database field: `BRUCHENDE`
*   **Use rush orders**: This field refers to existing rush orders.
    *   ✅ The selected master organization uses existing rush orders.
    *   ⬜ No rush orders will be used.
    *   **Technical info**: database field: `USEBRUCH`

**More information on Master organization**
*   ⇨ Tutorial, "Master organization" on page D-319
*   ⇨ Tutorial, "Special Elements" on page D-278
*   ⇨ Overview, "Buttons" on page A-90

### Organization

`Master data > Detailed scheduling > Organization > Production sequence tab > Select organization > [Settings]`

[Image: Fig. D-51 - The Organization settings dialog.]

This dialog is used to define new organizations, or change existing ones. Further details are available in the corresponding fields.

**Technical info**: database table: `FEIN_ORGA`

**Description of fields**

*   **Name of organization type**: Enter the name of the organization.
    *   **Technical info**: database field: `NAME`
*   **Type**: Select the organization type from this combo box. Organization types are **Standard**, **Rack**, and all batch types in the system except cutting. You can select only batch types from this field which have been defined before! These are defined in dialog **Batch types**.
    *   **Technical info**: database field: `LOSTYP`
*   **Production**: The checkbox defines whether this is a production or application organization.
    *   ✅ This organization is a production organization
    *   ⬜ This organization is an application organization.
    *   **Technical info**: database field: `PRODUKTION`
*   **Rack mode**: Use the options to set the default rack mode for A racks for this organization. These settings can be overridden at any time. The default value for the rack mode is **Unit**. Valid options:
    *   Glass
    *   Unit
    *   Production
    *   VABGLA
    *   **Technical info**: database field: `BELEGUNGSMODE`
*   **No splitting of ... if rack contains more than ... percent**: Valid options:
    *   **Groups**: If a group of lites is put on a rack but does not fit because of the rack depth, the group will not be split if the rack load is over X percent.
        *   **Technical info**: database field: `USETIEFE_GRUPPE`
    *   **Units**: If a group is split and part of it is put onto a rack, a unit could be split, theoretically. The unit will not be split if the rack load is over X per cent. Splitting a unit always necessitates to split a group; the value for groups should therefore always be bigger than that the entry for units.
        *   **Technical info**: database field: `USETIEFE_EINHEIT`

**More information on the organization**
*   ⇨ Tutorial, "Organizations" on page D-316
*   ⇨ Overview, "Buttons" on page A-90

### Organization Groups

`Master data > Detailed scheduling > Organization > Production sequence tab > Organization group > [Settings]`

[Image: Fig. D-52 - The Organization group settings dialog.]

Use this dialog to enter settings for existing or new organization groups. This means that you enter or change the name of the organization group, and allocate so-called groupings and/or sortings to the organization group. Further details are available in the corresponding fields.

**Technical info**: database table: `FEIN_ORGAGRUPPE`

**Description of fields**

*   **Name**: Enter the name of the organization group.
    *   **Technical info**: database field: `NAME`
*   **DynOpt settings**: This checkbox must be ticked if the organization group is meant for A+W DynOpt. This means that lites which are meant for A+W DynOpt can be assigned only to an organization group with this code.
    *   **Technical info**: database field: `DYΝΟΡΤ`
*   **Group formation**: This field defines whether groups shall be created for the organization group in question. The combo box contains all defined groups from which you can select the required one. The groups are defined in master data. Select the required group from the combo box.
    *   **Technical info**: database field: `GROUPINDEX`
*   **Sorting of groups**: The checkbox is related to field **Group formation** and defines whether the selected group shall be sorted.
    *   ✅ The groups will be sorted.
    *   ⬜ The groups will not be sorted.
    *   **Technical info**: database field: `HASGSORT`
*   **Sorting within groups**: The combo box defines whether the groups selected in field **Group formation** shall be sorted. The sorting options are:
    *   None = The groups will not be sorted.
    *   General = The default settings will be adopted.
    *   Self-defined sorting.
    *   **Technical info**: database field: `SUBSORTINDEX`

> **Organization group settings**
> Once the grouping and sorting of an organization group has been defined, you do not have to define grouping/sorting for the rack because this will be adopted from the organization group. Settings made for the rack will override the grouping/sorting defined for the organization.

**More information on organization groups**
*   ⇨ Tutorial, "Organizations" on page D-316
*   ⇨ Tutorial, "Production Sequence" on page D-330
*   ⇨ Overview, "Buttons" on page A-90

### Workstation Settings

`Master data > Detailed scheduling > Organization > Production sequence tab > Settings > tab [Application]`

[Image: Fig. D-53 - The Workstation settings dialog.]

This dialog allows allocating names and number ranges to racks. Please make sure that the names and number ranges match to the rack type (A rack, harp rack, etc.). Additionally, grouping, sorting, and rack modes can be allocated.

**Technical info**: database table: `FEIN_BOCKTYP`

**Description of fields**

*   **Name**: Enter the name of the rack type.
    *   **Technical info**: Compulsory field, alpha-numeric, 32-digit, database field: `NAME`
*   **Group formation**: This field defines whether groups shall be created for the rack type in question. The combo box contains all defined groups from which you can select the required one. The groups are defined in master data. Select the required group from the combo box.
    *   **Technical info**: database field: `GROUPINDEX`
*   **Sorting within groups**: The combo box defines whether the groups selected in field **Group formation** shall be sorted. The sorting options are:
    *   None = The groups will not be sorted.
    *   General = The default settings will be adopted.
    *   Self-defined sorting.
    *   **Technical info**: database field: `SUBSORTINDEX`
*   **Check inversion**: In the case of processings that are removed from the BOM within detailed scheduling via the lot type setting `Do not use, Properties only` or `Use sub-part`, the responsible logical machine can be used to specify whether the sequence on A racks must be inverted by this processing step. In the number ranges for detailed scheduling, you can then specify whether the logical machine indicator should be used. If this is the case and there is an uneven number of processings between the step to be produced and the step used that have the above indicator, the sequence within the stacks is inverted on A racks. For this purpose, lites with different inversion behavior are placed on separate stacks. For cutting, this means that the break sequence is also adapted accordingly.
    *   **Technical info**: database field: `INVERT_SEQUENCE`
*   **Group stacking mode**: This field will be analyzed only if optimization mode 6.1 or 5.1 is used. In this case, the combo box defines the stacking of groups. Select the required rack mode from the combo box. Valid options:
    *   just 1 group per stack.
    *   complete groups together.
    *   fixed sequence.
    *   just 1 split group per stack.
    *   alternating.
    *   **Technical info**: database field: `BELEGMODE`
*   **Optimization behavior**: This combo box is related to field **Group formation**. Please select the required optimization mode from the combo box. Options:
    *   free groups (6.1)
    *   groups sorted (6.2)
    *   everything free (5.1)
    > **Use optimization mode**
    > Optimization modes 6.1 and 6.2 will be used only if the grouping and sorting codes include the order number and the item number. If this is not the case, optimization mode 5.2 will be used.
*   **Buffer rack**: This checkbox defines the buffer rack. The selected buffer rack will collect all elements of a batch that cannot be allocated to another rack because they do not fulfil any condition required by the other racks.
    *   ✅ This rack is the buffer rack for the organization.
    *   ⬜ This rack is not the buffer rack for the organization.
    *   **Technical info**: database field: `AUFFAENGER`
*   **From/To**: For each rack type, enter at least one range of numbers that can be used for this rack type. Application rack types can even have two number ranges if production racks are assigned as well. Number ranges must not overlap in an organization or master organization (the program will prevent this and will issue error reports to that effect). Master organizations can even include additional number ranges for specialities (rejects, fillers, residue).
    *   **Technical info**: database field: `MINIMUM`
    *   **Technical info**: database field: `MAXIMUM`
*   **Maximum number of groups**: This field refers to the maximum number of groups that can be put on this rack. If any number of groups can be put onto the rack, enter `0`.
    *   **Technical info**: database field: `MAXNUMBER`
*   **Separate next step**: If this checkbox is active, the batch formation of the next step will be taken into account for A racks, checking what can be stacked together.
*   **Free optimization (only for A racks)**: This checkbox defines for each number range, whether all A racks of this number range will automatically use the Free optimization.
*   **Stacking mode**: The listed values refer to the field **Rack type**.
    *   If the radio button **A rack** is ticked:
        *   **Global**: The mode defined for this organization will be used.
        *   **Glass**: Each glass type gets its own number and is put onto a separate rack.
        *   **Unit**: lites that belong to the same unit (laminated glass, IG) will be put onto the same rack, with a common rack number. Different glass types will be automatically separated by the system and will be put onto separate, adjoining stacks.
        *   **Production**: Several glass types are put together on a rack in separate stacks per glass type. These stacks can be used for producing different products/combinations.
        *   **VAGBLA**: For every glass type, there is a logical rack with just one stack. Unlike in case of the Glass mode, the groups will be split when the maximum rack load has been reached. For details please refer to the description of modes in the tutorial.
    *   If the radio button **Harp Rack** is ticked:
        *   **Together**: lite and counter lite(s) will always be put together onto a harp rack.
        *   **Glass**: The lites will always be stacked separately.
        *   **Compact**: Only lites with a common flag are put on a harp rack. Depending on the configuration, this flag can be the fields `XOPT_TISCH.CUTGO` or `POOL_TEILE.SONDERKZ3`.
    *   If the radio button **Fixed racks** has been ticked, section **Stacking mode** is disabled.
    *   **Technical info**: database field: `BELEGMODE`
*   **Rack type**: The options define the rack type. Valid options:
    *   A Racks
    *   Harp racks
    *   Fixed Racks
    The combo box below always refers to the active rack type. If there are several types of A racks for instance, these will be listed in the combo box.
    *   **Technical info**: database field: `TYPE`

**Description of buttons**

*   **Racks**: Use this button to open the dialog **Racks**.

**More information on tab Application**
*   ⇨ Tutorial, "Storage Locations" on page D-286
*   ⇨ Tutorial, "Grouping Key for Organization Groups" on page D-331
*   ⇨ Overview, "Buttons" on page A-90

### Default Settings

`Master data > Detailed scheduling > Presettings`

[Image: Fig. D-54 - The Presettings dialog.]

These settings will be used if no entries are made for the organization, for grouping and sorting for the organization, and sorting on the rack. We recommend to define settings at this point lest an error message should appear when detailed scheduling is started.

**Description of fields**

*   **Processing sequence**: This combo box allows to select a sorting. Sorting is defined in master data and controls the criteria used for the processing of lites.
*   **Organization**: This combo box allows to select a master organization. Master organizations are defined in master data and determine the master organization used for detailed scheduling.
*   **Group creation**: This combo box allows to select a grouping. Groupings are defined in master data and determine the criteria for group formation.
*   **Sort to rack**: This combo box allows to select a sorting. Sortings are defined in base data and control the sorting criteria for lites.

**More information on default settings**
*   ⇨ Tutorial, "Global Settings" on page D-327
*   ⇨ Overview, "Buttons" on page A-90

## Grouping and Sorting

The settings made in section **Grouping/Sorting** shall be used for grouping and sorting the lites on the racks. The lites will be collected in **Groups**, and sorted within the groups. The sequence of groups can be defined as well.

### Grouping/Sorting Dialog

The dialog consists of three tabs:
*   Editor - Grouping Tab
*   Editor - Sorting Tab
*   Additional Sorting Tab

**More information on grouping and sorting**
*   ⇨ Tutorial, "Grouping and Sorting" on page D-270
*   ⇨ Overview, "Buttons" on page A-90

### Editor - Grouping Tab

`Master data > Detailed scheduling > Grouping > Editor - Grouping tab`

[Image: Fig. D-55 - The Grouping/sorting dialog, showing the grouping tab.]

This dialog is used to define new groups, or change existing ones. The entries on **Editor - grouping tab** will be used in the following areas:
*   Software Reference, “Workstation Settings" on page D-383
*   Software Reference, "Organization Groups" on page D-381
*   Software Reference, “Master Organization" on page D-375
*   Software Reference, "Default Settings" on page D-387

**Technical info**: database table: `SORTING`

**Description of fields**

*   **Left window**: This window shows all defined groups or sortings. The individual groups/sortings are arranged in a tree structure; their characteristics can be displayed by opening the tree structure. Example: `Group +Article number+Stacking width` includes the properties `Article number` and `Stacking width`. The plus or minus sign in front of the properties shows the direction in which this property is sorted. Example: `+Article number` means that the article numbers are sorted in ascending order. `-Article number` means that the article numbers are sorted in descending order.

**Fields in section Sorting direction**

*   **Ascending**: This field is active only if a property of the group/sorting is tagged. Tick the radio button **Ascending** to sort the selected property in ascending order. This is marked by the plus sign in front of the property.
*   **Descending**: This field is active only if a property of the group/sorting is tagged. Tick the radio button **Descending** to sort the selected property in descending order. This is marked by the minus sign in front of the property.

**Description of buttons in section Sorting Direction**

*   **Delete**: Use this button to delete the selected group/sorting property, or to delete the entire group/sorting. This depends on which entry has been selected. When a property of the group/sorting is selected, only this property will be deleted. When a group/sorting is selected however, the entire group/sorting will be deleted.
*   **Add**: This button refers to the right window. The property or formula selected in the right window can be added by using the [Add] button, either as a whole group/sorting, or as a property in the group/sorting. This depends on the selected entry. When a group/sorting is selected, the property or formula will be added to the selected group/sorting. If you select the top entry on the left list (on tab **Editor - Grouping**, this is the entry `Grouping` and on tab **Editor - Sorting**, this is the entry `Sorting`), a new group/sorting will be created.

**Descriptions of options**

*   **Property**: If the radio button **Property** is ticked, the right window shows all existing properties.
*   **Formula**: If the radio button **Formula** is ticked, the right window shows all existing formulas.

**Description of the button**

*   **Formulas ...**: Use this button to open the dialog **Select formulas --1--**. You can change an existing formula or define a new one. For more information please refer to the documentation on **Formula editor**.

**More information on groups**
*   ⇨ Tutorial, "Grouping and Sorting" on page D-270
*   ⇨ Overview, "Buttons" on page A-90

### Editor - Sorting Tab

`Master data > Detailed scheduling > Grouping > Editor - Sorting tab`

[Image: Fig. D-56 - The Grouping/Sorting dialog, showing the sorting tab.]

This dialog is used to define new sortings, or change existing ones.
Apart from the button below, the contents of **Editor - Sorting tab** is the same as the contents of **Editor - Grouping tab** and will therefore not be described in detail at this point. For details please refer to the **Editor - Grouping tab**.

**Technical info**: database table: `SORTING`

**Description of the button**

*   **Additional sorting**: Use this button to open the dialog **Additional sorting** for the selected sorting.

**More information on sorting**
*   ⇨ Tutorial, "Grouping and Sorting" on page D-270
*   ⇨ Overview, "Buttons" on page A-90

### Additional Sorting Tab

`Master data > Detailed scheduling > Grouping > Additional Sorting tab`

[Image: Fig. D-57 - The Grouping/Sorting dialog, showing the Additional sortings tab.]

This dialog shows all additional sortings. Additional sortings are defined in dialog **Define additional sorting**.

**Technical info**: database table:

**Description of fields**

*   **Key**: Column **Key** shows the key for which the additional sorting is used.
*   **Value**: This field shows the value for the additional sorting.
*   **Additional Sorting**: The field shows the complete sorting this key has an effect on.

**More information on Additional sorting**
*   ⇨ Tutorial, "Additional Sorting" on page D-277
*   ⇨ Overview, "Buttons" on page A-90

### Defining an Additional Sorting

`Master data > Detailed scheduling > Grouping > Editor - Sorting tab > [Create additional sorting]`

[Image: Fig. D-58 - The Define additional sorting dialog.]

Sortings can be completed by additional sortings. You only need to define an additional sorting to which the combination of sorting key/value is allocated. If a sorting ends with the defined sorting key, the group all elements of which match the defined sorting key, will be sorted into more groups. Example: The items on a rack are sorted by `ROUTE+CUSTOMERNUMBER+`. If there is an additional sorting `SMALLSIZE+` for `CUSTOMERNUMBER=4711`, the extended sorting will be only applied to customer number 4711. For all other customers, the sequence does not matter. You can of course allocate different additional sortings to different customers.

**Technical info**: database table: `MORESORTING`

**Description of fields**

*   **Value**: Enter the name of the additional sorting. The radio buttons **Number**, **thickness**, **text**, **length**, and **airspace** define the value. Additional sortings are shown on **Additional sorting** tab.

**Description of the button**

*   **Do not check value**: Press this button to use the additional sorting, notwithstanding the last sorting key.

**More information on how to define additional sorting**
*   ⇨ Tutorial, "Additional Sorting" on page D-277
*   ⇨ Overview, "Buttons" on page A-90

### Racks

The dialog consists of three sections:
*   A Racks
*   Harp racks
*   Fixed Racks

`Master data > Detailed scheduling > Racks`
`Master data > Detailed scheduling > Organization > Production sequence tab > Select rack for the organization group > [Settings] button`

[Image: Fig. D-59 - The Racks dialog showing sections for A Racks, Harp Racks, and Fixed Racks.]

Use this dialog to define the racks existing in your production, or to change the defined racks. The defined racks are used in the following detailed scheduling areas:
*   Software Reference, "Workstation Settings" on page D-383
*   Software Reference, “Organization Tab” on page D-430

**Technical info**: database table: `ABSTELLPLATZ`

#### Description of the fields in section A racks

*   **Combo box**: The combo box below the buttons [Add], [Delete] and [Rename] shows the names of the racks defined for the A racks in the system.
*   **Rack depth**: Enter the rack depth in mm. 1200 mm means that the stack can be up to 1200 mm deep. Please note that rack depths over 20 m will automatically be treated like unlimited rack depths.
    *   **Technical info**: database field: `TIEFE`
*   **Width**: This field defines the total width of the rack in mm. 2000 mm for example means that lites can be stacked on the rack up to a width of 2000 mm.
    *   **Technical info**: database field: `BREITE`
*   **Max. racks/rack**: Enter the number of available slots per rack. Valid options:
    *   1 = one storage location per rack.
    *   2 = there are two storage locations per rack.
    *   4 = there are four storage locations per rack.
    *   **Technical info**: database field: `MAXCOUNT`
*   **L rack**: Tick this checkbox if the rack is an L rack (instead of an A rack).
*   **Robot**: Tick this checkbox if the A rack is a robot rack. Robot racks are racks controlled by a robot. Valid options:
    *   0 = no robot rack.
    *   1 = single = robot rack, single.
    *   2 = reflected = robot rack, reflected.
    *   3 = double = robot rack, exists twice, both racks can be controlled separately.
    *   **Technical info**: database field: `ROBOT`
*   **Quantity**: This field is active only if the A rack is a robot rack. You can define the number of robot racks existing in your production. Also, you can enter whether these racks exist once or twice, or whether the robot racks actually exist twice, but the system decides which one will be used. The rack with the given number from the first or second quantity.
*   **Max. no. of A racks**: The maximum number of A racks is important for creating optimization groups. When a glass type reaches the maximum quantity allowed, the current optimization group will be closed for all optimizations, and a new one will be started. This can be cut once the racks are empty.
*   **Check quantity (cutting)**: The checkbox refers to the entry in field **Max. no. of A racks** and checks this if necessary.
*   **Sortjet**: If a Sortjet is being used, please tick this checkbox.
    *   **Technical info**: database field: `SORTJET`
*   **Maximum Weight (kgs)**: Maximum weight of all lites on the A rack. When this weight is reached, a new rack will be started. 0 means that there is no weight limit.
    *   **Technical info**: database field: `GEWICHT`
*   **ID for Stack Opti**: If you work with the Stack Optimizer, the ID of the physical storage location used is stored here. The application gets the possible values from the configuration files of the Stack Optimizer.
    *   **Technical info**: database field: `STACK_ID`

#### Description of fields in section Harp Racks

*   **Combo box**: The combo box below the buttons [Add], [Delete] and [Rename] shows the names of the harp racks defined.
*   **Number of slots**: This field defines the number of slots on the rack. If there is one slot per number, the number of slot numbers matches the number of slots on the rack.
    *   **Technical info**: database field: `FACHANZAHL`
*   **Width**: This field defines the width of the slots.
    *   **Technical info**: database field: `BREITE`
*   **Two slots/number**: This checkbox defines whether two lites each shall get a common slot number. In this case, there are twice as many slots than there are slot numbers. This means that two lites can be put into the same slot.
    *   **Technical info**: database field: `FACH_PRO_NR`
*   **Start = 0**: The checkbox defines whether the slot numbers will be counted from 0, or from 1.
    *   ✅ The slot numbers will be counted from 0.
    *   ⬜ The slot numbers will be counted from 1 (default).
    *   **Technical info**: database field: `STARTFACH`
*   **Slot number digits**: This radio button defines the number of digits of the rack number to be reserved for slot numbers.
    *   2 means that the last two digits are reserved.
    *   3 means that the last three digits are reserved.
    *   4 means that the last four digits are reserved.
    With 50 slot numbers, this will be 2 digits, starting from 100 slot numbers, 3 digits, etc.
    *   **Technical info**: database field: `DIGITSFACH`
*   **Max. number of harp racks**: The maximum number of harp racks is essential for the creation of optimization groups. When a glass type reaches the maximum quantity, the current optimization group will be closed for all optimizations, and a new one will be started. This can be cut once the racks are empty.
*   **Check quantity (cutting)**: The checkbox refers to the value in field **Max. number of harp racks** and checks this if necessary.
    *   ✅ The value in field **Max. number of harp racks** will be checked. An error message appears if this is exceeded. In this case, detailed scheduling can neither be optimized, nor saved.
    *   ⬜ There will be no quantity check.
*   **Sortjet**: If a Sortjet is being used, please tick this checkbox.
    *   **Technical info**: database field: `SORTJET`
*   **Maximum weight (kgs)**: Maximum weight of all lites on the harp rack. When this weight is reached, a new rack will be started. 0 means that there is no weight limit. If you enter 0, the number of lites to be put onto the harp rack will be limited only by the number of slots.
    *   **Technical info**: database field: `GEWICHT`
*   **Empty weight (kg)**: Empty weight of rack in kilogram.
    *   **Technical info**: database field: `LEERGEWICHT`
*   **Distance first/last slot from axis**: Distance between outer edge and axis (left/right).
    *   **Technical info**: database field: `ABSTAND_FACH_ACHSE`
*   **Max. deviation center of gravity fr. middle (%)**: Permitted deviation from center of gravity from middle in percent (+/-).
    *   **Technical info**: database table: `ABWEICHUNG_SP`

#### Description of the fields in section Fixed Racks

*   **Combo box**: The combo box below the buttons [Add], [Delete] and [Rename] shows the names of the fixed racks defined.
*   **Stacking depth**: Enter the rack depth in mm. Example: 1200 mm means that the stack can be up to 1200 mm deep. Please note that rack depths over 20 m will automatically be treated like unlimited rack depths.
    *   **Technical info**: database field: `TIEFE`
*   **Width**: This field defines the total width of the rack in mm. 2000 mm for example means that lites can be stacked on the rack up to a width of 2000 mm.
    *   **Technical info**: database field: `BREITE`
*   **Max. number of fixed racks**: The maximum number of fixed racks is essential for the creation of optimization groups. When a glass type reaches the maximum quantity, the current optimization group will be closed for all optimizations, and a new one will be started. This can be cut once the racks are empty.
*   **Quantity check (cutting)**: The checkbox refers to the value in field **Max. number of fixed racks** and checks this if necessary.
    *   ✅ Checks the value in field **Fixed racks**. An error message appears if this is exceeded. In this case, the detailed scheduling job can neither be optimized, nor saved.
    *   ⬜ There will be no quantity check.
*   **Maximum weight (kgs)**: Maximum weight of all lites on the fixed rack. When this weight is reached, a new rack will be started. 0 means that there is no weight limit.
    *   **Technical info**: database field: `GEWICHT`

**More information on racks**
*   ⇨ Tutorial, "Storage Locations" on page D-286
*   ⇨ Overview, "Buttons" on page A-90

### Lots

Dialog **Lot types and processings** serves to make the settings for the lot creation for a lot type. Processing or related processing will then be allocated to the lot type.

#### Lot Types and Processings

The dialog consists of three tabs:
*   Lot Types Tab
*   Processings Tab
*   Implicit Processing Tab

**Lot Types Tab**
`Master data > Detailed scheduling > Lot types`

[Image: Fig. D-60 - The Lot types and processings dialog, showing the Lot types tab.]

Use this dialog to define new lot types, or change existing ones.

**Technical info**: database table: `FEIN_LOSTYP`

**Description of fields**

*   **Lot type/name**: The view shows all defined lot types including lot type numbers and names. Detailed scheduling saves the lot type number in the database. The lot type name is used in the detailed scheduling views.
*   **Name/Type/Procurement**: The view shows all combinations of Processing type and Procurement allocated to this lot type. Double-click on an entry to switch to the appropriate page in the dialog, and view the processing. An asterisk (*) behind an entry in column Type marks a related processing.
*   **Lot type(-number)**: The lot type number must be equal or bigger than 100, and also the multiple of 10. The reason for this is that for application lots, the lot number is raised by one, and saved in the database. Detailed scheduling will also save the lot type number in the database.
    *   **Technical info**: database field: `LOSTYP`
*   **Name**: This field shows the lot type name used in the detailed scheduling views.
    *   **Technical info**: database field: `NAME`
*   **Grouping**: The combo box contains all defined groups. This group can be used to distribute lites of the same lot type to different production lots. Without such a group, lots will be created only for real machines. When a group is defined, the production lots for IG e.g. can be assembled according to airspace (AIR). The group key only has to include the element "airspace" (AIR). An important exception is cutting. For cutting purposes, lots are always assembled by glass type, glass thickness, and real tables. The groups are defined in master data.
    *   **Technical info**: database field: `GRUPPIERUNG`
    > **Grouping**
    > Groups can be used to form production lots. Application lots will be created by lots type only.
*   **Technology type**: The combo box shows all defined machine types. The machine type comes from machinery allocation. The machine type can be **0** if none has been allocated.
    *   **Technical info**: database field: `TECHNOTYP`
*   **Production sequence**: The combo box shows all defined groupings. For related processing steps, the production sequence of the original processing will be used as a rule. You can use the **Production sequence** to define an individual sequence. Should the set production sequence allow freedom with regards to the sequence, the direct or reversed sequence of the original processing will be used, depending on the checkbox **Reverse sorting**.
    *   **Technical info**: database field: `PROD_RF`
*   **Reverse sorting**: This checkbox is active only if the combo box **Production sequence** shows the entry (unequal `None`). See explanation.
    *   **Technical info**: database field: `INVERT_RF`

