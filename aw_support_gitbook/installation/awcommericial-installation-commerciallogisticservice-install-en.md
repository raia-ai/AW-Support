---
title: "EN-INST-AW_Commericial_Logistic_Service"
source: "EN-INST-AW_Commericial_Logistic_Service.pdf"
tags: ["A+W", "Installation", "Commercial Logistic Service", "Software", "Glass and Windows", "Configuration", "Version 6", "Setup", "Uninstallation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "An installation guide for the A+W Commercial Logistic Service, version 6. It details the steps for a new installation, including prerequisites, dependencies, configuration, and uninstallation procedures. The document is intended for consultants installing the software."
long_description: "This document provides detailed installation instructions for the A+W Commercial Logistic Service, specifically for a new installation of version 6. It is designed to guide consultants through the entire process, from initial preparation to final configuration and verification. The guide begins by outlining the change history and the general process flow, which includes checking installation requirements, collecting necessary data, and estimating the required time. The core of the document focuses on the new installation of version 6, explaining its purpose in facilitating communication between A+W products like A+W Business and the A+W Logistics Optimizer. It covers essential prerequisites, such as the co-location of A+W Business and the necessary language packs. The guide also highlights dependencies on A+W infrastructure services. The procedure involves running a setup launcher, followed by post-installation configuration through the A+W Infrastructure Web interface. This configuration includes setting up database connections for both A+W Business and the A+W Logistics Optimizer, as well as defining the logical user and backend type. Finally, the document explains how to verify a successful installation by starting the service via the Service Locator Administration and provides instructions for uninstallation through the Windows \"Programs and Functions\" dialog."
---

# Installation Instructions: A+W Commercial Logistic Service

---
## Change history:

| Date       | Edited by      | Comments         | Version |
| :--------- | :------------- | :--------------- | :------ |
| 2016-03-16 | Bastian Michel | Original Version | 1.0     |

The installation instructions guide the consultant through the installation and the configuration process of the cited software. Please proceed in the following order:

1.  Check the installation requirements.
2.  Collect the necessary data, additional programs, drivers, etc.
3.  Consider or calculate the time required.

## Content

- **Installation Instructions**
- **A+W Commercial Logistic Service**
    - **1 New installation of version 6**
        - 1.1 Overview and Basics
        - 1.2 Prerequisites
            - 1.2.1 A+W Business
        - 1.3 Dependencies
        - 1.4 Procedure
        - 1.5 Settings
        - 1.6 Installation Result
        - 1.7 Uninstalling

## 1. New installation of version 6

The following installation instructions assume that no previous version has been installed. Setup and additional configuration options are described in the configuration instructions.

### 1.1 Overview and Basics

Below you will find a list of the work to be carried out during the installation:
- Installation of the A+W Commercial Logistic Service

The A+W Commercial Logistic Service is used for the communication between A+W products (currently A+W Business and A+W Cantor) and the A+W Logistics Optimizer. It transports the required document data to the Logistics Optimizer and calculates the route data back again.

### 1.2 Prerequisites

There are various requirements for installation depending on the respective A+W program.

#### 1.2.1 A+W Business

For the use of A+W business, such a system has to be installed on the same system as the BusinessCom.exe is used in the Logistic Service. Plus the respective language package has to be installed so that the messages are displayed in the correct language.

### 1.3 Dependencies

In order for the service to function properly, the A+W infrastructure services must be installed on the system.

### 1.4 Procedure

The A+W Commercial Logistic Service has to be installed with the setup launcher.

### 1.5 Settings

Once the installation has been performed, the user has to be set up under which the service is to run.

