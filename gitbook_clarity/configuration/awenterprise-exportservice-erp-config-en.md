---
description: "EN-CONFIG-AW_Enterprise_Export_Service"
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

