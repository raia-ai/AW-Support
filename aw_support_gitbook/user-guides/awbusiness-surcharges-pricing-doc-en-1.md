---
title: "EN_AWBusiness_Master_Data_9_4-1"
source: "EN_AWBusiness_Master_Data_9_4-1.pdf"
tags: ["A+W Business Master Data", "Surcharges", "Pricing", "Shape Processing", "Miscellaneous Surcharges", "Automatic Surcharges", "Software Tutorial", "Glass Processing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial from the A+W Business Master Data guide, focusing on the configuration and function of various surcharges within the system. It covers shape surcharges, miscellaneous surcharges, and automatic surcharges, providing detailed instructions, examples, and exercises."
long_description: "This document serves as a comprehensive guide to understanding and implementing surcharges in the A+W Business Master Data software. It is structured as a tutorial, divided into three main sections: Shape Surcharges, Miscellaneous Surcharges, and Automatic Surcharges. The first section explains how to apply additional charges for processing non-rectangular lites (shapes), based on factors like edge length, surface area, or piece count. It provides step-by-step instructions on defining these surcharges, including screenshots of the user interface and explanations of segment-based calculations. The second section details Miscellaneous Surcharges, which are applied in addition to other charges for special cases like oversizes, small quantities, transport, or specific material thicknesses. It includes numerous examples and tables illustrating how these surcharges are calculated based on different types (e.g., Basic Price, Basic Item, Previous Processing). The final section introduces Automatic Surcharges, which are used for costs like transport or waste disposal and are added as separate line items to an order. The document explains their function, how they are allocated, and how they interact with product and customer master data. Throughout the tutorial, practical exercises and detailed calculation examples are provided to solidify the user's understanding."
---

# Surcharges

---
## Function of Shape Surcharges for Processing Steps

For the additional work in connection with the processing of non-rectangular lites (shapes), a surcharge is defined which is applied to the original processing price.

This surcharge can be calculated based on the following surcharge types:
- Edge length, e. g. for edgework
- Surface, e. g. for screen printing, enamel
- Piece, e. g. for corners, drill holes

*Fig. B-187 Processing surcharges for shapes*
*(Image shows a 'Shape Surcharges' dialog box with fields for Processing, Surcharges, and a Shape Sketch.)*

**A** Prices for shapes (glass of different product groups)
**B** Surcharge for processing the segments of a shape
**C** Shape number

In this example, calculation is based on the gross price of the processing (A).

The surcharge always applies to a certain shape (C) from the shape catalog. Since the surcharge is applied to the individual segments (B) of a shape, different surcharges can be entered per segment. Depending on the selected processing, the values in the segment fields refer to the corner or to the edges.

This example shows that the processing of edges 1 and 4 (red numbers outside the sketch) will incur no additional work. Edges 2 and 3 can only be processed manually. The numbers of the corners are green (inside the sketch).

## Defining a Shape Processing Surcharge

Shape processing surcharges are applied to non-rectangular lites. This surcharge is applied to the processing price.

### How to enter a processing surcharge for shapes

1.  Go to menu **Master data > Prices > Shape surcharges**.
    Dialog **Shape processing surcharges** appears.
2.  Go to the menu **Start > New** to switch to the input mode.

*Fig. B-188 Fields for the new shape processing surcharge are accessible*
*(Image shows an empty 'Shape Surcharges' dialog box, with fields ready for input.)*

**A** Select the price table (processing)
**B** Rate
**C** Price or surcharge type
**D** Enter the shape number

3.  Select the price table (A) for the processing to which a shape surcharge shall be applied.
4.  Select the rate (price list, key) (B).
    These surcharges must be entered in the same rate in which the processing prices have been entered. If you have got several rates for processing, you have to define the shape surcharge for every rate.
5.  Select the price type (C).
    Selection of the price type (surcharge type) is restricted to a proportional increase (Gross %), to the edge length (lin.m), and to the quantity (pcs.).
6.  Enter the shape number (D) and proceed by pressing the `<Tab>` key.
    The shape data are imported. The segment numbers of the edges and/or corners to be processed are marked on the shape sketch. The corresponding fields will be released.

*Fig. B-189 Segment fields per edge/corner accessible*
*(Image shows the 'Shape Surcharges' dialog box after a shape number has been entered, making segment fields active.)*

**A** Minimum values for price and quantity
**B** Segment fields
**C** Numbering of edges and corners

7.  Enter the surcharge for the individual segments (B).
    Edgework defined in the order refers to the edges. If rounded corners are entered, the corresponding values apply to the corners.
8.  Enter a minimum price and/or a minimum quantity (A).
    These are mandatory fields which must be filled in.
    If you do not want to define minimum values, enter 1 in both fields. This price and quantity will always be reached. Both values can be amended later.
9.  Select in the menu **Start > Save** to save the data.
    The data will be saved. The new surcharge appears on the list.

## Exercises

- Decide which shape processing results in additional work:
  - Drill holes?
  - Coating?
  - Edgework?
  - Corner processing?
- Enter a processing surcharge for the following shapes:
  - Trapezium (5)
  - Triangle (20)
  - Hexagon (22)

The shape numbers are shown in brackets. Define the segments which cause additional work in connection with certain processing steps. How does this affect the surcharge (amount)?

**Additional information**
⇨ Software Reference, "Shape Processing Surcharges" on page B-697

# Miscellaneous Surcharges

## Objectives

- Introducing the function of the so-called miscellaneous surcharges.
- Introducing surcharge types and how they are calculated.
- Defining a miscellaneous surcharge.

## Benefit

- Miscellaneous surcharges can be applied in addition to other surcharges. They refer either to a product or will be applied in general.
- Energy surcharge-, transport/toll-, spacer-, small/oversize-, minimum quantity-, thickness surcharges are defined as miscellaneous surcharges.

## Note

| Term | Description |
| :--- | :--- |
| **Surcharge type** | The surcharge type defines how the surcharge is going to be calculated. |
| **Graduation** | The graduation of a miscellaneous surcharge is analysed in the sequence which appears in the dialog. A new limit will always be added at the end of the list even it has been defined with smaller limits. |
| **Reference** | Miscellaneous surcharges always refer to the basic price. They can be transferred within a BOM. |
| **Surcharge type** | Apart from referring to the basic item, proportional values can be used. The rule is: Gross price = before deduction of discounts. Net price = after deducting the discounts. |
| **Other surcharges for BOM elements** | The calculation of other surcharges by surcharge type can be switched off in general in company data for BOM elements for which such a surcharge has been defined in product master data. |
| **Display in the order** | Other surcharges are implicit only, i.e. they do not appear on the order. |

## The Function of Miscellaneous Surcharges

These surcharges are defined to be able to handle special cases, e. g. oversizes or especially small sizes. These surcharges are always applied to the standard price. They are always implicit, i. e. they are not stated in the order.

*Fig. B-190 Examples of miscellaneous surcharges*
*(Image shows the 'Misc. Surcharges' dialog with a list of defined surcharges like 'Oversize', 'Spacer variants', 'Edge length', etc.)*

Miscellaneous surcharges can be allocated in the following dialogs:
- **Product management > tab Price/surcharge:**
  The surcharge will always be applied even if other prices are used for calculation.
- **Prices > tab Price selection:**
  The surcharge will be applied only if this price is selected.
- **Group surcharges:**
  The surcharge will be applied whenever a price is determined by means of the price group, with a group surcharge.
- **Exchange surcharges > tab General, by thickness, by product:**
  The surcharge will be applied whenever an exchange surcharge is calculated.
- **Customer-, supplier discounts > tab Differences:**
  The surcharge will be applied if different discounts have been agreed with the partner.

> **Miscellaneous surcharges will be applied twice**
> If A+W Business detects a miscellaneous surcharge both for the price and for the product, both will be applied.

## Dialog Miscellaneous Surcharges

You can display a list of miscellaneous surcharges in dialog **Miscellaneous surcharges**.

*Fig. B-191 Dialog Miscellaneous surcharges*
*(Image shows the 'Misc. Surcharges' dialog, focusing on the table view for a specific surcharge, with columns for limits, types, and amounts.)*

**A** Surcharge table number
**B** Graded allowance
**C** Limit (1, 2)
**D** Limit type (1, 2)
**E** Take one or both limits into account
**F** Surcharge amount
**G** Unit to which the surcharge refers
**H** Surcharge type
**I** Validity in connection with manual price changes

If you are using two different limit types for graduation you have to define whether these shall be analysed together or alternatively (E):
- If you tick the checkbox, the surcharge will be applied to the limit that has been reached in the order. This can be limit 1 or limit 2.
- If this checkbox is not ticked, the surcharge will be applied only if both limits are reached.

Unlike shape-, grill- or exchange surcharges, miscellaneous surcharges will only be taken into account in case of manual price changes if they have been explicitly released (I).

### Example 1: Spacer surcharge

Example 1 shows a simple graduation with one limit type which is applied to the spacer.

| up to limit 1 (mm) | Limit type 1 | or | up to limit 2 | Limit type 2 | Surcharge | Price unit |
| :--- | :--- | :- | :--- | :--- | :--- | :--- |
| 12 | AIR | | | | 0.00 | Net % |
| 16 | AIR | | | | 5.00 | Net % |
| 20 | AIR | | | | 10.00 | Net % |

The following example shows one surcharge with two limit types.

### Example 2: Edge length surcharges

Example 2 shows two different surcharges for the edge length. The first edge length surcharge is e. g. applied whenever the lite exceeds a certain size and cannot be handled by one person alone. The OR connection in the second example means that the surcharge will be applied if either the defined width or the defined height is exceeded. The limit types can be exchanged in this case.

| up to limit 1 (mm) | Limit type 1 | or | up to limit 2 (mm) | Limit type 2 | Surcharge | Price unit |
| :--- | :--- | :- | :--- | :--- | :--- | :--- |
| 2000 | Width | | 2000 | Height | 0.00 | Net % |
| 9999 | Width | | 9999 | Height | 20.00 | Net % |
| 2000 | Width | or | 3500 | Height | 0.00 | Basic item (n. add.) |
| 9999 | Width | or | 9999 | Height | 20.00 | Basic item (n. add.) |

### Example 3: Thickness surcharge

In example 3, a surcharge is applied to the lite thickness which can be used e. g. for drilling. If the lite thickness is 10 mm or lower, no surcharge will be applied. A surcharge of 35.00 €/sqm will be applied to all thicker lites.

| up to limit | Limit type | Surcharge | Unit | Surcharge type |
| :--- | :--- | :--- | :--- | :--- |
| 10 | Thickness | 0.00 | Gross % | Basic price (n. add.) |
| 9999 | Thickness | 35.00 | Gross % | Basic price (n. add.) |

### Example 4: Small quantity surcharge

Example 4 shows a graduated surcharge for lites smaller than 0.5 sqm. In a first step, a surcharge of 100% will be applied if the lite surface is below 0.1 sqm. This surcharge is reduced in the next two steps to 50% and 30% for a surface of up to 0.15 sqm or up to 0.5 sqm respectively. No surcharge will be applied to lites larger than that.

| up to limit | Limit type | Surcharge | Unit | Surcharge type |
| :--- | :--- | :--- | :--- | :--- |
| 0.1 | sqm | 100.00 | Gross % | Basic price |
| 0.15 | sqm | 50.00 | Gross % | Basic price |
| 0.5 | sqm | 30.00 | Gross % | Basic price |

The surcharge type defines how the surcharge is going to be calculated. Surcharge types and the calculation are described in detail - including examples - in the following chapters.

## Surcharge Types

Surcharge types define the basis on which the corresponding surcharge shall be calculated:
- **Basic item:**
  For the top element (product) on the BOM to which a surcharge can be allocated as well
- **Basic item + processing:**
  For the top element on the BOM and all corresponding processing steps.
- **all previous processing steps:**
  For all processing steps executed before the selected BOM element.
- **all previous items:**
  For all elements listed in the BOM before the selected element.
- **Basic item + shape:**
  For the top element on the BOM and the corresponding shape.
- **Basic price:**
  For the price of the top element of the BOM.
- **previous processing:**
  All processing steps listed before the element for which the surcharge has been defined.
- **Parent + its lites:**
  For the top element of an assembly (parent) and the lites of this assembly.
- **Parent + its previous processing:**
  For the top element of an assembly (parent) and the processing attached to this element.
- **previous BOM with same parent:**
  All elements of the assembly.
- **Curr. processing:**
  For the selected BOM element only.
- **Basic item without other surcharges:**
  For the top element on the BOM without the surcharge that may be allocated to the product.
- **Complete item:**
  The surcharge is applied to the whole order item.

All surcharge types can be defined as **additional** or **non-additional**. The additional or non-additional calculation only refers to proportional surcharges however.

In case of **non-additional** calculation, the previous surcharge will not be taken into account for calculating the next surcharge.

In both cases, the resulting value serves as the basis for calculating the proportional surcharge.

**Example**

| | Basic price 100.00 € | |
| :--- | :--- | :--- |
| | **additional** | **non-additional** |
| Shape surcharge + 20% | + 20.00 € | + 20.00 € |
| **Subtotal** | **= 120.00 €** | |
| Coating + 25% | + 30.00 € | + 25.00 € |
| **Total** | **= 150.00 €** | **= 145.00 €** |

## Calculation by surcharge type

The surcharge type is chosen in dialog **Miscellaneous surcharges** by means of the Surcharge type. The gross price is the price prior to deduction of discounts while the net price is the price after deduction of discounts.

The following examples show eight versions of calculating surcharges.

> **Fictitious prices**
> The prices in the examples are fictitious. They have been chosen to make the calculation examples easier to understand.

### Example 1: Basic price

Gross or net surcharge on the price of the main item.

**Tab. B-4 Surcharge type Basic net price**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 25.00 | 50% | **25.00** |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 0.5 sqm | 50.00 | | 0% | 50.00 |
| Shape | Basic price (n.add.) | Net % surcharge | 100% | 25.00 | 100% of 25.00 | 0% | 25.00 |
| | | | | | | | **100.00** |

### Example 2: Basic item

Gross or net surcharge on the price of the main item including exchange surcharges.

**Tab. B-5 Surcharge type Basic gross price**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | **50.00** | 50.00 | 50% | 25.00 |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 0.5 sqm | **50.00** | 50.00 | 0% | 50.00 |
| Shape | Basic item (n.add.) | Gross % surcharge | 100% | 100.00 | 100% of 100.00 | 0% | 100.00 |
| | | | | | | | **175.00** |

**Tab. B-6 Surcharge type Basic net price**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 25.00 | 50% | **25.00** |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 0.5 sqm | 50.00 | 50.00 | 0% | **50.00** |
| Shape | Basic item (n.add.) | Net % surcharge | 100% | 75.00 | 100% of 75.00 | 0% | 75.00 |
| | | | | | | | **150.00** |

### Example 3: Basic item + processing

Shape surcharge on the basic item and all processing steps with surcharge type Basic item (additional).

**Tab. B-7 Surcharge type Basic item + Processing (added)**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 2 sqm | 200.00 | 100.00 | 50% | **100.00** |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 2 sqm | 200.00 | 200.00 | 0% | **200.00** |
| UV edge connection | Basic item | (add.) 1 lin.m at 4.00 | 6 lin.m. | 24.00 | 12.00 | 50% | **12.00** |
| Shape | Basic item + process. | Net % surcharge | 100% | 312.00 | 100% of 312.00 | 0% | 312.00 |
| | | | | | | | **624.00** |

**Tab. B-8 Surcharge type basic item + processing (not additional)**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 2 sqm | 200.00 | 100.00 | 50% | **100.00** |
| 1st lite = Float | | | | | | | |
| 2nd lite = TG | | Exchange surcharge 1 sqm at 100.00 | 2 sqm | 200.00 | 200.00 | 0% | **200.00** |
| UV edge connection | Basic item | (n.add.) 1 lin.m at 4.00 | 6 lin.m. | 24.00 | 12.00 | 50% | 12.00 |
| Shape | Basic item + process. | Net % surcharge | 100% | 300.00 | 100% of 300.00 | 0% | 300.00 |
| | | | | | | | **612.00** |

### Example 4: Basic item + shape

If the surcharge Inside pattern shall be applied to the basic item and the shape, you have to chose an additional surcharge type for the shape.

**Tab. B-9 Surcharge type Basic item + Shape**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IG | | 1 sqm at | 0.5 sqm | 50.00 | 25.00 | 50% | **25.00** |
| 1st lite = Float | | | | | | | |
| 2nd lite = patterned | | Exchange surcharge 1 sqm at 50.00 | 0.5 sqm | 25.00 | 25.00 | 0% | **25.00** |
| Grill | | 1 pc. at 50.00 | 1 pcs. | 50.00 | | 10% | 45.00 |
| Shape | Basic item + process. | (add.) Net % surcharge | 100% | 50.00 | 100% of 50.00 | 0% | **50.00** |
| Pattern inside | Basic item + shape | Net % surcharge | 10% | 10.00 | 100% of 100.00 | 0% | 10.00 |
| | | | | | | | **155.00** |

### Example 5: Previous processing

Oversize surcharge for edgework, the input sequence is important. The surcharge will be applied only to the previous processing step.

**Tab. B-10 Surcharge type Previous processing**

| Product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Single annealed | | 1 sqm at 100.00 | 4 sqm | 400.00 | | 50% | 200.00 |
| Edgework | Basic item | (add.) 1 lin.m at 15.00 | 8 lin.m. | **120.00** | 120.00 | 5% | 114.00 |
| Over-size surcharge | Previous processing | (add.) Gross % surcharge | 10% | 12.00 | 10% of 120.00 | 0% | 12.00 |
| | | | | | | | **326.00** |

### Example 6: All previous items

Surcharge type in connection with work performed, e.g. surcharge Surcharge.

**Tab. B-11 Surcharge type All previous items – surcharge**

| Item/ product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 001/IG | | 1 sqm at 100.00 | 0.5 sqm | 50.00 | 40.00 | 20% | **40.00** |
| 002/TG | | 1 sqm at 90.00 | 1.2 sqm | 108.00 | 86.40 | 20% | **86.40** |
| 003/LG | | 1 sqm at 80.00 | 2 sqm | 160.00 | 160.00 | 0% | **160.00** |
| 004/single annealed | | 1 sqm at 50.00 | 1.4 sqm | 70.00 | 42.00 | 40% | **42.00** |
| 005/Surcharge | All previous items | (add.) Net % surcharge | 20% | 328.40 | 20% of 328.40 | 0% | 65.68 |
| | | | | | | | **394.08** |

If the surcharge is entered with a negative sign, it will be applied as a discount, e.g. special discount.

**Tab. B-12 Surcharge type all previous items - Special discount**

| Item/ product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 001/IG | | 1 sqm at 100.00 | 0.5 sqm | 50.00 | 40.00 | 20% | **40.00** |
| 002/TG | | 1 sqm at 90.00 | 1.2 sqm | 108.00 | 86.40 | 20% | **86.40** |
| 003/LG | | 1 sqm at 80.00 | 2 sqm | 160.00 | 160.00 | 0% | **160.00** |
| 004/single annealed | | 1 sqm at 50.00 | 1.4 sqm | 70.00 | 42.00 | 40% | **42.00** |
| 005/Special discount | All previous items | (add.) Net % surcharge | -20% | 328.40 | 20% of 328.40 | 0% | -65.68 |
| | | | | | | | **262.72** |

### Example 7: Additional calculation

The surcharges for edgework and hole drilling are additional ones: Basis for calculating the proportional surcharge (shape) is the basic price plus the surcharges for edgework and drilling.

**Tab. B-13 Surcharge; additional calculation**

| Item/ product | Surcharge type | Price/ price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Single annealed | | 1 sqm at 100.00 | 1 sqm | 100.00 | 80.00 | 20% | **80.00** |
| Edgework | Basic item | (add.) 1 lin.m at 5.00 | 4 lin.m. | 20.00 | 20.00 | 0% | **20.00** |
| Drill hole | Basic item | (add.) 1 pc. at 30.00 | 1 pcs. | 30.00 | 30.00 | 0% | **30.00** |
| Shape | Basic item + process. | (n.add.) Net % surcharge | 50% | 65.00 | 50% of 130.00 | 0% | 65.00 |
| | | | | | | | **195.00** |

### Example 8: Non-additional calculation

The surcharges for edgework and hole drilling are non-additional ones: Basis for calculating the proportional surcharge (shape) is the basic item without edgework and drilling.

**Tab. B-14 Surcharge; non-additional calculation**

| Product | Surcharge type | Price/price unit | Quantity | Gross price/ piece | Calculation basis for proportional surcharge | Discount | Net price/ piece |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Single annealed | | 1 sqm at 100.00 | 1 sqm | 100.00 | 80.00 | 20% | **80.00** |
| Shape | Basic item + process. | (n.add.) Net % surcharge | 50% | 50.00 | 50% of 80.00 | 0% | 40.00 |
| Edgework | Basic item | (n.add.) 1 lin.m at 5.00 | 4 lin.m. | 20.00 | | 0% | 20.00 |
| Drill hole | Basic item | (n.add.) 1 pc. at 30.00 | 1 pcs. | 30.00 | | 0% | 30.00 |
| | | | | | | | **170.00** |

### Calculating surcharges for processing

If no length surcharge has been defined for a limit, all lites up to this limit will be calculated without a surcharge. Likewise, all airspaces up to 12 mm are calculated without a surcharge in example Limits for miscellaneous surcharges.

**Calculation of additional surcharges:**
```
Edgework                      4 lin.m x 6.25 €    25.00 €
Misc. surcharge Processing index 1  50% net on 25.00 €    12.50 €
Misc. surcharge Thickness 9 mm      10% net on 37.50 €     3.75 €
------------------------------------------------------------------
Total price of the processing                         41.25 €
```

**Calculation of non-additional surcharges:**
```
Edgework                      4 lin.m x 6.25 €    25.00 €
Misc. surcharge Processing index 1  50% net on 25.00 €    12.50 €
Misc. surcharge Thickness 9 mm      10% net on 25.00 €     2.50 €
------------------------------------------------------------------
Total price of the processing                         40.00 €
```

### Transfer of surcharge types

Depending on the surcharge type chosen, the surcharge is calculated for the BOM elements.

*Fig. B-192 Transfer of surcharge type in the BOM*
*(Image shows a diagram illustrating how a surcharge for 'Processing 2' can be applied to different elements of a Bill of Materials (BOM), such as 'Parent + glass', 'Previous BOM, same parent', 'Parent + previous processing', and 'Previous processing'.)*

This example shows the previous BOM elements to which the surcharge defined for processing 2 will be applied. The surcharge for processing 2 is applied to the laminated lite and the two single annealed lites for example if the surcharge type **Parent + glass** has been chosen.

## Defining a Miscellaneous Surcharge

Two limit types can be taken into account per record; the limit types can change from record to record.

> **Calculation of miscellaneous surcharges**
> Pricing of orders takes into account the sequence in which the discount levels are defined. This sequence can influence the calculation considerably. If e.g. the unit surcharge appears last instead of first, the resulting sqm prices will differ.
>
> **Example: 100 pcs. at 0.1 sqm / sqm at 100.00 (Euro)**
>
> | Sequence (Unit Surcharge First) | Amount | Sequence (Surface Surcharge First) | Amount |
> | :--- | :--- | :--- | :--- |
> | Basic amount | 100.00 € | Basic amount | 100.00 € |
> | Unit surcharge | + 35.00 € | Surface surcharge 100% | + 100.00 € |
> | **Total** | **135.00 €** | **Total** | **200.00 €** |
> | Surface surcharge 100% | + 135.00 € | Unit surcharge | + 35.00 € |
> | **sqm price for calculation** | **270.00 €** | **sqm price for calculation** | **235.00 €** |
>
> Therefore, please make sure to define new surcharge levels so that pricing meets your requirements.
> To enter several steps for a surcharge you should first define the correct sequence on a piece of paper.

There are the following instructions on this subject.
- "How to define a new surcharge" on page B-319
- "How to enter more steps for grading the surcharge" on page B-321
- "How to delete a step of the graduation" on page B-322

### How to define a new surcharge

1.  Go to menu **Master data > Prices > Misc. surcharges**.

    *Fig. B-193 View of a comparable surcharge*
    *(Image shows the 'Misc. Surcharges' dialog, displaying an existing surcharge table for 'Edge length surcharges'.)*

    If surcharges have been entered already, the values of the first surcharge (from tab Table) are shown. You can use the arrow keys to search for a surcharge that meets your expectations.
    If no surcharges have been defined yet you have to fill in all fields by hand.
2.  Go to the menu **Start > New** to switch to the input mode.

    *Fig. B-194 Release the fields for a new surcharge*
    *(Image shows the 'Misc. Surcharges' dialog in new entry mode, with fields for Number and Name ready for input.)*

    The fields are preset with the entries of the selected surcharge.
3.  Enter the number (A) and the name (B) of the new surcharge.
    To do so, change the entries in the two fields if these are preset.
4.  Position the cursor on the first field (A) of the list and change the entry.
5.  Press the `<Tab>` key to proceed to the next field (B) and choose the limit type.
6.  Edit all fields for the first entry in this way.
7.  Tick the checkbox **Valid for price definition** (F) if the surcharge shall also be applied if the price is changed manually.
8.  Select in the menu **Start > Save** to save the data.
    The data will be saved. You can now enter further steps for the graduation.

*Fig. B-195 Amend preset values*
*(Image shows a dropdown list for the 'Limit type 1' field, with options like 'Thickness', 'Diameter', 'Maximum edge length', etc.)*

**A** First value of limit type 1
**B** Limit type 1
**C** Surcharge amount
**D** Calculation unit
**E** Surcharge type
**F** Application of manual prices

### How to enter more steps for grading the surcharge

1.  Select the surcharge you want to edit.
2.  Open the context menu by a right mouse click on the line header.

    *Fig. B-196 Context menu for adding the next step of the graduation*
    *(Image shows a right-click context menu on a surcharge line, with 'Insert' and 'Delete' options.)*

3.  Select the entry **Insert (B)**.
    A new line is added at the end of the list. All fields except the first are preset by the entries from the previous line.

> **No sorting of entries**
> You cannot change the sequence of the surcharge levels. To put an entry before an existing one, you have to create all entries in the required sequence then delete the old ones.

*Fig. B-197 New line*
*(Image shows a new, empty line added to the surcharge table, ready for data entry.)*

4.  Enter the new limit and amend the entries in the other fields if necessary.
5.  Enter the required surcharge levels, e.g. three levels for a surcharge for overlong edges.
6.  Select in the menu **Start > Save** to save the data.
    The data will be saved. To apply the surcharge automatically, allocate the table number to the product or the price. It can also be entered manually in the order.

### How to delete a step of the graduation

1.  Select the surcharge to be edited.
2.  Open the context menu by a right mouse click on the line header.
    The context menu appears.
3.  Select the entry **Delete**.

    The line header is marked by an X.
4.  Go to menu **Start > Save**.
    A security query appears.
5.  Acknowledge the query by [Yes].
    The data will be deleted.

> **Deleting a table**
> If you select **Start > Delete**, the entire surcharge (the table) will be deleted.

## Exercises

- Enter a simple surcharge for lites which shall be applied if the weight exceeds 30 kg.
- Define a surcharge based on the edge length and the surface.
- Enter at least two steps for the edge length surcharge.
- Delete one of the graduations without deleting the whole table.

**Additional information**
⇨ Tutorial 2, "Available Limit Types" on page B-519
⇨ Software Reference, "Miscellaneous Surcharges" on page B-664

# Automatic Surcharges

## Objectives

- Introducing the automatic surcharge/discount function.
- Enabling automatic surcharges in master data.
- Defining an automatic surcharge.

## Benefit

- The so-called automatic surcharges are normally used for charging costs incurred e. g. through transport, waste disposal or similar things.
- These costs are defined as surcharges and entered in the document as a separate item, like any other product.

## Note

| Term | Description |
| :--- | :--- |
| **Automatic surcharges** | Automatic surcharges are displayed in partner management, product management, and in the order in section Surcharges/discounts. They can be used as surcharges or special discounts. They will be automatically added to the documents only if they have been enabled in product and customer master data. Surcharges or special discounts are treated like products and are entered as separate order items. |
| **Product allocation** | An automatic surcharge is defined as a product with its own price table (unit price) and is allocated to one of the available surcharges/discounts. |
| **Surcharge or discount** | Based on the unit price, a surcharge or discount is applied. |
| **Application** | A+W Business adds the automatic surcharges as order items when the order is saved. |
| **Calculation in the document** | The automatic surcharge refers to a single order item or to the whole order. |
| **Position in document** | The item number in the document defines the point at which the automatic surcharge will be added. Based on the item number in the document and by means of the surcharge type selected at product definition, a discount/surcharge can be applied to another discount/surcharge. This means that a special discount can be applied to the entire order, including the automatic toll surcharge. |

## The Function of Automatic Surcharges

For every product and every customer you can define one or more automatic surcharges which will always be applied. These automatic surcharges can e. g. be used as surcharges for transport-, toll fees, energy costs, or as special discounts. These surcharges can be defined for a customer or in general.

Surcharges or special discounts are treated like products and are entered as separate order items.

Surcharges/special discounts are defined acc. to the following rules:
- They are entered as products.
- They are always allocated to the product type and product group **Services/surcharges**.
- Basically, they have their own price table.
- They have to be allocated to the surcharges/special discounts in dialog **Product allocation, surcharges**.

Surcharges/special discounts can be allocated several times, either in general or for special customers only.

There are ten so-called special discounts available which can be applied as a discount (with a negative sign) or a surcharge (with a positive sign). This is e. g. useful for special promotions which are only valid for a certain time.

*Fig. B-198 Product allocation of surcharges/special discounts*
*(Image shows a flowchart illustrating the allocation of automatic surcharges. A 'Product' (e.g., energy) with its own 'Price table' is allocated to 'Product allocation, surcharges'. This can be valid for a specific customer or in general and is enabled either in 'Partner management' or 'Product management'.)*

These surcharges are enabled in product or partner master data. Active surcharges/discounts are automatically entered as items in the document when the item entry dialog is closed. Automatic surcharges/discounts can be disabled in the order, or another one can be enabled.
