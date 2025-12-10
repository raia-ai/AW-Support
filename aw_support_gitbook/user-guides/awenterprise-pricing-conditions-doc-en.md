---
description: EN_AWEnterprise_Prises_Conditions_2.20
---

# A+W Prices and Conditions

***

## Introduction

This part of the documentation contains editorial notes.

### Revisions Overview

| Part Version / Date | Description                                          |
| ------------------- | ---------------------------------------------------- |
| 2.20/02-2023        | Various field descriptions updated.                  |
| 2.10/05-2019        | Complete revision of software reference.             |
| 2.00/07-2018        | Tutorial.                                            |
| 1.01/01-2017        | Product and company name adjusted.                   |
| 1.00/10-2016        | Prices and conditions removed from Master Data part. |

### Editorial

The Editorial provides information on the following topics:

* Notes on this document
* Copyrights
* Trademark
* Contacts

#### Notes on this document

This document is intended exclusively for end users of A+W Enterprise.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The descriptions in this document are based on the full program level of A+W Enterprise.

### Copyrights

© 2020 A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, either electronically, mechanically, or by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademark

All hardware and software names mentioned in this documentation can also be registered trademarks. Third party copyrights have to be obeyed.

### Contacts

A+W Software GmbH Am Pfahlgraben 4-10 D-35415 Pohlheim +49 6404 2051 0 +49 6404 2051 877 Zentrale@a-w.com http://www.a-w.com

## Tutorial

### Introduction

> The tutorial for the Prices and Conditions module focuses on the basic principles for cost calculation in A+W Enterprise. The tutorial builds on knowledge about the article master data.
>
> **The functions depend on the released modules** Please note that the individual functions are available only if the corresponding modules and interfaces have been released.
>
> If you find functions in this description that are not accessible in your installation, please contact A+W Software GmbH.

#### Subjects

This tutorial includes the following subjects:

* "Basic Concepts of Price Determination" on page C-17
* "Price Definitions" on page C-23
* "Price Master Data" on page C-56
* "Conditions" on page C-121
* "Master Data for Conditions" on page C-128
* "Complex exercise" on page C-151

#### Prerequisite knowledge

The tutorial is aimed at users who manage the master data for price calculation in A+W Enterprise.

These users have to be familiar with the concept of general master data and the operating elements with which functions are called up and started. The basic principles of operation are described in the Overview section.

#### Goal of the tutorial

* Understand the difference between prices and conditions.
* Edit and define prices and conditions in the master data.
* Understand price determination of order entry.

### Documentation

The following documents are available for the Prices and Conditions module:

| Format      | Scope                                                                               |
| ----------- | ----------------------------------------------------------------------------------- |
| PDF         | Complete documentation: Tutorial, Software reference                                |
| Online help | Context-sensitive dialog help of the A+W Enterprise software reference and tutorial |

### Structure of the tutorial

The tutorial consists of subjects with several training modules each. Each session consists of the following elements:

* **Overview**: Each training session starts with an overview of the major topics:
  * **Objectives**: What shall be conveyed?
  * **Benefit**: What can this knowledge be used for?
  * **Maxims**: Which correlations are to be remembered?
* **Concepts**: Concepts and terms of the training session in question will be explained first. These are followed by examples and operating instructions.
* **Exercises**: For some learning units, there are exercises where you can apply the sequences of actions described.

#### Reading instructions

The contents of a training session are based on the knowledge conveyed in the previous session. We therefore recommend that you do not skip any units.

If you are already familiar with a subject you should at least read the summary at the beginning of the unit in order to bring the main details to mind.

Note also that the individual dialogs are described in the software reference. There will not be detailed references to these descriptions below.

### Display conventions

Certain parts of the sentences are specially marked. The meanings are:

| Term      | Meaning                                                                                                          |
| --------- | ---------------------------------------------------------------------------------------------------------------- |
| _Italics_ | marks character strings describing the software elements, e. g. the _Price properties_.                          |
| **Bold**  | marks character strings to be entered via keyboard, e.g. **Enter 5**.                                            |
| >         | The "bread crumb trail" marks the path that you can use to open a dialog, e.g. Master data > Prices > IG Prices. |
| \[]       | Square brackets mark the buttons in the dialog, e.g. \[OK] to save the data.                                     |
| < >       | Pointed brackets refer to keys or shortcuts on the keyboard, e. g. is used to open the online help.              |

### Menu Overview

This section provides a brief overview of the program sections that will be addressed in the thematic blocks of this training.

_Master Data > System > User > Prices / Conditions menus_

#### Prices

With this menu, you can access all dialogs on which you specify the data for the prices:

* a - d: With these menu elements, you access the dialogs on which you create the prices and surcharges.
* e - g: With these menu elements, you access the dialogs on which you define the keys and price control.
* h: With this menu element, you access the dialog for selection of the list that should be printed.

#### Conditions

With this menu, you access all dialogs on which you specify the conditions for the calculation of the prices:

* a: With this menu element, you access the dialogs on which you create the general daily conditions and the product group conditions.
* b: With this menu element, you access the dialogs on which you create the special conditions.
* c: With this menu element, you access the dialogs on which you create special prices.

### Basic Concepts of Price Determination

Price determination in A+W Enterprise considers, in addition to the fixed article prices, also deviations, e.g. the exchange of glass in an IG article or additional processings. In order to cover all possibilities, there are various building blocks available that are consulted automatically, e.g. the prices for the glass articles, special surcharges or discounts, etc.

The goal of this tutorial is to explain the relationships of article master data, prices, and conditions.

In the order, an item with a more or less complex BOM can be entered without having to specify the prices for the components individually.

_Fig. C-2 Schematic structure of a simple IG lite_

This simplified example illustrates the BOM structure for an IG lite. How the price for such an item in the order is created will be explained in the following sections.

#### Glossary

| Term                | Explanation                                                                                                                                                                              |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Matrix**          | Two-dimensional price table with a matrix number, a name, and the values for the prices. The prices depend on the height and width. ⇨ "Matrix editor" on page C-60                       |
| **Vector**          | One-dimensional price table with a vector number, a name, and the values for the prices. The prices depend, for example, on the quantity or the area. ⇨ "Vector assignment" on page C-78 |
| **PCd**             | **PriceCode** The (logical) price code is a link to a PLCD. ⇨ "Price code (PCd)" on page C-26                                                                                            |
| **PLCD**            | **PriceListCode** The price list code is a physical price list that includes any number of matrices and vectors. ⇨ "Price List Code (PLCD)" on page C-25                                 |
| **Price key**       | Price keys are numbers and names for lists, matrices, and vectors. ⇨ "Price keys" on page C-24                                                                                           |
| **Pricing methods** | The pricing method controls how the price for the articles included in the order or the PO is calculated. ⇨ "Pricing methods" on page C-44                                               |
| **Item article**    | The item article is an article that is entered in the order or the PO, e.g. a LAMI article. The price for this article is calculated. It can include a BOM.                              |
| **PLCD logic**      | The PLCD logic specifies how prices should be searched for in the price lists. ⇨ "PLCD logics" on page C-35                                                                              |
| **Article**         | All articles are created in the master data, e.g. float 4 mm, IG 2 x 5 mm, arrissing.                                                                                                    |
| **Glass**           | The glass is always the material for a single lite, e.g. wired glass, float.                                                                                                             |
| **Lite**            | Lites are entered in the order item, and the price is calculated precisely for this.                                                                                                     |

### Characteristics of prices and conditions

#### Prices

* are organized in price lists.
* have a price type.
* are specified in currency units.

The prices are always assigned to the articles. However, they are not entered directly with the articles in the master data, but rather in separate matrices, article vectors, processing vectors, and exchange lists that are assigned to the articles.

#### Conditions

* follow a hierarchy.
* can include prices.
* can include surcharges and discounts.
* can include percentage details.

Conditions are assigned to market partners, customer groups or projects and are structured hierarchically. They are linked to the prices via a code.

### Price calculation in the order

In the order, products are entered for which a price is calculated. A product can include a BOM with articles. Generally standard structures have a price in which prices for the BOM articles are already included.

In addition, conditions can be defined in which current deviations are specified for the price calculation, e.g. surcharges on particular product groups or special prices for particular market partners.

_Fig. C-5 Assignments for the pricing_

This simplified illustration demonstrates how the prices are combined using the assignments of articles and market partners for the calculation for order items.

For the price calculation, A+W Enterprise searches for the prices for the product or for the prices for the BOM articles. Here, exchange glass, additions, and processings are considered. Then the current conditions are searched. The price is calculated from the results of these searches.

In the order itself, you can change this price per article, item or overall manually. In addition, you can also change the conditions in the order.

**Example**

* Price for the item article, e.g. IG 2 x 5 mm - price per square m.
* Price for sub-parts with exchange/additional flag, e.g. exchange glass, accessories, and processings. = Price of the product

### Article master data

The pricing method has to be specified in the master data for the article.

Per article, you specify in addition to the pricing method (B) whether a cash discount on the price can be granted (F). ⇨ "Pricing methods" on page C-44

If you are working with the Cost Calculation module, you can specify whether the article is consulted during cost calculation (E) and/or how the costs for the article are calculated. The cost calculation is described in a separate section. ⇨ "Cost Calculation" on page C-152

The price characteristics for processings and accessories (A) are listed under: Article > > Price Characteristics. These settings are only evaluated if the article is installed as subpart.

You can specify the price characteristics for the article, the article types, the A+W processing types or a combination of article and A+W processing type.

If the article has been assigned an A+W processing type, no record for the article types can be specified. The price characteristics are then evaluated in this sequence:

* Article
* Article and A+W processing types
* A+W processing types

If the article has not been assigned an A+W processing type, only one record for the article or article type can be specified.

For a detailed description of the dialogs, see the _Master Data_ section.

### IG and PCd prices

* For price calculation, A+W Enterprise distinguishes between IG articles and other glass.
* Non-IG glass and processings normally include price vectors.
* Prices for IG lites can be defined according to three different methods: in price matrices, in vectors or as individual lites.
* There are only exchange lists for IG and LAMI lites.

_Fig. C-7 IG and PCd prices_

Various price definitions interact for the exact calculation of a lite. For special orders, however, surcharges are charged, which are assigned to the articles, e.g. for processings on the corners and/or edges, for jumbos, for small lites. This means that all elements that can be entered in the order's BOM can have a price.

### Price Definitions

In this subject module, you will learn how with which components the prices are defined in A+W Enterprise. The components include the "tools" or keys, the price control, and the prices themselves.

This section provides information on the following subjects:

* "Price keys" on page C-24
* "PLCD logics" on page C-35
* "Pricing components" on page C-43

### Price keys

**Objectives**

* Get to know the difference between price keys and price definitions.
* Get to know function of the price keys.
* Understand the benefits of PCd and PLCD.
* Currencies

**Benefits**

* The master data for the pricing is defined in two steps. You can only fill a price matrix with prices, for example, if you have previously stored a key for this new matrix.

**Please note**

* **PLCD**: The PLCD is a (physical) price list in which any number of price matrices and price vectors are combined, e.g. all price lists that apply for the calculation of IG lites including exchange and processings.
  * The price list number is the numeric designation of a price list.
  * The PLCD is defined by a number, a name, and a currency.
  * The PLCDs are used to sort price lists.
  * Number is in ascending order.
* **PCd**: The (logical) price code (PCd) is a link to a physical price list (PLCD) with which the price list is assigned to a market partner.
* **Price keys**: Price keys are numbers and names for all lists, matrices, and vectors.
* **Matrix number**: The matrix number is a key number and name, which are assigned to a two-dimensional price table, the matrix.
* **Vector number**: The vector number is a key number and designation that is assigned to a one-dimensional price table. Keys for vectors are created separately:
  * Article
  * Processings.
* **Muntin assignment**: For the calculation of muntin articles, muntin price classes and muntin codes are assigned to one another.
* **Currency**: Prices in different currencies can only be used if the multi-currency capability is configured.

### Price List Code (PLCD)

The PLCD is a (physical) price list in which any number of price matrices and price vectors are combined, e.g. all price lists that apply for the calculation of IG lites including exchange and processings. The PLCD itself does not include any prices.

* The PLCD is defined by a number, a name, and a currency.
* The PLCDs are used to sort price lists.
* Number is in ascending order.

So that the search for a price works perfectly, you should specify number ranges for the individual price lists/glass types, e.g. 1000 - 1999 for float, 2000 - 2999 for patterned glass, etc.

_Fig. C-8 Price list codes and number range_

The number ranges (A) play a decisive role for the logic of pricing. This logic is described in detail in a separate section. ⇨ "PLCD logics" on page C-35

Before you can specify any price, you have to specify the PLCD to which the price should belong. Since the PLCD is also consulted for the determination of PU prices, you should keep the PLCD numbers for PU and SA separately.

> **A separate price list for each currency** If you use prices in different currencies at your company, you have to create an individual price list for each currency. In the document entry it is checked whether the currency of the market partner and the price list match. If this is not the case, a message will be displayed. The prices from the price list are not converted to the market partner's currency.

If you create a PLCD, you have to pay attention to the following so that you can work with the OC PLCD logic:

* The price lists have to be sorted in groups, e.g. by SA, PU.
* The sales price lists have to be in a number range provided for this, e.g. PLCD 1\*\*\* to 3\*\*\*. In the respective number range, the price lists have to be created in numeric ascending order.
* The purchasing price lists have to be in a number range provided for this, e.g. PLCD 4\*\*\* to 6\*\*\*.
* Each foreign currency also has to have its own number range.
* A newer price list always has to have a higher number (PLCD) than the predecessor price list. However, the numbering does not have to be without gaps.

### Price code (PCd)

The abbreviation PCd stands for price code. Price codes include price generations that are created in the form of price lists. The (logical) PCd is a pointer to a physical price list (PLCD) with which the price list is assigned to a market partner.

The PCd does not include any price data, but rather establishes the link between the price list and current conditions without which no price can be calculated.

_Fig. C-9 Assignment of PCd and PLCD_

In this illustration, you see that there is a reference from a PCd to a PLCD. The PCd makes the assignment of market partners and price list in two stages.

If you have created a new price list or if the prices of a market partner should be calculated according to another price list, only the PCd has to be changed for this two-level assignment. To change the pricing, you therefore have the following possibilities:

* In the general conditions, you specify another PCd for the market partner.
* A (new) PCd is assigned to a new PLCD.

_Fig. C-10 Assignment of PCd and PLCD_

In this example, you can see that the customer is assigned precisely 1 PCd, but several customers can be assigned to one PCd (n:1). Each PCd refers to precisely one price list (PLCD).

This means that the customers A, B, and F receive the prices from PLCD 100. Customers C and D receive the prices from PLCD 200, and customer F from PLCD 300.

For the coming year, the old IG prices should be adjusted. For this, a new price list with the PLCD 400 is created. The new prices are not yet used to calculate orders and can therefore be prepared in peace.

Starting at a defined point in time, the PCd will be attached to the new price list.

_Fig. C-11 Assignment attached_

The assignment only has to be changed for the PCd in which the customer data and in the conditions nothing has to be adjusted.

From now on, the customers A, B, and F receive the prices from PLCD 400. For all other customers, nothing changes.

The _Price List Reference_ and _General Daily Conditions_ are available for these assignments.

_Fig. C-12 PCd-PLCD assignment and daily conditions_

Only if you have specified in the general daily conditions which PCd applies for the calculation method in question can the price lists and from these, the prices be determined.

In the unit about the conditions, you will learn how you can also control these assignments for individual market partners. ⇨ "General and special conditions" on page C-129

#### Advantages of the separation of PLCD and PCd

Thanks to the separation of PLCD and PCd, you have the following advantages:

* You can enter price lists in advance without time pressure.
* You can activate all appropriate price lists together at a particular point in time.
* You can access old price lists very easily.
* In case of price changes, you do not absolutely have to adjust the market partners' conditions.

### Price keys for matrices, vectors, and lists

Before you enter prices, you have to create the necessary keys. These are special codes for the matrix and vector prices and for simple price lists.

| Code for                      | Description                                                                                                                                                                                       |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Matrices**                  | The matrix number is a key number and name, which are assigned to a two-dimensional price table, the matrix.                                                                                      |
| **Vectors**                   | <p>The vector number is a key number and designation that is assigned to a one-dimensional price table. Keys for vectors are created separately:</p><ul><li>Article</li><li>Processings</li></ul> |
| **Exchange/additional lists** | The list number is a key number and designation to which a price list for articles is assigned, which are exchanged in or added to the BOM.                                                       |

These keys are each stored on a separate dialog.

_Fig. C-13 Dialogs for storing of the price keys_

#### Master list for exchange/additional lists

For the list numbers for exchange/additional lists, you have to specify whether the list should apply as master list. From the master list, the exchange price is determined, for example, if in the exchange list that is assigned to the item article no exchange prices is found.

### Linking of the keys

You need the keys that you have defined for the vectors, matrices, and exchange/additional lists along with the price list keys in order to create a price matrix, a price vector or a price list.

If, for example, you create the prices for a matrix price, you specify the key number of the matrix and the price list.

_Fig. C-14 Assignment of price keys and price list_

In the same way, you also use the key numbers for vector and exchange prices.

> **Additional information** ⇨ "Price matrices for IG lites" on page C-58 ⇨ "Price vectors" on page C-72 ⇨ "Exchange and additional prices" on page C-90

### Price keys for muntins

For the calculation of muntin articles, muntin price classes and muntin codes are used.

* You assign all muntins to the key _Muntin price class_ that are calculated at the same prices.
* You assign the currency to the key _Muntin code_ in which the muntin prices should be calculated.

_Fig. C-15 Definitions of muntin prices_ _Fig. C-16 Keys for muntin prices_

The currency is assigned for the muntin code in the key. If you are working with several currencies, you have to create an individual price list for each currency.

### Currencies

In a system configuration with several currencies, you can maintain and edit the prices in different currencies. For this, the currencies have to be created in which price lists should be kept. You create the currencies in the master data. ⇨ Master Data, "Currency" on page B-189

_Fig. C-17 Currencies_

If you are not working with several currencies, at least the local currency has to be created.

For each currency, you specify a number, the abbreviation, and the exchange rate (C). Furthermore, you have to specify how the amounts calculated (D) should be rounded.

**Example**

