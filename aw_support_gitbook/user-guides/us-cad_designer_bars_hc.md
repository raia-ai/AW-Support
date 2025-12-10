---
description: "US CAD Designer Bars HC"
---



# US CAD Designer Bars HC

CAD Designer (Bars)


                      Help Cards




            A+W CAD Designer
                 Help Cards                                                                             CAD Designer (Bars)




                 CAD Designer (Bars)
                 The displays in the Help Cards are based on delivery version A+W CAD Designer 2014. Individual steps
                 in the workflows may deviate, depending on the configuration.

                 Master data

                 Help Card                                   Subjects

                 • Tools                                     • You will get an overview of the tools.

                 • Catch points                              • You will get an overview of the catch points.

                 • Create muntins                            • Create a muntin article.

                 • Protect master data                       • Protecting your master data via a password.


                 Muntins

                 Help Card                                   Subjects

                 • Lite properties                           • Defining the lite properties.

                 • Position simple muntin pattern            • Position two vertical and two horizontal muntins.

                 • Place muntins by means of values          • Positioning muntins by means of fixed values.

                 • Positioning a shape with muntins          • Positioning a shape with muntins.

                 • Creating a free muntin pattern            • Creating a free muntin pattern.


                 Special patterns

                 Help Card                                   Subjects

                 • Create a house front                      • Position a house front.

                 • Load macro                                • Load existing macro.

                 • Change and save a macro                   • Changing and saving an existing macro.

                 • Create an individual macro                • Create an individual macro.
2.00 / 10-2014




                 A+W CAD Designer                                                                                        2
A+W CAD Designer


Master data                                                           Tools                                                               Bar 01-001


Objective of this activity
You will get an overview of the tools.


Requirements


Additional information




Overview                                                                 Muntin will be extended up to a selected object.
      Select an element.                                                 Divides all muntins.
      Creates a straight muntin between two catch points.                Connects all muntins.
      Creates a horizontal muntin between two catch points.              Sets or deletes a muntinin a clear field.
      Creates a vertical muntin between two catch points.                Creates a new lite.
      Creates a muntin between two catch points at a defined angle.      Creates a muntin pattern in the lite from a macro.
      Creates a curved muntin between three catch points.                Opens the dialog for entering vertical and horizontal muntins.
      Creates a circular muntin between two catch points.                Shows the corresponding quantities in the input area.
      Creates a sun in a clear field.                                    Changes the YT cutting.
      Creates a crescent.

      Creates an arc in a clear field.

      The uninterrupted direction will be changed for a 90° cross.

                                                                                                                                             2.00 / 10-2014
A+W CAD Designer


Master data                                                                                Catch points                                                               Bar 01-002


Objective of this activity
You will get an overview of the catch points.


Requirements


Additional information




Overview                                                                                      Creates catch points in all feasible centers of circles (two points).
      Deletes a catch point.                                                                  Creates catch points with a parallel shift from a straight line.
      Deletes all catch points.                                                               Creates a catch point along an arc, in definable distance.
      Enter the number of intervals for an object.                                            Creates catch points in the center of a circle (three points).
      Creates catch points wherever two objects cross.                                        Creates catch points in an adjustable angle from the reference point.
      Creates a catch point in relation to any point.                                         Creates a catch point on a straight line in a defined distance from the starting
                                                                                              point.
      Creates catch point on muntins, spacer bars, or the lite edge.

      Creates four catch points on the corners of a rectangle defined by double-click of
      the mouse.

      Creates catch points at all intersections with other muntins.

      Creates catch points on a straight line.

      Creates a catch point on an arc in definable distance.

                                                                                                                                                                          2.00 / 10-2014
A+W CAD Designer


Master data                                                                               Create muntins                                                        Bar 01-003


Objective of this activity
Create a muntin article.


Requirements



Additional information




Workflow                                                                                  10 Enable the Double Cutting checkbox to automatically double the quantity to be cut
                                                                                             for the muntin type in question (triple IG)
