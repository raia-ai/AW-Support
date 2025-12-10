---
description: "EN CONFIG A+W CAD Designer (Shapes)"
---



# EN CONFIG A+W CAD Designer (Shapes)

         Configuration


A+W CAD Designer (Shapes)




                                                                     english




   A+W Software GmbH                                         - INTERNAL -
                       EN-CONFIG-A+W CAD Designer (Shapes).docx      1
Change history


        Date        Author            Remarks                     Version
        2018-09-11 Dirk Langwald      Original version            1.0




A+W Software GmbH      EN-CONFIG-A+W CAD Designer (Shapes).docx             2
Content

1.   General information                                               4
     1.1. Tools                                                        4
2.   Drawing Configurator                                              5
3.   Profile View                                                      6
4.   Table of Figures                                                  8




A+W Software GmbH           EN-CONFIG-A+W CAD Designer (Shapes).docx       3
1. General information
A+W CAD Designer Shapes is largely configured with the configuration file SN.INI. A description of
the individual switches is here:
\\jupiter\Doku_DocuWare\Shaping_Nesting\!General\Installation_Configuration\SNINI_XML_Dok
u\SNINI-Doku.xml
Other important documentation is the manual that can be reached in the application directly via
the ? menu.


1.1. Tools
In A+W CAD Designer (Shapes) there are many tools for recording and processings. Each view has
a default selection of tools. If additional tools are required in a view, they can be added via the
configuration file. For this, in the [View] section, there is an individual switch for each view: <Name
of the view>additionalTools
The tools are assigned to the parameter in a list separated by spaces:
Example:
     GEOMETRYadditionalTools = JOINSHP RoundEdge RndAll CUTCORNR
A list of the available tools and their application is in the manual.




Figure 1.1 Sample tools in the manual




A+W Software GmbH              EN-CONFIG-A+W CAD Designer (Shapes).docx                              4
2. Drawing Configurator
In order to undertake configurations on the layout of SN drawings, the "Drawing Configurator" is
recommended. It is possible to load any SN file that is displayed with the current configuration. The
tool writes changes that are made back into the configuration file. Not all possible configurations
can be edited with this tool; the missing ones must still be edited directly in the configuration file.
The tool can be found in each installation in the following directory:
C:\Program Files (x86)\A+W\Techsoft\SN\SNDrawingConfig\




Figure 2.1 Drawing configurator

               For use, it is recommended that you first make a copy of the current configuration.
               It must also be noted that if there is a different configuration for the current user, it
               is taken over into the global configuration when saving.




A+W Software GmbH                 EN-CONFIG-A+W CAD Designer (Shapes).docx                            5
3. Profile View
In SN Live views or on sketches generated from A+W CAD Designer
(Shapes), it is possible to display a profile view of the unit.
The profile view is controlled by the [Picture] section in the
configuration file. It is activated via the switch ShowProfile = 1.
The profile view is only displayed if something about the unit in the
profile can be displayed that requires special attention. There are
    -   Offsets

    -   Drillings if the SN.INI key [Picture] ShowProfileDrilling = 1
    -   Countersunk drillings if the         SN.INI   key    [Picture]
        ShowProfileCounterSinking = 1
    -   Certain surface processings are there and one of the following keys is enabled:
            o [Picture] ShowProfileSurface is set to 1 or
            o [Picture] ShowProfileCoating is set to 1 or
            o [Picture] ShowProfileStructure is set to 1 or
    -   Bevels or miters if the SN.INI key [Picture] ShowProfileMitr = 1
    -   Surface processings exist from AW Processing Catalog (FrostingSurface, CoatingSurface,
        AreaStripping, SandBlastingSurface, ColorinfSurface, EnamelingSurface, SilkingSurface,
        HandleSurface, GroovingSurface, Masking, Stamp, Logo)

Size and position of the profile:
    •   ProfileWidthInPercent = 20
    •   ProfileHeightInPercent = 20
    •   MinProfileWidthInPercent = 10
    •   MinProfileHeightInPercent = 10
    •   ProfileShowRightViewAtRightSide = 1
General appearance of the profile view:
    •   ProfileFontSize = 9
    •   ProfileFontType = ARIAL
    •   ShowProfileDirection = 1
    •   ProfileSymbolSize = 0.05
    •   ProfileSymbol = ARROW
    •   DefaultProfile= BOTH
    •   ProfileUseLabel = 0
    •   ProfileFitToPixel = 1
Size of the individual elements to one another:
    •   ProfileGlassDepth = 2


A+W Software GmbH               EN-CONFIG-A+W CAD Designer (Shapes).docx                         6
    •    ProfileFrameDepth = 3
    •    ProfileGlassAdd = 1
    •    ProfileFrameAdd =1
    •    ProfileSurfaceDepth = 1
    •    ProfileFoilDepth = 1
    •    ProfileFoilAdd = 1
Drillings:
    •    ShowProfileDrilling = 1
    •    ShowProfileCounterSinking = 1
Spacers and foils:
    •    ProfileShowSchematicSpacer = 0
    •    ShowProfileFoil = 1
    •    ProfileDoubleInnerMargin = 0
Miters
    •    ShowProfileMitr = 1
    •    ProfileMitrScale = 1
Coatings, structure and surface processings:
    •    ShowProfileCoating = 1
    •    CoatingColor = RGB(255,0,0)
    •    SoftCoatingColor = RGB(255,0,0)
    •    HardCoatingColor = RGB(255,0,0)
    •    ShowProfileStructure = 1
    •    ShowProfileSurface = 1




A+W Software GmbH               EN-CONFIG-A+W CAD Designer (Shapes).docx   7
4. Table of Figures
Figure 1.1 Sample tools in the manual ............................................................................................... 4
Figure 2.1 Drawing configurator ........................................................................................................ 5




A+W Software GmbH                       EN-CONFIG-A+W CAD Designer (Shapes).docx                                                        8

