---
description: "EN-INST-AW Production Pattern Viewer"
---


# Installation Instructions: A+W Production Pattern Viewer

---
## Change history:

| Date       | Edited by | Remarks          | Version |
| :--------- | :-------- | :--------------- | :------ |
| 2019-06-04 | DLA       | Original version | 1.0     |

## Introduction

The installation instructions will assist the planner with the installation and configuration process for the software named. Please proceed in the following sequence:

1.  Check the installation requirements.
2.  Compile the required data, additional programs, drivers, etc.
3.  Note or determine the time required.

## 1. Installation

### 1.1 Requirements
In addition to a run-capable A+W Realtime Optimizer, the A+W Pattern Viewer requires an AWSOA environment with an A+W Planning Optimisation Service.

### 1.2 Installation location
The A+W Pattern Viewer is installed on the machines that output a cutting plan on a monitor. This can be an individual PC that outputs the cutting plan on a monitor on the cutting table, however it can also be the PC or server on which the A+W Realtime Optimizer is running and that outputs the cutting plan on a second monitor.

### 1.3 Procedure
On the machines in question, the A+W Production Pattern Viewer diskset is executed with all dependent disksets (A+W Infrastructure Middleware).

After the first installation on a machine, the A+W Pattern Viewer must be restarted manually and configured.

If the A+W Pattern Viewer is operated on a terminal server, the configuration must be done once under each Windows user who would like to use this tool.

If this has happened, the A+W Pattern Viewer must be connected to the respective A+W Realtime Optimizer.

There are more details in the Configuration chapter.

## 2. Registration
After the first start of the A+W Pattern Viewer on a machine under a Windows user, it must be registered in AWSOA. To do this, open the [Register user] menu in the settings.

First click the **[Register application]** button. The status for `ICE Node Registered` will change from `False` to `True`.

Then install the **[Tray application]** by clicking the `Install` button. The statuses for `Tray-Application Installed` and `Tray-Application Running` will change to `True`.

Now a node of this A+W Pattern Viewer is registered for this machine and Windows user in the AWSOA Service Locator. There are no services yet. An entry for the pattern viewer will appear in the IceGrid Admin tool under `Runtime Components` (e.g., `MAPS-MAPSADMIN-PatternViewer`).

Now the A+W Pattern Viewer has a tray symbol under this user with which you can end the node and re-start it. This tray symbol must be started when the Windows user logs in; the A+W Pattern Viewer creates a planned task for this in the Windows Task Scheduler.

For this Windows user, it is now possible to add a service for each client required.

Select the client, the ID of the cutting table, and a sequential number. For example:
-   **Site ID**: MAPS Client
-   **Table ID**: TB1
-   **Label ID**: 001

Now register this service by clicking the **[Register Application]** button. The application will confirm that it is registered with the specified parameters. Using this configuration, the services can also be removed again by clicking **[Deactivate Application]**.

Now you can exit A+W Pattern Viewer. In the AWSOA Service Locator, the service is now created and it can be started. The service has the name consisting of client number, ID of the cutting table, and the sequential number (e.g., `PatternViewer-1-TB1-001`).

This name of the service is displayed in the A+W Pattern Viewer title bar if it is started via the Service Locator Administrator.

### 2.1 Testing
Under tools, the installation includes the A+W Production Pattern Viewer Test Tool, with which it should be possible to start the A+W Pattern Viewer if it has been registered correctly.

## 3. Configuration

### 3.1 Connecting to the A+W Realtime Optimizer
So that the A+W Pattern Viewer is connected to the A+W Realtime Optimizer, the name of the AWSO service must be entered in the `XOPTON.CFG` file. Here the key consisting of client ID of the cutting table and sequential number is separated with a hashtag. In addition, the path is set permanently to the keyword ICE:

```ini
[XTV]
ServerName=1#TB1#001
Path=ICE
```

### 3.2 Breakage reasons
The breakage reasons can be configured in the settings that all A+W Pattern Viewers use. For this, the default group must be selected and the reasons to be used added. For each breakage reason, the number of the break from the A+W Production master data and a name must be entered. You can also assign a picture to each reason.

If different A+W Pattern Viewers require different breakage reasons, additional groups can be added.