| Currency | Places after the decimal point   | Rounding | Amounts           |
| -------- | -------------------------------- | -------- | ----------------- |
| Euro     | 2 places after the decimal point | To 0.01  | 179.321 -> 179.33 |
| SFr      | 2 places after the decimal point | To 0.05  | 179.321 -> 179.35 |
| CAD      | 2 places after the decimal point | To 0.10  | 179.321 -> 179.30 |

In this example, you see that the currencies are calculated with 2 places after the decimal point. For the prices in euros, the results calculated are rounded to the 2nd place after the decimal point; for Swiss Francs, to 0.05 Sfr; for the Canadian dollar to 0.10.

If you do not enter the smallest currency unit, the currency will be calculated with 2 places after the decimal point. If you do not store any details about rounding, the currency will be rounded commercially.

#### PU price calculation

If in a supplier's master data it is specified that the prices are calculated in foreign currency, the currency of the assigned price list absolutely has to match the supplier's currency. If you enter an article in the PO management or change the PU price list, it is checked whether the currency from the price list and the currency from the supplier's master data match. If this is not the case, a notice is displayed. In the order entry, the currency compatibility is not checked.

### PLCD logics

**Objectives**

* Understand evaluation logic and price list control.
* Be able to use starting with PLCD logic correctly.
* Use only PLCD logic.
* Understand the difference between basic PLCD with from PLCD logic and basic PLCD without from PLCD logic.

**Benefits**

* With the PLCD logic, prices for sale and purchasing can be maintained in different lists.
* Based on different settings for price allocations and with the surcharges, price lists can be created quite flexibly.

**Please note**

* **PLCD**: The PLCD is a (physical) price list in which any number of price matrices and price vectors are combined, e.g. all price lists that apply for the calculation of IG lites including exchange and processings.
  * The price list number is the numeric designation of a price list.
  * The PLCD is defined by a number, a name, and a currency.
  * The PLCDs are used to sort price lists.
  * Number is in ascending order.
* **PCd**: The (logical) price code (PCd) is a link to a physical price list (PLCD) with which the price list is assigned to a market partner.
* **PLCD logic**: Prices can be searched for in another price list if no price was found in the current PLCD. The configured PLCD logic applies for all dialogs in the price master data and conditions in which a from-PLCD can be specified. By default, A+W Enterprise works with the from logic.
* **Price lists control**: The from-PLCD logic can be overridden for individual price list codes. The override also applies for all price searches in which the specified PLCD is entered.
* **From PLCD logic**: If for the order entry for the article no price for the current PLCD is found, the program determines in numeric sequence the prior PLCD for which a price is defined.
* **Only PLCD logic**: For the pricing, the price is only determined from the specified PLCD.
* **Basic PLCD with from-PLCD logic**: For the pricing, first the current PLCD is determined. After that, it is checked which PLCD logic should be applied and the search is continued to the basic PLCD.
* **Basic PLCD without from-PLCD logic**: For the pricing, first the current PLCD is determined. After that, it is checked which PLCD logic should be applied and searched for in the PLCD, which is specified as basis.

### From-PLCD logic

A+W Enterprise works with the from-PLCD logic: if for the order entry for the article no price for the current PLCD is found, the program determines in numeric sequence the prior PLCD for which a price is defined. Thus, the price found applies starting from this PLCD.

A price is not searched for just in the price list (PLCD) that is assigned via the PCd. If no price was found in this PLCD, the search continues in the PLCD with the next-lowest number.

_Fig. C-18 Ascending PLCD and from-PLCD logic_

In these examples, you see that the price from vectors applies as long as a new price is found. That is, if in PLCD 2017 no price was found, the search continues in PLCD 2016; after that, in PLCD 2015, and then in PLCD 2014.

You can deviate from this from-PLCD logic on the Price List Control dialog for each individual PLCD. ⇨ "Price list control" on page C-40

> **Exception IG matrices** IG matrices are excepted from the from-PLCD logic. That's why the prices have to be maintained completely per PLCD.
>
> For the 2nd matrix, the price search ends in PLCD 2016 even if higher codes are set up. Vice-versa, this means that the prices for the 2nd matrix for the PLCD 2017 have to be maintained anew. There are copy functions available for this. ⇨ Software Reference, "Matrix Adoption" on page C-202

### Benefits of the from-PLCD logic

These are the benefits of the from-PLCD logic.

* Prices can be grouped by price lists, e.g. in order to separate PU lists from SA lists.
* You do not always have to enter all prices per price list, just the changes
* You can enter new price lists during normal daily business and activate them at a later point in time.
* You can trace the changes in the price list history.

#### Special features with the from-PLCD logic

With the from-PLCD logic, you have to heed the following:

* With this logic, it is possible to access price lists that may be assigned to another price list group or that are kept in another currency. That's why it is important to adhere to the number ranges and in the lowest PLCD of a group, all prices should be completely maintained.
* In the order you cannot detect if the price was determined as consequence of the from-PLCD logic from a lower PLCD.

### Only PLCD logic

If you do not want to use the from-PLCD logic for a particular PLCD, you have to switch off the from-PLCD logic for this PLCD. You specify this setting on the Price List Control dialog.

_Fig. C-19 Price list control_

For the only-PLCD logic, for the PLCD (A) and the basic PLCD (B), you have to specify the same number and select (C) N (No) in the _from-Logic_ field. This way, you have deactivated the from-PLCD logic for this PLCD.

For pricing in the document management, first the current PLCD is determined. After that, A+W Enterprise checks which PLCD logic (C) should be applied. The price is only determined from the specified PLCD. If no price is found in the specified price list, an appropriate notice is displayed. The search is not continued in another PLCD.

### Basic PLCD with from-PLCD logic

If you want to limit the from-PLCD logic for a particular number range, you have to override the from-PLCD logic for this PLCD, e.g. for different currencies.

_Fig. C-20 Price list control_

For the current PLCD (A) you have to specify a lower basic PLCD (B) and select Y (Yes) in the _from-Logic_ field (C).

For pricing in the document management, first the current PLCD is determined. After that, A+W Enterprise checks which PLCD logic should be applied. If for the order entry for the article no price is found in the current PLCD, the program determines only back to the basic PLCD. If no price is found, an appropriate notice is displayed in the document management.

### Basic PLCD without from-PLCD logic

If you want to specify a deviating price list for a particular PLCD, you have to override the from-PLCD logic for this PLCD.

_Fig. C-21 Price list control_

For the current PLCD (A), specify a lower basic PLCD (B) and select N (No) in the _from-Logic_ field (C).

For pricing in the document management, first the current PLCD is determined. After that, A+W Enterprise checks which PLCD logic should be applied and searches in the PLCD that is specified as basis. If no price is found in the specified price list, an appropriate notice is displayed in the document management.

That's why you have to pay attention that all prices are specified in the basic PLCD.

### Price list control

Since you generally create and maintain price list codes across decades for the various glass types, you have to control which PLCD should be used for price calculation.

Via the price list control, it is set from which price list a price is drawn if no price was found in the assigned price list.

If in the document management no price in the sense of the set PLCD logic is found, an error message is output.

In nearly all dialogs that are used for pricing, you can specify a PLCD from which the price applies. The from-PLCD logic applies separately for all dialogs on which a from-PLCD can be specified.

In individual cases, the from-PLCD logic can be overridden. The _Price List Control_ dialog is available for this:

_Fig. C-22 Price list control_

On this dialog, you create a deviating procedure for a particular PLCD (A). For the pricing, first the current PLCD is determined. After that, A+W Enterprise checks which deviating PLCD logic should be applied.

If you are working with internal client separation, you can also control pricing in the different sites this way.

#### Global and local price lists

For operations with internal client separation, the pricing can be controlled via global (site-spanning) and local (site-specific) price lists.

> For this, a price master site is set up, to which the employees are assigned who are responsible for the maintenance of the master data for prices and conditions. For the global price lists of the price master site, all types of price control can be used, while for the local price lists, only the PLCD and PLCD-basic methods can be used.
>
> **Requirements** The function for work with global and local price lists has to be configured by the A+W Software GmbH service.

_Fig. C-23 Global/local price lists_

In this schematic illustration, you see that the clients each work with their own local price lists. Customer 5000 is assigned site 5130 as debtor. In the general terms and/or the customer terms, it is assigned the appropriate price lists. Thus, the orders for him are calculated via the local price lists of the client 5130.

The customer can also be assigned the client 5400 via the site-specific details, so that his orders can also be calculated via the prices of the client 5400. For this setting, you need special administrator rights.

The global price list of the price master is superior to all clients, so that you can assign these price lists in the terms of the individual clients. Thus, the clients also have access to all pricing methods.

Via the rights management, you can control which employees may also access the global price lists in the order entry.

### Pricing components

**Objectives**

* Understand settings for pricing.
* Distinguish pricing methods for calculating lites.
* Use rounding methods in pricing correctly.
* Calculate price-relevant quantity.
* Calculate calculation bases according to basic quantities.

**Benefits**

* The different products can only be calculated exactly if the price definition is attuned to the product type.
* For this, you can use the components of the price definition in goal-oriented fashion.

**Please note**

* **Pricing method**: The pricing type and terms for an article are controlled by the pricing method that is assigned to the article. The pricing method is an algorithm for price calculation for the article of a particular product type. The pricing methods are defined by the system.
* **Price rounding**: Price rounding specifies whether the calculated price is rounded up or down and to how many places.
* **Price-relevant quantity**: Quantity for which the price is calculated. It is influenced by the minimum edge length, the dimension rounding, and the minimum calculation quantity. The price-relevant quantity can deviate from the actual physical quantity.
* **Calc. base**: The calculation base specifies how the price is determined, e.g. as single price, scaled price, variant price, etc.
* **Price calculation**: The search for the specifications for the price calculation is called price calculation in this document.
* **Price type**: The price type specifies to what the specified price refers, e.g. to the quantity unit from the article data, to meters, etc.
* **Base quantity unit (BQU)**: Unit of the article quantity from the article master data.

### Pricing methods

The pricing type and terms for an article are controlled by the pricing method that is assigned to the article. The pricing method is an algorithm for price calculation for the article of a particular product type.

For each product group, there is an individual pricing method, which considers the special properties of the product group in the pricing. The pricing method is assigned to the article in the article master data.

| Product type                   | Pricing method                   | Price definitions                                                                                                                                                                                                                  |
| ------------------------------ | -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **IG articles**                | 40-IG Switzerland, 41-IG current | Prices in matrices or vectors, Exchange prices for up to 3 exchange glasses, Individual lite prices, Processing and accessory prices, Surcharges for steps, sizes, shapes, Surcharge depends on the width of the AIR               |
| **LAMI articles**              | 29- PCd laminated                | Prices in article vectors, Exchange price for each exchange glass and each exchange foil, Additional price for additional articles, Step prices, Processing and accessory prices, Variant prices                                   |
| **TGH articles**               | 22-PC-TG                         | Prices in article vectors, Processing and accessory prices, Variant prices                                                                                                                                                         |
| **Float articles**             | 23 - PCd basic glass             | Prices in article vectors, Processing and accessory prices, Variant prices, Surcharges for sizes, shapes                                                                                                                           |
| **Accessory articles**         | 25- PC prices general            | Prices in article vectors, No additional processing and accessory prices                                                                                                                                                           |
| **Colored accessory articles** | 31-PCd colored articles          | Prices for each individual color possible                                                                                                                                                                                          |
| **Processing articles**        | 26 - PCd processings             | Prices in processing vectors                                                                                                                                                                                                       |
| **Patterned glass articles**   | 24 - PCd processed glass         | Prices in patterned glass classes                                                                                                                                                                                                  |
| **Muntin articles**            | 5 - Muntin prices                | Prices for muntin articles, Prices for muntin construction elements, e.g. crosses, fields, etc.                                                                                                                                    |
| **GDS**                        | 12 - PCd glass doors             | Prices in article vectors, Different article types allowed (60,100, 110, 120, 130, 140, 150, 170, 200), Glass with particular price methods allowed (PCd prices generally, PCd-TGH, PCd-LAMI, PCd base glass, PCd processed glass) |
| **Glazing**                    | 28- PCd glazing                  | Prices in article vectors                                                                                                                                                                                                          |
| **UV protections**             | 60 - protection                  | Vector price                                                                                                                                                                                                                       |
| **Manual price entry**         | 99 - manual prices               | Prices are specified only in the order                                                                                                                                                                                             |

### Rounding methods (pricing)

By default, the prices are rounded to the smallest currency unit that is specified in the currency, e.g. to 2 places after the decimal point. The rounding methods can refer to the individual price or the unit price.

> **Round sizes** Round sizes are always calculated before the determination and calculation of prices. With the round sizes, the price-relevant quantities are calculated, for which the prices are calculated. Only after that are the prices calculated rounded.

#### Rounding variables

In addition to the settings for size and price rounding, other settings are defined via the system configuration.

If you need additional settings, please contact a member of the A+W Software GmbH service team.

#### Commercial rounding

After each calculation step for pricing, the intermediate result is rounded. For this, there are the following rounding methods:

* **Up**: The price is rounded up to the hundreth value in currency units.
* **Down**: The price is rounded down to the hundreth value in currency units.
* **Com**: The price is rounded commercially to the hundredth value up or down.

**Example**

| Rounding | Value  | from   | to           |
| -------- | ------ | ------ | ------------ |
| to 10    | 4.38 € | 4.40 € | rounded up   |
|          | 4.73 € | 4.80 € |              |
| from 10  | 4.38 € | 4.30 € | rounded down |
|          | 4.73 € | 4.70 € |              |
| Com 10   | 4.35 € | 4.40 € | rounded up   |
|          | 4.34 € | 4.30 € | rounded down |
| Com 100  | 4.38 € | 4.00 € | rounded down |
|          | 4.73 € | 5.00 € | rounded up   |

#### Unit price rounding

To calculate the unit price, a unit price rounding is used, which can be specified in the terms.

**Example of unit price rounding** If unit price rounding = 100 is specified, the price will be rounded to the next full currency amount: 54.56 -> 55.00 54.46 -> 54.00

If unit price rounding = 10 is specified, the price will be rounded to the next tenth amount, e.g. 10 cents: 54.65 -> 54.70 54.64 -> 54.60

### Price-relevant quantity

The glass articles are generally created in the master data with the basic quantity unit (BQU) square meters.

To calculate the prices, you can specify how the price-relevant quantity is calculated. This includes the minimum edge length, the round size, and the minimum calculation.

_Fig. C-26 Article vectors - details_

The area of the glass is calculated as follows:

1. **Minimum edge length**: The height and width of the lite are compared to the stored minimum edge length. If the stored value is not reached, the minimum edge length is used for further calculation.
2. **Round size**: The width and height are rounded according to the specified round size. For round size, a size is specified, e.g. 30 mm. The edge length is thus rounded up to the next size that can be divided by this value (30 mm).
3. **Area**: The area of the glass is calculated with the current or minimum length of width and height.
   * (width x height)/1,000,000 produces the area in square meters.
   * The area calculated is rounded according to the system configuration. The rounded area is compared to the stored minimum area. The higher value is used for price calculation of the glass.

| Step | Size                          | Calculation                                                              | Rounding                                        |
| ---- | ----------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------- |
|      | Minimum edge length = 800 mm  |                                                                          | Round size = 30 mm                              |
|      | Minimum area = 0.5 sq m       |                                                                          |                                                 |
| 1.   | Width 1235 mm, Height 1895 mm |                                                                          | (minimum edge length reached)                   |
| 2.   | 1235 mm, 1895 mm              | Round size 1260 mm, Round size 1920 mm                                   |                                                 |
| 3.   | 1260 mm, 1920 mm              | Area 2.4192 square meters                                                | (minimum area reached), Area 2.42 square meters |
|      | Glass price 46.53 €           | Price calculation with the larger area = 2.42 square meters = 112.6026 € | 112.60 €                                        |

### Calculation bases

For scaled prices, calculation bases specify from which price level the price is determined:

* **1 - Single price**: For price calculation in the order, the level 1 price is used.
* **2- Scaled level**: For price calculation in the order, the price level is determined that is specified in the terms.
* **3 - Quantity scale per piece (BQU)**: To determine the price level, the quantity of the item is determined using the basic quantity unit (BQU) of the article. The price in the order is calculated according to the price level that is reached through the total quantity of the item.
* **4 - Quantity scale per piece (BQU)**: To determine the price level, the basic quantity in a piece of the item is determined.
* **5 - Total quantity per vector**: In the order, the prices are determined based on the total quantity. For this, all items are determined for which the same price vector applies. The quantities of the appropriate items are totaled. This total is compared to the defined price levels. The price is calculated using the price level determined.
* **6 - Total quantity per BOM header**: In the order, all items are determined that have the same BOM header number. The quantities of the appropriate items are totaled. This total is compared to the defined price levels. The price is calculated using the price level determined.
* **7 - Total quantity per color coating**: In the order, all items are determined that have the same color coating. For this, the color variant of the article is not checked; instead, the specification on the tab _Properties > field Prod. Seq_. The quantities of the appropriate items are totaled. This total is compared to the defined price levels. The price is calculated using the price level determined.
* **8- Total quantity per product group**: In the order, all items are determined that have the same product group. The quantities of the appropriate items are totaled. This total is compared to the defined price levels. This total is compared to the defined price levels.
* **9 - Pieces per item**: To determine the price level, the number of pieces of the item is used.
* **10 - Total quantity per order**: To determine the price level, the total quantity of all items in the order is determined.
* **11 - Variants**: With this calculation base, the prices can be scaled depending on 2 dimensions, e.g. height and width. To determine the price level, the smaller dimension is compared to the first column, the larger with the second column. The price is calculated in the order according to the price level for which the limit values of both dimensions are reached. ⇨ Software Reference, "Article Price Vectors" on page C-221
* **12 - Variants scale**: This calculation base makes sense for glass doors. With this calculation base, the width of the glass door is compared to the value from the first column and the height of the glass door with the value from the second column. Here it is important that the dimensions are entered in ascending order, first according to the first column and then according to the second column. The price is calculated in the order according to the price level for which the limit values of both dimensions are reached.

> **Variant scale vs. variant prices** For glass doors with standard dimensions, normal variant prices are stored. If glass doors with standard dimensions are ordered, the variant prices are used. For glass doors with special dimensions, vector prices with the calculation base Variant scale are stored. For price calculation, A+W Enterprise determines the vector prices with the calculation base Variant scale.

