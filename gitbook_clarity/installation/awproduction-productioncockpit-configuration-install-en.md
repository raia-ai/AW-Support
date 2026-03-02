---
description: "EN-INST-AW_Production_Cockpit"
---


# A+W Production Cockpit Installation Guide

Software for Glass and Windows

---
## History

| Date | Author | Modification/remarks | Version |
| :--- | :--- | :--- | :--- |
| 24.08.2012 | Peter Kühn | First Release | 1.0 |
| 11.07.2014 | Marco Meiser | Revised | 1.1 |

## Content

*   [**A+W Production Cockpit Installation Guide**](#a+w-production-cockpit-installation-guide)
    *   [**1. Introduction**](#1-introduction)
    *   [**2. Precondition**](#2-precondition)
    *   [**3. Installation**](#3-installation)
    *   [**4. Configuration**](#4-configuration)
        *   [**4.1. Main Settings**](#41-main-settings)
        *   [**4.2. Configuration of the Speedometer**](#42-configuration-of-the-speedometer)
        *   [**4.3. Configuration of the Performance-Diagram**](#43-configuration-of-the-performance-diagram)
        *   [**4.4. Configuration of the Pie**](#44-configuration-of-the-pie)
        *   [**4.5. Configuration of the Traffic-Light**](#45-configuration-of-the-traffic-light)
    *   [**5. Simulation**](#5-simulation)

## 1. Introduction

A+W Production Cockpit is a new monitor which shows the manager or the people on the shop-floor the actual performance of their production for different machines. Different groups of machines are displayed in separate tabs. A+W Production Cockpit uses the same technic like the new ToolTV's, so it is very easy to configure and to deploy on different computer.

The first tab "Overview” gives the managers the possibility to choose some machines explicitly to compare the productivity within a configurable timespan. Each machine is displayed in a separate color. With a filter it is possible to pre-configure which machines the manager can choose.

The other tab displays the performance of the production for a group of machines (cutting-tables, IG-lines, special-machines) with different design-elements:
a) **Speedometer**: displays the quantity produced in the last 60 minutes (actual situation)
b) **Diagram**: shows the quantity produced in the last 60 minutes (trend for the last 24 hours)
c) **Pie**: displays the percentage of the different machine status within the last 24 hours
d) **Traffic-light**: displays the actual machine status

To show the performance of the productivity, only the table `awbar_booking` is used. So it is very easy to create some data for simulation.

**Standard Configuration:**

*   **Tab "Cutting"**: Table 1, 2 and 3 = Registration Point 110, 120, 150
*   **Tab "IG Lines”**: Line 1, 2 and 3 = Registration Point 1610, 1620, 1630
*   **Tab "Special Machines”**: TG1, TG2, Lamy = Registration Point 1310, 1320, 1510

The tab "Special-Machines” is just a template and can be used also for all other registration points. It is also possible to add additional tabs for other machines. But for the standard we wanted to keep it as simple as possible and that it will work for the most of our customers with a minimum change of the configuration.

The different machine status are set by a ToolTV and also by Xopton (will be available in the Release 2012). The machine status have to be set up in the master data of ALCIM (see chapter "precondition”). The design elements “pie” and “traffic light” use the table `bdestat_es` to display the machine status.

**Standard Configuration:**
- **green** = status “501-Ready”
- **yellow** = status “502-Off”, “503-Break”, “504-Maintenance”, “505-Setup"
- **red** = status "506-Failure"

## 2. Precondition

To run the A+W Production Cockpit there must be a PPS-Webservice available and some machine status in the Alcim master data. For the standard A+W Production Cockpit you have to set up the following master data:

**Master Data > Barcoding > Status Types:**

You must define a `Status Type` for machine states. In the example screenshot, this is done by creating a new status type:
*   **ID**: 30
*   **Name**: Machine-State

