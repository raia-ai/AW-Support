---
description: "AW_Pattern_Viewer_-_CHANGESTARTOFBREAKAGE"
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
