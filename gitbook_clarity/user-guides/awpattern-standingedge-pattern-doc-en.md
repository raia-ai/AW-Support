---
description: AW_Pattern_Viewer_-_HIDESTANDINGEDGE
---

# awpattern-standingedge-pattern-doc-en

\*\*A+W \*\*\*\*PATTERN VIEWER **-** WORKFLOW STUDIO \*\***HIDE STANDING EDGE** In the document below we are going to show how to Hide the Standing Edge (Small Yellow Triangle) on the Pattern Viewer on each glass cut on the stockplate view.

#### HIDE STANDING EDGE EXAMPLE

In the example below we can see the Standing Edge marked by the yellow triangle on the right edge (edge 2) of the glass.&#x20;

#### A+W PATTERN VIEWER WORKFLOW STUDIO CUSTOMISING

Opening A+W Infrastructure 6 Workflow Studio - On the Process Server open the blue A+W Shortcut > Config Tools > A+W Infrastructure 6 Workflow Studio or run the Windows Executable "C:\Program Files (x86)\A+W\Sandpiper1\InfrastructureWorkflowStudio\WorkflowStudio.exe" **IMPORTANT** - This is a global change which will affect all Pattern Viewer screens unless a Workflow has been configured for each Pattern Viewer. Next, we need to check how many Pattern Viewer Workflows are current configured by choosing Configuration > Workflow Management. In the list should be an Extension Point that has the wording - PatternViewer as shown below. **Single PatternViewer Workflow Example**  **Multiple PatternViewer Workflows Example**&#x20;

Depending on if or how this has been configured the correct **Workflow** name will need to be opened in the next part described below. To open the Pattern Viewer Default Workflow choose File > Load then the Workflow that matches the name required or Pattern Viewer Default Workflow if it is the only one listed. **N\*\*\*\*ote** - In this instance the Pattern Viewer TB1 Workflow has been selected as it is the workflow that will be used with the Cutting Table 1 under A+W Realtime Optimizer else it may just be Pattern Viewer Default Workflow to be selected if it is the only workflow in use.  After the required workflow has been opened select File > Add Reference from the top menu. Open the folder and file - C:\Program Files (x86)\A+W\TECHSOFT\XoptOn\AW.Clarity.CIM.Cutting.Facade.dll. In the Toolbox list on the left hand side under AW.Clarity.CIM.Cutting.Facade.Activities of the screen click on HideStandingEdge and drag it over to the center Activity1 window and connect it into the workflow as shown below.  Select HideStandingEdge and then on the right hand side of the screen is a Misc entry that shows the following options.

* PatternIn
* PatternOut In this example, we are going to change the empty fields so that PatternIn has the value of PatternIn and PatternOut has the value PatternOut as shown in the image below.  Finally save the changes by using File > Save from the top menu. **Note** - It is recommended that A+W Realtime Optimizer is closed and opened again to have A+W Pattern Viewer read the new workflow configuration so that it no longer shows the Standing Edge Yellow Triangle on each glass cut item.

#### ADDITIONAL TEXT TESTING

In the previous Pattern Viewer display we had the Standing Edge Yellow Triangle shown on the screen.  This time when a batch is loaded for cutting the Standing Edge Yellow Triangle has now been removed.&#x20;
