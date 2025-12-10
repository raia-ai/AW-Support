---
description: "A+W Enterprise - Internal Multi-Site Logic"
---


# A+W Enterprise – Internal Multi-Site Logic

---
## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions that have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Enterprise |
| **Module number** | ./. |
| **Module** | Multisite System |
| **Brief description** | Multi-site capability |
| **Available** | Ab A+W Enterprise v5 |

### 3.2. Description

The internal site logic allows the mapping of several operations within one database. This increases the integration, important status information is available directly and does not have to be replicated. The master data only has to be maintained once and is then available directly in all operations. This saves a significant amount of money on management and synchronization in comparison to an external multi-site system with replication. Locally, only the particular features, such as procurement types, which can be different at different operations, are stored.

In addition, it is therefore possible in the A+W Enterprise system to deploy a central call center for order entry. In the process, all orders are entered in a central site (call center) and assigned automatically to the sites with a definable logic.

This functionality also supports the demand for "one fact to the customer." That is, the end customer orders from the company and not from the company's special sites. All of the handling, the products, papers, prices, and terms are identical. Which site or which sites will produce the customer order is decided within the company.

### 3.3. Requirements

**Processes**

The sites that work in a common multi-site system must have the same process flows. They must work in uniform fashion. Thus, for example, it is not possible that one operation works with a PO pool and another does not.

**Properties**

The multi-site logic assumes that all operations of the multi-site system work in the same environment:

This means for all sites:
- uniform system currency
- uniform language
- uniform default texts and keys
- uniform prices, terms, discounts, and surcharges for a customer (exceptions are possible)

**Conversion**

Before the conversion to a multi-site system, the master data of the individual sites must be synchronized since these are uniform in the multi-site system (e.g. same market partner numbers, same article numbers).
If existing operations should be converted, only one operation can continue its transaction data; all others must be newly integrated into the system.

**Number ranges**

The multi-site logic implies that there are central number ranges, especially for orders. It is possible to create site-related number ranges, but we recommend that you not do this since it reduces significantly the number of possible order numbers – and order numbers must be unique system-wide.

The storage of a central number range for orders is also a prerequisite for the deployment of a call center since with the use of different order number ranges, a site change is no longer possible after saving an order.

The use of site-specific number ranges for invoices and credits is possible and does not restrict the functionality of the multi-site system.

**A+W Production**

For each site that has a production facility, an individual local A+W Production must be configured.

### 3.4. List of functions

Essentially, all functionalities of a single site system are available in the multi-site system; in some cases with special adjustment of the multi-site functionality. In addition, there are a series of functionalities that are only available in a multi-site system.

**Call center functionality**

All orders are entered in a central site and assigned via a configurable assignment routine automatically to a site after an order is saved. For automatic site assignment, all data available in A+W Enterprise can be used.

**Via plant logic**

It is possible to deliver an order to the customer via another internal site (via plant). This can make sense for cost or technical reasons. During the delivery date calculation, the system considers both routes, that from the production site to the delivery site and that from the delivery site to the end customer. The organization of both routes is supported in the dispatch control.

**Change of site in orders**

In a multi-site system, it is, as long as an order has not been locked by production or purchasing, possible to easily change the site assignment. Prerequisite for this is the use of a company-wide order number range. Here the order data is adjusted to the new site. The procurement type, costs, routes, etc. are changed accordingly. In addition, when saving it is checked again online whether the order in production can still be canceled. Only after that does the change of site take effect.

The system then cancels the order in A+W Production of the first site and deletes the stock forecast and order proposals. After the adjustment to the local circumstances of the "new site," the order runs through the "normal" workflow for new orders (transfer to production, scheduling, order proposals, stock forecast, cost calculation, etc.).

This procedure can be repeated as often as desired as long as an order is not locked.

**Site-specific rights**

User rights can be stored site-specifically. For certain rights (see EN-CONFIG-A+W Enterprise EDV Modulkuerzel.docx) it is possible to define whether it should apply generally or only for one or several sites. Data access can also be restricted via the rights management. Thus, for example, you can ensure that an employee of Site A has no access to orders for Site B.

In addition to access to the orders, access to the market partner master data can therefore also be restricted.

**Limit check**

The A+W Multisite System supports both a central as well as site-specific limit check.

**Replication**

Within a multi-site system, no replication is required. It is replaced by site-spanning master data management. Site-spanning master data can be replicated between several multi-site systems. Site-specific data cannot be replicated.

### 3.5. Limitations

**Mapping of the site assignment**

The site assignment in the system cannot, from a database-technical point of view, as attribute be realized as an additional key. This means that the keys used in the system must also be unique without addition of the site number.

Concretely, this means that a customer, supplier, warehouse, order, PO or key number may exist only once in the system. If, for example, the warehouse number 1 is assigned to a warehouse of the site 10, a warehouse number 1 cannot also be created for site 20. A different key must be assigned (101 or 201, for example)

**Site-spanning functionality**

It is not possible to have a multi-site system with
- different system currencies
- site-specific default texts and keys
- site-specific prices, terms, discounts, and surcharges (possible with limitations).

**Site-specific languages**

Site-specific languages are now possible with a few exceptions (prices, list names and form names, etc.).

**Prices and terms**

In the interest of "one face to the customer," prices and terms are maintained uniformly centrally. If local/site-specific particular features should be mapped, this can be done with a site-specific condition debtor.

**Maximum number of sites**

Based on the use of 8-digit transaction numbers and the fact that particular number ranges must be stored disjunctively in the system, it is not possible to map as many sites as desired in one system. A significant factor is the number of transactions in the system.

The computer capacity must also be able to manage the total volume adequately.

The maximum number of sites is thus not fixed, but rather depends on the configuration and size of the individual operations. As a rough guideline: a maximum number of 15 sites in one system should not be exceeded. With respect to limits, a company-specific assessment in consultation with development makes sense.

**FinAc interface**

The FinAc interface should be identical for all sites. For example, in the standard, no different FinAc systems or accounts can be mapped. (special functionality required)

### 3.6. Notes

(No content provided in this section.)

## 4. Contact Address

A+W Software GmbH
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-Mail: info@a-w.com
Internet: http://www.a-w.com/
