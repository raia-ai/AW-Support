---
title: "EN-FUNC-AW_Business_Form_Printing_with_Crystal_Reports"
source: "EN-FUNC-AW_Business_Form_Printing_with_Crystal_Reports.pdf"
tags: ["A+W Business", "Crystal Reports", "Form Printing", "Reporting Service", "ERP", "Software", "Functional Description", "AWSOA", "iQuote"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This functional description outlines the A+W Business module for form printing using Crystal Reports. It details the transition from the Gupta Report Builder to a more modern, service-based architecture, enhancing performance by offloading print jobs from individual workstations."
long_description: "This document provides a detailed functional description of the 'Form printing with Crystal Reports' module for the A+W Business ERP system, available from version v6. The primary goal of this development was to shift form printing to a dedicated reporting service and adopt Crystal Reports as the new reporting tool. This architecture unburdens individual user workstations, allowing them to continue working immediately after submitting a print job. The document explains the advantages of Crystal Reports over the previous Gupta Report Builder, such as a wider range of design options. It supports a mixed-operation mode, enabling a gradual migration of existing forms. The system architecture is detailed, showing how A+W Business communicates with a .NET-based spooler and print service. The process involves activating the service in master data, configuring forms, and managing print jobs through a tool dialog. The document also covers system requirements, a list of functions including seamless ERP integration and multi-site support, and limitations, such as the need to adapt custom formulas and the lack of support for distributed printing of items on different forms."
---

# A+W Functional Description

---
## A+W Business - Form printing with Crystal Reports

