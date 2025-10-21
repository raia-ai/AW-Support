---
title: "EN-CONFIG-AW_Production"
source: "EN-CONFIG-AW_Production.pdf"
tags: ["A+W Production", "Software Configuration", "Production Terminal", "Database", "Remake Handling", "Scanner Configuration", "ERP", "Manufacturing Software", "Technical Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical guide for configuring A+W Production software, focusing on remake handling, production terminal settings, database interactions, and scanner integration. It details procedures for managing production defects, configuring user interfaces, and setting up various hardware and software components."
long_description: "This document serves as a comprehensive configuration manual for the A+W Production software suite. It provides detailed instructions for system administrators and technical users on setting up and managing various modules and functionalities. Key topics include remake handling, which covers the process of managing and remaking defective parts by reassigning labels and adjusting quantities in the system. The guide explains the database structure and specific fields related to orders, parts, and production quantities, detailing how original and remake items are handled. It also covers the configuration of the A+W Production Terminal, including settings for quality assurance (QA) dialogs, data formatting, scanner connections (both local and server-based), and performance counters. The document describes how to integrate with other systems like furnace bed optimization, quality scanners, and sorting systems. It provides step-by-step instructions, including parameter settings in the Parameter Administrator, UI configurations in the Designer, and explanations of underlying database views and functions (AUW functions). The manual is intended to ensure proper setup and efficient operation of the A+W Production environment."
---

If now in the above-mentioned situation the counterlite is an expensive (purchased) TG that should be coated before assembly, you have to be able to stop the original coating of the part and reschedule the production dates for the coating and the assembly with a transfer. For this, in the new item you must assign "real" label numbers from the original item:

**Original Item Structure (Before)**
*   **Auftrag: 123456, Pos: 1**
    *   A Bill of Materials (BOM) tree with components. A component `11` is marked in red.
*   **Auftrag: 123456, Pos: 2**
    *   A BOM tree with components. A component `15` is marked in red.

