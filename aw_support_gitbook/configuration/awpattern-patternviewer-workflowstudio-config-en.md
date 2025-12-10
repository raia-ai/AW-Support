---
title: "AW_Pattern_Viewer_-_CHANGESTARTOFBREAKAGE"
source: "AW_Pattern_Viewer_-_CHANGESTARTOFBREAKAGE.docx"
tags: ["A+W", "Pattern Viewer", "Workflow Studio", "ChangeStartOfBreakage", "StartPoint", "Breakpoint", "Realtime Optimizer", "Configuration", "Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document explains how to configure the A+W Pattern Viewer’s breakpoint (start point) using the A+W Infrastructure 6 Workflow Studio. It covers opening the Workflow Studio, identifying the correct Pattern Viewer workflow, and adjusting the ChangeStartOfBreakage StartPoint setting to change the starting corner of stockplates."
long_description: "This guide provides a concise, step-by-step reference for administrators and power users who need to adjust the starting breakpoint used by the A+W Pattern Viewer. The breakpoint, or start point, determines from which corner stockplates begin processing in the Pattern Viewer. In certain operational contexts, you may need to change the default start point from the bottom-left corner to a different corner to align with plant conventions, production flows, or optimization requirements.

The document begins by outlining how to open the A+W Infrastructure 6 Workflow Studio on the Process Server—either via the A+W shortcut (Config Tools) or by executing the WorkflowStudio.exe directly. A critical callout emphasizes that this is a global change affecting all Pattern Viewer screens unless each Pattern Viewer has its own dedicated workflow configuration. Users are guided to verify which Pattern Viewer workflows are currently configured under Configuration > Workflow Management, locate the PatternViewer extension point, and load the appropriate workflow definition. Where only a single workflow exists, this is typically the Pattern Viewer Default Workflow; the guide notes this scenario explicitly.

Once in the correct workflow, the ChangeStartOfBreakage entry contains the StartPoint parameter that controls the breakpoint corner. The guide enumerates the available StartPoint options—BottomLeft (the default, matching A+W Realtime Optimizer), BottomRight, Top Right, and Top Left—so that you can select the setting that matches your production needs. A separate section references the A+W Realtime Optimizer’s Plan Edit behavior for consistency with production.

By following the steps and reference screenshots (if applicable in your environment), you can quickly reconfigure the Pattern Viewer’s start point and ensure alignment with plant standards or downstream systems. This document is intended for technical users with access to the A+W Infrastructure 6 Workflow Studio and permissions to edit workflow configurations."
---

# A+W PATTERN VIEWER - WORKFLOW STUDIO CHANGESTARTOFBREAKAGE

## Opening A+W Infrastructure 6 Workflow Studio

On the Process Server open the blue A+W Shortcut > Config Tools > A+W Infrastructure 6 Workflow Studio or run the Windows Executable "C:\Program Files (x86)\A+W\Sandpiper1\InfrastructureWorkflowStudio\WorkflowStudio.exe"

> **IMPORTANT** - This is a global change which will affect all Pattern Viewer screens unless a Workflow has been configured for each Pattern Viewer.

## A+W Pattern Viewer Workflow Studio Customising

### Change Breakpoint Position

In some instances, it may be required that the breakpoint (start point) of the stockplates needs to be changed to a different corner than the default at the bottom left.

This is possible by changing the StartPoint found under the ChangeStartOfBreakage entry under Pattern Viewer Default Workflow under the A+W Infrastructure 6 Workflow Studio.

First we need to check how many Pattern Viewer Workflows are current configured by choosing Configuration > Workflow Management.

In the list should be an Extension Point that has the wording - PatternViewer as shown below.

Depending on if or how this has been configured the correct Workflow name will need to be opened in the next part described below.

To open the Pattern Viewer Default Workflow choose File > Load then the Workflow that matches the name required or Pattern Viewer Default Workflow if it is the only one listed.

Note - In this instance the Pattern Viewer Default Workflow has been selected as it is the only installed workflow in this instance.

### Workflow Configuration Steps

1. First we need to check how many Pattern Viewer Workflows are current configured by choosing Configuration > Workflow Management.
2. In the list should be an Extension Point that has the wording - PatternViewer as shown below.
3. Depending on if or how this has been configured the correct Workflow name will need to be opened in the next part described below.
4. To open the Pattern Viewer Default Workflow choose File > Load then the Workflow that matches the name required or Pattern Viewer Default Workflow if it is the only one listed.

> Note: In this instance the Pattern Viewer Default Workflow has been selected as it is the only installed workflow in this instance.

## A+W Realtime Optimizer > Plan Edit Same as Production

## ChangeStartOfBreakage

- **ChangeStartOfBreakage > StartPoint = BottomLeft (Same as A+W Realtime Optimizer)**
- **ChangeStartOfBreakage > StartPoint = BottomRight**
- **ChangeStartOfBreakage > StartPoint = Top Right**
- **ChangeStartOfBreakage > StartPoint = Top Left**