1 Open the Master Data Editor dialog [Master Data > Master Data Editor].
                                                                                          11 Enable the L fields with reduction checkbox to exclude the edge stoppers of the
2 Click on [Add]. Enter the required article number.                                         muntin from dimensioning.
3 Enter the muntin width in the Width field.                                           12 If there are several muntin production lines, you can enter the corresponding num-
4 Enter the corresponding value in the Milling depth field (adjustable stopper against    ber in the Line Number field.
  which the previously cut-off end of the muntin is positioned).                       13 Use the Color Code field to assign a RAL color to the muntin.
5 Enter the corresponding value in the Trim field (thickness of the plastic plug).        14 If the muntin is a standard muntin, click on the [Start] button.
6 If desired, activate the Special Cross checkbox (not a continuous muntin – plug-in
  connections) and enter the corresponding value in the Cross Width field.
7 Enter the length of the muntin in the Muntin length field.
8 Enter a value in the Add T-Cut field if the muntin is cut at a right angle to another
  bar.
9 The radio buttons in the Continuous section are used to define continuous muntins
  which are transferred externally to A+W CAD Designer by means of transfer files.
                                                                                                                                                                   2.00 / 10-2014
A+W CAD Designer


Master data                                                                            Protect master data   Bar 01-004


Objective of this activity
Protecting your master data via a password.


Requirements
Master data has been created


Additional information




Workflow
1 Open the Master Data Editor dialog [Master Data > Master Data Editor].
2 Enable the Password protection checkbox in the Options section.
3 Click on [OK]. An inquiry is displayed as to whether the master data should be
  saved.
4 Click on [Yes]. The Password? dialog opens.
5 Enter the desired password in the Password field.
6 Repeat the entered password in the Confirm password field.
7 Click on [OK].
8 The next time you open the Master Data Editor you will be asked to enter the pass-
  word.




                                                                                                                2.00 / 10-2014
A+W CAD Designer


Muntins                                                                                    Lite properties   Bar 02-001


Objective of this activity
Defining the lite properties.


Requirements
•   Master data must be available.


Additional information




Workflow
1 Click on the icon button [New lite]. The Shape Input dialog opens.
2 Select the shape no. and enter the dimensions.
3 Subsequently, the Lite Properties dialog opens. Use the fields X- and Y-Position to
  define the position on your work space. The Alignment field is used to turn the lite.
4 The fields in the lower section of the dialog are used to enter the order data. Com-
  plete them accordingly.
5 In the Extra area you can enter other details (e.g. delivery date, spacer, gas code,
  etc.). If the program is linked with A+W Production, these fields will be automatical-
  ly filled during transfer.
6 Press [OK] to close the dialog. The lite will be positioned now.




                                                                                                                2.00 / 10-2014
A+W CAD Designer


Muntins                                                                                 Position simple muntin pattern   Bar 02-002


Objective of this activity
Position two vertical and two horizontal muntins.


Requirements
•   Master data must be available.
•   Lite must be positioned.


Additional information




Workflow
1 Click on the icon button [New vertical/horizontal pattern]. The Vertical/horizontal
  pattern dialog opens.
2 Enter the number of muntins.
3 Enable the Identical clear fields option in the Horizontal split section.
4 In the Vertical split section, enable the Identical clear fields option.
5 Check the Vertical option in the Continuous muntins section.
6 Press [OK] to close the dialog. The muntins are positioned.




                                                                                                                            2.00 / 10-2014
A+W CAD Designer


Muntins                                                                                   Place muntins by means of values                                Bar 02-003


Objective of this activity
Positioning muntins by means of fixed values.


Requirements
•   Master data must be available.
•   Lite must be positioned.


Additional information




Workflow                                                                                  6 Press [OK] to close the dialog. The muntins are positioned.
1 Click on the icon button [New vertical/horizontal pattern] and then on the lite. The
  Vertical/horizontal pattern dialog opens.
2 Enter 2 in both the Number of horizontal and Number of vertical field. Enable the
  Customized option in the Horizontal split and Vertical split sections. Click on [OK].
  The Customized VH pattern dialog opens.
