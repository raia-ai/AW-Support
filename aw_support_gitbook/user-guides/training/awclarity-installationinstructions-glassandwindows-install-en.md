---
title: "AWClarity InstallationInstructions GlassAndWindows Install EN"
category: "training"
product: "AWClarity"
doc_type: "Unknown"
language: "EN"
tags: ["AWClarity", "InstallationInstructions", "GlassAndWindows", "Install"]
version: "1.0"
last_updated: "2025-12-10"
description: "Text file: AWClarity-InstallationInstructions-GlassAndWindows-Install-EN.md Latest content with line numbers: 2	source: "EN-INST-AW_Clarity_Experience.pdf" 3	tags: ["A+W Clarity Experience", "Installation Instructions", "Software Installation", "Glass and Windows", "A+W Enterprise", "Version 6", "Linux/AIX", "Dependencies", "Setup"] 4	version: "1.0" 5	last_updated: "2025-10-03" 6	short_description: "This document provides installation instructions for A+W Clarity Experience, a software for the g"
source_file: "AWClarity-InstallationInstructions-GlassAndWindows-Install-EN.md"
---


Text file: AWClarity-InstallationInstructions-GlassAndWindows-Install-EN.md
Latest content with line numbers:
2	source: "EN-INST-AW_Clarity_Experience.pdf"
3	tags: ["A+W Clarity Experience", "Installation Instructions", "Software Installation", "Glass and Windows", "A+W Enterprise", "Version 6", "Linux/AIX", "Dependencies", "Setup"]
4	version: "1.0"
5	last_updated: "2025-10-03"
6	short_description: "This document provides installation instructions for A+W Clarity Experience, a software for the glass and windows industry. It outlines the process for a new installation of version 6, detailing requirements, dependencies, and procedures for both the main suite and its add-ins."
7	long_description: "This document serves as the official installation guide for 'A+W Clarity Experience,' a software solution designed for the glass and windows industry. It is intended for planners and system administrators responsible for deploying the software. The guide begins with a change history log and an introductory overview of the installation steps. The core of the document focuses on the new installation of version 6, assuming no prior version is present. It details the necessary components, such as A+W Infrastructure 6 Middleware and Collector Service, and optional services like A+W CIM 6 for production data integration. A significant section is dedicated to system dependencies, including specific instructions for Linux/AIX environments, listing critical files and scripts required for the back-end services to function correctly. The guide concludes with a step-by-step procedure for using the A+W SetupLauncher, notes on configuration settings, expected results post-installation, and instructions for uninstalling the software."
8	---
9	
10	# Installation Instructions: A+W Clarity Experience
11	
12	## Change history:
13	
14	| Date       | Edited by    | Remarks                               | Version |
15	| :--------- | :----------- | :------------------------------------ | :------ |
16	| 2019-02-01 | André Münch  | Original Version                      | 1.0     |
17	| 2020-12-04 | André Münch  | Back end dependencies in Chapter 1.3  | 1.1     |
18	
19	The installation instructions will assist the planner with the installation and configuration of the software named. Please proceed in the following sequence:
20	
21	1.  Check the installation requirements.
22	2.  Compile the required data, additional programs, drivers, etc.
23	3.  Note or determine the time required.
24	
25	---
26	
27	## 1. New installation of version 6
28	
29	The following installation instructions assume that there is no previous version installed. Setup and additional configuration options are described in the configuration instructions.
30	
31	### 1.1 Overview and the basics
32	
33	The following list provides an overview of the work that must be done during installation:
34	
35	- Installation of the A+W Clarity Suite
36	- Installation of the A+W Clarity Suite add-ins (Dispatch, Sales, etc.)
37	
38	The A+W Clarity Suite is the new interface for A+W Enterprise. In the first step, the Dispatch Control module will be made available. The Sales module is planned in the second step.
39	
40	### 1.2 Requirements
41	
42	So that the new interface can establish a connection to A+W Enterprise, the following components have to be installed on the PC:
43	
44	- A+W Infrastructure 6 Middleware
45	- A+W Infrastructure 6 Collector Service
46	
47	#### 1.2.1 Data from production
48	
49	In order to be able to display data from production within the A+W Clarity Suite, the following AWSOA services have to be installed and accessible:
50	
51	- A+W CIM 6 Barcoding Services
52	- A+W Planning 6 Job Services
53	
54	The installation instructions are available at `Installation CIM`.
55	
56	However, these services are optional. The A+W Clarity Suite can also run without them. However, if the services are installed and accessible, the production information is added to the data automatically.
57	
58	### 1.3 Dependencies
59	
60	In order for the service to function properly, the A+W infrastructure services has to be installed on the system.
61	
62	The Service Locator has to be accessible.
63	
64	### 1.3.1 A+W Clarity Suite dependencies under Linux/AIX
65	
66	For the set-up of the ICE environment, you have to pay attention to Chapter 8 of the A+W Enterprise configuration instructions! Without this environment, none of the back end services will run!
67	
68	Essentially, before the set-up, you have to check the following files under Linux/AIX (these should always be up-to-date if possible):
69	
70	- `$ALCIBPRG/install/config/iceconfig.1.0.gz` (templates for set-up of the services)
71	- `$ALCIBPRG/cmd/iceconfig` (script for configuration of the services)
72	- `$ALCIBPRG/cmd/icenodestart` (script for set-up of the ICE node)
73	- `$ALCIBPRG/cmd/icenodestartint` (internal script for starting the ICE node)
74	- `$ALCIBPRG/cmd/icenodestop` (script for stopping the ICE node)
75	- `$ALCIBPRG/cmd/icegridservers` (script for querying the ICE node)
76	- `$ALCIBPRG/al_bin/Linux/dispatchservice` (binary with the dispatch functionalities)
77	
78	For the use of the A+W Logistic Optimizer also:
79	
80	- `$ALCIBPRG/al_bin/Linux/logistickbackendservice` (binary with the functionalities for route optimization)
81	
82	### 1.4 Procedure
83	
84	The A+W Clarity Suite has to be installed in the A+W SetupLauncher. The dependent components should be selected automatically in the SetupLauncher.
85	
86	The additional add-ins can then be installed on each computer.
87	
88	### 1.5 Settings
89	
90	None.
91	
92	### 1.6 Result of the installation
93	
94	After the installation, the program can be called from the A+W Start menu folder.
95	
96	### 1.7 Uninstalling
97	
98	The program can be uninstalled via the Programs and Functions dialog in Windows.
99	
