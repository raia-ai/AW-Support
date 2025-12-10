---
title: "EN INST A+W Production Cockpit"
category: "installation"
product: "A+W Production Cockpit"
doc_type: "Installation"
language: "EN"
tags: ["INST", "A+W Production Cockpit"]
version: "1.0"
last_updated: "2025-12-10"
description: "A+W Production Cockpit                                Installation Guide  History     Date             Author                   Modification/remarks                                                        Version    24.08.2012       Peter Kühn               First Release                                                               1.0    11.07.2014       Marco Meiser             Revised                                                                     1.1   Content"
source_file: "EN-INST-A+W Production Cockpit.pdf"
---


# EN INST A+W Production Cockpit

                             A+W Production Cockpit
                               Installation Guide

History

   Date             Author                   Modification/remarks                                                        Version
   24.08.2012       Peter Kühn               First Release                                                               1.0
   11.07.2014       Marco Meiser             Revised                                                                     1.1


Content


   A+W Production Cockpit Installation Guide................................................. 1

   1.        Introduction .................................................................................... 2

   2.        Precondition .................................................................................... 4

   3.        Installation ...................................................................................... 6

   4.        Configuration ................................................................................ 12
   4.1.      Main Settings ....................................................................................................... 12
   4.2.      Configuration of the Speedometer ...................................................................... 13
   4.3.      Configuration of the Performance-Diagram ........................................................ 14
   4.4.      Configuration of the Pie ....................................................................................... 14
   4.5.      Configuration of the Traffic-Light......................................................................... 15

   5.        Simulation ..................................................................................... 17




19.02.2021                                 EN-INST-A+W Production Cockpit.docx                                                     1
1. Introduction

A+W Production Cockpit is a new monitor which shows the manager or the people on the
shop-floor the actual performance of their production for different machines. Different
groups of machines are displayed in separate tabs. A+W Production Cockpit uses the same
technic like the new ToolTV’s, so it is very easy to configure and to deploy on different
computer.
The first tab “Overview” gives the managers the possibility to choose some machines
explicitly to compare the productivity within a configurable timespan. Each machine is
displayed in a separate color. With a filter it is possible to pre-configure which machines the
manager can choose.
The other tab displays the performance of the production for a group of machines (cutting-
tables, IG-lines, special-machines) with different design-elements:
    a) Speedometer: displays the quantity produced in the last 60 minutes (actual
       situation)
    b) Diagram: shows the quantity produced in the last 60 minutes (trend for the last 24
       hours)
    c) Pie: displays the percentage of the different machine status within the last 24 hours
    d) Traffic-light: displays the actual machine status
To show the performance of the productivity, only the table awbar_booking is used. So it is
very easy to create some data for simulation.
Standard Configuration:
Tab “Cutting”: Table 1, 2 and 3 = Registration Point 110, 120, 150
Tab “IG Lines”: Line 1, 2 and 3 = Registration Point 1610, 1620, 1630
Tab “Special Machines”: TG1, TG2, Lamy = Registration Point 1310, 1320, 1510
The tab “Special-Machines” is just a template and can be used also for all other registration
points. It is also possible to add additional tabs for other machines. But for the standard we
wanted to keep it as simple as possible ant that it will work for the most of our customers
with a minimum change of the configuration.
The different machine status are set by a ToolTV and also by Xopton (will be available in the
Release 2012). The machine status have to be set up in the master data of ALCIM (see
chapter “precondition”). The design elements “pie” and “traffic light” use the table
bdestat_es to display the machine status.




19.02.2021                       EN-INST-A+W Production Cockpit.docx                              2
Standard Configuration:
- green = status “501-Ready”
- yellow = status “502-Off”, “503-Break”, “504-Maintenance”, “505-Setup”
- red = status “506-Failure”




19.02.2021                     EN-INST-A+W Production Cockpit.docx         3
2. Precondition

To run the A+W Production Cockpit there must be a PPS-Webservice available and some
machine status in the Alcim master data. For the standard A+W Production Cockpit you
have to set up the following master data:
Master Data > Barcoding > Status Types:




19.02.2021                    EN-INST-A+W Production Cockpit.docx                      4
Master Data > Barcoding > Status Values:




Additionally there are some Registration Points necessary, which are used in the default-
configuration:
ALCIM Master Data > Barcoding > Registration Points
Tab “Cutting”:
110 = Table 1
120 = Table 2
150 = Table 3 (Lamy)
Tab „IG Line“:
1610 = IG-Line 1
1620 = IG-Line 2
1630 = IG-Line 3
Tab „Specials“:
1310 = Furnace 1
1320 = Furnace 3
1510 = Lamy Line 1




19.02.2021                      EN-INST-A+W Production Cockpit.docx                         5
3. Installation

First you have to install the A+W Production Cockpit – Deployment on the server, where the
PPS-Webservice is running, by starting the setup.exe (actually there is no need to use the
setuplauncher, but this will be changed in the future).
If the A+W Production Cockpit – Deployment is installed, you have to open the internet-
explorer on the PC where you like to run the A+W Production Cockpit and type in the
following web-address:
\\<servername>\awfactoryinstall
If you want to run the A+W Production Cockpit on the process server (where the PPS-
Webservice is running) you can also use the address \\localhost\awfactoryinstall.
Then follow the installation-instructions…




… until you get an error message like this (its only because the designer form is not
available and not setup correctly):




Just click “OK” and import the Designer Form:




19.02.2021                      EN-INST-A+W Production Cockpit.docx                          6
19.02.2021   EN-INST-A+W Production Cockpit.docx   7
Actually there are two Designer Forms available for the different languages (DE / US). In the
future we will use the same technic as in ToolTV to change the language.
AUW_AWFactory_Cockpit_DE.DesignerForm = german-form
AUW_AWFactory_Cockpit_US.DesignerForm = english form


Now you should have the A+W Production Cockpit-shortcut on your desktop:




               Double click on it while keep the “shift” button pressed to enter the
configuration menu




19.02.2021                      EN-INST-A+W Production Cockpit.docx                             8
- use only the checkbox “Webservice”
- click on the button “Konfigurieren” to set up the correct Webservice (confirm with “OK”)
- click on “Anlegen” …




… and import the default parameter…




19.02.2021                      EN-INST-A+W Production Cockpit.docx                          9
… choose the station “AUW_01”




19.02.2021                  EN-INST-A+W Production Cockpit.docx   10
Confirm with “OK” and restart A+W Production-Cockpit




19.02.2021                    EN-INST-A+W Production Cockpit.docx   11
4. Configuration

The configuration of A+W Production Cockpit is similar to the new ToolTV’s. With
<Ctrl>+<F9> you can enter the parameter administrator.
Attention: even if you want to make changes at the standard configuration (design AUW-
Cockpit or station AUW_01), you have to create a copy with another name! During the next
setup everything which is called AUW_xxx is automatically overwritten!

4.1. Main Settings




Designer Form Name                  Name of the designer form

Ausgewählte Registrierkarte         Default tab which is shown after start of A+W
                                    Production Cockpit. 0 = first tab (overview), 1 = second
                                    tab (cutting), 2 = third tab (IG Lines)…

Starte maximiert                    A+W Production Cockpit is starting maximized (use the
                                    full screen and hide the taskbar; useful if the Cockpit is
                                    running on a big monitor inside the factory). You can
                                    toggle with <Ctrl>+<Shift>+<F11> between maximized



19.02.2021                     EN-INST-A+W Production Cockpit.docx                               12
                                    and normal mode

Tachoanzeige der BDE Buchungen Configuration of the Speedometer

Kuchendiagramm der BDE              Configuration of the Pie
Statusbuchungen

Ampelanzeige der BDE                Configuration of the Traffic light
Statusbuchungen

Buchungsanzeige                     Configuration of the Performance diagram



4.2. Configuration of the Speedometer




Action                     This is the link between this parameter and the different
                           speedometer inside the design.
                           PRODVIEW_AWBARBOOKINGGAUGE_CONTROL_1 = first
                           speedometer in tab “cutting” (table 1)
                           PRODVIEW_AWBARBOOKINGGAUGE_CONTROL_2 = second
                           speedometer in tab “cutting” (table 2)
                           …

Endwert gelber Bereich     Max-value for the yellow area

Endwert roter Bereich      Max-value for the red area

Erfassungsstellenbarcode   Barcode of the registration-point

Maximalwert                Max-value of the speedometer



19.02.2021                     EN-INST-A+W Production Cockpit.docx                     13
4.3. Configuration of the Performance-Diagram




Action                     This is the link between this parameter and the different
                           performance-diagrams inside the design.
                           PRODVIEW_AUTOUPDATE_CONTROL_1 = first performance-
                           diagram in tab “cutting” (table 1)
                           PRODVIEW_AUTOUPDATE_CONTROL_2 = second
                           performance-diagram in tab “cutting” (table 2)
                           …

Erfassungsstellenbarcode   Barcode of the registration-point

Zielbuchungen              Value for the green target-line



4.4. Configuration of the Pie




Action                     This is the link between this parameter and the different pies
                           inside the design.



19.02.2021                     EN-INST-A+W Production Cockpit.docx                          14
                             PRODVIEW_BDESTATPIE_CONTROL_1 = first pie in tab
                             “cutting” (table 1)
                             PRODVIEW_BDESTATPIE_CONTROL_2 = second pie in tab
                             “cutting” (table 2)
                             …

Erfassungsstelle             Number of the registration point

Gelber Status                Status values which should be shown in yellow

Grüner Status                Status values which should be shown in green

All other status-values which are from status type 30 are displayed in red


4.5. Configuration of the Traffic-Light




Action                       This is the link between this parameter and the different
                             traffic-lights inside the design.
                             PRODVIEW_BDESTATLIGHT_CONTROL_1 = first traffic light in
                             tab “cutting” (table 1)
                             PRODVIEW_BDESTATLIGHT_CONTROL_2 = second traffic light
                             in tab “cutting” (table 2)
                             …

Erfassungsstelle             Number of the registration point

Gelber Status                Status values which should be shown in yellow




19.02.2021                       EN-INST-A+W Production Cockpit.docx                     15
Grüner Status   Status values which should be shown in green

Schriftart      Font for the status description. If you use no font “(keine)”
                then the font will be automatically sized (but it looks not very
                professional)




19.02.2021         EN-INST-A+W Production Cockpit.docx                             16
5. Simulation

Because A+W Production-Cockpit uses only the database-tables awbar_booking and
bdestat_es it is very easy to create some data for simulation.
You can enter some data by an insert or use the attached script to create some
Informix.sql’s. All you need is:
Alcimbasic.exe  script-executable
Daten.bas  her you can enter a timeframe (from… to…) to create simulation-data
Daten.bat  batch file to run the script
The result is two sql-statements:
AUW_SIMBooking.sql = simulation data for the speedometer and performance diagram
AUW_SIMStatus.sql = simulation data for the pie and the traffic light




19.02.2021                      EN-INST-A+W Production Cockpit.docx                17

