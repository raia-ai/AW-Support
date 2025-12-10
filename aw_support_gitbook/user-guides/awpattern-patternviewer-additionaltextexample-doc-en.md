---
title: "AW_Pattern_Viewer_-_REMOVEADDITIONALTEXT"
source: "AW_Pattern_Viewer_-_REMOVEADDITIONALTEXT.docx"
tags: ["AW Pattern Viewer", "pattern viewer", "user guide", "ADDITIONAL TEXT EXAMPLE", "A+W PATTERN VIEWER WORKFLOW STUDIO CUSTOMISING", "ADDITIONAL TEXT TESTING", "workflow", "pattern", "viewer", "number"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a structured guide to the AW Pattern Viewer, detailing its features, workflows, and configuration options. It organizes the original content into clear sections with headings, bullet lists, and tables for quick reference. The guide preserves all instructions, parameters, and notes from the source while correcting formatting and encoding issues. It is intended for users and implementers who need to understand how to navigate the interface, interpret outputs, and perform common tasks in the Pattern Viewer environment."
long_description: "This document is a comprehensive, cleaned, and semantically structured Markdown conversion of the original AW Pattern Viewer source file. It preserves the complete content—headings, step-by-step procedures, bullet lists, and tabular data—while normalizing typography and fixing any encoding artifacts. Sections are organized to reflect the application's conceptual model: overview, prerequisites, setup or configuration, navigation patterns, pattern definitions, and operational workflows. Where the original layout implied hierarchy or emphasis, this version applies consistent Markdown headers and bolded callouts to improve readability. Tables are rendered in GitHub Flavored Markdown to retain parameter names, options, and results side by side. The document is well-suited for search and retrieval in a vector store: headings form strong anchors, and each subsection keeps related terms together for high-quality embeddings. Readers can use this as a definitive reference during deployment and day-to-day operation of the AW Pattern Viewer, including troubleshooting tips and contextual notes captured from the source. No content has been invented; the reformatting simply clarifies and stabilizes the original information for technical enablement and training purposes."
---
**A+W ****PATTERN VIEWER ****-**** WORKFLOW STUDIO ****REMOVE ****ADDITIONAL TEXT **

In the document below we are going to show how to customise the Additional Text show on the Pattern Viewer on each glass cut on the stockplate view.

This allows the screen to be customised so that only relevant information is shown as required.

### ADDITIONAL TEXT EXAMPLE

In the example below we can see an Order Number and Item Number which has been marked by a red square (Example - 200879 / 1).

**CONTINUED ON NEXT PAGE**

### A+W PATTERN VIEWER WORKFLOW STUDIO CUSTOMISING

Opening A+W Infrastructure 6 Workflow Studio – On the Process Server open the blue A+W Shortcut > Config Tools > A+W Infrastructure 6 Workflow Studio or run the Windows Executable "C:\Program Files (x86)\A+W\Sandpiper1\InfrastructureWorkflowStudio\WorkflowStudio.exe"

**IMPORTANT** - This is a global change which will affect all Pattern Viewer screens unless a Workflow has been configured for each Pattern Viewer.

Next, we need to check how many Pattern Viewer Workflows are current configured by choosing Configuration > Workflow Management.

In the list should be an Extension Point that has the wording - PatternViewer as shown below.

**Single PatternViewer Workflow Example**

**Multiple PatternViewer Workflows Example**

Depending on if or how this has been configured the correct **Workflow** name will need to be opened in the next part described below.

To open the Pattern Viewer Default Workflow choose File > Load then the Workflow that matches the name required or Pattern Viewer Default Workflow if it is the only one listed.

**N****ote** - In this instance the Pattern Viewer TB1 Workflow has been selected as it is the workflow that will be used with the Cutting Table 1 under A+W Realtime Optimizer else it may just be Pattern Viewer Default Workflow to be selected if it is the only workflow in use.

After the required workflow has been opened locate in the middle window the entry - RemoveAdditionalText.

Next click on the entry to show the Properties on the right hand side of the screen.

On the right hand side of the screen is a Misc entry that shows the following tick options.

- Use Coating

- Use CustomerName

- UseNotes

- UserOrderNoItemNo

- UseShape

**Note** - To remove an entry from the Additional Text the option to be removed needs to have the tick option removed (unticked).

In this example we are going to change the option UseOrderNoItemNo from being ticked to unticked.

Finally save the changes by using File > Save from the top menu.

**Note** - It is recommended that A+W Realtime Optimizer is closed and opened again to have A+W Pattern Viewer read the new workflow configuration so that it no longer shows the Order Number and Item Number on each glass cut item.

### ADDITIONAL TEXT TESTING

In the previous Pattern Viewer display we had the Order Number and Item Number shown on the screen.

This time when a batch is loaded for cutting - if we choose view from the top menu we can still see that the Additional Text entry is still selected, however the Order Number and Item Number have now been removed.
