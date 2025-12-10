---
title: "EN-CONFIG-AW_Business-4"
source: "EN-CONFIG-AW_Business-4.pdf"
tags: ["A+W Business", "ERP", "Crystal Reports", "Configuration", "Software Manual", "Print Service", "SAFT-PT", "Technical Documentation", "Form Printing", "Customizing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical configuration guide for the A+W Business software, focusing on specialized features such as Portuguese Certification (SAFT-PT), advanced email sending capabilities, and the integration of a print service using Crystal Reports. It provides step-by-step instructions for system administrators and developers."
long_description: "This comprehensive technical manual details the configuration of several advanced modules and features within the A+W Business ERP system. It begins by covering the requirements for Portuguese Certification, including how to lock documents after an invoice is printed and manage user rights to prevent unauthorized changes (Fig. 69-70). It also explains the process for invoice cancellation and the mandatory SAFT-PT XML export for legal compliance in Portugal. The guide then transitions to communication features, explaining how to configure E-mail sending per document type (e.g., quotations, invoices) by managing multiple email addresses per customer (Section 3.8) and how to connect to the ActiveFax third-party software (Section 3.9). The largest portion of the document (Section 3.10) is a detailed walkthrough of installing, configuring, and utilizing the Print Service with Crystal Reports. This includes infrastructure setup, printer installation, A+W Business activation, and in-depth instructions on creating and customizing Crystal Reports. Topics cover setting data sources, managing report sections, creating subreports, using special action fields, and adapting existing customizing formulas for the new service. The document concludes with an extensive FAQ section addressing common issues related to printers, report fields, and sub-report formatting."
---

---
## Portuguese Certification Configuration

### Fig. 69: Portug. Certi. - Document lock
In management of rights (Master data > Company > User rights), a new restriction must be defined for users who are not entitled to change documents after the invoice has been printed. The following settings are relevant:

- **Lock document after invoice printout**: Set to `0 - Yes`.
- **Lock docs beginning from status point**: Set to `0103 - Rechnung Druck` (Invoice Print).

