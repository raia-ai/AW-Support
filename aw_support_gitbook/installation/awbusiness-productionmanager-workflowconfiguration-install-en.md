---
title: "EN-INST-AW_Business_Production_Manager_2"
source: "EN-INST-AW_Business_Production_Manager_2.pdf"
tags: ["A+W Software", "Production Manager", "Workflow Configuration", "Realtime Optimizer", "Database Configuration", "Technical Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides technical instructions for configuring and managing the A+W Business Production Manager software. It covers workflow tasks, data configuration, Realtime Optimizer (RTO) setup, and various system parameters."
long_description: "This technical manual is a comprehensive guide for system administrators and technical personnel responsible for the installation, configuration, and maintenance of the A+W Business Production Manager software for glass and windows manufacturing. The document details a wide range of configuration tasks, starting with setting up automated workflow tasks for capacity planning and archiving. It provides step-by-step instructions for creating and managing formulas, workflow tasks, and their automated execution schedules within the A+W Business environment. A significant portion is dedicated to configuring the Realtime Optimizer (RTO) as a stand-alone system, including setting up cutting drivers, managing import/export of optimization data, and handling specific configurations like article numbers, shape imports, and feedback mechanisms. The guide also covers advanced topics such as configuring bender text placeholders, machine drivers, and handling partial deliveries. It includes an extensive reference section detailing the meaning of variables in formulas and the configuration parameters in the PROD_PARAMETER table, which control everything from job number ranges to label printing and optimization behavior. Finally, the document offers tips and tricks for updates, handling new database fields, and managing stock plates and residual plates in optimization."
---

# Software for Glass and Windows

---
## 4.7 Create workflow task for archiving production manager jobs

A workflow task has to be set up in order to ensure that the finished orders of the Production Manager are transferred automatically to the archive.

- Call Master data > Company > Formulas.

