---
title: "EN-CONFIG-AW_Pattern_Viewer"
source: "EN-CONFIG-AW_Pattern_Viewer.pdf"
tags: ["A+W", "Clarity", "Pattern Viewer", "Software for Glass", "Configuration", "Workflow", "Realtime Optimizer", "Installation", "Customizing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A configuration guide for the A+W Clarity Pattern Viewer, a software solution for the glass industry. It covers installation, registration, and customization of the viewer, along with its integration with the A+W Realtime Optimizer."
long_description: "This document provides comprehensive instructions for the installation, configuration, and customization of the A+W Clarity Pattern Viewer. It is intended for technical personnel responsible for setting up and maintaining A+W software solutions for glass manufacturing. The guide begins with system requirements and the installation of necessary components, including the A+W Clarity Pattern Viewer, A+W Planning 6 Optimization Services, and A+W Production 6 Realtime Optimizer. It details two methods for viewer registration: one through the application's UI and another using the `PreparePatternViewer` command-line tool, explaining the differences and use cases for each. The document then covers the configuration of the A+W Realtime Optimizer to work with the Pattern Viewer, including settings in the `XOPTON.CFG` file. A significant portion is dedicated to customizing the Pattern Viewer's display through the A+W Infrastructure 6 Workflow Studio. This includes modifying the starting point of patterns, adding custom text and colors, displaying logos, and changing breakout sequences. The guide also addresses troubleshooting common issues, setting up table-dependent workflows, and using the A+W Push Button Tool for remote control."
---

# A+W Clarity Pattern Viewer

---
## Change history

| Date | Author | Notes | Version |
| :--- | :--- | :--- | :--- |
| | Todd Leiseman | Draft | 1.0 |
| | Todd Leiseman | Workflow Studio Customizing | 1.1 |
| | Todd Leiseman | Workflow Studio Clean Up Scripts | 1.2 |
| | Jens Schmidt | RegisterForCurrentUser | 1.3 |
| | Jens Schmidt | Workflow activities: describing pictures and other activities | 1.4 |
| | Jens Schmidt | Logos, stamps, reference marks | 2.0 |

## Content

1.  **A+W Clarity Pattern Viewer installation and customizing**
    1.1. Installed diskset requirements
    1.2. Extra component installation
    1.3. Pattern Viewer configuration
        1.3.1. Registration in the Pattern Viewer
        1.3.2. PreparePatternViewer Tool
        1.3.3. Differences between the two procedures
    1.4. IceGrid review and testing
    1.5. A+W Pattern Viewer tester
    1.6. Known issue messages
2.  **A+W Realtime Optimizer configuration**
    2.1. RegisterForCurrentUser
    2.2. A+W Infrastructure 6 workflow studio configuration
    2.3. Known issue message
    2.4. Server with workstation A+W Pattern Viewer configurations
    2.5. A+W Realtime Optimizer usage
3.  **A+W Pattern Viewer workflow studio customizing**
    3.1.1. Setting starting point of the pattern
    3.1.2. AddCustomText
    3.1.3. AddCustomType
    3.1.4. ReferenceMark
    3.1.5. MirrorStripe
    3.1.6. MoveWaste
    3.1.7. RemoveAdditionalText
    3.1.8. Format Rack
    3.1.9. Prefix2ndGlassType
    3.1.10. Add2ndGlassTypeToAdditional
    3.1.11. Change Sequence
    3.1.12. Processing marker
    3.1.13. Remove depiction of the support edge
    3.2. Table-dependent workflows
    3.3. Workflow clean up scripts
    3.4. Breakage reason
4.  **Configuration**
    4.1. Rotating subplates automatically
5.  **A+W Push Button Tool**
6.  **Ice know how**
    6.1.1. Pattern tray and IceNode
    6.1.2. Callback
7.  **Research options**

## 1. A+W Clarity Pattern Viewer installation and customizing

The documentation below shows the steps to complete an installation of A+W Pattern Viewer when being configured with one cutting table (TB1).

Plus, how to customize the A+W Clarity Pattern Viewer Workflow to change how the screen can be presented to the operator.

Please ensure the latest installation of A+W Clarity is downloaded with all current hotfixes and the system is installed with the latest Windows Updates for the system in question.

### 1.1. Installed diskset requirements

- A+W Infrastructure Process Server Diskset with an AWSOA Database and valid ICEGrid connection

### 1.2. Extra component installation

- Component Selection > A+W Clarity > A+W Clarity Pattern Viewer
- Component Selection > A+W Common > A+W Planning 6 Optimization Services
- Component Selection > A+W Production > A+W Production 6 Realtime Optimizer