3 Enable the Lite edge option in the Horizontal muntin section. Enable the radio but-
  ton Horizont. Click on [Add]. The Enter distances between muntins dialog opens.
  Enter 150 mm. Click [OK]. The dialog closes. Repeat these steps with 300 mm.
  Enable the radio button From bottom.
4 Enable the Lite edge option in the Vertical muntin section. Enable the radio button
  Vertical. Click on [Add]. The dialog Enter distances between munitns opens. Enter
  200 mm. Click on [OK]. The dialog closes. Repeat these steps with 400 mm. En-
  able the radio button From the left. Press on [OK] to close the dialog.
5 Check the Vertical option in the Continuous muntins section in the Vertical/horizon-
  tal pattern dialog.
                                                                                                                                                             2.00 / 10-2014
A+W CAD Designer


Muntins                                                                                      Positioning a shape with muntins   Bar 02-004


Objective of this activity
Positioning a shape with muntins.


Requirements
•   Master data must be available.


Additional information




Workflow
1 Click on the icon button [New lite] and then on the work space. The Shape Input
  dialog opens.
2 Open the Shape number combo box and select shape number 065. The shape is
  800 high and has a width of 600. Click on [OK]. The shape is positioned and the
  Lite Properties dialog opens.
3 Complete the fields accordingly and click on [OK].
4 Click on the icon button [New vertical/horizontal pattern] and subsequently the
  shape. The Vertical/horizontal pattern dialog opens.
5 Enter 2 in the Number of horizontal field and 1 in the Number of vertical field.
6 Enable the Identical clear fields option in the Horizontal split and Vertical split sec-
  tions.
7 Check the Vertical option in the Continuous muntin section. Click on [OK].
8 The muntins are positioned.

                                                                                                                                   2.00 / 10-2014
A+W CAD Designer


Muntins                                                                                    Creating a free muntin pattern                                 Bar 02-005


Objective of this activity
Creating a free muntin pattern.


Requirements
•   Master data must be available.


Additional information




Workflow                                                                              6 Enable the Sun tool. Click on the field in which the sun shall be inserted. The Sun
                                                                                        and stars dialog opens. Enable the radio button Star and check the Joint cutting
1 You can find steps 1 through 3 in exercise Creating a free muntin pattern (dimen-     checkbox. The radial pattern has identical angles and three rays.
  sions: Width=500, height=600).
                                                                                      7 Click on [OK]. The dialog closes, and the radial pattern is added.
2 Click on the icon button [New vertical/horizontal pattern] and then the shape. The
  Vertical/horizontal pattern dialog opens. Enter 3 in the Number of horizontal field
  and 2 in the Number of vertical field.
3 Enable the radio button Customized in the Horizontal split section. Check the Hor-
  izontal checkbox in the Continuous muntins section. In the Vertical split section, en-
  able the radio button Identical clear fields. Click [OK]. The Customized VH pattern
  dialog opens. Check the Add up checkbox in the Horizontal muntins section. Enter
  three muntins with distances of 120. Confirm by clicking on [OK].
4 Set three catch points each on the top parts of the vertical muntins and connect the
  catch points in the middle with a horizontal muntin.
5 Delete the catch points and enable the Set/delete muntin tool. On the left hand side,
  mark the vertical muntin where it should be cut. The upper section of the vertical
  muntin is deleted. Repeat this process for the right hand side.
                                                                                                                                                               2.00 / 10-2014
A+W CAD Designer


Special patterns                                                                        Create a house front   Bar 03-001


Objective of this activity
Position a house front.


Requirements
•   Master data must be available.


Additional information




Workflow
1 In the menu, select Macro > Special pattern > House front. This will open the House
  front...dialog.
2 Enter the following lite dimensions:
  Lite A and D: Width=800, Height=600
  Lite B: Width=400, Height=300
  Lite C: Width=200, Height=100
  The distances that are calculated by the program are adopted.

    Confirm by clicking on [OK]. The Lite Properties dialog opens. Make the corre-
    sponding entries.
