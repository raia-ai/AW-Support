---
title: "EN-CONFIG-AW_Enterprise_Export_Service"
source: "EN-CONFIG-AW_Enterprise_Export_Service.pdf"
tags: ["A+W Enterprise", "Export Service", "Software for Glass", "ERP", "PPS", "Webservice", "Database Interface", "WAEINALCIM", "CANCELORDER", "Configuration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides configuration and technical details for the A+W Enterprise Export Service. It explains the procedure for transferring events and data from A+W Enterprise to other programs' Web services, detailing the use of interface tables, Windows services, and specific interfaces like WAEINALCIM, CANCELORDER, and BESTINFOALCIM."
long_description: "This is an internal configuration manual for the A+W Enterprise Export Service, a solution designed to bridge the gap between A+W Enterprise and external Web services. A+W Enterprise cannot directly address Web services, so this service acts as an intermediary. It works by polling a dedicated interface table (`exportinfo`) in the database, which is populated by A+W Enterprise whenever a transfer event occurs. The Windows service then reads records from this table, processes them, and passes the relevant data to the appropriate target Web service (e.g., a PPS or ERP Webservice). The document outlines the general procedure, logging mechanisms, and details of the transfer tables (`exportinfo` and `exportinfook`). It provides in-depth descriptions of various implemented interfaces, including those for goods received (WAEINALCIM), registration point creation (ERFSTELLENALCIM), purchase order information (BESTINFOALCIM), order cancellation (CANCELORDER), and production release (PRODRELEASE). It also covers multi-site capabilities, cleanup logic, and a troubleshooting guide for common issues like service hangs and database lock problems."
---

# A+W Configuration
# A+W Enterprise Export Service
- -INTERNAL-
A+W - Software for Glass

---
## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2017-05-08 | SVH | Copy of DE-TU_AlcibExportService_2012.doc, modified | 1.0 |
| 2019-02-18 | SVH | P.O. modes | |
| 2023-05-04 | SVH | Logging | |
| 2023-05-04 | SVH | [AW-126899] - Production release | |
| 2023-07-27 | SVH | [AW-149830] - Clean-up logic | |
| 2024-01-31 | SVH | Troubleshooting chapter | |

## 1. Introduction
Web services cannot be directly addressed from A+W Enterprise. Since A+W are using Web services at many points for program-wide communication, we have implemented a solution that allows to pass on events and data from A+W Enterprise to other program's Web services.

## 2. Procedure
The database offers a new interface table filled by A+W Enterprise should transfer events occur. Moreover, a new Windows service („A+W Enterprise 5 Export Service“) has been implemented for polling this interface table. If a corresponding entry is found, the service selects the necessary information from the database and passes it on to the appropriate Web services.

