---
title: "EN-CONFIG-AW_Residual_Stock_Manager"
source: "EN-CONFIG-AW_Residual_Stock_Manager.pdf"
tags: ["A+W", "Residual Stock Manager", "Configuration", "Planning Web", "Realtime Optimizer", "Software for Glass", "xopton.cfg", "ODBC", "Infrastructure Web", "Glass Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical configuration guide for the A+W Residual Stock Manager. It covers requirements, setup of the Planning Web for rack types and stock, stock label printing via ODBC, and configuration of the Realtime Optimizer and optimization kernel (xopt.cfg)."
long_description: "This document provides detailed instructions for configuring the A+W Residual Stock Manager, a software solution for managing residual glass stock. It begins with the initial installation requirements and then delves into the configuration of the A+W Planning Web. This section covers setting up various rack types (like L-racks and harp racks), defining stock areas, and configuring stock label printing, which involves ODBC data source setup and printer configuration on the infrastructure web. The guide then explains how to configure the A+W Realtime Optimizer, detailing adjustments needed in the `xopton.cfg` file and settings within the program itself to activate and manage residual plate stock. It also covers the broader configuration of the infrastructure web, including settings for stock label printing, stock connection settings for external systems like Hegla ReMaster, and assigning cutting tables to specific stocks. Finally, the document discusses advanced tuning of the optimization kernel via the `Xopt.cfg` file, explaining parameters like `ForceStockplateSequence` and `ConsumeResidualsFirst` to control how residual plates are prioritized and used during the optimization process. The guide is intended for internal use by technical personnel responsible for setting up and maintaining the A+W software environment."
---

# A+W Configuration
# A+W Residual Stock Manager

**-INTERNAL-**

**A+W - Software for Glass**

---

---
## Content

1.  **Requirement** - 3
2.  **Planning Web** - 4
    *   2.1. Rack types - 4
    *   2.2. Stock incl. rack - 5
    *   2.3. Stock Label Printing - 9
        *   2.3.1. ODBC configuration - 9
        *   2.3.2. Printer configuration on the infrastructure web - 10
3.  **Realtime Optimizer** - 12
    *   3.1. Xopton.cfg - 12
    *   3.2. Settings directly in the program - 13
4.  **Configuration of the infrastructure web** - 14
5.  **Optimization kernel: Xopt.cfg** - 18

---

## 1. Requirement

The installation was executed successfully according to the INST-A+W Planning Stock installation instructions.

---

## 2. Planning Web

### 2.1. Rack types

For configuration of the rack types, you must take the following steps:

*   Open the A+W Planning Web, for example via the A+W folder on the desktop. Normally this page is hosted under `http://[processserver]/Planning.Web`. Then the browser opens with the start page of the A+W Planning Web. (see Figure 2-1)
*   Press the Stock button.

