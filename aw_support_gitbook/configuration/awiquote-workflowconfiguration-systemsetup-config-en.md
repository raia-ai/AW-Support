---
title: "EN-CONFIG-AW_iQuote_2"
source: "EN-CONFIG-AW_iQuote_2.pdf"
tags: ["A+W iQuote", "workflow configuration", "system setup", "product management", "user interface", "software documentation", "ERP integration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed technical guidance on configuring A+W iQuote, focusing on workflows, system setup, and activity parameterization. It covers topics such as color filters, two-phase commits, file uploads, multi-site capabilities, and UI customization."
long_description: "This is a comprehensive configuration manual for the A+W iQuote system. It details the setup and customization of various features through a workflow-based approach. Key areas covered include defining filters for product colors and special colors, managing transactions with a two-phase commit process to prevent duplicate orders, and integrating file uploads and web links at both item and document levels. The document explains how to configure system behaviors like pattern/coating side selection, project-specific product offerings, and the insertion of processings via workflows. It also provides instructions for system-level configurations, such as incorporating iQuote into a start page using an IFrame, setting up product images, and customizing UI texts and browser icons. A significant portion of the manual is dedicated to a detailed breakdown of all available workflow activities and their parameters for the Configurator, Check-in, Checkout, and Model Mapping processes. This includes activities for product selection, geometry entry, processing, pricing, and more, offering a complete reference for developers and system administrators to tailor the A+W iQuote application to specific business needs."
---

---
## 2.27. Color filter and special colors

Now filters can be defined for the product colors. These must be inserted in the workflow behind the product color activity.

