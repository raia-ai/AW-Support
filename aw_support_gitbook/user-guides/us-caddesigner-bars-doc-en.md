---
title: "US-CAD_Designer_Bars_HC"
source: "US-CAD_Designer_Bars_HC.pdf"
tags: ["A+W", "CAD Designer", "Bars", "Muntins", "Software Guide", "Help Cards", "Technical Documentation", "Glass Design", "Window Design", "Macros"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A collection of help cards for the A+W CAD Designer (Bars) software, version 2014. This guide provides step-by-step instructions for managing master data, creating and positioning muntins, and working with special patterns and macros."
long_description: "This document serves as a practical user guide, formatted as a series of 'Help Cards,' for the A+W CAD Designer (Bars) software, based on the 2014 version. It is designed for users involved in the design and manufacturing of glass, windows, and doors. The guide is structured into three main sections: Master Data, Muntins, and Special Patterns. The 'Master Data' section covers fundamental setup tasks, including an overview of design tools, the use of catch points, the creation of muntin articles in the database, and how to password-protect master data. The 'Muntins' section provides detailed workflows for defining lite properties and positioning muntins, from simple grid patterns to placing them with precise values and applying them to complex shapes. The 'Special Patterns' section focuses on advanced features, explaining how to create a multi-lite 'house front,' load and modify existing macros, and build a custom macro from scratch. Each help card clearly states its objective and provides a numbered workflow, making it a comprehensive and accessible quick-reference tool for designers and technicians."
---

# A+W CAD Designer (Bars) Help Cards

**A+W - Software for Glass, Windows and Doors**

---

---
## Introduction

The displays in the Help Cards are based on delivery version **A+W CAD Designer 2014**. Individual steps in the workflows may deviate, depending on the configuration.

### Master data

| Help Card | Subjects |
| :--- | :--- |
| **Tools** | You will get an overview of the tools. |
| **Catch points** | You will get an overview of the catch points. |
| **Create muntins** | Create a muntin article. |
| **Protect master data** | Protecting your master data via a password. |

### Muntins

| Help Card | Subjects |
| :--- | :--- |
| **Lite properties** | Defining the lite properties. |
| **Position simple muntin pattern** | Position two vertical and two horizontal muntins. |
| **Place muntins by means of values** | Positioning muntins by means of fixed values. |
| **Positioning a shape with muntins** | Positioning a shape with muntins. |
| **Creating a free muntin pattern** | Creating a free muntin pattern. |

### Special patterns

| Help Card | Subjects |
| :--- | :--- |
| **Create a house front** | Position a house front. |
| **Load macro** | Load existing macro. |
| **Change and save a macro** | Changing and saving an existing macro. |
| **Create an individual macro** | Create an individual macro. |

---

## Master data

### Tools (Bar 01-001)

**Objective of this activity**
> You will get an overview of the tools.

**Requirements**
*   None

**Additional Information**
*   None

**Overview**

| Icon/Action | Description |
| :--- | :--- |
| **Select an element** | Selects an element. |
| **Straight muntin** | Creates a straight muntin between two catch points. |
| **Horizontal muntin** | Creates a horizontal muntin between two catch points. |
| **Vertical muntin** | Creates a vertical muntin between two catch points. |
| **Angled muntin** | Creates a muntin between two catch points at a defined angle. |
| **Curved muntin** | Creates a curved muntin between three catch points. |
| **Circular muntin** | Creates a circular muntin between two catch points. |
| **Sun** | Creates a sun in a clear field. |
| **Crescent** | Creates a crescent. |
| **Arc** | Creates an arc in a clear field. |
| **Change direction** | The uninterrupted direction will be changed for a 90° cross. |
| **Extend muntin** | Muntin will be extended up to a selected object. |
| **Divide muntins** | Divides all muntins. |
| **Connect muntins** | Connects all muntins. |
| **Set/delete muntin** | Sets or deletes a muntin in a clear field. |
| **New lite** | Creates a new lite. |
| **Macro pattern** | Creates a muntin pattern in the lite from a macro. |
| **V/H muntin dialog** | Opens the dialog for entering vertical and horizontal muntins. |
| **Show quantities** | Shows the corresponding quantities in the input area. |
| **Change YT cutting** | Changes the YT cutting. |

---

### Catch points (Bar 01-002)

**Objective of this activity**
> You will get an overview of the catch points.

**Requirements**
*   None

**Additional Information**
*   None

**Overview**

| Icon/Action | Description |
| :--- | :--- |
| **Delete catch point** | Deletes a catch point. |
| **Delete all catch points** | Deletes all catch points. |
| **Enter intervals** | Enter the number of intervals for an object. |
| **Crossing points** | Creates catch points wherever two objects cross. |
| **Relative point** | Creates a catch point in relation to any point. |
| **Point on object** | Creates catch point on muntins, spacer bars, or the lite edge. |
| **Rectangle corners** | Creates four catch points on the corners of a rectangle defined by double-click of the mouse. |
| **Intersection points** | Creates catch points at all intersections with other muntins. |
| **Points on line** | Creates catch points on a straight line. |
| **Point on arc** | Creates a catch point on an arc in definable distance. |
| **Circle centers** | Creates catch points in all feasible centers of circles (two points). |
| **Parallel shift** | Creates catch points with a parallel shift from a straight line. |
| **Point along arc** | Creates a catch point along an arc, in definable distance. |
| **Circle center (3 points)** | Creates catch points in the center of a circle (three points). |
| **Adjustable angle** | Creates catch points in an adjustable angle from the reference point. |
| **Distance from start** | Creates a catch point on a straight line in a defined distance from the starting point. |

---

### Create muntins (Bar 01-003)

**Objective of this activity**
> Create a muntin article.

**Requirements**
*   None

**Additional Information**
*   The following workflow describes creating a muntin article using the Master Data Editor dialog.

**Workflow**
1.  Open the **Master Data Editor** dialog via the menu: `Master Data > Master Data Editor`.
2.  Click on **[Add]**. Enter the required article number.
3.  Enter the muntin width in the **Width** field.
4.  Enter the corresponding value in the **Milling depth** field (adjustable stopper against which the previously cut-off end of the muntin is positioned).
5.  Enter the corresponding value in the **Trim** field (thickness of the plastic plug).
6.  If desired, activate the **Special Cross** checkbox (for non-continuous muntin plug-in connections) and enter the corresponding value in the **Cross Width** field.
7.  Enter the length of the muntin in the **Stocklength** field.
8.  Enter a value in the **Add T-Cut** field if the muntin is cut at a right angle to another bar.
9.  The radio buttons in the **Continuous** section are used to define continuous muntins which are transferred externally to A+W CAD Designer by means of transfer files.
10. Enable the **Double Cutting** checkbox to automatically double the quantity to be cut for the muntin type in question (e.g., for triple IG).
11. Enable the **L fields with reduction** checkbox to exclude the edge stoppers of the muntin from dimensioning.
12. If there are several muntin production lines, you can enter the corresponding number in the **Line Number** field.
13. Use the **Color Code** field to assign a RAL color to the muntin.
14. If the muntin is a standard muntin, click on the **[Start]** button.

---

### Protect master data (Bar 01-004)

**Objective of this activity**
> Protecting your master data via a password.

**Requirements**
*   Master data has been created.

**Additional Information**
*   None

**Workflow**
1.  Open the **Master Data Editor** dialog via the menu: `Master Data > Master Data Editor`.
2.  Enable the **Password protection** checkbox in the **Options** section.
3.  Click on **[OK]**. An inquiry is displayed as to whether the master data should be saved.
4.  Click on **[Yes]**. The `Password?` dialog opens.
5.  Enter the desired password in the **Password** field.
6.  Repeat the entered password in the **Confirm password** field.
7.  Click on **[OK]**.
8.  The next time you open the **Master Data Editor**, you will be asked to enter the password.

---

## Muntins

### Lite properties (Bar 02-001)

**Objective of this activity**
> Defining the lite properties.

**Requirements**
*   Master data must be available.

**Additional Information**
*   None

**Workflow**
1.  Click on the icon button **[New lite]**. The **Shape Input** dialog opens.
2.  Select the shape number and enter the dimensions.
3.  Subsequently, the **Lite Properties** dialog opens. Use the fields **X-** and **Y-Position** to define the position on your work space. The **Alignment** field is used to turn the lite.
4.  The fields in the lower section of the dialog are used to enter the order data. Complete them accordingly.
5.  In the **Extra** area, you can enter other details (e.g., delivery date, spacer, gas code, etc.). If the program is linked with A+W Production, these fields will be automatically filled during transfer.
6.  Press **[OK]** to close the dialog. The lite will be positioned now.

---

### Position simple muntin pattern (Bar 02-002)

**Objective of this activity**
> Position two vertical and two horizontal muntins.

**Requirements**
*   Master data must be available.
*   Lite must be positioned.

**Additional Information**
*   None

**Workflow**
1.  Click on the icon button **[New vertical/horizontal pattern]**. The **Vertical/horizontal pattern** dialog opens.
2.  Enter the number of muntins.
3.  Enable the **Identical clear fields** option in the **Horizontal split** section.
4.  In the **Vertical split** section, enable the **Identical clear fields** option.
5.  Check the **Vertical** option in the **Continuous muntins** section.
6.  Press **[OK]** to close the dialog. The muntins are positioned.

---

### Place muntins by means of values (Bar 02-003)

**Objective of this activity**
> Positioning muntins by means of fixed values.

**Requirements**
*   Master data must be available.
*   Lite must be positioned.

**Additional Information**
*   None

**Workflow**
1.  Click on the icon button **[New vertical/horizontal pattern]** and then on the lite. The **Vertical/horizontal pattern** dialog opens.
2.  Enter `2` in both the **Number of horizontal** and **Number of vertical** fields. Enable the **Customized** option in the Horizontal split and Vertical split sections. Click on **[OK]**. The **Customized VH pattern** dialog opens.
3.  Enable the **Lite edge** option in the **Horizontal muntin** section. Enable the radio button **Horizont**. Click on **[Add]**. The **Enter distances between muntins** dialog opens. Enter `150 mm`. Click **[OK]**. The dialog closes. Repeat these steps with `300 mm`. Enable the radio button **From bottom**.
4.  Enable the **Lite edge** option in the **Vertical muntin** section. Enable the radio button **Vertical**. Click on **[Add]**. The dialog **Enter distances between muntins** opens. Enter `200 mm`. Click on **[OK]**. The dialog closes. Repeat these steps with `400 mm`. Enable the radio button **From the left**. Press on **[OK]** to close the dialog.
5.  Check the **Vertical** option in the **Continuous muntins** section in the **Vertical/horizontal pattern** dialog.
6.  Press **[OK]** to close the dialog. The muntins are positioned.

---

### Positioning a shape with muntins (Bar 02-004)

**Objective of this activity**
> Positioning a shape with muntins.

**Requirements**
*   Master data must be available.

**Additional Information**
*   This workflow applies a muntin grid to an arched shape.

**Workflow**
1.  Click on the icon button **[New lite]** and then on the work space. The **Shape Input** dialog opens.
2.  Open the **Shape number** combo box and select shape number **065**. The shape is 800 high and has a width of 600. Click on **[OK]**. The shape is positioned and the **Lite Properties** dialog opens.
3.  Complete the fields accordingly and click on **[OK]**.
4.  Click on the icon button **[New vertical/horizontal pattern]** and subsequently the shape. The **Vertical/horizontal pattern** dialog opens.
5.  Enter `2` in the **Number of horizontal** field and `1` in the **Number of vertical** field.
6.  Enable the **Identical clear fields** option in the **Horizontal split** and **Vertical split** sections.
7.  Check the **Vertical** option in the **Continuous muntin** section. Click on **[OK]**.
8.  The muntins are positioned.

---

### Creating a free muntin pattern (Bar 02-005)

**Objective of this activity**
> Creating a free muntin pattern.

**Requirements**
*   Master data must be available.

**Additional Information**
*   This workflow describes creating a custom pattern with a radial "star" element.

**Workflow**
1.  Follow steps 1 through 3 from the "Positioning a shape with muntins" exercise (Bar 02-004), but use dimensions: Width=500, Height=600.
2.  Click on the icon button **[New vertical/horizontal pattern]** and then the shape. The **Vertical/horizontal pattern** dialog opens. Enter `3` in the **Number of horizontal** field and `2` in the **Number of vertical** field.
3.  Enable the radio button **Customized** in the **Horizontal split** section. Check the **Horizontal** checkbox in the **Continuous muntins** section. In the **Vertical split** section, enable the radio button **Identical clear fields**. Click **[OK]**. The **Customized VH pattern** dialog opens. Check the **Add up** checkbox in the **Horizontal muntins** section. Enter three muntins with distances of `120`. Confirm by clicking on **[OK]**.
4.  Set three catch points each on the top parts of the vertical muntins and connect the catch points in the middle with a horizontal muntin.
5.  Delete the catch points and enable the **Set/delete muntin** tool. On the left hand side, mark the vertical muntin where it should be cut. The upper section of the vertical muntin is deleted. Repeat this process for the right hand side.
6.  Enable the **Sun** tool. Click on the field in which the sun shall be inserted. The **Sun and stars** dialog opens. Enable the radio button **Star** and check the **Joint cutting** checkbox. The radial pattern has identical angles and three rays.
7.  Click on **[OK]**. The dialog closes, and the radial pattern is added.

---

## Special patterns

### Create a house front (Bar 03-001)

**Objective of this activity**
> Position a house front.

**Requirements**
*   Master data must be available.

**Additional Information**
*   This feature creates a pattern consisting of multiple, separate lites.

**Workflow**
1.  In the menu, select `Macro > Special pattern > House front`. This will open the **House front...** dialog.
2.  Enter the following lite dimensions:
    *   **Lite A and D:** Width=800, Height=600
    *   **Lite B:** Width=400, Height=300
    *   **Lite C:** Width=200, Height=100
    *   The distances that are calculated by the program are adopted.
3.  Confirm by clicking on **[OK]**. The **Lite Properties** dialog opens. Make the corresponding entries.
4.  Click on **[OK]**. The dialog closes and the house front is positioned.

---

### Load macro (Bar 03-002)

**Objective of this activity**
> Load existing macro.

**Requirements**
*   Master data must be available.

**Additional Information**
*   None

**Workflow**
1.  Position shape no. 0 with a width=800 and a height=600.
2.  Complete the **Lite Properties** dialog. Mark the **Consignment text** entry in the **Extra** section and enter `Housing Area II`.
3.  Click on the icon button **[New macro]**. Position the cursor on the shape and press the left mouse key. This opens the **Select macro** dialog.
4.  Select macro `York3H1S` and click on **[OK]**.
5.  The **Macro parameters** dialog opens. Mark **Width of diamond shape** and confirm using the **[Amend...]** button.
6.  The **Relative distance** dialog opens. Enter `125 mm` for the width of the diamond shapes. Close the dialog using the **[OK]** button.
7.  Mark **Height of diamond shape** and click on the **[Amend...]** button.
8.  The **Relative distance** dialog opens. Enter `150 mm` for the height of the diamond shapes. Close the dialog using the **[OK]** button.
9.  Exit the **Macro parameters** dialog using the **[OK]** button.
10. The macro will be positioned now.

---

### Change and save a macro (Bar 03-003)

**Objective of this activity**
> Changing and saving an existing macro.

**Requirements**
*   Master data must be available.

**Additional Information**
*   None

**Workflow**
1.  Position macro `York3H1S` as described in the exercise **Load macro**.
2.  Enable the **Select element** tool.
3.  Mark the top muntin of the central diamond shape. Press `<Del>` on your keyboard.
4.  Repeat the process for the lower muntin of the central diamond shape.
5.  Open the **File** menu. Select the **Save as** menu item.
6.  Enter `York3H1S-WAII` in the **File name** field and use **[OK]** to close the dialog.

---

### Create an individual macro (Bar 03-004)

**Objective of this activity**
> Create an individual macro.

**Requirements**
*   Master data must be available.

**Additional Information**
*   None

**Workflow**
1.  Open the **New Macro** menu item in the **Macro** menu. A lite is displayed on the screen. The dimensions of the lite are 3 m x 3 m and it has 8 catch points (4 each on the interior frame and 4 each on the outside edge of the lite).
2.  Now position one catch point (interval = 2) on the top and the bottom frame each.
3.  In the next step, you will define the distance of the horizontal muntin from the edge of the lite. Click on the **Relative** button and subsequently on the catch point on the top edge of the lite. The dialog box **Relative distance** opens. Enter a distance of `0` under **Relative DX** since the new catch point on the x-axis does not change. If you confirm the entries now, you will be prompted to enter **Relative DY**. Enter the distance of `300 mm` here. Since the horizontal muntin is located below the catch point (on the top edge of the lite), you must enter `-300`. This value can be edited and will be requested when the macro is reloaded. Please enter explanatory text; in our example, "Distance from edge of lite to center of muntin."
4.  In the next step, you will set the catch points on the right and left lite edge. Start with the left lite edge. Click on **Relative** again and subsequently on the top catch point on the left edge of the lite. The **Relative distance** dialog box reopens. **Relative DX** is at `0` again. For **Relative DY**, click on **Same as other entry** and subsequently on **[OK]**. The **List of existing entries** dialog box opens. Select the **Distance lite edge to muntin center** entry. Confirm your selection using **[OK]**.
5.  Place the catch point that is still missing on the right lite edge.
6.  Subsequently, insert the muntins. First of all, enable the muntin button, click on the left and then on the right catch point of the lite edge. Now enter the missing vertical muntin.
7.  Select **Save** in the **Macro** menu. The **Save macro** dialog opens. Enter the name of the **T Muntin**.
8.  Confirm by clicking on **[OK]**. The macro will be saved.