3 Click on [OK]. The dialog closes and the house front is positioned.




                                                                                                                  2.00 / 10-2014
A+W CAD Designer


Special patterns                                                                      Load macro                                                  Bar 03-002


Objective of this activity
Load existing macro.


Requirements
•   Master data must be available.


Additional information




Workflow                                                                              9 Exit the Macro parameters dialog using the [OK] button.
1 Position shape no. 0 with a width=800 and a height=600.                             10 The macro will be positioned now.
2 Complete the Lite Properties dialog. Mark the Consignment text entry in the Extra
  section and enter Housing Area II.
3 Click on the icon button [New macro]. Position the cursor on the shape and press
  the left mouse key. This opens the Select macro dialog.
4 Select macro York3H1S and click on [OK].
5 The Macro parameters dialog opens. Mark Width of diamond shape and confirm
  using the [Amend...] button.
6 The Relative distance dialog opens. Enter 125 mm for the width of the diamond
  shapes. Close the dialog using the [OK] button.
7 Mark Height of diamond shape and click on the [Amend...] button.
8 The Relative distance dialog opens. Enter 150 mm for the height of the diamond
  shapes. Close the dialog using the [OK] button.

                                                                                                                                                     2.00 / 10-2014
A+W CAD Designer


Special patterns                                                                    Change and save a macro   Bar 03-003


Objective of this activity
Changing and saving an existing macro.


Requirements
•   Master data must be available.


Additional information




Workflow
1 Position macro York3H1S as described in exercise Load macro.
2 Enable the Select element tool.
3 Mark the top muntin of the central diamond shape. Press <Del> on your keyboard.
4 Repeat the process for the lower muntin of the central diamond shape.
5 Open the File menu. Select the Save as menu item.
6 Enter York3H1S-WAII in the File name field and use [OK] to close the dialog.




                                                                                                                 2.00 / 10-2014
A+W CAD Designer


Special patterns                                                                                Create an individual macro                                              Bar 03-004


Objective of this activity
Create an individual macro.


Requirements
•   Master data must be available.


Additional information




Workflow                                                                                           on the left edge of the lite. The Relative distance dialog box reopens. Relative DX
                                                                                                   is at 0 again. For Relative DY, click on Same as other entry and subsequently on
1 Open the New Macro menu item in the Macro menu. A lite is displayed on the                       [OK]. The List of existing entries dialog box opens. Select the Distance lite edge to
  screen. The dimensions of the lite are 3 m x 3 m and it has 8 catch points (4 each               muntin center entry. Confirm your selection using [OK].
  on the interior frame and 4 each on the outside edge of the lite).
                                                                                                5 Place the catch point that is still missing on the right lite edge.
2 Now position one catch point (interval = 2) on the top and the bottom frame each.
                                                                                        6          Subsequently, insert the muntins. First of all, enable the muntin button, click on the
3 In the next step, you will define the distance of the horizontal muntin from the edge            left and then on the right catch point of the lite edge. Now enter the missing vertical
  of the lite. Click on the Relative button and subsequently on the catch point on the
                                                                                                   muntin.
  top edge of the lite. The dialog box Relative distance opens. Enter a distance of 0
  under Relative DX since the new catch point on the x-axis does not change. If you 7              Select Save in the Macro menu. The Save macro dialog opens. Enter the name of
  confirm the entries now, you will be prompted to enter Relative DY. Enter the dis-               the T Muntin.
  tance of 300 mm here. Since the horizontal muntin is located below the catch point 8             Confirm by clicking on [OK]. The macro will be saved.
  (on the top edge of the lite), you must enter -300. This value can be edited and will
  be requested when the macro is reloaded. Please enter explanatory text; in our ex-
  ample, "Distance from edge of lite to center of muntin."
4 In the next step, you will set the catch points on the right and left lite edge. Start with
  the left lite edge. Click on Relative again and subsequently on the top catch point

                                                                                                                                                                             2.00 / 10-2014

