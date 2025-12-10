---
title: "EN-CONFIG-AW_Business-16-1"
source: "EN-CONFIG-AW_Business-16-1.pdf"
tags: ["A+W Business", "Configuration", "OMS Integration", "Glass4U", "Exchange Service", "MQTT", "Workflow", "ASN", "EDI"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides technical configuration instructions for A+W Business software, focusing on integrating external systems. It covers Phase III (status changes to OMS), Phase IV (ASN transfer), connection to the SGG Glass4U system, and the setup of the modern Exchange Service for workflow execution and the MQTT-based Feedback Service."
long_description: "This is a detailed configuration manual for the A+W Business system. It outlines the procedures for setting up and managing integrations with various external and internal services. The document is divided into several key sections. It begins with instructions for Phase III of OMS integration, which involves the transfer of order status changes. This includes installation of required packages, database configuration, trigger adjustments, and webservice setup. Phase IV covers the transfer of Advanced Shipping Notices (ASN) to OMS, detailing the installation, configuration, and process description. The manual then describes the connection to the SGG Glass4U system, a tool for handling logistic processes. It details the data flow from A+W Business to Glass4U and the feedback mechanism from Glass4U back to the ERP, including webservice URL definitions, status point configurations, and workflow setup. A significant portion is dedicated to the new A+W Exchange Service, a multithreaded replacement for the older Interface Service, which enhances workflow execution. Instructions cover installation, prerequisites, infrastructure setup, service configuration, and specific settings within A+W Business, including the management of production reports and workflow threads. Finally, the document introduces the MQTT-based Feedback Service, a general data interface for all A+W systems, explaining its architecture, installation, and configuration within A+W Business."
---

# 21.8. Phase III (transfer of status changes to OMS)

At that moment, the EDI files are generated with the new workflow if the orders are in the correct status area.

---
### 21.8.1. Installation

The following packages must be installed:
- ALFAK 2011 Basis
- ALFAK 2011 French
- ALFAK 2011 Server
- Complete infrastructure and commercial (see Chapters 1-3)

All new formulas and triggers are in the subdirectory of the ALFAK 2011 installation `\Formula\SGGATP`.

### 21.8.2. Configuration

The database must be brought up to the current state (all scripts including `20170313a.sql`).

The database triggers `SQLBase BW_AUFTR_HIST OMS_Insert.sql` and `SQLBase BW_AUFTR_KOPF OMS Delete.sql` must be installed on the database.

**Before installation of the triggers, the architect number must be adjusted.**

The Webservice address must be entered on the eCommerce/OMS login dialog:

