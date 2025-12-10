---
title: "AW_Pattern_Viewer_-_WEIGHTREFERENCEMARK"
source: "AW_Pattern_Viewer_-_WEIGHTREFERENCEMARK.docx"
tags: ["A+W", "Pattern Viewer", "Workflow Studio", "Reference Mark", "Base64", "SQL Server", "Glass Cutting", "Manufacturing IT", "A+W Infrastructure"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document explains how to configure an A+W Pattern Viewer workflow to display a weight-based reference mark on stockplate cuts. Using a SQL statement that evaluates item weight in kilograms, the workflow shows a red or green indicator to signal manual handling requirements. It includes base64 image assets, guidance on converting images to and from base64, and detailed steps for adding the Reference Mark activity in A+W Infrastructure 6 Workflow Studio. The content also covers testing via order entry and how to swap indicator graphics."
long_description: "This guide provides an end-to-end procedure for adding a weight-driven reference mark to A+W Pattern Viewer screens so operators can quickly recognize whether a glass piece exceeds a manual handling threshold. The workflow leverages a SQL Server statement that converts POOL_TEILE.GEWICHT_FORM from grams to kilograms and returns a categorical result used by the Reference Mark control to display either a red (manual handling prohibited) or green (single-person) indicator. The document supplies ready-to-use base64-encoded images for both red and green circles, along with examples sourced from emojipedia.org (Yellow Warning Sign and Grey OK) to demonstrate how to change icons. It also references free online tools for converting images to and from base64 for rapid prototyping.

Within A+W Infrastructure 6 Workflow Studio, the instructions show how to add the AW.Clarity.CIM.Cutting.Facade.Activities library, place a Reference Mark activity into the Pattern Viewer workflow, set key properties (DisplayName, PatternIn/Out, and the SQL Statement), and relink variables so data flows correctly. Practical testing guidance describes creating an order with two differently sized 12 mm Clear Float items to validate that the Pattern Viewer displays the expected red/green indicators and the WEIGHT label at the specified corner and offsets. The guide concludes with steps to replace the indicator artwork by updating the Logo1Base64 and Logo2Base64 values, notes on image sizing (32×32 px), and reminders to save workflow changes. All original SQL snippets, configuration values, and example assets are retained to support accurate implementation."
---

## Overview

A+W PATTERN VIEWER - WORKFLOW STUDIO WEIGHT REFERENCE MARK

In the document below we are going to show how to add a Reference Mark - Green or Red Circle to a Stockplate Cut to show if a glass item has a calculated weight of a specified value to show the cutting table operator that the glass can the handled in a single person or multiple person lift.

Here is how we will allocate the graphics in this document.

### Graphic Allocation Examples

| A+W | EMOJIPEDIA.ORG |
| --- | --- |
| Green Circle - Single Person Lift<br>Red Circle - Multiple Person Lift | Grey OK - Single Person Lift<br>Yellow Warning Sign - Multiple Person Lift |

| YELLOW WARNING SIGN | GREY OK |
| --- | --- |
|  |  |

## BASE64 TO IMAGE INFORMATION

Base64 To Image Converter - https://codebeautify.org/base64-to-image-converter

### Logo1Base64 — Red Circle

$$$ START IMAGE STRING $$$

```
iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAK3RFWHRDcmVhdGlvbiBUaW1lAE1vIDEzIE9rdCAyMDAzIDAwOjAxOjA4ICswMTAwjAm/sgAAAAd0SU1FB9MKDBYBH9SggE4AAAAJcEhZcwAACvAAAArwAUKsNJgAAAAEZ0FNQQAAsY8L/GEFAAACV0lEQVR42u2UTU/UUBSGn9tpp2WG+RIyRmOCn4RootGVIW5cmGiC+A+Enfwk3OnOtRCJcWVwpTESQ6IYJYCOEgYG5numn55OTdwUGF0qJznp7e3p+/S+5/bCUfzzoQ4rCK6Rl6oZfCYkxwhkUmNFcl7uZ9USu38NCK5zG5vHnQ5F9/xFgtEraEoRrC6jf3yPZVJGZ0q9ZuGPAT3xDk8b2aKhT9xHGzmHlh4Ez8evV/F/rOMvPCFVKTkkubcfJBbQswVWWlahmLg5iZbNodIZlJWShz5Bu0lQFUijivdqgVR7dyu0L84uLfbzfWZsj6J+6jRGbZtEdRtdUtvbkhRXajskmhWM+g768RM4UitvPYiTigXYSEMljJ2vqFYVzesI1Ea5bVRv7KCF9/VtjK2Nng92wGSclh436XmMWUkZdJuojQ9QLUFK/DeMqMCRT2jUUNL9UEE3FJ1OMNo/QLaiSqchl4NBER4YAMuSaimXXYQr9KTAWi25mihNw23X6BvguKx45sB4IhTPZiNIKhUBwnBdWV1XxAWUSOB1bJmqfeob4MN8q+2OZzIinMn8hphmtAJbLGo2pYNRC1vrmzgw13eTh9rM1jf3yn6QiIRDSGjX0FCU+Xw0J8986XD9e6VsNXjYN0Cts3tSMVV6+dZxZQ+S/bWKQgGGhyNYLiu2eJRevHGkdjr3jUqsFgdE9yx31jo8yoxfLh67dQPz6qVwy9BdWqbyfJHa4rvyGYtpc5Vn+2kceth9yZKvW/LjdblrO1wIDzsjyWczyVwhzezI2sGH3VH8B/ET00ni9b42DhAAAAAASUVORK5CYII=
```

$$$ END IMAGE STRING $$$

### Logo2Base64 — Green Circle

$$$ START IMAGE STRING $$$

```
iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAK3RFWHRDcmVhdGlvbiBUaW1lAFNv IDEyIE9rdCAyMDAzIDIzOjQxOjM2ICswMTAwojoQ3QAAAAd0SU1FB9MKDBUpO7e4dGwAAAAJcEhZ cwAACvAAAArwAUKsNJgAAAAEZ0FNQQAAsY8L/GEFAAACNUlEQVR42u1UTWsTURQ9kbb5cEysiTaI iFpq1JWbSKFLcSPanQtp/oH+Af+IK5exRdy1a7vRhXRpESqWCIkRmolN2sxkPt6bGc8dAiKMdupS e+HAm8fknHvPPRngpP75yhz1wsI7ZFW31Bj76qEfqhu+H2V8hDs6CjcwiyYewf1rgfrW+fqordcu Vy/OX6tWUcjn4fg+vu3vY7vTQau718IFPKbI1rEFbr+t1KeGM5v3FxeN2WIRluPA9jyMCVepGF/7 fWxuf7RQxF2sJIucSrq88go5ey9YE/JLlQoQRb+8HBJBGOKsYWCpVjPQxyqeI59aAFGpcZW2lNm5 TUs0yUKKRJlMPHIkz4IgwBmjgLlzpXluYiW1gO17D8TzQ9eFTbi0RWkNRUJNIeleZgp41ryfK5cA jeUkrqmkS1eHN2Wh4rd0EBBCrjiNovdaziSWyQKec9lp+dn11AI6VHFapNPYMemUZ+nWI6Ev5DLN ZCIl7wXJgUm0yNPRjkRRrHEkOezaIcYUlWePAi4hQjKJZTuSx0+pBdjPxod2Gy47tESEexgTMpXE 0yfEKhWITRpmb8QxsZ4+RWU0v3R7rY7Zh0cia5J/ERDEk2gVTzAYjTEc2C0M8DKJ6vf/5Ne4AxNv lm7VjGKhEC9ZdvJzwRoHJP+827NQiO7hCd4fT0CqSZHvWJWcSxRzM9Pxsg/puWmOcCCdn2b+nyaT Hy0g9QJZDNHgaZlZX5jc7k48b+LZnz92J/Uf1A/wJ3Aw7mXNnAAAAABJRU5ErkJggg==
```

$$$ END IMAGE STRING $$$

## IMAGE TO BASE64 INFORMATION

Image To Base64 Converter - https://codebeautify.org/image-to-base64-converter

IMPORTANT - The two following image examples have been taken from the emojipedia.org website and there use in this document is for informational purposes only. Any use of these images in a business environment need to investigated by the business at its own time and expense.

### emojipedia.org — Yellow Warning Sign, 32 Pixels

$$$ START IMAGE STRING $$$

```
iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAACxEAAAsRAX9kX5EAAAUgaVRYdFhNTDpjb20uYWRvYmUueG1wAAAAAAA8P3hwYWNrZXQgYmVnaW49Iu+7vyIgaWQ9Ilc1TTBNcENlaGlIenJlU3pOVGN6a2M5ZCI/PiA8eDp4bXBtZXRhIHhtbG5zOng9ImFkb2JlOm5zOm1ldGEvIiB4OnhtcHRrPSJBZG9iZSBYTVAgQ29yZSA1LjYtYzE0MCA3OS4xNjA0NTEsIDIwMTcvMDUvMDYtMDE6MDg6MjEgICAgICAgICI+IDxyZGY6UkRGIHhtbG5zOnJkZj0iaHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyI+IDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PSIiIHhtbG5zOnhtcD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wLyIgeG1sbnM6ZGM9Imh0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvIiB4bWxuczpwaG90b3Nob3A9Imh0dHA6Ly9ucy5hZG9iZS5jb20vcGhvdG9zaG9wLzEuMC8iIHhtbG5zOnhtcE1NPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvbW0vIiB4bWxuczpzdEV2dD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIiB4bXA6Q3JlYXRvclRvb2w9IkFkb2JlIFBob3Rvc2hvcCBDQyAyMDE4IChNYWNpbnRvc2gpIiB4bXA6Q3JlYXRlRGF0ZT0iMjAxNi0wOS0yOVQxMDozNTo0NC0wNzowMCIgeG1wOk1vZGlmeURhdGU9IjIwMTgtMDctMjZUMTQ6NDQ6MTktMDc6MDAiIHhtcDpNZXRhZGF0YURhdGU9IjIwMTgtMDctMjZUMTQ6NDQ6MTktMDc6MDAiIGRjOmZvcm1hdD0iaW1hZ2UvcG5nIiBwaG90b3Nob3A6Q29sb3JNb2RlPSIzIiBwaG90b3Nob3A6SUNDUHJvZmlsZT0ic1JHQiBJRUM2MTk2Ni0yLjEiIHhtcE1NOklu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
```

$$$ END IMAGE STRING $$$

### emojipedia.org — Grey OK, 32 Pixels

$$$ START IMAGE STRING $$$

```
iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAACxEAAAsRAX9kX5EAAAUgaVRYdFhNTDpjb20uYWRvYmUueG1wAAAAAAA8P3hwYWNrZXQgYmVnaW49Iu+7vyIgaWQ9Ilc1TTBNcENlaGlIenJlU3pOVGN6a2M5ZCI/PiA8eDp4bXBtZXRhIHhtbG5zOng9ImFkb2JlOm5zOm1ldGEvIiB4OnhtcHRrPSJBZG9iZSBYTVAgQ29yZSA1LjYtYzE0MCA3OS4xNjA0NTEsIDIwMTcvMDUvMDYtMDE6MDg6MjEgICAgICAgICI+IDxyZGY6UkRGIHhtbG5zOnJkZj0iaHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyI+IDxyZGY6RGVzY3JpcHRpb24gcmRmOmFib3V0PSIiIHhtbG5zOnhtcD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wLyIgeG1sbnM6ZGM9Imh0dHA6Ly9wdXJsLm9yZy9kYy9lbGVtZW50cy8xLjEvIiB4bWxuczpwaG90b3Nob3A9Imh0dHA6Ly9ucy5hZG9iZS5jb20vcGhvdG9zaG9wLzEuMC8iIHhtbG5zOnhtcE1NPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvbW0vIiB4bWxuczpzdEV2dD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIiB4bXA6Q3JlYXRvclRvb2w9IkFkb2JlIFBob3Rvc2hvcCBDQyAyMDE4IChNYWNpbnRvc2gpIiB4bXA6Q3JlYXRlRGF0ZT0iMjAxNi0wOS0yOVQwOTo1NjoxOC0wNzowMCIgeG1wOk1vZGlmeURhdGU9IjIwMTgtMDctMjZUMTQ6MzY6MzAtMDc6MDAiIHhtcDpNZXRhZGF0YURhdGU9IjIwMTgtMDctMjZUMTQ6MzY6MzAtMDc6MDAiIGRjOmZvcm1hdD0iaW1hZ2UvcG5nIiBwaG90b3Nob3A6Q29sb3JNb2RlPSIzIiBwaG90b3Nob3A6SUNDUHJvZmlsZT0ic1JHQiBJRUM2MTk2Ni0yLjEiIHhtcE1NOklu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
```

$$$ END IMAGE STRING $$$

## REFERENCE MARK WORKFLOW STATEMENT

The following statement is using the POOL_TEILE.GEWICHT_FORM field which is in grams and converting it to kilograms (Example - 25000g to 25kg).

**SQL Server Query**

```sql
SELECT 'WEIGHT', CASE WHEN pt.gewicht_form/1000 > 25 THEN 1 ELSE 2 END AS manual_handling_prohibited,1,1,100,100 from pool_teile pt, fein_unit fu where pt.auftnr = fu.auftnr and pt.pos = fu.pos and pt.u_pos = fu.u_pos and pt.teile_nr = fu.teile_nr and fu.job < 10000 and fu.typ = 100 and fu.etikettnr = '#barcode#'
```

Explanation - If gewicht_form is greater than 25kg then use Red Circle (Logo1Base64) else use Green Circle (Logo2Base64).

> CONTINUED ON NEXT PAGE

**SQL Server Query Result**

**Reference Mark Information Example**

```sql
SELECT 'WEIGHT', CASE WHEN pt.gewicht_form/1000 > 25 THEN 1 ELSE 2 END AS manual_handling_prohibited,1,1,100,100
```

In the information in points 1 - 6, outline how to configure the values so that a specific point can be selected for the graphic to be located and information will be shown.

1. Reference text = WEIGHT
2. Layer = 1 (Column Name - manual_handling_prohibited)
3. Edge = 1
4. Corner = 1
5. Dist_Hor = 100
6. Dist_Ver = 100

## A+W PATTERN VIEWER WORKFLOW STUDIO CUSTOMISING

Opening A+W Infrastructure 6 Workflow Studio – On the Process Server open the blue A+W Shortcut > Config Tools > A+W Infrastructure 6 Workflow Studio or run the Windows Executable "C:\Program Files (x86)\A+W\Sandpiper1\InfrastructureWorkflowStudio\WorkflowStudio.exe"

IMPORTANT - This is a global change which will affect all Pattern Viewer screens unless a Workflow has been configured for each Pattern Viewer.

Next, we need to check how many Pattern Viewer Workflows are current configured by choosing Configuration > Workflow Management.

In the list should be an Extension Point that has the wording - PatternViewer as shown below.

Single PatternViewer Workflow Example

Multiple PatternViewer Workflows Example

Depending on if or how this has been configured the correct Workflow name will need to be opened in the next part described below.

To open the Pattern Viewer Default Workflow choose File > Load then the Workflow that matches the name required or Pattern Viewer Default Workflow if it is the only one listed.

Note - In this instance the Pattern Viewer TB1 Workflow has been selected as it is the workflow that will be used with the Cutting Table 1 under A+W Realtime Optimizer else it may just be Pattern Viewer Default Workflow to be selected if it is the only workflow in use.

Next, we need to add the AW.Clarity.CIM.Cutting.Facade.Activities to the Toolbox by selecting File > Add Reference from the top menu.

Then under C:\Program Files (x86)\A+W\TECHSOFT\XoptOn choose the file AW.Clarity.CIM.Cutting.Facade.dll and then click Open.

This will show a new Entry called AW.Clarity.CIM.Cutting.Facade.Activities which has the required ReferenceMark control that will be used to show a Red or Green Dot if a glass item is above a specified weight.

To add the ReferenceMark control to the screen click and drag the option Reference Mark under AW.Clarity.CIM.Cutting.Facade.Activities to the middle window and then make the following changes.

- DisplayName = WeightIndicator
- PatternIn = PatternIn
- PatternOut = PatternOut
- Statement = SELECT 'WEIGHT', CASE WHEN pt.gewicht_form/1000 > 25 THEN 1 ELSE 2 END AS manual_handling_prohibited,1,1,100,100 from pool_teile pt, fein_unit fu where pt.auftnr = fu.auftnr and pt.pos = fu.pos and pt.u_pos = fu.u_pos and pt.teile_nr = fu.teile_nr and fu.job < 10000 and fu.typ = 100 and fu.etikettnr = '#barcode#'
Relink Variables so they flow between each other as shown below.

Finally save the changes by using File > Save from the top menu.

> CONTINUED ON NEXT PAGE

## ORDER ENTRY TESTING

In the sample order below we are using 12mm Clear Float

Which contains two order items

12mm Clear Float – Width 500mm x Height 500mm = Weight 7.5kg

12mm Clear Float – Width 2000mm x Height 200mm = Weight 120kg

In this instance we are expecting the PatternViewer Stockplate of this order to show a Green Dot with the 500mm x 500mm order (item one) and a Red Dot with the 2000mm x 2000mm order (item two) with the word WEIGHT and the coloured dot at the bottom left of each cut.

## PATTERNVIEWER FINAL RESULT

In the image below we can see the Red Circle being above 25kg in weight and the Red Circle image. If the glass was below 25kg in weight then we have the Green Circle.

In the image below we can see the two coloured dots in question next to the word WEIGHT.

## CHANGING REFERENCE MARK GRAPHICS

In this document are two example graphics taken from emojipedia.org which have been converted to a Base64 String.

In both these instances the graphics have be resized from 160x160 pixels to 32x32 pixels so that they fit into the Pattern Viewer screen with minimal loss to image quality.

To change the graphic a change needs to be made under the A+W Infrastructure 6 Workflow Studio and the PatternViewer Workflow.

In the Workflow example below we have the previous WeightIndicator that was created with the Logo1Base64 field selected - Red Circle.

In this instance we need to update the Logo1Base64 and Logo2Base64 with the string required as shown in the two red boxes on the right hand side of the screen.

In this instance Logo1Base64 will be the Yellow Warning Sign and Logo2Base64 will be the Grey OK.

Finally save the changes by using File > Save from the top menu.

In the image below we are going to review how the graphic change has affected the Pattern Viewer Reference Mark display.

Below we can see the glass that is over 25kg showing the Yellow Warning Sign while the glass under 25kg is showing the Grey OK.
