---
description: "EN CONFIG A+W BoraIdent LaserBird"
---



# EN CONFIG A+W BoraIdent LaserBird

     Configuration


A+W Production Terminal -
BoraIdent Laserbird Interface




                                english




                          -INTERNAL-
Change history

Date       Author       Comments              Version
2024-02-21 Peter Kühn   First Draft Version   1.0
Content

1.   General                                                          4
2.   Configuration                                                    4
     2.1. A+W Business                                                4
     2.2. A+W ProductionTerminal                                      4
          2.2.1. Necessary components:                                4
          2.2.2. New Button                                           5
          2.2.3. Special Panorama                                     5
          2.2.4. XML file with parameter templates                    6
     2.3. Shapes                                                      7
     2.4. LaserBird Simulator                                         7




A+W Software GmbH            EN-CONFIG-A+W BoraIdent LaserBird.docx       3
1. General
This document is about the configuration of the connection between an A+W Production Terminal
Processing and the Hegla BoraIdent Laserbird.
The LaserBird machine is able to laser different pattern into the glass for bird protection.


This Feature is developed in DevOps Feature: 101781 / PF Ticket: [AW-143731]

2. Configuration
2.1. A+W Business
In A+W Business, the LaserBird is treated with the processing Logo:




The bird friendly pattern process is treated in A+W Business as logo processing. There must be a
predefined pattern template stored, which the user selects, and the driver fills the interface. The
size of the dots and the distance between the dots are all saved in the template. The coordinates
and where to place the template on the pane are calculated by the Hegla software.
We recommend adding a separate Logo-Type for this processing.


2.2. A+W Production Terminal
2.2.1. Necessary components:
    -   A+W Production Terminal Version 13.6.10719 or higher
    -   Special Panorama
    -   XML file with parameter templates




A+W Software GmbH              EN-CONFIG-A+W BoraIdent LaserBird.docx                                 4
2.2.2. New Button
A button with action PANORAMAUSERACTION1 should be added to the form (see example below)
to send the data to the LaserBird machine.
This button will automatically be enabled/disabled when the current sheet contains the data for
the LaserBird process or not.
Once this request will be accepted by the machine the button will be disabled until the sheet is
either produced or canceled.




2.2.3. Special Panorama
Special new panorama named “ProcessingWithLaserBird.cs”.
This has to be set for the TTV in Parameters Administrator as follows:




A+W Software GmbH             EN-CONFIG-A+W BoraIdent LaserBird.docx                               5
This panorama script must be configured. The Panorama contains option class where the
setting can be adjusted.




2.2.4. XML file with parameter templates
XML file with parameter templates e.g. LaserBirdFuntionTemplates.xml.
Path to that file has to be set in the A+W Production Terminal in Parameters Administrator's field
"File for Laser Processing Steps" (see picture above).
The existence of this setting activates the support for the LaserBird processing.
This file contains templates of parameters for the LaserBird machine e.g.




where 'Id' refers to the number chosen in the AWB.


A+W Software GmbH             EN-CONFIG-A+W BoraIdent LaserBird.docx                                 6
    2.3.        Shapes
As Hegla BoraIdent has their own shape-catalogue, there is a mapping them the A+W catalogue
(as entered in A+W Business) and the Hegla catalogue. Not all shapes are supported, as some of
them are not existing in the Hegla catalogue.

All supported shapes are documented here: Laserbird Shapes.xlsx

Shapes which have no standing edge, (e.g.circles), need a special frame around. This need to be
checked by the user at the machine, as there are no defined rules for it. As soon as a shape need
to be produced, a new dialog as for the parameter of the frame:




If the shape has a well defined standing edge, the user just need to unselect the checkbox
“produce with frame” on top of the dialog. If a frame is needed, the user need to enter the
dimensions of the frame and the offset between frame and glass.


2.4. LaserBird Simulator
Hegla LaserBird simulator 1.2.1 or higher (InterfaceTester.exe)
LaserBird machine act as the server, so you have to start the Server part of the simulator.




A+W Software GmbH              EN-CONFIG-A+W BoraIdent LaserBird.docx                               7
A+W Software GmbH   EN-CONFIG-A+W BoraIdent LaserBird.docx   8