* **13 - Quantity scale/package size**: This calculation base is used if a price for an article has a very low value that cannot be depicted with a precision of two places after the decimal point.

**Example** Article with unit price of 0.0254 EUR with quantity 100 = EUR 2.54 GR/piece. The unit price for a sack with 1000 cork sheets is EUR 25.40. Per lite, 5 sheets are needed. With an item quantity of 15 lites, 75 sheets are needed. The item price is calculated as precise unit price and then rounded to two places after the decimal point.

* Calculation: 75 pieces x 0.0254 EUR = EUR 1.905
* after rounding = EUR 1.91

### Price type

For each price, you have to specify to what the value specified refers. For each price, a calculation base and a type are selected. The price types and calculation bases are specified permanently by the system.

The price type specifies to what the specified price refers. Here, the currency unit (CU) underlies in which the system calculates.

* **CU/BQU**: The price is specified per basic quantity unit (BQU), which is stored in the article master data, e.g. per piece, linear m, etc.
* **CU/piece**: The price is specified per piece.
* **CU/sq m**: The price is specified per square meter.
* **CU/lm**: The price is specified per linear meter. This price type is only selected for processings.
* **Percent**: The prices are calculated percentage wise from the base price of the item article. This price type is only selected for exchange articles or processings.

### Quantity calculation by BQU

Prices are oriented according to the quantity in the order. That's why it's possible to store the prices in quantity scaling. There are various total quantity calculation bases for this.

> **Round sizes** Round sizes are always calculated before the determination and calculation of prices. With the rounded sizes, the price-relevant quantities are calculated, for which the prices are calculated. Only after that are the calculated prices rounded. In the following examples, round sizes and other size definitions are not considered. Number refers depending on the calculation base to the number of IG units, the single lites or the item quantity.

| Basic quantity units (BQU)  | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ton, liter, kilogram, hours | One-dimensional units. For calculation of the quantity, the number is multiplied by the value from the _Width_ field (mas1). If, however, the price is calculated with Quantity scale per piece, the system assumes the quantity = 1. Depending on the configuration, rounding is done commercially to one place after the decimal or 2 places after the decimal.                                                                                                                                                                                                                                                                                                                                                                                                           |
| Millimeters                 | This is generally a one-dimensional unit. The millimeters are first converted into meters (division by 1000). After that, for calculation of the quantity, the number is multiplied by the value from the _Width_ field (mas1). If, however, the price is calculated with Quantity Scale per Unit, the system assumes the number = 1. The calculated quantity is rounded to one place after the decimal point. If a millimeter article is entered for a two-dimensional article, mas2 is greater than 0. The millimeters are first converted into meters. For calculation of the quantity, the item quantity is multiplied by (2xmas1 + 2xmas2). The calculated quantity is rounded to one place after the decimal point. The variable AUFRUNDEN\_FLAECHE is not evaluated. |
| Meter                       | One-dimensional unit. For calculation of the quantity, the number is multiplied by the value from the _Width_ field (mas1). If, however, the price is calculated with Quantity Scale per Unit, the system assumes the number = 1. The calculated quantity is not rounded. If, however, a millimeter article is entered under a two-dimensional article, mas2 is greater than 0. For calculation of the quantity, the number is multiplied by (2xmas1 + 2xmas2). The variable AUFRUNDEN\_FLAECHE is not evaluated.                                                                                                                                                                                                                                                           |
| Square meter                | Two-dimensional unit. For calculation of the quantity, the _Width_ field is multiplied by the _Height_ field (mas1xmas2). Since the items are always entered in millimeters, there is then a conversion from square millimeters to square meters (division by 1,000,000). Depending on configuration, the resulting square meters are rounded commercially up to one place after the decimal point or 2 places after the decimal point. Finally, the rounded square meters are multiplied by the number. If, however, the price is calculated with Quantity Scale per Unit, the system assumes the number = 1.                                                                                                                                                              |
| Pieces                      | Number equals quantity. If, however, the price is calculated with Quantity Scale per Unit, the system assumes the number = 1. The variable AUFRUNDEN\_FLAECHE is not evaluated.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Circumference               | Two-dimensional unit. The millimeters are first converted into meters (division by 1000). Depending on configuration, the resulting quantity is rounded commercially to one or 2 places after the decimal point. With these rounded meters, the circumference is then calculated (2 x mas1 + 2 x mas2). With this BQE, there is no multiplication by the number.                                                                                                                                                                                                                                                                                                                                                                                                            |

### Creating keys

In this unit, you will learn how to create the keys for the price definitions. The steps shown apply analogously for all price keys.

This unit includes the following action sequences:

* Here's how to create a muntin code
* Here's how to create a muntin price class

#### Here's how to create a muntin code

1. Select _Master Data > Keys > Prices > Muntin Price Code_.
2. Press `<F6>` to insert a new row. _Fig. C-28 New row cleared_
3. Enter the code number (B) for the new M-PCd.
4. Enter a meaningful description (C) of what the key should be used for.
5. Select the currency.
6. Confirm the data with `<Enter>`. The data will be saved and a new row inserted.
7. Repeat steps 3 to 6 for another M-PCd or close the dialog.

Next, create a muntin price class.

#### Here's how to create a muntin price class

1. Select _Master Data > Keys > Prices > Muntin Price Classes_.
2. Press `<F6>` to insert a new row. _Fig. C-29 New row cleared_
3. Enter the key number (B) for the new muntin price class.
4. Confirm the data with `<Enter>`. The data will be saved and a new row inserted.
5. Repeat steps 3 and 4 for another muntin price class or close the dialog.

### Exercises

Make sure that with the login in A+W Enterprise you have acquired all user rights that are required for working with the master data.

For the exercises in the following units, create the following keys:

* **Price list code**, e.g. 9999 - Training.
* Create at least one key for a matrix, an article, a processing vector, and an exchange list. Also select numbers and descriptions that differ significantly from the default keys.
* For the lists, make sure that you do not change the specification of the master list.
* Create a muntin price class and a muntin code. Here, be sure to assign the right currency.

### Price Master Data

In this subject module, you will learn how to create prices in A+W Enterprise. You can only create the prices if you have stored the necessary keys.

This section provides information on the following subjects:

* "Workflow: creating prices" on page C-57
* "Price matrices for IG lites" on page C-58
* "Price vectors" on page C-72
* "Exchange and additional prices" on page C-90
* "Muntin prices" on page C-102
* "Surcharges" on page C-108
* "Global price changes" on page C-120

### Workflow: creating prices

So that the prices can be calculated correctly, the following steps are required:

1. **1st step: Create price list code (PLCD)** Each price list is created with a unique number and a designation, the price list code (PLCD). In addition, the currency is specified with which the prices are calculated, e.g. euros.
2. **2nd step: Enter keys for matrices, vectors, etc.** A number and a designation are specified for each key.
3. **3rd step: Enter prices in price lists** Article prices are entered in matrices and vectors. A price list can consist of many matrices and vectors.
4. **4th step: Specify price list reference** For the references, the price codes (PCd) are defined. The price code is assigned the respectively valid price list (PLCD) with the article prices.
5. **5th step: Assign price code (PCd) to the market partners** The current PCd for each pricing method is specified in the General Daily Conditions. Each market partner can be assigned a deviating price code (PCd) per pricing method. The same PCd can be used for several market partners.

### Price matrices for IG lites

**Objectives**

* Understand differences in the matrix forms.
* Get to know application possibilities for price matrices.
* Understand evaluation of the matrix during price searching.
* Get to know function of the base prices.
* Define and assign base prices.

**Benefits**

* With price matrices, prices can be scaled very finely. Here, the article has to be considered that should be calculated via a price matrix.
* With the definition of the base prices, you can specify the price calculations with price matrices in great detail.

**Please note**

* **Triangle**: In the triangle, the limit values can be interchanged. Therefore not all combinations of the limit values with prices have to be filled. Prices in a triangular matrix make sense if, for example, the same price applies for the dimensions 500 x 750 mm and 750 x 500 mm.
* **Limit value**: The limit value specifies the steps of a scaling. Depending on the matrix type, the limit values relate to edge lengths, areas, and quantities.
* **Base prices**: With the definition of base prices, you specify details for the calculation of IG lites.
* **Matrix**: Two-dimensional price table for scaling of the prices. In price matrices, IG prices are defined that depend on two limit values, e.g. height and width.
* **Type**: The type specifies whether the prices are created in a triangular or square matrix. The selection of the type depends on the matrix type.
* **Matrix type**: The matrix type specifies whether the limit values are compared to the edge lengths or with the quantity and the area.
  * **Width x height**: Both limit values for the scaling are specified in mm.
  * **Pieces x square m**: The limit value of the column is specified in pieces, the limit value for the rows in square m.
* **Square**: In the square form, the limit values may not be interchanged. Therefore, all combinations of the limit values have to be filled with prices. The square is used for glass with patterns where the pattern has a direction. This form also has to be used for the matrix type Pieces x sqm.
* **Requirements**: Keys for price lists and matrices are created. Limit values are specified as limit dimensions (optional).

### Matrix editor

A matrix is a two-dimensional price table in which the price depends on two variables, e.g. width and height of the item entered.

Matrices are suitable for IG articles with the pricing method _IG current_ or processings with the pricing method _Processing matrices_.

In this example, you see a price matrix for the calculation of IG prices:

* In the header area of the dialog, the keys (C, D), the price type and the shape of the matrix (G, E and F) are specified.
* In the column header (A) and in the row header (B), limit values are specified.

In a matrix, you can specify up to 30 x 30 values. This means that you can specify up to 900 prices that are used in the order.

A+W Enterprise also offers the opportunity to import matrices from ASCII files with fixed formats, e.g. csv files.

> **Tip** If you want to create a new matrix, you can copy a similar matrix and then adjust the values. Note that the from PLCD logic for matrices does not apply. If you create a new matrix, it has to be assigned to precisely the PLCD according to which the prices should be calculated. If necessary, you also have to first create a new PLCD.

#### Matrix type

The matrix type specifies whether the limit values are compared to the edge lengths or with the quantity and the area.

* **Width x Height**:
  * If the dimensions from the order item may be turned, it applies that:
    * The smaller dimension is compared to the column limit values.
    * The larger dimension is compared to the row limit values.
  * If the dimensions from the order item may not be turned, it applies that:
    * The column limit values are compared to the dimension of the width.
    * The row limit values are compared to the dimension of the height.
  * Whether the dimensions from an order item may be turned depends on the matrix type and the environment variables set. ⇨ "Type" on page C-61
* **Pieces x sqm**:
  * The column limit values are compared to the area.
  * The row limit values are compared to the quantity.

#### Type

A matrix can be defined as a triangular matrix or as a square matrix. Which shape you choose depends on the article that should be calculated with the matrix.

* **Triangular matrix**: Prices in a triangular matrix make sense if, for example, the same price applies for the dimensions 500 x 750 mm and 750 x 500 mm. By default, the smaller length measurement of the item is compared to the column limit values; the larger with the row limit values. If necessary, the dimension details are turned for this. _Example of a triangular matrix_ In this example, the colored fields of the triangular matrix do not have to be filled because they arise from length = width.

> **Non-applicability of the triangle** You have to enter prices for glass that may not be turned, e.g. patterned glass whose pattern has a direction, as a square matrix. This also applies if the environment variable `MATRIXMASSE_UNGEDREHT` is set at your company and the dimensions may not be turned. Essentially, the first length specification in the order is compared to the column limit values and the second length specification with the row limit values.

* **Square matrix**: If the price is determined from a square matrix, you have to fill all fields of the matrix. The square matrix makes sense if the dimensions for price determination may not be turned, e.g. for patterned glass whose pattern has a direction or for the matrix type _Pieces x sqm_ for IG lites. _Example of a square matrix_ In this example, the colored fields are filled because the prices of length x width and width x length are different.

#### Price type

For the calculation of prices in the order, the following price types are used:

* **Unit price**: The price is calculated per unit. This price type is not supported for exchange glass or processings.
* **Prs/sqm**: The price is calculated per square meter. This price type is supported for all articles.
* **Percent**: The price is calculated as a percentage from the base price of the item article. This price type is not supported for exchange or IG glass.
* **Im**: The price is calculated per linear meter. This price type is only supported for processings.

### Limits

If the dimension exceeds the specified limit value, the next value applies. Here, the dimensions are rounded before the comparison of the values. ⇨"Price-relevant quantity" on page C-47

You can define templates for length limit values on the _Matrix Limits_ dialog. You can call up this dialog in the matrix editor in the fields _PLCD_ and _Matrix_ with `<Shift> + <F11>`. You can use the limit values for the matrix type _Width x Height_ if you create a new matrix. You can then import these limit values via the _Columns_ and _Rows_ fields and adjust them.

_Fig. C-31 Matrix limits for type Width x Height_

In the template, enter a meaningful name from which you can tell for what the dimensions are intended. The number specifies how many columns or rows should be created for the limit values in this matrix.

You can also define templates for area limit values on the _Matrix Area Limits_ dialog. You can call up this dialog in the matrix editor in the _PLCD_ and _Matrix_ fields with `<Ctrl> + <F11>`. You can create the limit dimensions for the matrix type _Pcs x sqm_ and the price type _Pr-sqm_ if you create a new matrix. You can then import and adjust these limit values via the _Rows_ field.

If you have imported the values into a new matrix, you can adjust the values and then define additional columns and rows.

### Creating a price matrix for IG lites

In this example, you create a matrix by importing the limit dimensions and then entering the prices. As alternative, you import an (old) matrix and then change the prices.

This unit includes the following action sequences:

* "Here's how to create a matrix" on page C-65
* "Here's how to take over prices from another matrix" on page C-67
* "Here's how to convert the matrix prices" on page C-68

If you create a price matrix, you will see that you cannot make any other specifications, e.g. surcharges for small lites or for which IG articles the matrix applies. You create these details for price calculation on the _IG Basic Prices_ dialog. ⇨ "Base prices for IG lites" on page C-69

> **Prerequisite** You have the required user rights. You have created at least one key for matrices.
>
> Note that the from PLCD logic for matrices does not apply. If you create a new matrix, it has to be assigned to precisely the PLCD according to which the prices should be calculated. If necessary, you also have to first create a new PLCD.

#### Here's how to create a matrix

1. Select menu _Master Data > Prices > IG Prices > Matrix Editor_.
2. Use `<F9>` to select a PLCD (A) and a matrix number (B) that you have stored for practicing. Skip the following steps and change to the next action sequence if you want to take over the prices from another matrix. ⇨ "Here's how to take over prices from another matrix" on page C-67
3. Select the following data and confirm with `<Enter>`:
   * C: the matrix type _W x H_.
   * D: the matrix type _Triangular_.
   * E: price type _sqm-Pr_.
4. Use `<F9>` to select the columns (F) and rows (G) for an IGU.
5. Enter the desired prices in the matrix and confirm with `<Enter>`.
6. Select `[OK]` to save the matrix.

#### Here's how to take over prices from another matrix

> **Prerequisite** A matrix from which prices can be imported has to be created.

1. Place the cursor in the _Matrix Type_ field.
2. Use `<F5>` to select a matrix.
3. Use `<F9>` to select the PLCD and the matrix number.
4. Trigger the takeover with `<F3>`.
5. Confirm the query about overwriting the matrix with `[Yes]`.
6. Check and correct and/or complete the prices.

> **Change all matrix prices** You can correct all prices by increasing or reducing the values by an amount or a percentage. ⇨ "Here's how to convert the matrix prices" on page C-68

7. Select `[OK]` to save the matrix.

#### Here's how to convert the matrix prices

> **Prerequisite** The key for the target has to be created.

1. Select menu _Master Data > Prices > IG Prices > Convert Matrix_.
2. Enter the PLCD and the number of the matrix (A), from which the prices should be imported.
3. Enter the PLCD and the number of the matrix (B), into which the prices should be imported. Source and target have to have different PLCD or matrix numbers.
4. If the target matrix already exists, a query is displayed. Confirm the query with `[Yes]`.
5. Use `<Toggle>` in the _Target = Source_ field (C) to select the entry _+ IG value_. The input field (E) for the value is displayed.
6. Enter the amount by which the prices should be increased, e.g. 5.
7. Check the rounding rule (D) and correct it if the currency prescribes other roundings.
8. Trigger the action with `<F3>`.
9. Close the dialog and open your training matrix.
10. Check whether the prices have been changed as desired.

### Base prices for IG lites

The prices for IG lites are generally calculated with the pricing method _IG current_. For this, you create price matrices and assign the respective IG article. Furthermore, you specify the calculation rules, e.g. specifications for minimum calculation, rounding or for surcharges and exchange prices. The _IG Basic Prices_ dialog is available for this.

On this dialog, you assign the calculation rules per price list to the IG articles with which the prices in the order should be calculated. For the assignment of the IG base prices, the from-PLCD logic applies again; that is, if in the specified price list no price is found, there is a search in the price list with the next-lowest number. Generally the prices for IG articles are drawn from a matrix (B). The IG prices can also be calculated by vectors or individual lites.

> **Calculation type individual lites** If _Single lites_ is selected as calculation type, the prices are determined according to a special calculation rule. For this, the individual lite prices have to be specified separately. This type of price calculation for IG lites is used primarily in France.The prices are specified on the _Single lites for IG articles_ dialog.

In addition, you can specify the details with which the calculation of the assigned price matrix is completed. As minimum values (C), you can specify the edge length and/or the area. Thus you specify that the price is calculated for at least this size. ⇨"Price-relevant quantity" on page C-47

With the round size (D) you specify how the dimensions of the order item are rounded for the price calculation.

**Example** 30 mm is defined as round size. The IG article entered has the dimensions 1000 x 1000 mm. The next edge length divisible by 30 is 1020 mm. The price is calculated from the dimensions 1020 x 1020 mm = 1.04 sq m.

Furthermore, you can specify the rounding to the surcharges and various surcharges (E), e.g. for the installation of steps, for jumbos, etc. The surcharges are created in the dialogs intended for this. The surcharges will be described in more detail in a separate unit. ⇨ "Surcharges" on page C-108

