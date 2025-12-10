---
title: "EN_AWBusiness_ShortGuide_ConformityPack"
source: "EN_AWBusiness_ShortGuide_ConformityPack.pdf"
tags: ["A+W Business", "Conformity Pack", "Declaration of Performance", "DoP", "CE Marking", "Construction Products Regulation", "Software Guide", "ERP", "Glass Industry"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A short guide for end-users of A+W Business on implementing the Conformity Pack. It details the setup and management of Declarations of Performance (DoP) and CE Marking as required by the European Construction Products Regulation."
long_description: "This document, the 'Implementation of the Conformity Pack in A+W Business' short guide, provides comprehensive instructions for users of the A+W Business software. It addresses the legal requirements of the European Construction Products Regulation (CPR) effective from July 1, 2013, which mandates the creation, management, and provision of Declarations of Performance (DoP) for construction products. The guide explains the entire workflow, from the initial registration of DoPs in the system to their application in various business processes. It covers master data setup, including company, product, and partner data configurations. Key features like the Utilities Module for defining product structures, management of forms for automated dispatch, and user rights management are detailed. The guide also illustrates the practical application in document management, showing how DoPs are assigned to order items, and explains the process for printing forms and transferring DoP data to the A+W Production system. This guide is essential for ensuring compliance with CPR using the A+W Business software suite."
---

# A+W Short Guide: Implementation of the Conformity Pack in A+W Business

**A+W - Software for Glass**

---
## Editorial

### Notes on this document
This document is intended for end users of A+W Business. This documentation and the software it describes are issued only in connection with licences and must be used and copied only in accordance with this licence. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action. This document describes the full scope of A+W Business in connection with A+W Production.

A+W Software GmbH cannot be held liable for data errors resulting from the basics of the standard functions provided by Microsoft or Unix.

### Copyrights
© 2013, A+W Software GmbH, all rights reserved, including the right of reprint, production of copies, and translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Without the prior, written consent of A+W Software GmbH, the documentation must not be passed on to third parties, neither electronically, mechanically, by recording, or in any other way.

### Trademarks
All hardware and software names mentioned in this documentation can also be registered trademarks, and should be considered as such. Third party copyrights have to be obeyed.

### Value+
The right to use these functions and services is granted only in connection with a valid value+ contract or based on a special, individual agreement. We reserve the right to audit the licences and their utilization.

Should you have questions regarding this subject please contact a member of the A+W sales team or please refer to our homepage http://www.a-w.com/.

**A+W Software GmbH**  
Konrad-Adenauer-Straße 15  
35440 Linden, Germany

Tel. +49 6403 970-0 Fax +49 6403 64390  
www.a-w.com · zentrale@a-w.com  
© 2013 A+W Software GmbH

## Legal Background and Motivation

As from 1 July 2013, the European Construction Products Regulation prescribes that all manufacturers and intermediate dealers in the EU issue, manage, and provide declarations of performance (DoP for short).

### Declaration of Performance and CE Marking

*Fig. 1: Interaction of Declaration of Performance and CE code (direct process)*

A producer creates products, a Declaration of Performance (DoP), and CE-Marking. The DoP (as a pdf/docx) is sent to the customer. The CE Marking, along with the product, packing, or additional papers, is sent to the construction area.

*Fig. 2: Interaction of Declaration of Performance and CE code (dealer process)*

A producer creates products, a DoP, and CE-Marking. This is sent to a Dealer/Distributor, who has to hand over the DoP and CE-Markings. The dealer then sends the DoP to the customer and the CE Mark to the construction area. Dealers must create their own DoPs and CE-Markings when importing products from outside the EU region.

A declaration of performance must be issued if a construction product belongs to a harmonized standard, or is consistent with a European Technical Assessment (ETA). Statements and information on the performance/characteristics of a product can be made only (e.g. in advertisements) if these are stated and specified in the same way in the declaration of performance.

> "By issuing the declaration of performance, the manufacturer takes the responsibility for the construction product being in compliance with the stated performance." ¹

The application of the Construction Products Regulation requires that a declaration of performance is issued for every product/every product structure. The declaration of performance must be provided at the latest upon delivery, per order item, and in electronic form (PDF/DOCX). If an order includes several identical products it is sufficient to supply the declaration of performance just once per product. It is also permitted to issue a declaration of performance which comprises all order items. If requested by the customer, the declaration of performance must be provided in printed form.

The declaration of performance must be kept for ten years and must be presented upon request (e.g. customer's or auditor's request).

*Fig. 3: Declaration of performance - an example*

**Leistungserklärung Nummer 10001**

| No. | Description | Value |
| --- | --- | --- |
| 1. | Eindeutiger Kenncode des Produkttyps | 101 - A+W TOP Energiegewinnglas |
| 2. | Typen-, Chargen- oder Seriennummer... | 10105 - A+W TOP Premium 1.1 |
| 3. | Vom Hersteller vorgesehener Verwendungszweck... | Isolierglas zum Wärme- und Sonnenschutz zum Einbau in Metall-, Holz- oder Kunststofffenster |
| 4. | Name, eingetragener Handelsname... | Glas Mustermann GmbH, Musterstraße 12, D-12345 Musterstadt |
| 5. | Gegebenenfalls Name und Kontaktanschrift des Bevollmächtigten... | Angaben durch den Hersteller |
| 6. | System oder Systeme zur Bewertung und Überprüfung der Leistungsbeständigkeit... | Angaben durch den Hersteller |
| 7. | Im Falle der Leistungserklärung, die ein Bauprodukt betrifft, das von einer harmonisierten Norm erfasst wird: | EN 1279-5 2005 A2/2012 |
| 8. | Im Falle der Leistungserklärung, die ein Bauprodukt betrifft, für das eine Europäische Technische Bewertung ausgestellt worden ist: | ift Rosenheim NB Nr. 0575 |
| 9. | **Erklärte Leistung** | |
| Nr. | Wesentliches Merkmal | Leistung | Harmonisierte, technische Spezifikation |
| 1.1 | Thermische Eigenschaften (Ug-Wert) | 1,1 Ug W/m²K | EN 673-15 K |
| 1.2 | Lichttransmissionsgrad (%) | 80% | EN 410 |
| 1.3 | Gesamtenergiedurchlassgrad (g-Wert) | 63% | EN 410 |
| 10. | Die Leistung des Produkts... | |

> ¹ Official gazette of the European Union, issue 04.04.2011 (L 88 / 12), paragraph 4, section 3

## Master Data Input and Management

Using the new functions with regard to the declarations of performance according to the Construction Products Regulations requires the following settings in your system's master data:

-   **Declaration of performance management:** Registration of declarations of performance
-   **Company master data:** tab Parameters - email dispatch, standard DoP
-   **The Utilities module:** Declaration of performance - product structure
-   **Product master data:** tab Attachments
-   **Partner master data:** tab Attachments
-   **Management of forms:** tab Form
-   **Management of rights:** Right to effect manual changes in the documents, per user

Below, we are going to describe these settings in detail.

### Management and Registration of Declarations of Performance

To be able to attach a declaration of performance to a document (or a specific order) or to assign a declaration of performance to a product or a business partner by default, the declaration of performance has to be registered in the system first.

This registration can be made centrally in `Master Data > Products > General > Declaration of Performance, Management`.

*Fig. 4: Dialogue "Declaration of performance management"*

*Fig. 5: Registering a declaration of performance*

**Number**
Number of the declaration of performance (alpha-numerical).

**Name**
Name of the declaration of performance. This should be unique and descriptive.

**Language**
Language in which the declaration of performance is issued. The combination of number, name, and language of the declaration of performance allows keeping and registering a DoP with a certain number in different languages.

**Link**
`<Reference_Path>\dop`; path for saving the declarations of performance. It is defined in `Company master data > tab Documents`.

**[Add], [Remove]**
These buttons are used for adding a language version of the DoP, or removing it from the list.

#### How to register a declaration of performance
1.  Go to `Master data > Products > General > Declaration of performance management`.
2.  Go to `Menu > Start > New` to register a new declaration of performance.
3.  Enter the number and name. You can choose these entries at random. Every DoP number must exist only once however.
4.  Select the language of the DoP. Alternatively, you can allocate different languages (documents) to a DoP with a unique number.
5.  Click on the [File] icon next to the field **Link** to open the directory.
6.  Choose the required template.
7.  Go to `Menu > Start > Save` to save the data. The DoP is now available in product management and can be assigned as required.

Alternatively you can register a DoP in product master data (as a default for a certain product) or in company master data (as a default for a business partner). These declarations of performance will be automatically loaded and dispatched if no specific, individual DoP is assigned to a product structure or document.

> **Registering a Declaration of Performance**
> To assign a declaration of performance to a document (e.g. a specific order) or to assign a declaration of performance to a product by default, the declaration of performance must be registered in the system first.
> A+W Business offers a new table for this purpose in which all defined combinations of product structure (ID) and declaration of performance are saved. Default product structures defined in master data will be taken into account as well as alternative product structures which e.g. result from a sheet being exchanged at item entry.
> **Technical information:** Product structure table (BW_PRODUKT_AUFBAU_LENR)

### The Utilities Module

`Module Utilities > System > Declaration of Performance, Product Structure`

*Fig. 6: Declaration of performance, product structure*

This dialogue serves to define the distinctive features to be analysed in product structures. Every defined product type/product group combination is treated as an individual feature.
Should this distinction be insufficient you can also define that the corresponding article number shall be used as well.

### Company Master Data

`Master Data > Company > Company data > tab Parameter`

*Fig. 7: Company data - tab Parameter*

**Dispatching declarations of performance**
This setting serves to activate the dispatch of declarations of performance for this business partner. In management of forms you can also define whether the declaration of performance shall be dispatched upon printing.

**Standard Declaration of Performance**
This field serves to define the DoP to be dispatched by default to the business partner if an order item has not been assigned any specific, separate DoP. The declarations of performance are saved in the standard directory for file attachments in `<Reference_Path>\dop`. This directory is defined in `Company data > tab Documents`.

### Product Master Data

`Master Data > Products > Products > tab Attachments`

*Fig. 8: DoP allocation/registration in article master data*

In product master data you can assign a declaration of performance which shall be dispatched by default for this product/product structure. In the actual order, this DoP can be amended for the individual items, e.g. after a sheet has been exchanged.

**Number**
Number of the specific declaration of performance assigned to this product/structure by default. The combination of product structure (product structure ID) and DoP number is saved in the system.

The [File] button can be used to register a declaration of performance for this product/product structure. Use the [Zoom] icon to display a list of declarations of performance already registered in the system and saved in the defined directory in `<Reference_Path>\dop`.

**Declaration of performance required**
This setting defines whether a DoP is required for the product in question (a spacer will not require a separate DoP for example). The code and the assigned DoP will be adopted for the order item. If no DoP is assigned, the standard DoP defined in company master data will be used.

> **Registering a Declaration of Performance**
> To assign a declaration of performance to a document (e.g. a specific order) or to assign a declaration of performance to a product by default, the declaration of performance must be registered in the system first.

### Partner Master Data

`Master data > Partners > Customer > Customer > tab Attachments`

*Fig. 9: Partner master data (example customer)*

**Dispatching declarations of performance**
This setting is used for activating the dispatch of declarations of performance for the partner (customer) in question.

### Management of Forms

`Master Data > Forms > Form Management > tab Form`

*Fig. 10: Form Management*

**Email dispatch**
This setting defines the print point at which the DoP shall be emailed.

### Management of Rights

`Master Data > Products > General > Declaration of Performance, Management`

*Fig. 11: Partner master data (example customer)*

This dialogue serves to define the user rights with regard to the management of declarations of performance. You can e.g. define whether a user shall be entitled to manually assign a declaration of performance at item entry.

## Application in Document Management

When a new item is entered, the declaration of performance number for the item is initially loaded from product master data.

When an item is changed (e.g. glass exchange), the product structure of the current item will be checked/re-determined. This product structure is searched in the product structure table, and the product structure ID plus the corresponding DoP number are adopted for the item. If the structure cannot be determined, the declaration of performance number will be removed from the item.

This is followed by an input check at item entry. The program checks whether the flag for determining the declaration of performance has been set in product master data for the product in question and if so, whether a declaration of performance exists in the item. If the code has been set but no declaration of performance has been assigned, a message to that effect will be issued. This permits to assign a DoP by hand at a later stage. This message can also be disabled on user level.

The item is saved now. If the declaration of performance number for the current item has been changed by hand, it will be saved for the item. If the product structure of the item has been changed (e.g. glass exchange), the new product structure - along with the assigned declaration of performance number - is saved in the product structure table. If the product structure has already been entered in this table, the assigned declaration of performance number will be replaced.

*Fig. 12: Process of determining the DoP at document entry*

A flowchart shows the following logic:
1.  Save Item.
2.  BOM changed?
    *   If no, proceed to Product: PoD needed?
    *   If yes, check BOM available in PoD?
        *   If no, delete no. of PoD in item.
        *   If yes, proceed to Product: PoD needed?
3.  Product: PoD needed?
    *   If no, save (new) PoD in item.
    *   If yes, check PoD available?
        *   If no, set manual.
        *   If yes (ja), save (new) PoD in item.

`Module Documents > Order > Order > tab Items`

*Fig. 13: Assigning a declaration of performance to an item*

**Declaration of Performance**
Number of the assigned declaration of performance.

**DoP search**
Starts the search dialogue for the manual search for a registered declaration of performance.

## Printing of Forms

When the form is printed, the system first checks in which language the form (order confirmation, delivery note, etc.) shall be printed. In customer master data, the standard language assigned to the customer is checked. If no language settings for the declaration of performance are found for the item (neither in the forms nor in customer master data), the standard DoP will be loaded from company master data.

After the declaration of performance has been dispatched, an internal note is made in customer data (technical info: table DR_KUNDEN_LENR). This makes sure that this DoP will not be dispatched again next time the customer orders the same product structure. As an additional information, the printing date and the shipping information (type of printout and document number) are also saved in the table. When printing is repeated, this table will be checked; emailing of this declaration of performance will be suppressed.

## Transfer to Production

The transfer to the production planning system A+W Production must include the DoP number as a text record in the Order.xml. Enter the appropriate standard text with a special text code and allocate it in product data.

`Module Master data > Text > Text`

*Fig. 14: Example: Standard text for transfer to production*

The link to the declaration of performance can also be transferred to A+W Production via Order.xml. Enable the Code for file attachments to be transferred > A All for this purpose.

`Module Production > Production > Transfer to Production > Menu Functions > Settings > tab Text/Attachments.`

*Fig. 15: Transferring text and attachments to production*

The settings dialog allows selecting which codes for texts and file attachments should be transferred.
- For "Code of texts to be transferred", `D Declaration of Performance` should be checked.
- For "Code of file attachments to be transferred", `A All` should be checked.

