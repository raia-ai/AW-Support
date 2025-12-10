---
title: "EN-CONFIG-AW_Business-6"
source: "EN-CONFIG-AW_Business-6.pdf"
tags: ["A+W Business", "Configuration", "Production", "ERP", "OrderXML", "ALCIM", "Production Transfer", "Status Management", "Webservice", "Technical Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed configuration instructions for the A+W Business software, focusing on production management, data transfer, and reporting. It covers topics such as master data setup, order transfer types, production feedback mechanisms, and the structure of various data exchange files like OrderXML."
long_description: "This is a technical configuration manual for A+W Business, an ERP system for the glass and window industry. The document outlines the necessary setup for managing the entire production lifecycle, from order entry to final reporting. It begins by detailing the required master data, including company, employee, and customer information. A significant portion is dedicated to the 'Transfer to Production' process, explaining different methods like Standard, Capacity Planning, and automatic transfers. It includes detailed flowcharts and configuration tables for status points, ERP/PPS webservices, and various transfer switches. A comprehensive section describes the OrderXML data format, providing a field-by-field mapping between A+W Business (ALFAK) and production systems (ALCIM). The manual also covers a wide array of file-based and file-less production feedback reports (e.g., STSP, STSL, STSD, AWBar), explaining their structure, purpose, and how they update order statuses within the ERP. Finally, it touches on production overviews, capacity management, and the creation of production orders for stock replenishment. This guide is intended for system administrators and technical consultants responsible for implementing and maintaining the A+W Business production environment."
---

---
### 3.15.2. Export management

### 3.15.3. Master data

**Company master data**
The company master data includes the surrounding data; it is transferred as seller data.