Finally, you can assign exchange lists (F) with which the glass is calculated that is exchanged in the IG. In order to assign exchange lists, these have to be assigned on the _Exchange/Additional Lists_ dialog. The lists are described in more detail in a separate unit. ⇨ "Exchange and additional prices" on page C-90

So that the IG lites are calculated according to your definitions, the price code (PCd) has to be specified in the daily terms. The terms are described in a separate unit. ⇨ "Conditions" on page C-121

### Exercises

For the exercise, use the keys that you have created for the training. If necessary, add the keys for the exercises. For the PLCD and PCd use only your training keys.

* Create a price matrix for an IG article.
* Copy the prices for a second price matrix and increase the copied prices by 5%.
* Assign the new matrices to the IG articles.

### Price vectors

**Objectives**

* Get to know application possibilities for price vectors.
* Understand evaluation of the price vectors during price searching.

**Benefits**

* With price vectors, prices can be scaled very finely. Here, the article has to be considered that should be calculated using a price vector.
* With the from-PLCD logic, you can control the price search for vector prices.

**Please note**

* **Article vectors**: Sensibly, vectors have the same number as the article whose prices should be created in the vector.
* **Processing vectors**: Processing vectors can also be distinguished by glass thickness, product group, and quantity. Alternatively, processing prices can be defined in matrices.
* **Limit value**: The limit value specifies the steps of a scaling. Depending on the calculation base, the limit values relate to quantities, basic quantity unit, area or for processings to edge lengths.
* **Round size**: For the price calculation, the height and width of the order item are rounded up to the next-higher length in mm, which can be divided by the specified round size.
* **Minim. Calculat.**: For vector prices, minimum sizes can be specified, e.g.:
  * minimum calculation by quantity units from the article master data.
  * Min. price per piece.
  * Min. Edge Length per piece.
* **PLCD logic**: For vector prices, the from-PLCD logic applies by default. The from-PLCD logic can be overridden for individual price list codes on the Price List Control dialog.
* **Vector**: One-dimensional price table for scaling of the prices. List with prices that generally depend on only one value, e.g. quantity or square meters. Vector to which the calculation base 11-Variants or 12 - Variant scale is assigned can also depend on two values, e.g. height and width.
* **Requirements**: Vectors are created for articles and processings. Keys for price lists and vectors are created.
* **Surcharges**: For vector prices, surcharges can be specified, e.g.:
  * size surcharges for area articles
  * Small glass surcharges
  * Excess length surcharges

### Vector prices

Vectors are one-dimensional price tables. The price generally depends on a single input variable, e.g. the quantity of an article. Depending on the pricing method, the details for the vector prices differ:

* Vector prices for articles
* Vector prices for processings
* Vector prices for LAMI
* Prices for color articles
* Variant prices.

_Fig. C-37 Price definition for vector (example article vector)_

In this example, you see a price vector for an article:

* In the header area of the dialog, the keys (A, B) and the calculation base (C) are specified.
* For this, the minimum values (D), the round size (F) for the calculation of glass prices, and a minimum price (G) can be specified.
* Depending on the calculation base, you can specify limit values for price levels (E), e.g. for the quantity. In a vector, you can specify up to 30 steps.

#### Vector prices for articles

With article vectors, the prices for single glass, LAMI or accessories can be calculated.

Vector numbers can be identical to article numbers. Thus, there is no assignment. If, however, several articles should be calculated with the same price vector, the articles have to be assigned to the vector.

> **Distinction between processed and unprocessed fixed dimensions** If the article structure is used according to stock dimensions, fixed dimensions, and processed fixed dimensions, e.g. it is not necessary to specify vectors for the recording of prices for processed fixed dimensions. These have the same prices as the unprocessed fixed dimensions. Through assignment of an article to a vector, in such a case the base prices of the unprocessed fixed dimensions can be accessed.

For the article vectors, you control the price calculation by specifying the calculation base. The calculation base determines on which price level the price should be used, e.g. for scaled prices. ⇨ "Price type" on page C-50

#### Vector prices for processings

For processings, the prices are also created in vectors. The processing vectors offer the opportunity to scale the processing prices also according to the thickness of the glass.

_Fig. C-38 Example of processing vector_

In this example, you see that several definitions are created for one processing vector (A). These definitions distinguish themselves through the assigned price list, the thickness (B) of the glass and the price type (C). In addition, it is possible, as for article vectors, to specify a scaling per definition.

#### Vector prices for LAMI

For LAMI, the prices are also created in vectors. The assignment of the article price vector is done via the LAMI base prices. For this, the LAMI glass has to be set up as article with the article type 170 or 183. The pricing method _PCd laminated_ has to be assigned to the articles of these article types.

_Fig. C-39 LAMI example_

In this example, you see that the LAMI article and the vector (A) have the same number. The vector is maintained for several price lists (B).

#### Prices for color articles

For colored articles, the prices are created per article and color. For this, the articles have to be set up as colored articles. The articles must be assigned a valid color and the pricing method _PCd colored articles_.

_Fig. C-40 Example of colored articles_

In this example you see that the price is specified per colored article (A) and color (B).

#### Variant prices

Articles for which variant prices should be used have to be created as size variants.

_Fig. C-41 Example of variants_

In this example you see that the price is specified per article (A) and variant (B).

#### Prices for glazing

For glazing and edge sealing, the prices are created per article and calculation type. For this, the article type _Glazing_ or _Installation_ and the pricing method _PCd glazing_ has to be assigned to the articles in the master data.

_Fig. C-42 Example of variants_

In this example you see that the price is specified per article (A) and calculation type (B).

### Vector assignment

If several articles should be calculated with the same price vector, the articles have to be assigned to the vector.

_Fig. C-43 Vector assignments_

In this example, you see that the article numbers (A) correspond to the vector numbers. The articles (B) are assigned vectors with other vector numbers. These articles are calculated according to the vector with the specified vector number.

From this, the following rule emerges:

* Each article can only be assigned a single vector.
* Each vector can be assigned several articles.

> **Articles with the pricing method PCd laminated and PCd processing** For articles with the pricing method _PCd laminated_, you store the assignments on the _LAMI Basic Prices_ dialog. Only if an article is not assigned a vector there is the assignment from the article-vector assignment dialog used. For articles with the pricing method _PCd processing_, you store the assignment on the _Processing - Vector Assignment_ dialog.

### Creating article prices

In this example, you create an article vector with scaled prices and assign it an article.

This unit includes the following action sequences:

* "Here's how to create a price vector for articles" on page C-79
* "Here's how to assign an article to the vector" on page C-81
* "Here's how to create variant prices for an article" on page C-82
* "Here's how to create prices for glazing" on page C-84

> **Prerequisite** You have the required user rights. You have created the keys for the training.

#### Here's how to create a price vector for articles

1. Select _Master Data > Prices > PCd prices > All Article Price Vectors_ or _Spec. Article Price Vectors_. The following actions are identical for both dialogs.
2. Press `<F6>` to insert a new row. _Fig. C-44 Creating a price vector for an article_
3. Press `<F9>` and select the article vector (A) that you have created for the training.
4. Select the PLCD (B) that you have created for the training.
5. Select the calculation base _3-Quantity Scale per Unit (BQU)_ (C). With this calculation base, you can create scaled prices according to the basic quantity unit (BQU) of the article.
6. Use `<F2>` to change to the detail view in order to complete the settings. _Fig. C-45 Entering scaled prices_
7. Enter the price for the first price level and select the price type _GR/BQU_ (B).
8. Enter two additional quantity levels (A) and the associated prices. In the next action sequence, you will assign your price vector to a glass. Consider with the quantities according to which quantities you have to specify the scaled prices. Enter simple prices that you can easily convert to the limit quantities. So that you can trace the price calculation in the order, leave the fields for the minimum calculations and round sizes free.
9. Press `<End>` to save the data and close the dialog.

Now you have to assign all glass articles to the price vector that should be calculated with these prices.

#### Here's how to assign an article to the vector

1. Select menu _Master Data > Prices > PCd Prices > All Vector Assignments_.
2. Press `<F6>` to insert a new row. _Fig. C-46 Assigning articles to the vector_
3. Press `<F9>` and select a single glass (A), e.g. float 4 mm.
4. Select your vector (B).
5. Repeat steps 3 and 4 if you want to assign other kinds of glass to your vector.
6. Press `<End>` to save the data and close the dialog.

So that the vector prices are calculated according to your definitions, the price code (PCd) has to be specified in the daily terms. The terms are described in a separate unit. ⇨ "Conditions" on page C-121

#### Here's how to create variant prices for an article

1. Select menu _Master Data > Prices > PCd Prices > Variant prices_. _Fig. C-47 Creating variant prices for an article_
2. Press `<F6>` to insert a new row. _Fig. C-48 New row inserted_
3. Press `<F9>` and select the article (A) that you have created for the training.
4. Complete the PLCD, the variant, the calculation base, the price, and the price type.
5. Use `<F2>` to change to the detail view in order to specify scaled prices for the variant and a round size if necessary. _Fig. C-49 Creating scaled prices for an article variant_
6. Use `<F2>` or `<F6>` to change back to the list view.
7. Repeat steps 2 to 6 until you have created the prices for all variants of the article.
8. Press `<End>` to save the data and close the dialog.

#### Here's how to create prices for glazing

1. Select menu _Master Data > Prices > PCd Prices > Glazing_. _Fig. C-50 Creating glazing price_
2. Press `<F6>` to insert a new row.
3. Press `<F9>` and select the glazing article.
4. Add the PLCD, the calculation type, and the price.
5. Press `<End>` to save the data and close the dialog.

### Creating processing price

In this example, you create a processing vector with scaled prices and assign it a processing article.

> **Edge processing on shapes** Note that the length of the shape edges cannot be calculated precisely for price calculation. You can define in the master data which edge of the shape is calculated as width and height.

This unit includes the following action sequences:

* "Here's how to create a price vector for a processing" on page C-85
* "Here's how to assign a processing to the price vector" on page C-87

> **Prerequisite** A+W Enterprise is started. You have the required user rights. Processings are created as articles. You have created the keys for the training.

#### Here's how to create a price vector for a processing

1. Select menu _Master Data > Prices > PCd Prices > Processing Vectors_.
2. Press `<F6>` to insert a new row. _Fig. C-51 Creating a price vector for a processing_
3. Press `<F9>` and select the processing vector (A) that you have created for the training.
4. Select the PLCD (B) that you have created for the training.
5. Specify the glass thickness (C),e.g. 99. Note that this thickness is the upper limit value. The price is calculated up to this thickness.
6. Specify the quantity, e.g. 1. Note that the price is calculated starting with this quantity of processings per lite, e.g. 5 drillings on a lite.
7. Use `<F2>` to change to the detail view in order to complete the settings. _Fig. C-52 Entering scaled prices_
8. Select the calculation type _Qty/Item_ (B), e.g. for drillings.
9. Enter the price for the first price level.
10. Enter two additional quantity levels and the associated prices. Consider whether the price is reduced for drillings if there are several drillings on an item.
11. Press `<End>` to save the data and close the dialog.

Now you have to assign all processing articles to the price vector that should be calculated with these prices.

#### Here's how to assign a processing to the price vector

1. Select menu _Master Data > Prices > PCd Prices > All Vector Assignments_.
2. Press `<F6>` to insert a new row. _Fig. C-53 Assigning processing article to the vector_
3. Press `<F9>` and select the processing (A), e.g. a countersunk drilling.
4. Select your processing vector (B).
5. Repeat steps 3 and 4 if you want to assign other additional processings to your vector.
6. Press `<End>` to save the data and close the dialog.

### Base prices for LAMI lites

The prices for LAMI lites are generally calculated with the pricing method _PCd laminated_. For this, the price vectors are evaluated that are assigned to the respective LAMI article.

_Fig. C-54 LAMI base prices - details_

On this dialog, you see the details with which the calculation of the assigned price vector (A) is completed.

Furthermore, you can assign exchange and addition lists (B) with which glass is calculated that is exchanged or added to the article. In order to assign exchange and/or addition lists, these have to be created on the _Exchange/addition Lists_ dialog. The lists are described in detail in a separate unit. ⇨ "Exchange and additional prices" on page C-90

You can also assign step surcharges (C). Additional surcharges, e.g. for oversizes, can be created on the dialogs intended for this. The surcharges are described in detail in a separate unit. ⇨ "Surcharges" on page C-108

So that the LAMI lites are calculated according to your definitions, the price code (PCd) has to be specified in the daily terms. The terms are described in a separate unit. ⇨ "Conditions" on page C-121

### Exercises

For the exercise, use the keys that you have created for the training. If necessary, add the keys for the exercises. For the PLCD and PCd use only your training keys.

* Create a vector price for an accessory item.
* Create a vector price for a LAMI article.
* Assign the new LAMI vectors to the articles.

### Exchange and additional prices

**Objectives**

* Understand the meaning of exchange and additional prices.
* Get to know peculiarities for the exchange of patterned glass.
* Be able to distinguish particularities of the exchange lists for IG and LAMI.
* Create exchange lists with scaled prices.

**Benefits**

* With exchange lists, prices can be calculated if the BOM in an order item deviates from the defined article. Thus, it is not necessary to define an individual article and price vector for each possible BOM structure.

**Please note**

* **Exchange/additional lists**: These lists summarize the prices for BOM components that are exchanged in an IG or LAMI.
  * Individual keys are defined for exchange lists.
  * The prices are specified in the exchange lists.
  * Exchange lists are assigned in the base prices to the IG and/or LAMI articles.
* **Calculation type**: The calculation type specifies on which basis the price should be calculated.
* **Factor**: With factors, you can modify the calculation of the prices from the price lists without changing the prices individually. A factor of 100% means that the price is multiplied by 1. With a factor of 50%, the price is multiplied by 0.5. Generally a discount is granted with a factor. For this, the factor is < 100%.
* **Patterned glass exchange**: Patterned glass articles are assigned patterned glass classes.
* **Patterned glass classes**: Patterned glass classes summarize the exchange prices for the patterned glass. They are assigned to an exchange list.
* **Requirements**:
  * **Article master data**:
    * Item article: BOM permitted and changeable.
    * BOM: exchange allowed.
    * Exchange article: article type Part, FD.

### Exchange/additional lists

In lites with several layers of glass, single glass layers and/or foils can be exchanged or added.

> **Requirements** In the master data of the item articles and the exchange articles, it has to be specified that the exchange and installation is permitted. For details, see the Master Data section.
>
> IG exchange prices can only be created for articles that are marked in the article master data as fixed dimension (FD). LAMI exchange prices can also be created for articles that are marked as stock dimension (SD). Frames, muntins, and processings are additions to the BOM, but they are not calculated via exchange/additional lists. The prices for these components are described in separate units.

#### Keys and lists

In order to be able to calculate the exchange and addition articles, special price lists for exchange and additions are maintained. The exchange and additional lists are set up separately for IG and LAMI. However, both lists can access the same keys.

_Fig. C-55 Exchange/additional lists for IG and LAMI_

In this example, you see an exchange list (B) for the glass thickness 5 mm in which various articles (A) are assigned, each of which can be installed. In the exchange lists for LAMI, foils (A) can be specified in addition to glass.

With the factor (C), you can specify whether the price should be reduced or increased. A factor of 100% calculates the specified price. If you want to reduce prices, you can simply reduce the factor. Thus, all price levels are multiplied by the factor.

**Example**

| Factor: | Scaled price: | Price: |
| ------- | ------------- | ------ |
| 100%    | 15.00         | 15.00  |
|         | 21.00         | 21.00  |
|         | 27.00         | 27.00  |
| 90%     |               | 13.50  |
|         |               | 18.90  |
|         |               | 24.30  |

For the exchange of patterned glass, the same keys and lists can be used as for the exchange in IG and LAMI. The assignment of the articles is very different, however.

#### Assignment

The exchange and additional lists are assigned to the IG and LAMI articles separately. For this, they are specified in the base prices.

_Fig. C-56 Exchange lists in the base prices_

In these examples, you see that the exchange lists are set up per glass thickness. From the assigned lists, the prices are drawn that are specified for the exchange glass.

Theoretically, you can set up an individual key for each glass type, however with this, there is a lot more maintenance effort.

### Exchange prices for patterned glass

Patterned glass is calculated for exchange in IG lites via the exchange/additional lists. In the base prices for IG, you specify the exchange list from which the prices for patterned glass should be drawn. The prices for patterned glass are organized in patterned glass classes.

_Fig. C-57 Schema: definition of exchange prices for patterned glass_

#### Patterned glass classes

The permanently specified patterned glass classes are defined with the letters A - U. In these classes, the different exchange prices are stored per exchange list.

_Fig. C-58 Prices for patterned glass classes_

In this example, you see that for an exchange list (B), different prices (C) are specified for the price classes (D). These prices apply for a particular PLCD (A). Thus, all patterned glass that is assigned to this patterned glass class with this PLCD is calculated according to the prices specified.

#### Patterned glass exchange

The patterned glass articles are assigned to the patterned glass classes via which they should be calculated during exchange.

_Fig. C-59 Assignment of the patterned glass class to the patterned glass article_

In this example, you see that the price group B (D) is assigned to the selected patterned glass article (B). In addition, it is specified that the price from the price group B applies to this article per square meter (C).

**Example**

| Article               | Exchange list | Patterned glass class | Price |
| --------------------- | ------------- | --------------------- | ----- |
| Ornamental glass 4 mm | 4 mm glass    | B                     | 11.00 |

Exchange in the order: IG article 4x4 Dimensions: 1200 mm x 1800 mm

The exchange price is calculated according to the specified price type CU/sqm:

* Area calculation: 1200 mm x 1800 mm = 2.16 qm
* 2.16 qm x 11.00 € = 23.76 €

The exchange price for an IG article 4x4 with an ornamental glass 4 mm is EUR 23.76.

> **No From PLCD logic for patterned glass classes** The PLCD logic does not apply for patterned glass classes. Therefore, the prices in the patterned glass classes have to be maintained completely per PLCD.
>
> The price for an exchange patterned glass can only be calculated if an exchange list is defined for the PLCD that is used in the order for the price calculation.

### Creating exchange prices

In these examples, you create exchange lists for the exchange of glass in IG and LAMI.

> **Prerequisite** For the examples and exercises, you need an individual key for exchange and additional lists. Create one if you haven't done this in the unit about keys.

This unit includes the following action sequences:

* "Here's how to create an exchange list for IG" on page C-95
* "Here's how you create prices for patterned glass" on page C-97
* "Here's how to assign patterned glass classes” on page C-98
* "Here's how you assign the IG article an exchange list" on page C-99
* "Here's how to create an exchange list for LAMI" on page C-100
* "Here's how you assign the LAMI article an exchange list" on page C-101

#### Here's how to create an exchange list for IG

1. Select menu _Master Data > Prices > IG Prices > TG/LAMI/Special Exchange_. _Fig. C-60 Creating exchange list for IG_
2. Select the key (A) for the exchange/additional list and the PLCD (B).
3. Select the glass article (C) that can be installed in an IG lite with 6 mm float glass, e.g. sun protection glass. Note that in all examples and exercises for the exchange lists, the same glass thickness is always assumed.
4. Enter the factor 100 % (D) and the price (E).
5. Use `<F2>` to change to the detail view in order to complete the settings. _Fig. C-61 Creating exchange list for IG_
6. Enter the minimum area (A) that should be calculated.
7. If necessary, enter the round size if round sizes are typically used at your company. Note that the prices in the order can be more difficult to calculate. You can also expand the detailed settings step by step after the fact.
8. Select the calculation type (B):
   * Select _Area_ if the exchange price is defined by area. This is the default setting.
   * Select _Matrix_ if the exchange price should be read out of a matrix. With this selection, the Matrix field is also displayed, in which you have to select the number of the matrix. This setting only makes sense if the price of the specified article is defined in a matrix.
9. Enter at least 2 scale levels and the associated prices.
10. Repeat steps 3 to 9 for additional glass articles, e.g. for a TG and a LAMI. If necessary, note the article numbers so that you can check the prices of the articles.

#### Here's how you create prices for patterned glass

Make a plan according to which criteria you want to divide the patterned glass into classes, e.g. by manufacturer, pattern, etc.

1. Select menu _Master Data > Prices > IG Prices > Patterned Glass Classes_.
2. Select the key (A) for the exchange/additional list and the PLCD (B). Note that in all examples and exercises for the exchange lists, the same glass thickness is always assumed.
3. Select the patterned glass article (C) that can be installed in an IG lite with 6 mm float glass.
4. Enter the price (C) for at least the class A. If you have entered all prices, you can assign the patterned glass articles.

#### Here's how to assign patterned glass classes

1. Select menu _Master Data > Prices > IG Prices > Exchange Prices for Patterned Glass_.
2. Select the patterned glass article (A) and the PLCD (B).
3. Select the price type (C) with which the price should be calculated:
   * Select _CU/sqm_ if the price from the price group (class) should apply per area.
   * Select _Percent_ if the price from the price group (class) should be interpreted as a percentage value. The base price of the IG article is used as basis for the price calculation.
4. Enter the patterned glass class (D) with which the article should be calculated.
5. If necessary, add the factor and the minimum price.
6. Repeat steps 2 to 5 for at least 2 additional patterned glass articles.

Thus, you have created the exchange prices. Now you need to assign the price lists.

#### Here's how you assign the IG article an exchange list

1. Select menu _Master Data > Prices > IG Prices > Basic Prices_.
2. Select the IG article (A) and the PLCD (D).
3. Select the price type (B) with which the price for the IG article should be calculated, e.g. _Matrix_.
4. Select the matrix number (C).
5. Switch to the Detail view using `<F2>`.
6. Enter the number of your exchange list for all glass types (F).
7. If necessary, add the details for minimum calculation and round size.
8. Press `<End>` to save the data and close the dialog.

Thus, you have assigned the exchange lists.

#### Here's how to create an exchange list for LAMI

1. Select menu _Master Data > Prices > PCd Prices > LAMI Article > LAMI Exchange/Additional Prices_.
2. Select the key (A) for the exchange/additional list and the PLCD (B).
3. Select the glass article (C) that can be installed in a LAMI lite with 6 mm float glass, e.g. sun protection glass. Note that in all examples and exercises for the exchange lists, the same glass thickness is always assumed.
4. Select the calculation type (D).
5. Enter the factor 100 % and the price (E).
6. Use `<F2>` to change to the detail view in order to complete the settings.
7. Add the following details:
   * Area for the minimum calculation.
   * Round size.
   * At least 2 scale levels and scaled prices.
8. Repeat steps 3 to 7 for additional glass articles.

You can now assign these exchange lists to the LAMI articles.

#### Here's how you assign the LAMI article an exchange list

1. Select menu _Master Data > Prices > PCd Prices > LAMI Articles > LAMI Basic Prices_.
2. Select the LAMI article (A) and the PLCD (B).
3. Select the vector number (C).
4. Enter the number of your exchange list for the LAMI glass (D).
5. If necessary, add the details for step surcharges. Switch to the Detail view using `<F2>`.
6. Press `<End>` to save the data and close the dialog.

Thus, you have assigned the exchange list.

### Muntin prices

**Objectives**

* Get to know the relationship of price class and price code for muntins.
* Define muntin price class with prices.
* Get to know calculation types for muntins.
* Assign muntin articles.

**Benefits**

* With the breakdown of the muntin prices into price classes, there is no maintenance of the individual muntin articles.

**Please note**

* **Muntin code**: The prices lists for muntins are kept with their own price list codes, the M-PCd.
* **Muntin price classes**: Prices for muntins are combined into muntin price classes (M-class).
* **Muntin assignment**: Each muntin article has to be assigned a muntin price class so that the prices are calculated.

#### Definition scheme for muntin prices

The prices for muntins are combined into muntin price classes (MCPL) and organized in price lists (M-PCd). For this, individual muntin codes are created.

_Fig. C-67 Schema: definition of the muntin prices_

#### Muntin assignment

If you create the prices for muntins, enter the muntin code (M-PCd) and the muntin price class (MCPL). Assign the muntin class to the muntin article.

_Fig. C-68 Muntin prices and article assignment_

With the muntin price class, you combine muntin prices that are generally the same for a group of muntins. The muntin price classes are assigned to the appropriate muntin articles.

#### Calculation types for muntins

The specified price of a muntin class can refer to different elements of a muntin pattern.

_Fig. C-69 Reference elements of the calculation types_

The specified price refers to a reference element or a combination of the elements of a muntin construction. The prices can be calculated for the following elements:

