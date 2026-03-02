---
description: "EN-FUNC-AW_Enterprise_Order_Invoice_to_XML"
---


# A+W Functional Description: Export of invoices in the XRechnung/ZUGFeRD format

**A+W - Software for Glass**

---
## 1. Contents

1.  Contents
2.  Notes on this Document
    2.1. Trademarks
    2.2. Copyrights
    2.3. Exclusion of liability
3.  Performance Description
    3.1. Data
    3.2. Description
    3.3. Requirements
    3.4. List of functions
    3.5. Limitations
    3.6. Notes
4.  Contact Address

## 2. Notes on this Document

This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### 2.2. Copyrights

© 2023, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. The documentation may not be transmitted electronically, by recording or in any other form without the prior written permission of A+W Software GmbH.

### 2.3. Exclusion of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions that have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| Product | A+W Enterprise |
| :--- | :--- |
| **Module number** | ###(vorl. 200021)### |
| **Module** | Order Invoice to XML (XRechnung) |
| **Brief description** | Provision of invoices in the XRechnung/ZUGFeRD format |
| **Available** | A+W Enterprise v6 – starting with QR[2410] + current AWE B2B Service and Print Service |

### 3.2. Description

The XRechnung is a specified format for electronic invoices in Germany, which implements the EU-wide standard for electronic invoice exchange. It was developed as part of the EU directive 2014/55/EU, which encourages the digitalization and standardization of invoicing within public administration.

An XRechnung is based on XML structures and includes standardized data fields to ease the exchange of invoice information. Public authorities in Germany are obliged to accept invoices in electronic form since November 27, 2020 and they may only accept e-invoices that correspond to this standard.

Due to the growth opportunity act, the introduction of obligatory e-invoicing for domestic B2B sales was determined starting on January 1, 2025.
Starting on January 1, 2025, all companies (even small companies) must be in a position to receive electronic invoices. Sending e-invoices will become mandatory for all companies starting on January 1, 2025; however, there will be transitional rules.

Starting on January 1, 2027, companies with a previous year's sales of more than EUR 800,000 in the B2B sector must send e-invoices.

Starting on January 1, 2028, all companies in the B2B sector must send e-invoices.

A+W Enterprise offers the opportunity to generate electronic invoices in the XRechnung format.

The format to be exported (XRechnung/ZUGFeRD) can be defined in the customer master data.

After the invoice booking, form dispatch can be used to send the export file (XML for XRechnung/PDF for ZUGFeRD) to the customer.

The XRechnung standard is implemented in Version 3.0 (more precisely, 3.0.2)
The schema used is "UBL Invoice 2.3".

For ZUGFeRD: ZUGFeRD Version 2.3.3 (CII)

### 3.3. Requirements

*   **Discount logic**
    The new discount logic must be active. (RABATTLOGIK_2005 = ON)
*   **Checking the invoice reports/invoice form**
    The use of CrystalReport reports is obligatory; old rep reports are not permitted.
    If the reports contain calculations, this can cause deviations between the printout (report PDF) and XML format. Both documents should match. In case of deviations, the e-invoice (XML) is always the valid document.
*   **Clarification of the archiving**
    Electronic invoices must, like paper invoices, be archived properly. There are strict regulations for the electronic archiving of invoices, which correspond to the legal requirements of the GoBD.
    In particular, the XRechnung must be archived in the form in which it was transmitted.
*   **Viewer for the XRechnung**
    A view for XRechnung is a software tool that was developed for visually displaying the content of XRechnungen (in XML format). Since XRechnungen exist in a structured, machine-readable form, they are difficult for people to read in their pure XML form. A viewer enables you to display the content of the invoice in a comprehensible manner. Many viewers include a conformity check and validate the XRechnung.
    If the viewer used displays errors or warnings for an XRechnung, to solve the problem, the viewer used must be known to A+W.
*   **Validation tool**
    Validation tools for XRechnung are specialized software solutions that check the technical and content correctness of electronic invoices in XRechnung format. Since the XRechnung uses a standardized XML format and is subject to strict legal and technical specifications, the validation is decisive for ensuring that the invoices were created correctly and correspond to the legal requirements.
    If the validation tool used displays errors or warnings for an XRechnung, to solve the problem, the tool used must be known to A+W.
*   **Checking the A+W Enterprise version**
    "Order invoice to XML (XRechnung)" is only available with A+W Enterprise v6 (starting with QR [2410]). Older versions are not supported.
*   **Checking the Skonto logic**
    It is recommended that you put the "new Skonto logic" into operation.

### 3.4. List of functions

*   **Master data configuration**
    *   Legal seller
    *   Marking of the customer as recipient of electronic invoice
    *   Set-up of the special document type "E-Rechnung"
    *   Contact person with assigned company position (management, chair of the supervisory board)
    *   Bank details with prioritization
    *   Individual XRechnung texts can be specified as header and footer texts.
    *   Designations used in the XRechnung are managed and adjusted via special report texts.
*   **Generation of the XRechnung during invoice booking**
    *   Both a document-related invoice and a manual invoice without reference to an XRechnung can be generated.
    *   Language of the texts is determined by the language setting of the invoice
    *   The XRechnung file is saved as file attachment to the invoice. The file name of the XRechnung can be specified individually via an SP.
    *   With renewed generation of the XRechnung, the older file remains (if necessary, with modified file name).
    *   A subsequent (manual) new generation of the XRechnung is possible via a script.
    *   Invoice correction is done via cancellation, credit note, and new invoice (normal AWE process).
*   **Sending of the XRechnung from the form printing**
    *   No special authorization required, the general authorization to send invoices is sufficient.
    *   Dispatch via e-mail as file attachment (in addition to PDF invoice)
    *   It is possible to activate SSL encryption for e-mail sending.
    *   Company advertising can be placed in the e-mail.
*   **Archiving**
    *   The archiving can be done analogous to the existing archiving logic.

### 3.5. Limitations

*   The XRechnung does not include a signature
*   No advertising may be placed in the XRechnung.
*   The use of CrystalReport reports is obligatory; old rep reports are not permitted.
*   For start-up, it must be ensured that only original data from the database is used in the report. Calculations and roundings to change the data in the printout (also PDF generation) must be avoided since they can cause deviations from the XML format. If both XRechnung and a PDF invoice are to be sent to the invoice recipient, in case of deviations, the E-Rechnung (XML) is always the valid document.
*   The module only includes the generation of the format and the dispatch via mail. If in the future the legislator allows the transfer only via portals and/or certified providers, there will be additional costs.
*   There is no certified transfer of the documents exported.
*   The XRechnung generated (xml file) is not protected against manipulation. It is the recipient's responsibility to keep the file in the original state.
*   There is no end-to-end encryption of the electronic invoice when sending via e-mail. However, SSL encryption can be activated.
*   The following functionalities will not be implemented (status as of 09/26/2024):
    *   Old discount logic
    *   Sending via FTP
    *   Export of file attachments (e.g., declaration of performance, production sketches, etc.)
    *   Sending of several XRechnung files with a single e-mail

### 3.6. Notes

*(This section is intentionally left blank as per the source document.)*

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-Mail: zentrale@a-w.com
Internet: http://www.a-w.com/