* **Fields**: Price per field.
* **LM**: Price per linear meter.
* **/**: Price per intersection.
* **E**: Price per edge connection.
* **Special**: Individual price for each pattern element. Only available customer-specifically.
* **Percent**: Price as percentage that is calculated from the IG price.
* **sqm price**: Price per sqm of the glass.
* **Pieces**: For the muntin, a flat total price is stored, e.g. for the muntin pattern in the shape of a sun.

The prices can also be calculated for combinations of the reference elements. ⇨ Prices and Conditions, "Muntin Price Classes - Overview" on page C-273

The price-relevant quantity of muntin patterns is multiplied by the muntin price per muntin element. Here, up to two different muntin articles can be calculated, e.g. 12 mm muntin horizontal and 14 mm muntin vertical.

> **Different muntin articles** Muntin articles always count as different if they are entered in the muntin entry in different BOM entries. This means that two muntins with the same article number count as different muntin articles if they are entered in separate BOM entries, e.g. for a multiple IG.

### Creating a muntin price

In these examples, you create prices for muntins and assign the muntin articles.

> **Prerequisite** For the examples and exercises, you need an individual code for muntin price code and muntin price classes. Create at least one if you haven't already done this in the unit for the codes.

This unit includes the following action sequences:

* "Here's how to create the price for a muntin price class" on page C-105
* "Here's how to assign the muntin article to a muntin price class" on page C-107

#### Here's how to create the price for a muntin price class

1. Select _Master Data > Prices > Muntin Prices > Muntin Price Classes_. _Fig. C-70 Creating muntin prices_
2. Select the muntin price code (A) in which you want to specify the price.
3. Select the price code (B) that you have created for muntins.
4. Select the calculation type (C) according to which the muntin price should be calculated.
5. Enter the SA price for the pattern element that should be calculated, e.g. for the edge and the fields.
6. Use `<F2>` to change to the detail view in order to complete the settings. _Fig. C-71 Creating muntin prices_
7. Specify the minimum number of fields (B) that should be calculated.
8. Repeat steps 2 and 7 for another muntin price class (MCPL) and/or for another muntin price code (M-PCd).

#### Here's how to assign the muntin article to a muntin price class

1. Select _Master Data > Prices > Muntin Prices > Muntin Assignment_.
2. Press `<F6>` to insert a new row. _Fig. C-72 Article assignment_
3. Select a muntin article. You can only select the articles that are not assigned to a muntin price class.
4. Select the muntin price class that you have created for the exercise.
5. Repeat the steps for additional muntins.

So that the muntins are calculated according to your definition, you have to specify the muntin price code (M-PCd) in the daily terms. The terms are described in a separate unit. ⇨ "Conditions" on page C-121

### Surcharges

**Objectives**

* Distinguish possible applications for surcharge types.
* Distinguish calculation possibilities for surcharges.
* Create surcharges.

**Benefits**

* With surcharges, you expand the price definition. Thus, you can react to special steps in the production process without binding the appropriate prices to article prices.

**Please note**

* **Surcharges processing group**: Processing group surcharges are defined for processing groups. The surcharge is added to the price of a processing or a subpart. For this, the processing group has to be assigned to the article in the master data.
* **Shape surcharges**: Shape surcharges are distinguished by shape types or product groups, which are created for a PLCD. An individual surcharge is defined per shape number.
* **Pricing method**: Not all surcharges are evaluated for all pricing methods.
* **Surcharge type**: The surcharge type specifies how the surcharge is calculated, e.g. as fixed amount.
* **Surcharge base**: The surcharge base decides to what the surcharge refers, e.g. to the edge length.
* **Surcharge matrices**: Surcharge matrices are two-dimensional surcharges with the fixed quantity of 6 rows and columns. They can be assigned to IG base prices, articles, and processing vectors.

### Surcharge bases

Surcharges are created for the calculation of prices that depend on a production step:

* Size surcharges for order items that cannot be produced in standard production flows, e.g. for especially small lites or for overlong lites that have to be handled separately in dispatch.
* Shape surcharges for non-rectangular lites for which the waste is especially great or that have to be cut by hand.
* Surcharges for processing groups.
* Surcharges for steps on IG or LAMI lites.

Shape surcharges are calculated if a shape is assigned in the order item. All other surcharges are only calculated if they are specified in the base prices for IG or for LAMI lites.

### Shape surcharges

Non-rectangular shapes (shapes) require higher prices than standard articles due to the increased amount of processing and handling they require. That's why surcharges on shapes can be managed separately.

_Fig. C-73 Shape surcharges_

In this example, you see that for the individual shape numbers (A) per shape type (C) and PLCD (B), a surcharge (D) is created. In addition, there is a surcharge for processings (E) on the shape. As an alternative to shape types (C), you can specify a product group.

The shape surcharges can be calculated as percentage on the glass piece price, the base price of the item article or the base price of the glass including any exchange glass. How the shape surcharge is calculated depends on the stored terms. The processing surcharges are calculated as percentage surcharge on the processing price.

> **Edge processing on shapes** Note that the length of the shape edges cannot be calculated precisely for price calculation. You can define in the master data which edge of the shape is calculated as width and height. ⇨ Master Data, "Edge Allocation" on page B-164

#### Shape type

If you select the shape type, you may not specify a product group.

* **IG shape**: The surcharge is only charged if the item article is calculated according to the IG-current or IG-Switzerland pricing method.
* **TG shape**: The surcharge is only charged if the item article is calculated according to the PCd-TG pricing method.
* **LAMI shape**: The surcharge is only charged if the item article is calculated according to the PCd-laminated pricing method.
* **Retail shape**: The surcharge is only charged if the item article is calculated according to the PCd-basic glass or PCd-finishing pricing method.

#### Product group

As an alternative to the shape type, you can specify the surcharge for a product group. The price is then searched for using the product group logic.

**Example** The article in the order item belongs to product group 10 A2 21. During the price calculation, A+W Enterprise checks whether a surcharge is defined for precisely this product group. If no surcharge is found, the system searches in the product group 10 A2 \*_. If there is no surcharge found here, the product group 10 \*\* \*\* is checked. With an appropriate system setting, A+W Enterprise searches precisely to the place, that is, in the sequence: 10 A2 21, 10 A2 2_, 10 A2 \*\*, etc.

#### Minimum shape surcharge

The minimum shape surcharge is considered during the calculation of the sales and purchase prices and in the cost calculation for ordered glass. It is not used for processings. The minimum shape surcharge is not charged on exchange glass. It is displayed in the item terms and can be overwritten.

The minimum shape surcharge is charged if the following conditions are fulfilled:

* Pricing method: IG-current, IG-Switzerland, PCd-basic glass, PCd-finished glass, PCd-TG, PCd-laminated.
* Definitions in the terms and/or in the master data for the prices.

Depending on the specification in the daily and/or general terms, the minimum shape surcharge is calculated as follows:

| Setting     | Calculation                                                                                                                                                                        |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Base price  | The shape surcharge is only calculated from the glass base price. Then this value is compared to the minimum shape surcharge.                                                      |
| Glass price | The shape surcharge is calculated from the glass base price and in each case from the exchange prices. The minimum shape surcharge is compared to each of these individual values. |
| Item price  | The minimum shape surcharge is calculated from the item price. Then this value is compared to the minimum shape surcharge.                                                         |

> **Shape surcharge on exchange glass** If the environment variable `MINMODZU_NUR_AUF_GRUNDPREIS` is active and has the value ON, the shape surcharge for the pricing method IG-current is calculated only on the glass base price and not on the exchanged glass. For this, the shape surcharge Glass price has to be assigned in the terms master data.

### Surcharge matrix

In a surcharge matrix, percentage or currency surcharges or discounts can be stored. Surcharge matrixes can be assigned IG base prices, article and processing vectors, as well as individual lites for IG articles. They apply if the dimension of an item is no longer covered by the overlarge surcharge.

By default, searching in the surcharge matrix is done with rounded dimensions. If the environment variable `ZUSCHLAGSMATRIX_OHNE_MASSRUND` is active, searching is done with the precise dimensions.

In contrast to the price matrices, the surcharge matrices are limited to six columns and rows.

> **Specifying limit values** The row and column limit values have to be entered without gaps in the fields for the limit values. A field without limit value cancels the determination of the surcharge.

_Fig. C-74 Surcharge matrix_

In this example, you see a rectangular matrix for oversizes for TG glass. The surcharge is charged as fixed value (B) on the base price.

> **Surcharge calculation for IG articles** The surcharge for IG articles is not calculated on exchange prices, but rather directly on the IG base price.

When the surcharges are calculated depends on the surcharge type (C), e.g.:

* Starting with a particular area.
* Starting with a dimension for the longer edge.
* Starting with a particular edge dimension for both edges (overdimension).
* For particular aspect ratios.
* If the surcharge matrix is assigned to a processing vector.

The surcharge can also be charged as a percentage on the glass base price. For this, select the price type _Percentage_. ⇨ "Surcharges Matrices" on page C-286

> **Prio before size surcharges** For the pricing methods IG-current, PCd-laminated, and Calculation by single lites, you can specify that the surcharge matrices have higher priority than the size surcharges. This setting depends on the configuration in question.

Quantity discounts are generally only set up for processings if the machine only has to be set up once, e.g. for the dimension of drillings. Discounts are only considered if the surcharge matrix is assigned to a special article price.

> **Processing surcharge on the glass base price** Processing surcharges can be charged not only on the processing prices, but also on the glass base price. For this, in the surcharge matrix in the _Base_ field, the surcharge type _Glass base price_ has to be selected. In addition, in the _Minimum price_ field, a minimum surcharge can be specified that is charged on the glass base price if the processing in question is attached to the BOM.

### Size surcharges

Size surcharges are required for lites that fall outside of the default manufacturing process. If the lite is larger or smaller than a defined size, the surcharges are charged on the glass base price.

Size surcharges can be assigned to IG base prices, article vectors, LAMI exchange/addition prices, special IG base prices, special LAMI exchange/addition prices, and special article prices.

_Fig. C-75 Size surcharges_

For all size surcharges, you specify a value (D). For this, you specify the surcharge type (E), which specifies to what this value refers, e.g. as percentage surcharge on the glass price.

> **Evaluation of the surcharges** You can create a surcharge with all surcharges and assign the articles. However, the surcharges are only evaluated for the articles that are calculated with the appropriate pricing methods.

#### Size surcharges for vector prices

You can create the following size surcharges for pricing methods by vectors:

* Small glass surcharges (A) are scaled by area.
* Excess length surcharges (B) are scaled by edge length. Decisive is the longest edge in each case.
* Oversize surcharges (C) are scaled by the length of both glass edges. The surcharge is calculated if both edges have reached or exceeded the limit value.

The surcharges are charged one after another in the following sequence and calculated from the intermediate result: Base price

* Surcharge from the surcharge matrix
* Small Glass Surcharge
* Overlength Surcharge
* Oversize Surcharge

These surcharges are shown separately in the item terms.

#### Size surcharges for IG prices

For the pricing method IG-current by matrix and single lites, you can also create the following size surcharges:

* Aspect ratio surcharges (G) are scaled according to the aspect ratio of the sides. They are calculated if the specified aspect ratio 1:x is reached or exceeded.
* Surface surcharges (F) are scaled according to the area. They are calculated if the specified area is reached or exceeded.

> **Size surcharges on exchange prices** The size surcharges can also be calculated on exchange prices with appropriate configuration. For this, the variable `ISO_GROSSZU_AUF_AUSTAUSCH` has to be active. The surcharges are calculated directly on the glass base price. In the item conditions, the glass base price has already increased.

> **Tip - area surcharge for vector prices** If you want to create an area surcharge for vector prices, you can use the Small glass surcharges area for this. Enter the following values for this

| Up to quantity | Surcharge | Type    |
| -------------- | --------- | ------- |
| 0.50 sqm       | 10        | percent |
| 4.99 sqm       | 0         | percent |
| 5.00 sqm       | 20        | percent |
| 20.00 sqm      | 80        | percent |

> With these details, a surcharge for small glass and large glass is calculated. For the area from 0.51 - 4.98 sqm, there is no surcharge.

#### Oversize surcharge

For the oversize surcharges, surcharge levels have to be created in the correct sequence so that the program finds the correct value. If you create a surcharge for which both dimensions on the next level are not larger than on the previous one, the surcharge is not found.

| Examples                                                                    | Program instruction                                                                                                                                                                                                                                                                                                                                                                               |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Case 1: lite 2400 x 2400**                                                | check 2400 >= 2000 = yes > check 2400 >= 3200 = no: no surcharge since the first surcharge is defined for a larger lite.                                                                                                                                                                                                                                                                          |
| Sequence of the surcharge dimensions: 2000 x 3200, 2400 x 2400, 2400 x 3200 |                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Case 2: lite 2400 x 2400**                                                | check 2400 >= 2400 = yes > check 2400 >= 2400 = yes > surcharge, keep checking. Check whether a dimension is specified in the last row? = yes > check 2400 >= 2400 = yes > check 2400 >= 3200 = no. Check whether a dimension is specified in the second row? = yes > check 2400 >= 2000 = yes > check 2400 >= 3200 = no. check 2400 >= 2400 = yes > prüfe 2400 >= 2400 = yes: take the surcharge |
| Sequence of the surcharge dimensions: 2400 x 2400, 2000 x 3200, 2400 x 3200 |                                                                                                                                                                                                                                                                                                                                                                                                   |

### Processing group surcharges

The surcharges for processings are organized in processing groups.

_Fig. C-76 Scheme: processing group surcharges_

Processing group surcharges are charged on the base price of the processing from the master data:

* They are only charged if the price is determined from the master data.
* They are not charged if the base price is entered in the order entry manually or stored in the subparts or the terms, special terms, e.g. as a special price.

The processing group surcharge is charged if one of the following pricing methods is assigned to the processing article:

* 7 - Processing matrices
* 25 - PC prices general
* 26 - PCd processings
* 31- PCd colored articles
* 60 - protection

### Step surcharges

This function is only available with appropriate configurations. The prices of steps on IG and LAMI lites are calculated with step surcharge vectors. In the IG or LAMI base prices, you assign the step surcharge vector to the respective IG articles.

> **Step surcharge in the base prices** As an alternative to a step surcharge vector, you can create four scaled surcharges for LAMI in the base prices. In the base prices for IG< you can assign a surcharge and different calculation types.

### Exercises

For the exercise, use the keys that you have created for the training. If necessary, add the keys for the exercises. For the PLCD and PCd use only your training keys.

* Create an exchange price for glass.
* Create an exchange price for patterned glass. Use a patterned glass class for this that is not yet assigned data.
* Create a muntin price.
* Create surcharges for small glass and oversizes.
* Create shape surcharges.
* Assign the exchange prices and surcharges to the articles. Also select a LAMI article and a triple IG for which you also specify the exchange lists for the middle lite.
* Check the article master data and the price characteristics. ⇨ "Article master data" on page C-21

In order to calculate the SA prices, enter an order with the different items. Use simple quantities and dimensions, e.g. 1 pc. 1000 x 1000 so that you can check the calculation more easily.

Check in each case:

* Quantity and item price.
* Item characteristics.
* Order and/or item terms ( > price details).

Switch off the round size in the order terms and the surcharge if necessary so that you can better trace the amounts calculated.

### Global price changes

To change whole price lists, you have various possibilities. For example, you can change the daily terms or convert the prices on the price lists on the _Global Price Changes_ dialog. You can call up this dialog from the following dialogs with `<F4>`:

* TG/special exchange prices
* LAMI exchange/additional prices
* All article price vectors
* Processing vectors
* Colored articles
* Variant prices
* Muntin price classes
* Shape surcharges
* Article prices (no copy function).

_Fig. C-78 Global price maintenance_

On this dialog, you can change the prices in the following ways:

* Copy prices of a price list to a new PLCD and change them.
* Transfer whole price list or parts of the price list to an existing PLCD.
* Change prices of a price list, an article or a variant.
* Change prices of a series of price lists, articles or variants.
* Change prices of individual price levels.

You can also combine these functions. For a description of this, see the example for matrix conversion. For the conversion of matrices, the Convert matrices function is available in the matrix editor. ⇨ "Here's how to convert the matrix prices" on page C-68

### Conditions

Conditions are set up in the master data and in the order. This chapter only describes the terms from the master data.

The conditions include customer, supplier, industry, project, product group, and article-specific conditions and individual prices. The evaluation of these conditions follows a specified hierarchy, which is also reflected in the sequence of the condition dialogs.

This section provides information on the following subjects:

* "Priorities of condition determination" on page C-122
* "General and special conditions" on page C-129
* "Special prices" on page C-145
* "Complex exercise" on page C-151

### Priorities of condition determination

The evaluation of the conditions follows a specified hierarchy that is crucial for the determination of prices.

_Fig. C-79 Condition hierarchy_

* **1. Daily conditions**: The daily conditions are the basic conditions. They are always evaluated first for the condition determination. The following condition types are distinguished:
  * General daily conditions
  * Product group conditions In the _daily conditions_ it is specified which price lists, surcharges, and factors apply generally. Each market partner receives these conditions at first.
* **2. Special conditions**: The special conditions are conditions that only apply for particular market partners or product groups. They are evaluated according to the daily conditions. The following condition types are distinguished:
  * Customers
  * Suppliers
  * Project sales
  * Project purchasing
  * Conditions for industries. Market partner-specific prices lists, surcharges, and factors are stored in the special conditions. They override the entries from the daily conditions.
* **3. Special prices**: The special prices apply for market partners. They are evaluated last. The following types of conditions are distinguished:
  * Customers
  * Suppliers
  * Project sales
  * Project purchasing
  * Conditions for industries. The special prices override the conditions. If no special price is found, then the price from the assigned article vector or from the matrix is obtained with the PLCD determined.

All prices and conditions can be displayed in the order or item conditions and overwritten if necessary.

> **The more particular a condition, the higher its priority** The menu structure in A+W Enterprise is created as follows: The higher the priority, the deeper down in the menu tree it is. The higher priorities override the conditions found before them.

### Pricing sequence in the order

_Fig. C-80 Example: sequence for vector price_

* \* Search in general daily conditions to special conditions.
* \*\* Starting with PLCD logic: search again in older price lists with the smaller number.

### Example for determining the conditions

_Fig. C-81 Evaluation of the conditions, sequence_

In this example, you see that the conditions are evaluated according to the assigned PCd. The details from the current daily conditions apply until they are overridden on a higher priority level. In the order, the price of EUR 50.70 is calculated since the special article prices have the highest priority.

The calculation steps are described in detail below:

* In the general daily conditions, it is defined that the price is drawn from the PCd 200. In addition, the surcharge of 0% and a factor of 100% are assigned. On the price from the PCd 200, neither a surcharge nor a discount is calculated.
* In the special general conditions, no new price list is assigned. Thus, the PCd 200 still applies. However, a surcharge of 10% is assigned. In addition, in the product group conditions, a factor of 80% is defined. The special conditions override the daily conditions. A surcharge of 10% and due to the factor of 80%, a discount of 20% is calculated on the price from the PCd 200.
* In the special prices, an article price of EUR 50.70 is assigned. This special price overrides the price from the price list. Thus, no longer the price from the PCd 200, but rather the special article price of EUR 50.70 is used. By default, the surcharge of 10% and the factor of 80% are calculated on the special price. If, however, the environment variable `KEIN_TZ_BEI_SPEZARTPRS` is active, the surcharge is set to 0 and the factor to 100 if a special article price is found. The special article price of EUR 50.70 overrides the price from the PCd 200. Since the environment variable `KEIN_TZ_BEI_SPEZARTPRS` is active, a surcharge of 0% and a factor of 100% are calculated on the special price.

### Components of the conditions

Surcharges (SC) and factors can be specified in most conditions. They are specified in percentages and always refer to the article price.

_Fig. C-82 Example for surcharge and factor_

In this example, you see that for each pricing method, a surcharge (A) and a factor (B) are specified.

#### Surcharge

With the surcharge (SC), you increase the prices of a price list without changing the prices individually. If you enter the value 0 or a value < 0, no surcharge is calculated. If you do not want to calculate the general surcharge for a market partner, you have to set up individual conditions for this market partner in which the surcharge is specified as -1.

> **Environment variable KEIN\_TZ\_BEI\_SPEZARTPRS** With the environment variable `KEIN_TZ_BEI_SPEZARTPRS`, the surcharge and the factor can be switched off. If this variable is set, for special article prices the surcharge and discounts are switched off, so TZ=0 and factor=100. Here it plays no role where the surcharge is entered. This setting applies for purchasing and sales.

#### Factor

Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally, you set up factors for customers or projects in order to grant a special discount.

**Example**

| Factor                           | Base price | Final price |
| -------------------------------- | ---------- | ----------- |
| 100                              | 20.00 €    | 20.00 €     |
| 80 (corresponds to a discount)   | 20.00 €    | 16.00 €     |
| 150 (corresponds to a surcharge) | 20.00 €    | 30.00 €     |

### Master Data for Conditions

In this subject module, you will learn how to specify conditions in A+W Enterprise. Here, you have to consider the hierarchy of the evaluation of the conditions.

This chapter presents information about the following topics:

* "General and special conditions" on page C-129
* "Special prices" on page C-145
* "Complex exercise" on page C-151

### General and special conditions

**Objectives**

* Understand hierarchy of conditions.
* Distinguish condition types.
* Get to know function of the conditions.

**Benefits**

* With the General conditions, you can quickly make changes to the calculation specifications.
* If you have defined General daily conditions, you do not need to specify the conditions individually for each market partner.
* With the Special conditions, you can further differentiate calculation specifications for individual market partners product groups, and product types.

**Please note**

* **General conditions**: With the General conditions, you define calculation specifications that apply globally. Without the General daily conditions, no prices are calculated if no other conditions are specified.
* **Factor**: With factors, you can modify the calculation of the prices from the price lists without changing the prices individually. Generally a discount is granted with a factor. For this, the factor is < 100%.
* **Validity**: Conditions are defined for a particular period of time. When the end date is reached the conditions are no longer evaluated.
* **Condition type**: General daily conditions and (general) Product group conditions are only distinguished by the condition types Sales and Purchasing. Special conditions are distinguished by market partners.
* **Market partner**: Market partners in the sense of conditions are:
  * Customers
  * Suppliers
  * Industries
  * Projects in sales or in purchasing.
* **PCd**: The PCd refers to the price list from which the prices should be taken. The current PCd is assigned in the conditions.
* **Priority**: For the conditions, it applies that:
  * Daily conditions have the lowest priority.
  * Special conditions have a higher priority than the daily conditions.
  * Special prices override the Daily conditions and the Special conditions.
* **Special conditions**: With the Special conditions, you define calculation specifications that apply only for individual market partners.
* **Surcharge (SC)**: The surcharge (SC) is a percentage surcharge on a price list.

### General daily conditions

With the general daily conditions, you specify the calculation specifications per price calculation method. The general daily conditions apply for all market partners, insofar as no special conditions are defined.

_Fig. C-83 General daily conditions_

In this example, you see the General daily conditions for sales (A). A PCd (F) is assigned per price calculation method (B). The PCds are assigned to a price list from which the current prices are read out.

If you have created a new price list for a price calculation method, you can activate this price list in different ways:

* You assign the new price list to the PCd. Thus, this price list applies for all market partners insofar as the setting is not overridden by other conditions.
* You create a new PCd to which you assign the new price list.
  * You can enter the new PCd in the conditions for all market partners for whom the prices from the new price list should apply. You leave the old PCd in the general daily conditions.
  * You enter the new PCd in the general daily conditions. This way, the prices are read from the new price list. The deviating settings for the market partners still apply.

The assignment is described in a separate unit: ⇨ "Price code (PCd)" on page C-26

The surcharge (G) is an additive surcharge on all prices that are read from the respective price lists. Thus, you have the opportunity to increase the prices in the short term without having to adjust the price lists themselves. ⇨ "Surcharge" on page C-127

The factor (H) is a multiplier, that is generally used as discount for a customer. ⇨ "Factor" on page C-127

> **Environment variable KEIN\_TZ\_BEI\_SPEZARTPRS** With the environment variable `KEIN_TZ_BEI_SPEZARTPRS`, the surcharge and the factor can be switched off. If this variable is set, for special article prices the surcharge and discounts are switched off, so TZ=0 and factor=100. Here it plays no role where the surcharge is entered. This setting applies for purchasing and sales.

For scaled prices, with the scale level (I), you specify from which level the price should be read out. The setting is evaluated for article price vectors with the price type _2-Scal.Level_. In the _General daily conditions_, you generally specify the level 1. With this setting possibility, you can create scaled prices and specify the appropriate step in the conditions for market partners.

The minimum processing price (K) generally applies to all relevant processings of the BOM. For this, the following conditions must be met:

* Processing articles for which the minimum processing prices should be calculated have to be marked in the master data as minimum price-relevant. The minimum price always applies per lite. For price calculation, the amounts per processing are added up. The minimum processing price is calculated if the total is smaller than the defined minimum price.
* The environment variable `VSG_MIN_BEAPREIS` or `ESG_MIN_BEAPREIS` has to be active. The minimum processing prices are only calculated for item articles with the pricing method _PCd-tempered_ or _PCd-laminated_.

To calculate the unit price, you can activate a unit price rounding (J). ⇨ "Unit price rounding" on page C-46

The validity (L) of conditions is for a limited time, so that after the end date, they are no longer checked. For the General daily conditions, this means that no more prices can be calculated.

### Special general conditions

You can override all settings in the General daily conditions for individual market partners, projects or industries.

_Fig. C-84 Special conditions_

In this example, you see that a market partner (C) is selected. For this market partners, some other calculation specifications apply (B). For all fields without specifications, the General daily conditions apply.

### Product group conditions

On this dialog, you specify the conditions that apply only for particular product groups. These conditions take precedence over the General daily conditions.

With the Product group conditions, you define calculation specifications for individual product groups. The general Product group conditions apply for all market partners insofar as no special conditions are defined.

You can specify any level of the product groups, e.g. 10\*\*\*\*, 11A1\*\*, 20G131. The conditions apply only for the product group of the item article.

_Fig. C-85 General conditions for product groups_

In this example, you see that you can specify not just other values for the PCd, the surcharge, and/or the factor of a product group, but you can also other assign other surcharges (B - E). These surcharges are described in a separate unit. ⇨ "Surcharges" on page C-108

Furthermore, per product group, you can specify a different round size (F) for glass.

### Special product group conditions

You can override all settings in the (general) product group conditions for individual market partners, projects or industries.

_Fig. C-86 Special conditions for product groups_

In this example, you see that for the selected market partner, some different calculation specifications apply for the specified product group.

In addition, instead of a factor, you can specify five different discounts. These discounts are totaled up and combined into a factor:

**Example**

* **Discount 1: 80%**
  * Factor = 20% The customer pays 20% of the price.
  * Base price = 100 €
  * End price = 20 €
* **Discount 1: 80%, Discount 2: 60%**
  * Factor = 8%
  * Base price = 100 €
  * End price = 8 €
  * 100 € - 80% = 20 €, 20 € - 60% = 8 €

For all fields without specifications, the General daily conditions, Product group conditions or the Special general conditions apply.

### Article conditions

You set up the Article conditions analogously to the special Product group conditions. These conditions override the general and special daily and product group conditions.

With these conditions, you define the calculation specifications for individual articles. The Article conditions apply for a particular market partner, a project or an industry.

_Fig. C-87 Special conditions for article conditions_

In this example, you see that sometimes different calculation specifications apply for the selected project.

The Article conditions are especially suitable for construction projects for which special conditions are granted and that apply for several customers and/or suppliers. The conditions are each evaluated if the appropriate project is specified in the order.

### Discount scaling

On this dialog, you can define scaled discounts that only apply for particular customers. The _Scales of Discount_ are only evaluated for item articles to which the pricing method _IG-Switzerland_ is assigned.

You can specify different quantity discounts for the item articles and the exchange glass of the IG article. Quantity discounts refer to the physical total quantity of all articles of an order with the pricing method _IG-Switzerland_. Depending on configuration of the environment variable `AUFRUNDEN_FLÄCHE`, the total quantity is rounded up or commercially rounded. The discount is specified in percentage. The quantity discount for item articles is deducted from the glass base price, the quantity discount for exchange glass from the exchange price.

In addition to the quantity scale discounts, you can set up a series discount. The series discount refers to the item quantity of an article. It is deducted from the glass base price.

_Fig. C-88 Discount scaling for customers_

In this example, you see that for the selected customer, a special quantity discount is specified for item articles (A). A quantity discount for exchange glass (B) or a series discount for the individual item articles (C) has not yet been set up for the customer.

The scaled discount is only valid up to a particular end date (D). By default, a validity date of 5 years is set. You can overwrite this value manually. After the end date, the general prices and conditions are used for the price calculation. If you still want to work with the special conditions, you have to redefine the scaled discount.

### Special factors

For product groups, articles, muntins, and exchange lists, you can set up special factors that are generally used like discounts. The factors apply for particular market partners, projects or industries.

The factors can be set up as surcharge or discount on the prices. If you specify a factor < 100%, it is used as discount. A factor > 100% increases the price accordingly.

#### Product group and article factors

Product groups and article factors are created the same way. For product groups and articles, you can define several factors as quantity scale. For this, you have to specify the type of factor determination. The type specifies how the limit quantities are interpreted:

* **BQU**: The limit quantity corresponds to the basic quantity unit (BQU) that is stored in the article master data, e.g. per square m, linear m, etc.
* **Pcs**: The limit quantity corresponds to the number of articles.

_Fig. C-89 Special factors for product groups, articles_

In these examples, you see factors scaled by quantities (C) for a product group (B) and for an article (D). These conditions apply only for the specified market partner (A). The factors are used for price calculation if the specified limit quantity is reached.

#### Muntin factors

For muntin articles, you can specify a factor per muntin price class and muntin price code.

_Fig. C-90 Special factors for muntins_

In this example, a special factor (D) is set up for all muntins that are assigned to the muntin price class 1 (A) and the muntin price code 1 (C). The factor only applies for the market partners to whom the specified industry (B) is assigned.

#### Exchange list factors

For exchange lists, you can create a factor per IG and/or LAMI product group and PLCD.

_Fig. C-91 Special factors for exchange lists_

In this example, for the exchange list 5 (D) starting with the PLCD 5000 (E) a special factor (F) is specified. The factor is used for price calculation if an exchange glass of the product group 35F304 (C) in an IG article (A) is exchanged. The factor only applies for the specified market partner (B).

> **Product group logic for exchange list factors** By default, the product group refers to the product group of the exchange glass. You can configure A+W Enterprise so that the exchange list factors for the product group apply, which arise according to the exchange for the header part. For this, the environment variable `SPEZATLFAKT_KOPFTWAGRP` has to be active.

### Surcharges for shapes, AIR

For shapes and airspace (AIR), you can set up surcharges that are only used for a particular market partner.

_Fig. C-92 Shape surcharges_

In this example, you see various shape surcharges (A) for a market partner. Here, you can distinguish between a surcharge for the shape (D) and a surcharge for the processing (F) on the shape. For both surcharges, it applies that:

* Enter -1.0 if no surcharge should be charged.
* Leave the field empty if the surcharge should be drawn from the _Shape surcharges_ price dialog.

You can restrict the calculation of a surcharge either to a product group (B) or to a shape type (C). The shape type refers to the pricing method of the item article:

* **IG-shape**: Pricing method IG-current or IG-Switzerland.
* **TG shape**: Pricing method PCd-tempered.
* **LAMI shape**: Pricing method PCd-laminated.
* **Retail shape**: Pricing method PCd-basic glass or PCd-finished glass.

Furthermore, you can specify a minimum value (E) for the shape surcharge. This surcharge is charged if the calculated shape surcharge in the order is less than this minimum surcharge.

### Creating AIR surcharges

For the spacers, you can create surcharges for up to 12 different AIR. The AIR surcharges are charged if the AIR underruns the specified mm scales on the assigned IG article.

#### Here's how to create surcharges for the AIR in IG

1. Select _Master Data > Conditions > Special Conditions > AIR Surcharges_. _Fig. C-93 Creating AIR surcharges_
2. Use `<Toggle>` to select the condition type (A), e.g. Customer.
3. Jump to the next field (B) and specify the customer number or select it.
4. Press `<Enter>` to import the data.
5. Press `<F6>` to insert a new row. _Fig. C-94 New row inserted_
6. Select the IG article (A) and enter the PLCD (B).
7. Switch to the Detail view using `<F2>`. _Fig. C-95 Creating a scaled surcharge_
8. Enter the first limit value (A) for the AIR up to which the surcharge should apply, e.g. 8 mm.
9. Enter the surcharge value (B) and the surcharge type (C), e.g. 2 percent.
10. Repeat steps 8 and 9 until you have specified all levels for the current IG.
11. Repeat steps 6 and 9 for the next IG article.

### Special prices

**Objectives**

* Get to know the difference between special prices and special conditions.
* Get to know priority of the special prices.

**Benefits**

* With the Special prices, you can specify individual prices for a market partner, which are time-limited, e.g. during a construction project.

**Please note**

* **Factor**: With factors, you can modify the calculation of the prices from the price lists without changing the prices individually. Generally a discount is granted with a factor. For this, the factor is < 100%.
* **Validity**: Special prices are defined for a particular period of time. When the end date has been reached, the conditions are no longer evaluated.
* **Market partner**: Market partners in the sense of prices are:
  * Customers
  * Suppliers
  * Industries
  * Projects in sales or in purchasing.
* **Priority**: For the conditions, it applies that:
  * Daily conditions have the lowest priority.
  * Special conditions have a higher priority than the daily conditions.
  * Special prices override the Daily conditions and the Special conditions.
* **Surcharge (SC)**: The surcharge (SC) is a percentage surcharge on a price list.
* **Special prices**: The special prices override all prices from the master data and price lists. Special prices can be created for the following prices:
  * Article prices
  * Variant prices
  * Prices for colored articles
  * Muntin prices
  * Processing prices
  * IG exchange prices
  * IG single lite prices
  * IG base prices
  * UV coating prices
  * Glazing prices
  * Patterned glass exchange prices
  * LAMI exchange/additional prices

### Special prices for articles and colored articles

With the Special prices, you specify prices for market partners. The special prices override details from the master data for the prices.

The Special prices are set up analogously for all prices. On the following dialogs, the special prices are created for articles and colored articles.

_Fig. C-96 Special prices for articles, colored articles_

In these examples, you see that the definitions for market partner-specific prices are defined with the same components are the BQU prices for articles. ⇨ "Pricing components" on page C-43

In addition, you can specify a step surcharge vector (A). The from-PLCD logic (D) also applies for the special prices.

> **Only specify deviations** On all dialogs for special conditions and special prices, you only have to fill the fields that should be calculated differently from the master data prices and conditions.

### Special prices for IG single lite prices

In this example, you create special prices for IG single lite prices.

For the calculation of IG prices from the installed single lites, you can create special prices for a market partner, an industry or a project.

> **Prerequisite** The IG has to be assigned the type _Single lite_ in the IG base prices. ⇨ "Special IG Basic Prices" on page C-420

This unit includes the following action sequences:

* "Here's how to create special single prices for IG single lites" on page C-148
* "Here's how to create special scaled prices for IG single lites" on page C-149

#### Here's how to create special single prices for IG single lites

1. Select _Master Data > Conditions > Special Prices > Single Lites for IG Products_.
2. Use `<Toggle>` to select the condition type (A), e.g. Project-Sales.
3. Jump to the next field (B) and specify the project number or select it.
4. Press `<Enter>` to import the data.
5. Press `<F6>` to insert a new row.
6. Select the single lite (A) and enter the PLCD (B).
7. Enter the price type _1 Single price_ (C) and select the price type _GR/BQU_ (D).
8. Specify the price (E) for this single lite. The price is calculated if this glass is installed in an IG for the specified project.
9. Press `<End>` to save the data and close the dialog.

#### Here's how to create special scaled prices for IG single lites

1. Enter the individual lite as described in steps 1 to 5 of the action sequence above.
2. Select the single lite and enter the PLCD.
3. Enter the price type _3 - Quantity Scale per Item (BQU)_ or _4 - Quantity Scale per Unit (BQU)_ and select the price type _GR/BQU_ or _GR/Unit_.
4. Specify the price (E) for this single lite. The price is calculated if this glass is installed in an IG for the specified project.
5. Use `<F2>` to change to the detail view in order to scale the price for the single lite.
6. Specify the first limit value (A) for the glass starting with which the price should apply, e.g. 0.5. This value refers to the calculation base. The quantity unit for glass is generally square meters. If you have selected the price type _3 - Quantity Scale per Unit (BQU)_, this corresponds to the total square meters for an item, that is, number of square meters of the lite x number of lites in the item.
7. Specify the price (B) for the scale level.
8. Repeat steps 6 and 7 until you have specified all levels for the current glass.
9. Press `<End>` to save the data and close the dialog.

### Complex exercise

Create a training customer and set up the conditions with your PLCD.

Check:

* Have you entered at least one IG price completely: matrix, assign articles, assign surcharges (base prices)?
* Have you assigned your PCd to your PLCD?

Try to trace the price calculation in the order:

* Enter an order with one IG item with shape apiece, with muntins, with processing, and with exchange.
* Copy this order for your training customer and compare the prices.
* Are there deviations? Can you trace your prices? What do you need to correct?

### Cost Calculation

With the cost calculation, you can calculate per order item how high the current costs are and check the contribution margin. In the configuration of A+W Enterprise it is specified whether only the material costs are determined or also the machine and personnel costs.

The cost calculation determines the following costs:

* Material costs are calculated by A+W Enterprise for the item entry using the details from the article master data. If the environment variable `NEUKALK_VKEK` is active, with each change in the item, a query for recalculation of the material costs is displayed.
* Machine costs and personnel costs are determined by A+W Production and A+W Capacity Planner using the costs for machines and wages, as well as the planned duration of work per machine.

For calculation of the machine and personnel costs, the order is transferred to production. The personnel and machine costs are determined and reported back.

> **Environment variable AWC\_POOL\_NO\_KOSTENKALK** If the environment variable `AWC_POOL_NO_KOSTENKALK` is active, the order has to be released and scheduled in production so that the costs are determined.

If the production transfer for quotations is configured in A+W Enterprise, the costs for quotations can also be calculated. Quotations are only scheduled in A+W Production in preliminary fashion and deleted from the production batch after reporting of the costs.

> **Machine and personnel costs** The settings for the calculation of machine and personnel costs are described in the documentation for A+W Production and/or A+W Capacity Planner.

The material costs in the order item will be updated in the following cases:

* For price-relevant changes to the order, which cause a recalculation of the prices, e.g. processing of the dimension of an item article.
* In case of change to prices in an order-related PO or in incoming goods and active purchasing cost recalculation.

### Material costs

Decisive for the calculation of material costs is the supply type. It is assigned to the article in question in the article master data. It can be changed per BOM element. Decisive for the calculation of material costs in the order is the supply type that is set in the item and the BOM.

The supply type specifies where the article comes from:

* **Stock**: The article will be kept in stock and can be removed directly from there.
* **Production**: The article will be created by production.
* **PO**: The article will be purchased.

#### Material costs for stock materials

The material costs are calculated depending on the configuration of the environment variable `KOSTENKALK_MIT_LAGERPREIS` as follows:

* `KOSTENKALK_MIT_LAGERPREIS` not active: The material costs are calculated using a material cost list. This list includes the average PU price including storage costs, material overhead costs, etc. You assign the material cost list for the condition type _Purchased_ on the _General daily conditions_ dialog. ⇨ "General Daily Conditions" on page C-308
* `KOSTENKALK_MIT_LAGERPREIS` active, value PRIO: The material costs are calculated using the stock average price of the default stock. You specify the default stock in the article master data. If no price can be determined, the material cost list is used.
* `KOSTENKALK_MIT_LAGerpreIS` active, value ON: The material costs are calculated using the material cost list. If no price can be determined, the average stock price of the default stock is used.

In addition, in the article master data in the _Loss of material_ field, an average loss can be stored that is used automatically for the calculation.

#### Material costs for purchased goods

The costs for purchased goods are calculated using the stored PU prices and the conditions. This also applies for purchased subparts.

The price changes from the order-related POs are written back for the following procedures to the material costs for the order:

* PO generation
* PO change
* Creation of a dispatch notification
* Manual goods receipt
* Manual invoice creation
* Invoice control

The Purchasing module has to be used for this and the environment variable `EK_RUECKRECHNUNG` has to be active.

#### Article master data

In the article master data, you specify whether an article is included in the cost calculation.

> **Calling up stock costs without price list** A+W Enterprise can be configured so that the stock costs are drawn directly from the stock regardless of the material cost list. Here, the current average price of the default stock is used. Thus, the price list no longer has to be updated if new articles are booked to stock or booked out of the stock.

**Cost calculation** The field is evaluated only if for the article, the supply type Production is selected in the order. For articles with the supply type Stock or PO, the costs are always calculated.

* **no**: The BOM subpart is not evaluated in the cost calculation. The article BOM will be searched in descending order for other, cost-relevant articles.
* **yes**: This BOM subpart is included in the cost calculation. The material costs are calculated from the material cost list. The BOM of the article is not searched further for cost-relevant articles.
* **yes/next**: The costs for the article are calculated from the material cost list. They are incorporated in the costs as an internal contribution margin. The article's BOM is searched in ascending order for additional cost-relevant articles.
* **Loss/next**: The loss is analyzed for all BOM elements if the supply type is Production or Stock and if they are marked as Loss/next.

Even the main BOM element will be evaluated if its supply type is _Production_ or _Stock_ and is marked by Loss/next.

The loss of material (B) can be used at will, e.g. for waste. A loss will be calculated when the article is produced or when stock dimensions are withdrawn from stock. The loss of material affects the quantity used to calculate the unit price based on the quantity unit price.

The loss of material for a float stock size that is part of a TG, is calculated as follows: loss-WM x loss FD x loss-TG

**Example:**

* **TG 300008**
  * Supply type: Production
  * Cost calculation: Loss/next
  * Loss: 10%
* **Float-FM 110008**
  * Supply type: Production
  * Cost calculation: Loss/next
  * Loss: 5%
* **Float CS 100008**
  * Supply type: Stock
  * Cost calculation: Loss/next
  * Loss: 8%

The loss for the article 30008:

* Step 1 - Float BM: 1.08 x 1.05 = 1.134 commercially rounded, is 1.13
* Step 2 - TG: 1.13 x 1.10 = 1.243, after rounding 1.24
* Loss: 24%

The calculation of the material requirements goes from top to bottom in the BOM tree. The calculated value is commercially rounded after each step. This logic applies analogously for subparts with the supply type _Production_ and the cost calculation flag _yes_. For purchased subparts, generally no loss is calculated.

> **Calculating material loss for subparts** The environment variable `KOSTENKALK_MIT_VERLUST` can include a list with up to 10 article types. If this environment variable is active, the costs with material loss for all subparts are calculated in the cost calculation whose article type is included in the list and that have the supply type Stock or PO.

### Relationship of supply type and cost calculation

_Fig. C-102 BOM with different supply types_

In this example, you see an IG BOM that consists of articles with the supply types _Production_ and _Stock_.

#### Supply type Production

If the BOM contains an article with supply type _Production_, the cost calculation flag belonging to this article determines whether or not the sub-tree of this article is included in the cost calculation.

* **Cost calculation = yes**: The sub-tree of the article is not checked. The costs of the current article are drawn from the material cost list.
* **Cost calculation = no**: The costs of the sub-tree of the article are checked, that is, the BOM is broken down further. The costs of the subarticles are used for cost calculation, those of the item article not.
* **Cost calculation = yes/next**: The sub-tree of the article is checked and the costs of the subparts added to the costs of the article. This does not apply if the article is an item article.
* **Cost calculation = Loss/next**: All parts of the BOM are checked and the loss of the subparts and the item articles added. The material loss is drawn from the article master data.

## Software Reference

### Overview

Generally the prices are calculated automatically when the items in the order are entered.

For each product group, an individual pricing method is used, which is attuned to the specific properties of the product group, e.g. the pricing method _IG-current_. The pricing method is assigned to the article in the article master data.

For the calculation of the prices, the master data has to be created completely for the prices. The _Prices and Conditions_ section describes the master data that is used for the price calculation.

In addition, you can overwrite the prices in the order manually. These functions are described in the _Sales_ section.

In the _Prices and Conditions_ section, you will find the following topics:

* "Price Keys" on page C-167
* "Prices" on page C-176
* "IG Prices" on page C-182
* "PCD Prices" on page C-220
* "Muntin Prices" on page C-272
* "Surcharges" on page C-279
* "Price Control" on page C-299
* "Conditions" on page C-306
* "Daily Conditions" on page C-307
* "Special Conditions" on page C-321
* "Special Prices" on page C-377

### Price Menu

Some of the available menu entries branch out to submenus. If these include more than three entries, they are listed separately according to the following overview.

All dialogs and functions where you set up the prices and price calculation can be reached via the _Master Data > Prices_ menu:

| Shortcut | Description                                                                                                         |
| -------- | ------------------------------------------------------------------------------------------------------------------- |
| a        | ⇨ "IG Prices Menu" on page C-162                                                                                    |
| b        | ⇨ "PCD Prices Menu" on page C-163                                                                                   |
| ca       | ⇨ "Muntin Price Classes" on page C-175                                                                              |
| cb       | ⇨ "Muntin Assignment" on page C-278                                                                                 |
| d        | ⇨ "Surcharges Menu" on page C-163                                                                                   |
| e        | ⇨ "Price Keys Menu" on page C-164                                                                                   |
| f        | ⇨ "Price Control Menu" on page C-164                                                                                |
| g        | Opens the _External Formats_ dialog where you can write matrices in other formats. ⇨ "Price Export" on page C-181   |
| h        | Opens the _List Print_ dialog in order to print lists of the defined prices. ⇨ Sales, "List Printing" on page D-368 |

#### IG Prices Menu

_Master Data > Price > IG Prices_

With this menu, you can access all dialogs on which you set up the prices for articles with the pricing methods _IG-current_ and _IG-Switzerland_.

| Shortcut | Description                                       |
| -------- | ------------------------------------------------- |
| a        | ⇨ "IG Basic Prices" on page C-183                 |
| b        | ⇨ "Single Lites for IG Products" on page C-189    |
| c        | ⇨ "Matrix Editor" on page C-194                   |
| d        | ⇨ "Matrix Calculation" on page C-203              |
| e        | ⇨ "Pattern Classes" on page C-206                 |
| f        | ⇨ "Pattern Exchange" on page C-207                |
| g        | ⇨ "TG/LAMI/Special Exchange Prices" on page C-209 |
| h        | ⇨ "AIR Surcharges" on page C-215                  |
| i        | ⇨ "UV Protection" on page C-217                   |

#### PCD Prices Menu

_Master Data > Prices > PCD Prices_

With this menu, you can access all dialogs on which you set up the prices for articles with PCD pricing methods _PCD-tempered_ and _PCD-laminated_.

| Shortcut | Description                                               |
| -------- | --------------------------------------------------------- |
| a        | ⇨ "Article Price Vectors" on page C-221                   |
| b        | ⇨ "Special Article Vectors" on page C-228                 |
| c        | ⇨ "Article Vector Assignment" on page C-230               |
| d        | ⇨ "Special Vector Assignments" on page C-231              |
| e        | ⇨ "Processing Vectors" on page C-232                      |
| f        | ⇨ "Special Processing Vectors" on page C-237              |
| g        | ⇨ "Processing - Vector Assignment" on page C-240          |
| h        | ⇨ "Processing - Matrix Assignment" on page C-241          |
| i        | ⇨ "Minimum Processing Price" on page C-243                |
| ja       | ⇨ "LAMI Basic Prices" on page C-245                       |
| jb       | ⇨ "Special LAMI Basic Prices" on page C-249               |
| jc       | ⇨ "LAMI Exchange/Additional Prices" on page C-251         |
| k        | ⇨ "PCD Prices for Colored Articles" on page C-256         |
| l        | ⇨ "Special PCD Prices for Colored Articles" on page C-261 |
| m        | ⇨ "Variant Prices" on page C-263                          |
| n        | ⇨ "Special Variant Prices" on page C-266                  |
| o        | ⇨ "PCD Glazing Prices" on page C-269                      |

#### Surcharges Menu

_Master Data > Prices > Surcharges_

With this menu, you can access all dialogs on which you set up surcharges.

| Shortcut | Description                                                                                    |
| -------- | ---------------------------------------------------------------------------------------------- |
| a        | ⇨ "Shape Surcharges" on page C-280                                                             |
| b        | ⇨ "Special Shape Surcharges" on page C-284                                                     |
| c        | ⇨ "Surcharges Matrices" on page C-286                                                          |
| d        | ⇨ "Thickness Surcharges Vectors" on page C-289                                                 |
| e        | ⇨ "Size Surcharges" on page C-291                                                              |
| g        | ⇨ "Processing Group Surcharges" on page C-297                                                  |
| h        | Opens the _Offset surcharge vectors_ dialog. The dialog is only enabled customer-specifically. |

#### Price Keys Menu

_Master Data > Prices > Price Keys_

With this menu, you can access all dialogs on which you set up the price keys.

| Shortcut | Description                                 |
| -------- | ------------------------------------------- |
| a        | ⇨ "Price Lists (PLCD)" on page C-168        |
| b        | ⇨ "Price Code (PCD)" on page C-169          |
| c        | ⇨ "Matrices" on page C-170                  |
| d        | ⇨ "Exchange/Additional Lists" on page C-171 |
| e        | ⇨ "Article Vectors" on page C-172           |
| f        | ⇨ "Processing Vectors" on page C-173        |
| g        | ⇨ "Muntin Price Code" on page C-174         |
| h        | ⇨ "Muntin Price Classes" on page C-175      |

#### Price Control Menu

_Master Data > Prices > Price Control_

With this menu, you can access all dialogs on which you set up special rules for price calculation.

| Shortcut | Description                               |
| -------- | ----------------------------------------- |
| a        | ⇨ "Price Control" on page C-300           |
| b        | ⇨ "Rules: SA-PU Factor" on page C-302     |
| c        | ⇨ "Bonus Rules" on page C-303             |
| d        | ⇨ "Price List Control" on page C-304      |
| e        | ⇨ "Price List Restrictions" on page C-305 |

### Conditions Menu

Some of the available menu entries branch out to submenus. If these include more than three entries, they are listed separately according to the following overview.

You can access all dialogs and functions where you specify the market partner-specific conditions via the _Master Data > Conditions_ menu:

| Shortcut | Description                                |
| -------- | ------------------------------------------ |
| aa       | ⇨ "General Daily Conditions" on page C-308 |
| ab       | ⇨ "Product Group Conditions" on page C-315 |
| b        | ⇨ "Special Conditions Menu" on page C-165  |
| c        | ⇨ "Special Prices Menu" on page C-166      |

#### Special Conditions Menu

_Master Data > Conditions > Special Conditions_

With this menu, you access all dialogs on which you specify the special conditions for market partners and industries. The special conditions overwrite the daily conditions.

| Shortcut | Description                                                          |
| -------- | -------------------------------------------------------------------- |
| a        | ⇨ "Special General Conditions" on page C-322                         |
| b        | ⇨ "Special Product Group Conditions" on page C-331                   |
| c        | ⇨ "Special Article Conditions" on page C-339                         |
| d        | ⇨ "Scales of Discount" on page C-348                                 |
| e        | ⇨ "Product Group Factors" on page C-350                              |
| f        | ⇨ "Article Factors" on page C-353                                    |
| g        | ⇨ "Muntin Factors" on page C-356                                     |
| h        | ⇨ "Shape Sucharges" on page C-359                                    |
| i        | ⇨ "AIR Surcharges" on page C-363                                     |
| j        | ⇨ "Exchange List Factors" on page C-367                              |
| ka       | ⇨ "IG Single Lite Conditions - Article Factors" on page C-371        |
| kb       | ⇨ "IG Single Lites Conditions - Product Group Factors" on page C-374 |

#### Special Prices Menu

_Master Data > Conditions > Special Prices_

With this menu, you can access all dialogs on which you specify the market partner-specific prices.

| Shortcut | Description                                             |
| -------- | ------------------------------------------------------- |
| a        | ⇨ "Article Prices" on page C-378                        |
| b        | ⇨ "Special Variant Prices" on page C-386                |
| c        | ⇨"Prices for Colored Article" on page C-391             |
| d        | ⇨ "Muntin Prices" on page C-397                         |
| e        | ⇨ "Processing Prices" on page C-401                     |
| f        | ⇨ "IG Exchange Prices" on page C-408                    |
| g        | ⇨ "Single Lites for IG Products" on page C-415          |
| h        | ⇨ "Special IG Basic Prices" on page C-420               |
| i        | ⇨ "UV Protection Prices" on page C-429                  |
| j        | ⇨ "Glazing Prices" on page C-433                        |
| k        | ⇨ "Exchange Prices Pattern Glass Classes" on page C-436 |
| l        | ⇨ "LAMI Exchange/Additional Prices" on page C-441       |

#### General control elements

In the _Overview_ section, there is a description of the general control elements and key combinations.

### Section Index

* **Index** C-449

### Index

**A**

* Accessories
  * daily conditions C-308
  * general conditions C-322
  * special conditions C-322
* Additional lists
  * price codes C-171
* Additional prices
  * spec. assignment for LAMI C-444
* AIR surcharges
  * IG prices C-215
* Area limit values C-200
* Article
  * assign price vector C-81
* article
  * glazing prices C-84
  * variant prices C-82
* Article conditions
  * factor C-340
  * minimum price C-340
  * offset C-340
* Article factors
  * scaling C-355
* article master data
  * price setting C-21
* Article price vector
  * spec. article price vectors C-228
* Article price vectors
  * minimum price C-225
  * PCD prices C-221, C-228
  * price codes C-172
  * scaled prices C-225
* Article prices
  * spec. scaled discount C-344
  * vector prices C-221
* assign exchange list
  * LAMI C-99, C-101
  * assign IG exchange list C-99, C-101

**B**

* Base prices
  * IG C-69
  * LAMI C-88
* Basic PLCD
  * with from-logic C-39
* basic PLCD
  * without from-logic C-39
* Basic prices
  * exchange lists C-185
  * LAMI C-249
  * -IG C-183
  * minimum price C-185
  * surcharges C-185

**C**

* Calc. base C-48, C-50
* Calculation
  * quantities by BQU
  * quantity
  * calculation by BQU C-51
* calculation
  * IG by single price C-69
* Codes
  * matrices C-170
  * muntin price codes C-174
  * processing vectors C-173
* Colored article
  * minimum price C-262
  * scaled prices C-262
  * spec. scaled prices C-394
* Colored articles C-256
  * minimum price C-259
  * PCD prices C-256, C-261
  * scaled prices C-259
  * spec. colored articles C-261
  * spec. minimum price C-394
* Conditions C-136
  * article conditions
  * determination example C-125
  * priorities C-122
  * product group conditions C-134
  * SC, factor, factor type C-127
  * spec. surcharges C-141
* conditions
  * daily conditions C-131
  * spec. conditions C-133
  * spec. factors C-138
  * spec. prices C-147
  * spec. product group conditions C-134
* convert prices C-68
* copy prices C-67
* create article price C-79
* create muntin price C-105
* Create price
  * article price C-79
  * processing price C-85
  * workflow C-57
* create price
  * matrix C-64
* create processing price C-85
* create workflow price C-57
* Creating exchange prices C-95
* Currencies C-33

**D**

* Daily condition
  * per price method C-308
* Daily conditions
  * PCd assignments C-131
  * processings C-308
* Definition scheme
  * IG and PCd prices C-22
  * matrices C-61
* definition scheme
  * muntin prices C-32, C-103
  * patterned glass prices C-93
  * PCd - PLCD C-26
* Display conventions C-15

**E**

* Exchange
  * assign exchange list C-99, C-101
  * create exchange list for IG C-95
  * create exchange list for LAMI C-100
  * create patterned glass prices for IG C-97
* Exchange list
  * mater code C-30
* Exchange prcies
  * spec. exchange list factors C-369
* Exchange prices
  * codes for exchange/additional lists C-171
  * minimum price C-211
  * patterned glass C-207
  * price codes C-171
  * scaled prices C-211
  * size surcharges C-211
  * spec. assignment for LAMI C-444
  * spec. assignments of pattern classes C-439
  * spec. minimum price for pattern classes C-439
  * TG/LAMI/Special C-209
* Exchange/additional lists C-91
* Exchange/additional prices C-90

**F**

* Factor
  * spec. factors C-138
* factor C-127
* factor type C-127
* from-PLCD logic C-37

**G**

* General conditions
  * daily conditions C-308
* Glazing C-269
  * minimum price C-271, C-435
  * spec. prices C-435
* global price changes C-120
* Global price maintenance C-177

**IG**

* base prices C-69
* calculation type single price C-69
* create exchange list C-95
* IG exchange prices
  * spec. minimum price C-411
  * spec. surcharges C-411
* IG prices
  * AIR surcharges C-215
  * basic prices C-183
  * convert matrices C-203
  * master data C-182
  * Matrix editor C-194
  * minimum price C-192
  * patterned classes C-206
  * scaled prices C-192
  * single lites C-190
  * size surcharges C-115
  * UV protection C-217
* IG single lites
  * spec. scaled prices C-418

**K**

* keys
  * assignment for matrix C-31
  * muntins C-32

**L**

* LAMI
  * base prices C-88
* LAMI Basic Prices C-245
* LAMI basic prices
  * offset surcharges C-247
  * PCD prices C-245, C-249
  * spec. offset surcharges C-250
* LAMI exchange list C-100
* LAMI exchange/additional prices C-251
  * minimum prices C-254
  * PCD prices C-251
  * scaled prices C-254
  * spec. assignments C-444
* Limit values C-198

**M**

* Market partner
  * colored articles C-394
  * glazing, sealing prices C-435
  * IG basic prices C-423
  * quantity scaled prices C-352
  * round size C-389
  * UV protection prices C-431
* market partner
  * offset surcharges C-382
  * special prices C-147
* Market partners
  * article price vectors C-228
  * exchange list factors C-369
  * general conditions C-322
  * processing price C-405
  * processing vectors C-237
  * special conditions C-321
  * special prices C-377
* market partners
  * product group conditions C-335
* Master data
  * price codes C-167
* master list C-30
* Matrices
  * convert C-203
  * Matrix area limit values C-200
  * Matrix limit values C-198
  * price codes C-170
* matrices
  * definition C-58
* Matrix
  * Area limit values C-200
  * assignment C-241
  * assignments of the keys C-31
  * base C-61
  * convert IG prices C-203
  * convert prices C-68
  * copy prices C-67
  * create price matrix C-64
  * definition C-58
  * editor C-60
  * IG prices C-194
  * limit values C-198
  * Matrix assignment C-241
  * Matrix editor C-194
  * square matrix C-62
  * triangular matrix C-61
  * type C-61
* matrix
  * keys C-30
* Matrix assignment
  * data record C-242
* PCD prices C-241
* matrix base C-61
* Minimum price
  * article price vectors C-225
  * colored articles C-259, C-262
  * daily conditions C-308
  * exchange prices C-211
  * glazing C-271
  * IG single lites C-192
  * LAMI exchange/additional prices C-254
  * muntin price classes C-275
  * processing prices C-243
  * processing vectors C-234
  * product group conditions C-317
  * sealing C-271
  * spec. article price C-382
  * spec. assignments of pattern classes C-439
  * spec. colored articles C-394
  * spec. IG basic prices C-423
  * spec. IG prices C-418
  * spec. muntin prices C-400
  * spec. product group codnitions C-335
  * special article conditions C-340
* Minimum surcharge
  * spec. shape surcharge C-362
* Muntin price classes
  * minimum prices C-275
  * muntin prices C-273
  * price codes Codes
* muntin price classes C-175
* muntin price classes
  * assign article C-107
* Muntin price codes C-174
* Muntin prices
  * assign article C-107
  * calc. bases C-104
  * create price class C-105
  * definition scheme C-103
  * muntin assignment C-278
  * muntin price classes C-273
  * price classes C-272
  * spec. assignments C-322
  * spec. minimum price C-400
* Muntins
  * keys C-32
  * spec. factors C-358
  * spec. products group conditions C-335
* muntins
  * codes C-32
  * price classes C-32
* price list code C-168
* PLCD logic
  * basic PLCD with from-logic C-39
  * basic PLCD without from-logic C-39
  * from-logic C-37
  * only PLCD logic C-38
  * price list control C-304
  * price lists/units C-305
* Price calculation
  * characteristics C-19
  * in the order C-20
* price calculation
  * calc. base C-48
  * price type C-50
  * round size C-51
  * rounding methods C-45
* Price classes
  * muntin prices C-272
* Price code C-169
* Price codes
  * article vectors C-172
  * exchange/additional lists C-171
  * master data C-167
  * matrices C-170
  * muntin price classes C-175
  * muntin price codes C-174
  * processing vectors C-173
* Price determination
  * basic principles C-17
* Price groups
  * patterned glass C-206
* Price keys
  * matrices C-30
  * PCd C-26
  * PLCD C-25
  * price keys C-32
  * lists C-30
  * vectors C-30
* Price list control
  * PLCD logic C-40
* Price lists
  * control C-304
  * currency C-26
  * global, local C-40
  * prices C-168
  * units C-305
* price lists
  *
    * keys C-30
* Price-relevant quantity
  * calculation C-47
* Prices
  * article vectors C-172
  * exchange/additional lists C-171
* global price maintenance C-177
* Matrix area limit values C-200
* matrix limit values C-198
* menu overview C-16
* muntin price classes C-175
* muntin price codes C-174
* muntin prices C-278
* patterned glass C-93
* price code C-169
* price lists C-168
* setting in article master data C-21
* shape surcharges C-281
* spec. prices C-147
* spec. shape surcharges C-284
* vector prices C-74
* prices
  * global price changes C-120
  * vectors C-72
* Pricing method
  * accessory article (25) C-45
  * base glass (23) C-44
  * colored accessory article (31) C-45
  * IG-current (41) C-44
  * LAMI (29) C-44
* master data C-44
  * muntin article (5) C-45
  * processings (26) C-45
  * TG (22) C-44
  * UV protections (60) C-45
  * whole-glass systems (12) C-45
* pricing method
  * articles C-44
* priorities
  * conditions C-122
* Processing vectors
  * codes C-173
  * details C-238
  * minimum price C-234
  * overview C-237
* Processings
  * PCD prices C-232
  * scaled price C-234
  * spec. processing vectors C-237, C-238
* Processings
  * daily conditions C-308
  * general conditions C-322
  * minimum price C-308
  * price codes C-173
  * processing surcharge for shapes C-283, C-285
  * product group conditions C-317
  * spec. assignments C-322
  * spec. minimum price C-405
* spec. product group conditions C-335
* spec. scaled prices C-405
* spec. surcharge for shapes C-362
* Product group conditions
  * minimum price C-317
  * spec. minimum price C-335
* Product group factors
  * spec. scaled prices C-352
* product groups
  * conditions C-134

**Q**

* quantity
  * price-relevant quantity C-47
* Quantity scale
  * colored articles C-259
  * single lites C-192
  * spec. article factors C-355
  * spec. offset surcharges C-382
  * spec. product group factors C-352

**R**

* Round size C-51
* Rounding C-45
  * unit price C-46
* rounding
  * round size C-51
* Rules SA-PU factors C-302

**S**

* SA-PU factors C-302
* Scaled discount
  * spec. article conditions C-344
* Scaled prices
  * article price vectors C-225
  * colored articles C-259, C-262
  * exchange prices C-211
  * IG single lites C-192
  * LAMI exchange/additional prices C-254
  * offset surcharges LAMI C-247
  * processing vectors C-234
  * spec. AIR surcharges C-365
  * spec. article prices C-382
  * spec. IG prices C-418
  * spec. processing price C-405
  * spec. product group factors C-352
  * spec. UV protection prices C-431
  * spec. variant prices C-268
  * UV protection C-218
  * variant prices C-265
* Scaling
  * quantities in spec. article factors C-355
* Sealing C-269
  * minimum price C-271, C-435
  * spec. prices C-435
* Shape surcharges
  * calc. bases C-110
  * calculation of the minimum surcharge C-111
  * minimum surcharge C-283, C-285
  * prices C-281, C-284
  * processing surcharge C-283, C-285
  * spec. minimum surcharge C-362
  * spec. shape surcharges C-284
* Single lites
  * IG prices C-190
  * minimum price C-192
  * prices C-190
  * scaled prices C-192
* Size surcharges
  * exchange prices C-211
  * IG prices C-115
  * sequence of the price levels C-116
  * vector prices C-114
* size surcharges C-114
* Special article conditions C-340
* Special basic prices C-249
* Special prices C-377
* Special variant prices C-266
* square matrix C-62
* surcharge bases C-109
* surcharge matrix C-112
* Surcharges C-108, C-127
  * AIR surcharges C-215
  * general conditions C-322
  * processings C-117
  * product group conditions C-317
  * size surcharges C-114
  * spec. AIR surcharges C-365
  * spec. assignments C-322
  * spec. IG basic prices C-423
  * spec. offset surcharges for LAMI basic price C-250
  * spec. product group conditions C-335
  * spec. shape surcharges C-284, C-362
  * special conditions C-322
  * step surcharges C-118
* surcharges
  * surcharge bases C-109
  * surcharge matrix C-112
  * surcharges C-141
* switching off C-141

**T**

* triangular matrix C-61

**U**

* unit price
  *
    * rounding C-46
* UV protection
  * IG prices C-217
  * scaled prices C-218

**V**

* Variant prices C-263
  * PCD prices C-263, C-267
  * scaled prices C-265, C-268
  * spec. round size C-389
* Vector
  * assignment C-78
  * colored article C-76
  * create article price C-79
  * create glazing price C-84
  * create variant price C-82
  * definition C-72
  * glazing C-77
  * LAMI price C-76
  * processing price C-75
  * variant price C-77
* vector
  * assign to the article C-81
  * create processing price C-85
  * keys C-30
  * step surcharges C-118
* Vector assignment
  * PCD prices C-240
* Vector assignments
  * PCD prices C-230
  * spec. assignments C-231
* Vector prices C-220
* vector prices C-74
  * create article price C-79
  * size surcharges C-114
