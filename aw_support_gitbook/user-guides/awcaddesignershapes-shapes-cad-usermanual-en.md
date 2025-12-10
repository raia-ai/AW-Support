---
title: "EN-UM-AWCADDesignerShapes_4"
source: "EN-UM-AWCADDesignerShapes_4.pdf"
tags: ["A+W CAD Designer", "Shapes", "Software Reference", "CAD", "CNC", "Technical Manual", "File Handling", "Key Combinations", "User Interface", "Software Operation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a detailed software reference manual for the A+W CAD Designer (Shapes) application. It covers software operation, user interface elements, file handling procedures, and various editing and transformation functions."
long_description: "This comprehensive user manual provides an in-depth software reference for the A+W CAD Designer (Shapes) program. The document begins with an overview of basic software operation, including how to start and close the program, and defines key software terms and user interface components like buttons, hotkeys, combo boxes, and menu bars. It features a detailed list of key combinations for quick access to commands. The manual extensively covers file management under 'Handling of Files,' detailing procedures for creating, opening, inserting, saving, importing, and exporting various file formats such as SN, DXF, IGES, and CAMXML. It also explains how to manage global and local shape data, set passwords, and use the print and preview functions. Further sections describe the 'Temporary Stacker' for editing operations like undo, redo, copy, paste, and shape correction. The manual outlines how to create products, apply technology-related processing (e.g., cutting, grinding), control machinery, work with BOMs, and transform contours. Finally, it details the different 'Views' and 'Tools' available to the user, providing a complete guide to operating the A+W CAD Designer software effectively."
---

# Software Reference

---
## A+W CAD Designer (Shapes) Overview

### Table of Contents
- Views: A-196
- Tool bar: A-199
- Tools: A-199
- Select edge: A-200
- Input window: A-201
- Text format: A-202
- Lines and fillings: A-202
- Status bar: A-202
- BOM Info: A-203
- Window: A-204
- How to Use the Help Function: A-205
- About A+W CAD Designer (Shapes): A-206

---

## Operation of A+W CAD Designer (Shapes)

The program is started either via a desktop shortcut which you can define yourself, or by means of the corresponding entry in menu Start > Programs (in Windows).

We are now going to explain the terms used in the manuals, and how to terminate the program.
- Software Terms
- Closing the program

---

## Software Terms

This section deals with the general operation of menus and dialogs.

Below you will find information on:
- Buttons
- Hot key
- Radio button
- Combo box
- Checkbox
- Tab
- Menu bar/menu item
- Table/column header
- Key combinations

### Buttons

**Fig. A-132:** Buttons

### Hot key

**Fig. A-133:** Hot key

Apart from clicking on a function, most functions can be released by certain key combinations. One letter will be underlined on the buttons or menu bars. Press `<Alt>` and the underlined key at the same time, and A+W CAD Designer (Shapes) will perform this function.

### Radio button

**Fig. A-134:** Radio button

From a window with radio buttons you can always select one radio button at a time! In the example above, the radio button Complete has been selected. Clicking e.g. on the radio button Scale will automatically deselect the radio button Vertical.

### Combo box

**Fig. A-135:** Combo box

Clicking on the arrow on the right in a combo box will open a selection. Click on an entry to select it. The selected item will be displayed.

### Checkbox

**Fig. A-136:** Checkbox

Checkboxes allow to select several options. Clicking on a checkbox will enable or disable (no tick) it. You can enable several checkboxes at a time!

### Tab

**Fig. A-137:** Tab

For clarity's sake, the tabs split the dialogs into different subjects. To switch to another tab, click on the required tab.

### Menu bar/menu item

**Fig. A-138:** Menu bar

Also called pull-down menu. To create a new IG with 2-3 lites for example, click on the menu item New IG/LAMI to open the corresponding pull-down menu (see illustration above), then click on menu item 2-3 lites.

### Table/column header

**Fig. A-139:** Table/column header

Click on an entry in the column header to change the sorting sequence. At the first click, the table will be sorted in ascending order; click again to revert the sorting sequence.

### Key combinations

Hotkeys are keys or key combinations that are used to call a command or execute a function. Hotkeys will help the skilled user to achieve the required result quickly. The main hotkeys in A+W CAD Designer (Shapes) are listed below:

| Hotkey | Explanation |
| :--- | :--- |
| `<Ctrl>` + `<N>` | File New |
| `<Ctrl>` + `<O>` | Loads or opens an existing file. Dialog Open file appears. |
| `<Ctrl>` + `<S>` | Save file. Dialog Save file as ... opens. |
| `<Ctrl>` + `<P>` | Print document. Dialog Print appears. |
| `<Ctrl>` + `<R>` | Return to order processing |
| `<Ctrl>`+`<Z>` | Undo |
| `<Ctrl>`+`<Y>` | Restore |
| `<Ctrl>` + `<A>` | Select shape completely |
| `<Ctrl>` + `<Q>` | Select previous processing |
| `<Ctrl>` + `<C>` | Copy selection to the temporary memory |
| `<Ctrl>` + `<V>` | Insert Clipboard contents |
| `<Ctrl>` + `<X>` | Cut selection and copy it to the temporary memory |
| `<Del>` | Delete selection |
| `<Ctrl>` + `<Del>` | Delete contour in this and all next views |
| `<Ctrl>` + `<E>` | Edit object properties |
| `<Alt>` + `<E>` | Edit variables |
| `<Alt>` + `<B>` | Edit BOM |
| `<Ctrl>` + `>` | Move to next resolution level |
| `<Ctrl>` + `<` | Move to previous resolution level |
| `<Ctrl>` + `<0>` | Go to resolution level 0 |
| `<Ctrl>` + `<1>` | Go to resolution level 1 |
| `<Ctrl>` + `<2>` | Go to resolution level 2 |
| `<Ctrl>` + `<3>` | Go to resolution level 3 |
| `<Ctrl>` + `<M>` | Check dimensions |
| `<Ctrl>` + `<D>` | Redraw everything |
| `<Ctrl>` + `<B>` | Update BOM |
**Tab. A-2:** Key combinations

> **Active and inactive buttons**
> You will find that there are the active and inactive buttons in the individual menus. These buttons are enabled or disabled depending on your entries!

## Closing the program

There are different ways of ending A+W CAD Designer (Shapes).
- Click on the button [Close] in the top right corner of the program to end the program.
- Use menu **File > End**.

> **Notes on ending the program**
> If data have been changed or if new data have been entered and not saved yet, the program will issue a report to that effect. Select [Yes] to activate the dialog **Save file as...**. You can save the file and your amendments. The program closes after that. Select [No] to quit the program without saving the file or your amendments. Choose [Abort] to stop the End process and go on working with the program.

---

## Overview

The software reference provides information on the following subjects:
- Handling of Files
- Temporary Stacker
- Create a Product
- Technology-related Processing
- Machinery Control
- Working with BOMs
- Transform Contours
- Views
- Window
- How to Use the Help Function

> **Dialogs are accessible from different points**
> Please note that there are various ways of opening functions and dialogs. The corresponding dialogs will be described just once in this document.

---

## Handling of Files

Menu **File** includes all functions for editing (external) files and devices. By means of menu entries, functions can be directly performed, or dialogs are opened.

**Open the menu File**

The File menu offers the following options:

- **New:** This function is used to create a new SN file and to start a new A+W CAD Designer (Shapes) sketch. The currently open sketch will be kept. Several drawings can be open at the same time.
- **Open:** This function is used to load an existing A+W CAD Designer (Shapes) drawing. The dialog Open appears.
  ⇨ “Open” on page A-160
- **Insert:** This function is used to insert an existing contour to an open object. The dialog **Select file to insert** opens.
  ⇨ "Select paste file" on page A-163
- **Close:** This command closes the current SN file. If there are amendments that have not been saved yet, the program will ask whether you want to save them.
- **Save:** This command will save the current file by the name that has been used last. When you save a new sketch for the first time, the same dialog as for **Save as...** will appear. Command Save replaces the existing file of the same name on the hard disk by the new sketch from the working memory.
- **Save as:** Choose this menu item to save a file by the defined name, format, and storing place. When you save a file for the first time, the dialog **Save as** will appear automatically when you click on **Save**.
  ⇨ "Global shape data" on page A-164
- **Set password:** Choose this menu item to protect your drawings with a password.
  ⇨ "Set password" on page A-167
- **Import:** This function serves to import files of different formats which include no A+W CAD Designer (Shapes) objects.
  ⇨ "Select file..." on page A-168
- **Export:** This menu item allows to export SN files to different formats.
  ⇨ "Save file in (export)" on page A-171
- **Back to order processing:** This menu is active only if you are using A+W CAD Designer (Shapes) in connection with an external order processing system (e.g. A+W Enterprise). In this case, A+W CAD Designer (Shapes) will be started from the order processing system (OPS) and supplied with data from the current order. Shape information will also be adopted from the OPS. When all editing has been done in A+W CAD Designer (Shapes), use this menu item to return to your OPS. The SN file will be automatically saved in the process. The amendments and additions relevant for the OPS will be transferred; A+W CAD Designer (Shapes) will be closed.
  You can temporarily save the results while editing in A+W CAD Designer (Shapes). Please note that you must not change the file name your OPS has given the SN file!
  ⇨ Tools, "Interplay with other programs" on page A-483.
- **Resume order processing:** This menu is active only if you are using A+W CAD Designer (Shapes) together with an external order processing system (e.g. A+W Enterprise). In this case, A+W CAD Designer (Shapes) will be started from the order processing system (OPS) and supplied with data from the current order. Shape information will also be adopted from the OPS.
  Please use this menu if you want to reject manual amendments in A+W CAD Designer (Shapes) and want to start again from the original file. The current version of the SN file will be rejected; AWBroke will transfer the original file once more.
  ⇨ Tools, "Interplay with other programs" on page A-483.
- **Send Email:** You can use this function only if an email program has been installed on your computer. The email program will create an email. The current SN file will be attached to this.
- **Print:** Use this menu item to start printing.
  ⇨ "Print dialog..." on page A-172
- **Preview:** With this function A+W CAD Designer (Shapes) shows print result to be expected.
  ⇨ "Preview" on page A-175
- **Print setup:** A+W CAD Designer (Shapes) opens the dialog for configuring the printer in your operating system.
  ⇨ Documentation on your operating system
- **Previous files:** A+W CAD Designer (Shapes) shows a list of the last edited files.
- **Exit:** This function terminates A+W CAD Designer (Shapes). If the latest data have not been saved yet, A+W CAD Designer (Shapes) comes up with a dialog in which you can decide whether or not the data shall be saved.

### Open
**File > Open**

**Fig. A-140:** Open

This function is used to load an existing A+W CAD Designer (Shapes) drawing.

**Fields**
- **Search in:** This combo box allows to define in which directories A+W CAD Designer (Shapes) shall search for files to be opened (e.g. on the hard disk, on the server, or on a disk).
- **Files:** In the field Search in, A+W CAD Designer (Shapes) shows all files available in the selected directory that match the required type.
- **File name:** If you click on one of the files on the list, A+W CAD Designer (Shapes) shows the file name in this field. You can also enter the file name via keyboard. In this case, A+W CAD Designer (Shapes) shows a list of files starting with these characters.
- **File type:** Allows to define the file types (suffix) you are searching for. A+W CAD Designer (Shapes) only shows files of this type.
- **Display field:** In this field, A+W CAD Designer (Shapes) presents a short preview of the file you have selected. This will help identifying the file without having to open it. The system shows a preview (geometry, inside contours, ...) of the last saved version. This preview is available only for SN files Version 5.x or higher.
- **Buttons:** Apart from the input field Search in, the standard buttons of the operating system (Windows) are displayed; you can use them to go to another directory, create a new directory, or change the layout of the display.

**More information on opening files**
- ⇨ "File type" on page A-160
- ⇨ Tools, "Open File" on page A-424

### Open DXF file
**File > Open > Select and open DXF file**

**Fig. A-141:** Open DXF file

This dialog shows a preview of the DXF file to be imported. You have two possibilities to complete the dialog:
- **Import shape**
- **Data import**

With Import shape an import is started that is oriented toward detecting precisely one shape with its processings. Here, cut-outs, drillings, and roundings are detected automatically. The cutting form does not include the cut-outs.

With Import data, the data is more general (e.g. includes several shapes or additional objects). Then it may be necessary to rework it more manually in A+W CAD Designer (Shapes).

At the bottom left of the screen, you have the option to scale the DXF file to be read in. Here, the scaling factor can be entered as the ratio of shape dimensions to original dimensions. The default value is 1:1. If, for example, you enter 1:10, all geometric objects are multiplied by a scaling factor of 10.

### Select paste file
**File > Paste**

**Fig. A-142:** Select SN paste file...

Option Paste allows to add an existing contour (e. g. a certain inside contour) to an already open object (current contour) without deleting the current contour. The pasted file will be adopted with all its views and processing steps.

Paste loads a contour onto the drawing board while keeping the existing objects.

**More information on the inserting of contours**
- ⇨ "Open" on page A-160
- ⇨ Tools, "Open File" on page A-424

### Global shape data
**File > Save as**
**Edit > Object properties**
**`<Ctrl> + <E>`**

**Fig. A-143:** Global shape data

This dialog serves to save in a new file various information on the created sketch. This information can appear on the customer-bound drawing. Data shown in this dialog are valid for all lites of the sketch. Dialog Local shape data principally shows the same fields; the entries there are only valid for the defined lite however.

You can override the default settings in the fields.

> **Data transfer with order processing system**
> If you are using an order processing system, many fields will be preset from the corresponding order. Changes of settings will be passed on the linked order processing system.

**Description of fields**
A+W CAD Designer (Shapes) saves these details in the header of the SN file. You can display this information by means of the MS-DOS command TYPE (example: TYPE ORDER.SN).

- **Name:** Give a name to the contents of the file. The contents of this field are not the file name. A suitable name would be the order name for example.
- **Text:** Allows to enter a description.
- **Additional List:** This field is currently unused.
- **Additional text:** This field is currently unused.
- **Glass type:** Enter the glass type to be used for this contour.
- **Thickness:** Enter the lite thickness. You can use mm or inch.
- **Number of:** Enter the number of lites of a contour to be produced for this order.
- **Delivery:** Enter the shipping date for the lites.
- **Order:** Enter the order number this SN file belongs to.
- **Item:** Enter the order item this SN file belongs to.
- **Customer:** Enter the name of the customer for this order.
- **Reference:** Enter the customer reference this order belongs to.
- **Ins.c.code:** This field is currently unused.
- **Glass code:** Name for the glass unit. This is necessary if A+W CAD Designer (Shapes) is linked with an order entry system via AWBroke. AWBroke will fill this field with the data required.
- **Lite:** If a unit consists of several lites, this field shows the number of the lite belonging to the displayed shape data. This field also exists in dialog Global shape data but without an entry.
- **Unit:** If a sketch includes several units, this field shows the number of the lite that belongs to the shape data displayed in the dialog. There is no display in dialog Global shape data. A+W CAD Designer (Shapes) presets this field by 1. Several units in a SN file will be required for future A+W CAD Designer (Shapes) development.
- **User:** Enter the name of the user who has created this file.
- **Storing type:** This field is automatically filled in by A+W CAD Designer (Shapes). A+W CAD Designer (Shapes) defines if the file was created automatically (by A+W Business or AWBroke) or interactively (manually, by a user). The entry is based on the last processing.

**Description of buttons**
- **OK:** When you press this button, A+W CAD Designer (Shapes) will save the data with the sketch and opens the dialog **Save as** in which you can enter a name and path for the file.

**Additional information**
- ⇨ "Save as" on page A-166
- ⇨ "Local shape data" on page A-182

### Save as
**File > Save as... > [OK]**

**Fig. A-144:** Save as

Use this dialog to save your sketch by a certain name.

- **Save:** Choose the directory in which you want to save the file.
- **File name:** Enter the required file name. A+W CAD Designer (Shapes) automatically suggests the name from dialog **Global shape data**. You can override this if required. When saving, A+W CAD Designer (Shapes) attaches the suffix .SN to the file. If you enter an existing name for the sketch, the existing sketch will be overridden.
- **File type:** Use this dialog to save files of the A+W CAD Designer (Shapes) files type. If you need the contour in a different format, you have to export it.

### Set password
**File > Set password**

**Fig. A-145:** Set password

Use this dialog to protect your sketch.

- **Reading password:** Enter a password to protect your file against unauthorized reading (opening). If you enter a reading password, A+W CAD Designer (Shapes) will ask for this next time you try to open the file. You will not be able to open the file without a password. The same applies to entering data in this file.
- **Writing password:** Enter a password to protect your file against unauthorized changes (saving). If you enter a writing password, A+W CAD Designer (Shapes) will ask for it next time you try to open the file. Without a password, you cannot save this file by its old name. You can of course save the file by a new name without a password.

### Select file... (Import)
**File > Import > [Data format]**

**Fig. A-146:** Select DXF file

This function serves to import files of different formats which include no A+W CAD Designer (Shapes) objects.

Menu Import has a similar effect as Insert. This means that imported files do not override existing objects but will be added to those. For toughened glass, this is done in the Sketch view and for BLOCK.IND in the view that has been selected for the import.

At the Import, A+W CAD Designer (Shapes) adopts the geometry of the selected file. At Inserting all data of all views of a contour are imported into an existing file.

When you click on the Import menu, the following data formats will be available:
- **BLOCK.IND:** Format of contours saved in A+W CAD Designer (Shapes) in the database BLOCK.IND. These contours only include the coordinates of the segments used. Drill holes will be automatically created if BLOCK.IND shows them as two semicircles. This format serves as a data exchange format for geometries between A+W CAD Designer (Shapes) and XOPT, and all A+W machine drivers.
- **DXF:** Many CAD programs are using this data exchange format. Contours may have to be edited after importing (e. g. close contour).
- **TG:** Contours created by TG/CONTOUR and have been saved in this program with the suffix .ESG. A+W CAD Designer (Shapes) will only import the sketch with all sizes. Inside contours or edgework will be lost. This allows to import complex technical drawings without having to enter them again.
- **2D-IGES:** Use this format if a file includes 2D data acc. to IGES standard (Initial Graphics Exchange Specification).
- **2D-VDA:** Select this format if a file includes 2D data acc. to VDA-FS standard (Verband der Automobilindustrie – Flächenschnittstelle).
- **3D-IGES:** Use this format if a file includes 3D data acc. to IGES standard (Initial Graphics Exchange Specification).
- **3D-VDA:** Select this format if a file includes 3D data acc. to VDA-FS standard (Verband der Automobilindustrie – Flächenschnittstelle).
- **CAMXML:** Use this format to import contours from a CAMXML file.
- **Virtual Digitizing:** Choose this format to digitize a contour as a photograph by means of the Virtual Digitizing software.

**Fields**
- **Search in:** This combo box is used to define the directory in which A+W CAD Designer (Shapes) shall search for files to be imported.
- **Files:** In the field Search in, A+W CAD Designer (Shapes) shows all files available in the selected directory that match the required type.
- **File name:** If you click on one of the files on the list, A+W CAD Designer (Shapes) shows the file name in this field. You can also enter the file name via keyboard. In this case, A+W CAD Designer (Shapes) shows a list of files starting with these characters.
- **File type:** A+W CAD Designer (Shapes) automatically enters the file type you have chosen when loading the import function. A+W CAD Designer (Shapes) only shows files of this type.

**Additional information**
- ⇨ Tools, "Exporting a SN drawing" on page A-426
- ⇨ Tools, "Via CAMXML files" on page A-506
- ⇨ Tools, "Exporting part of a BOM" on page A-508
- ⇨ Tools, "Virtual digitizing" on page A-227
- ⇨ "File type" on page A-169

### Layer filter
**File > Import > DXF > File selection**

**Fig. A-147:** Layer filter

This A+W CAD Designer (Shapes) dialog shows the layers available in a DXF file. Tag the layers and press the corresponding button.

**Buttons**
- **->**: Use this button to select a tagged layer.
- **<-**: This button will remove a layer from your selection.
- **Show selection:** Use this button to show the contents of the selected layers in A+W CAD Designer (Shapes).
- **Import selection:** Press this button to import the contents of the selected layers into the SN file.

### Save file in (export)
**File > Export > [Data format]**

**Fig. A-148:** Global shape data

This option allows to export SN files to different formats.
Click on menu **Export** to open a sub-menu with the following options:

- **BLOCK.IND:** Contours saved in A+W CAD Designer (Shapes) on the database called BLOCK.IND. These files include neither sizes nor data from other views except the exported one. With this function, you can add the contours from the current view to this database.
- **CNC:** Standard format for CNC machine control, based on the IG standard.
- **DXF:** Standard format for various CAD programs. If you export the current object to the DXF format, you can import this file into CAD programs such as AutoCADä.
- **IGES:** Choose this format to save the contour acc. to IGES standard (Initial Graphics Exchange Specification).
- **Graphics file:** This option allows to export the sketch as a graphics file. A+W CAD Designer (Shapes) offers the following export formats:
    - BMP
    - EMF
    - GIF
    - TIF
    - JPG
    - EPS
    - PCX

**More information on exporting files**
- ⇨ Tools, "Exporting a SN drawing" on page A-426

### Print dialog...
**File > Print**

**Fig. A-149:** Print dialog...

Use this function to start printing the present drawing on the defined printer. Edition is done via the indicated printer. You can define the printer on your computer, in menu **Printer setup**.

**Description of fields**
- **Printer:** This field shows the printer on which A+W CAD Designer (Shapes) prints the drawing. If several printers are available, you can select another one via [Printer].
- **Copies:** Enter the number of copies A+W CAD Designer (Shapes) shall print.
- **Form:** Select the form on which the drawing shall be printed. You can create the layouts yourself. The following forms are available:
    - **<_>**: Select this entry to print the drawing on the A+W CAD Designer (Shapes) standard form.
    - **<SN>**: In this case, A+W CAD Designer (Shapes) will use the sn.ini settings for printing. This file defines the files from dialog **Global shape data** that shall be printed on the form, and where. You can also define the size and position of the contour on the page in sn.ini.
    - **<SNW>**: In this case, A+W CAD Designer (Shapes) will create a Word file that contains all available dummies A+W CAD Designer (Shapes) can use.
    - **COORDLST.DOC**: In this case, A+W CAD Designer (Shapes) will print a Word file listing all segments of the present contour, and their coordinates.
    - **Other Word files**: If other Word files are available, these are existing patterns that can be used to save the information of the SN file. The files will be printed on the Windows standard printer even if you have chosen another printer in A+W CAD Designer (Shapes).

**Fields in section Detail**
- **Complete:** Choose Complete to print the entire drawing. The drawing will be adapted to the available space.
- **Scale:** Use this radio button to print the drawing on a certain scale. Enter the required scale and the X/Y coordinates from where printout shall start. A+W CAD Designer (Shapes) will print the section on the defined scale that fits the available space.
- **Spacer:** Use this radio button to print a certain part of the drawing. In the following fields, enter the required part to be printed. Enter the X- and Y coordinates for start and end of the surrounding rectangle. A+W CAD Designer (Shapes) will fit this section into the available space.

**Description of buttons**
- **Printer:** This will open the dialog **Printer setup** in your operation system. For information please refer to the documentation on your operating system.
- **OK:** Starts printout of the drawing in the present view. If sizes have been entered, these may be shown in the drawing. Depending on the setting, a standard or customized form will be printed.

**For further information, please see:**
- ⇨ Tools, "Printing a drawing in a Word file" on page A-481
- ⇨ "Preview dialog..." on page A-174

### Preview dialog...
**File > Preview**

**Fig. A-150:** Preview dialog

Use this dialog to start the print preview. The functions are the same as in dialog **Print dialog...**

**For further information, please see:**
- ⇨ "Print dialog..." on page A-172

### Preview
**File > Preview > [OK]**

**Fig. A-151:** Preview dialog

A+W CAD Designer (Shapes) shows a preview of the printout. This will tell you whether the printout meets your expectations.

**Description of buttons**
- **Print:** This button will open in A+W CAD Designer (Shapes) the **Print dialog...**
- **Next page:** If the drawing consists of several pages, this button will bring you to the next page.
- **Prev page:** If the drawing consists of several pages, this button will bring you back to the previous page.
- **Two pages:** If the drawing consists of several pages, you can use this button to display two pages at once.
- **Zoom In:** Allows to enlarge the display.
- **Zoom Out:** Helps to reduce the size of the display.
- **Close:** Use this button to quit the preview.

**For further information, please see:**
- ⇨ "Print dialog..." on page A-172

---

## Temporary Stacker

Menu **Edit** includes all functions using the clipboard. **Edit** has nothing to do with the processing of glass, but means editing (changing) the complete or incomplete drawing (contour) in the current file. Menu offers the following menu items:

- **Undo:** This function will undo the last editing step. Selecting it again will cancel the last-but-one action, selecting it a third time will cancel the action before that, etc. The number of steps that can be cancelled can be set in sn.ini with parameter `NumberOfUndoableCommands`. This parameter is preset with 150 at installation. If you have cancelled too many actions by mistake, you can restore them by means of **Restore**.
- **Redo:** This function restores the last cancelled action. You can restore all cancelled actions unless the chain of actions is not interrupted by a new entry. If you cancel three actions for example and then enter a new segment, you will not be able to restore the previous three actions because these are based on a different starting point (without the new segment).
- **Select a contour:** You can use this option to select a connected contour. After clicking on one or more segment and selecting this function, all segments of the corresponding contour will be shown bold, marked in the selection colour. All inside contours are selected as well. These contours can now be edited in the following menus. Selecting a new object or a new tool will deselect the current contour.
- **Select actions:** This menu is only available in the A+W CAD Designer (Shapes) automotive glass version (ATM). This option allows to display all processing steps defined for this contour. Segments with processing are shown in red, original segments in light grey. Those part of the contour that shall not be processed, appear in black. When sketched again (`<Ctrl>` + `<D>`), the contour appears like normal. If more than one processing step has been defined for a segment, only the last one will be shown.
- **Copy:** This function copies all tagged segments to the clipboard without changing the present view. The former contents of the clipboard will be overridden, i.e. deleted. By means of the function **Paste**, the new contents of the clipboard can be inserted once or several times in other places of a contour (or in another view). Use this function to copy segments or contours. Please note that only the coordinates will be copied; this does not include sizes or different views of the segments. To insert a A+W CAD Designer (Shapes) object with all its properties, you have to save it as a file first, then import it via **File > Insert** into the present contour.
- **Insert:** This function inserts the actual contents of the clipboard into the current view. This includes copied objects as well as cut-out ones. **Insert** will not insert segments in the same place where they have been cut out. The copy will be inserted in a slightly different position. Once cut out, contours can be linked only with a special tool which automatically smoothes inaccuracies at the joint. You can undo the processing step however.
- **Cut:** Use Cut out to transfer the tagged segments to the clipboard. These segments will be removed from the sketch. This applies to the current view and to all views based on it.
- **Design shape:** This menu is only available in the A+W CAD Designer (Shapes) automotive glass version(ATM).
- **Clear:** This function removes tagged segments from the present view. Use **Undo** to restore the deleted object.
- **Delete shape:** Use this function to delete the entire contour that belongs to the tagged segment.
- **Clear all of this kind:** This function is used to delete contour processing or properties (e. g. edgework, rounded corner, sizes, starting point) that have been applied several times. If you choose a processing step, size, etc. and select **Edit > delete all of this kind**, all processing steps of this type will be deleted from all contours. If you select a segment, this function will delete the segment and all its processing steps. Deletion can be undone however.
- **Object properties:** This option opens the dialog **Global shape data**.
  ⇨ "Global shape data" on page A-164
- **Edit variables:** This option opens the dialog **Edit variables**.
  ⇨ "Edit variables" on page A-184
- **Edit BOM:** This option opens the dialog **Edit BOM**.
  ⇨ "Edit variables" on page A-184

### Shape correction
**Edit > Contour correction**

**Fig. A-152:** Shape correction

This dialog is used to enter measuring results for measuring points. If your contour shows measuring points, you can correct the contour by entering new values. A+W CAD Designer (Shapes) will replace the existing segments by new ones or correct the existing segments so that the required sizes are met.

**Description of fields**
- **Measuring point:** Enter the number of the measuring point for which you want to enter a contour. This number has to match the number shown in the sketch.
- **Distance:** Enter the distance (in direction of the next measuring point) from the measuring point where the correction value has been determined.
- **Correction:** Enter the value by which the defined position shall be corrected. A positive entry will shift the contour outwards; a negative entry will move it inwards.

**Description of icons**

| Symbol | Meaning |
| :--- | :--- |
| S | This icon is used to delete all existing entries, and start a new table |
| 📄 | This icon is used to insert a line below the current one. |
| 🗑️ | Use this icon to delete the current line. |
| 📍 | This icon is used to define the measuring point in the current line as the starting point for correction. |
| ↓↑ | Use this icon to reverse the sequence of measuring points. |
**Tab. A-3:** Icons in dialog shape correction

For an explanation of the meaning of the other icons, please see:

**Status area**
A+W CAD Designer (Shapes) informs you about detected problems or successful corrections.

**Additional information**
- ⇨ Tutorial, "SN tools (C)" on page A-24
- ⇨ Tools, "Digitizing measuring points" on page A-222

### Property description as per...
**Tag a contour segment > `<Ctrl> + <E>`**
**Tag a contour segment > Edit > Object properties**

**Fig. A-153:** Property description

This dialog serves to select the unit the shape data of which shall be displayed. Click on the required unit and confirm by [OK]. A+W CAD Designer (Shapes) will open the dialog **Local shape data**.

**Additional information**
- ⇨ "Local shape data" on page A-182

### Local shape data
**Tag contour segment > `<Ctrl> + <E>` > Select unit**
**Tag contour segment > Edit > Object properties > Select unit**

**Fig. A-154:** Local shape data

This dialog serves to save in a new file various information on the created sketch. This information can appear on the customer-bound drawing.

You can override the default settings in the fields.

> **Data transfer with order processing system**
> If you are using an order processing system, many fields will be preset from the corresponding order. Changes of settings will be passed on the linked order processing system.

In a A+W CAD Designer (Shapes) 4 stand alone installation, you can define several local shape data for a lite (contour). A lite has to have several numbers for this purpose.

You can assign local shape data to every number. This function is currently not available in connection with A+W Production or A+W Business.

**Description of fields**
These fields are identical with those in dialog Global Shape Data and are explained there already.

- **Remove:** This button is active only if there are several local shape data (numbers) for a lite. If you press this button, A+W CAD Designer (Shapes) will delete the displayed number including the corresponding local shape data.

**Additional information**
- ⇨ "Global shape data" on page A-164
- ⇨ Tools, "Define lite sequences for units" on page A-418

### Edit variables
**Edit > Edit variables**

**Fig. A-155:** Edit variables

This dialog offers the variables you have used for dimensioning your sketch. Dialog **Edit variables** is used to allocate values to the existing variables. You can also define new variables.

**Description of fields**
- **Name:** This column shows the name of the variable. You can use this variable in a suitable place for dimensioning the sketch.
- **Printing:** This column describes the variable as an expression of other variables (as a formula), or given a figure.

**Functions that can be used as expressions in the variable editor**

| Printing | Description |
| :--- | :--- |
| `sin(X)` | Sinus of X whereby X is an angle. A+W CAD Designer (Shapes) expects angles in ° (degrees). |
| `cos(X)` | Cosine of X, X being an angle. A+W CAD Designer (Shapes) expects angles in ° (degrees). |
| `tan(X)` | Tangent of X, X being an angle. A+W CAD Designer (Shapes) expects angles in ° (degrees). |
| `cot(X)` | Cotangent of X, X being an angle. A+W CAD Designer (Shapes) expects angles in ° (degrees). |
| `asin(X)` | Arc sinus of X, X being a number between -1.0 and 1.0. The result of this function is an angle between -90° and +90°. If you need the value as an arc measure, you have to apply to the result of the function `asin(X)` the `rad` function. |
| `acos(X)` | Arc cosine of X, X being a number between -1.0 and 1.0. The result of this function is an angle between 0° and +180°. If you need the value as an arc measure, you have to apply to the result of the function `acos(X)` the `rad` function. |
| `atan(X)` | Arc tangent of X, X being a number. The result of the function is an angle between -90° and +90°. If you need the value as an arc measure, you have to apply to the result of the function `atan(X)` the `rad` function. Please note that for many calculations, it is much easier to use the function `atan2(X;Y)` instead of function `atan(X)`. |
| `atan2(Y;X)` | Arc tangent of the quotient of Y/X, Y and X both being either a length or numbers without a measure. The result of this function is an angle between -180° and +180°. Atan2 uses the signum values of X and Y to determine the quadrant. This function calculates the correct result (±90°) if X=0. If you need the value as an arc measure, you have to apply to the result of the function `atan2(X; Y)` the `rad` function. Please note that the parameters are separated by semicolon not by comma. |
| `acot(X)` | Arc cotangent of X, X being a number. The result of the function is an angle between -90° and +90°. If you need the value as an arc measure, you have to apply to the result of the function `acot(X)` the `rad` function. |
| `sqr(X)` | X squared (X²). If X is a number, the result of this function is also a number (1st dimension). If X is a line, the result of this function is a surface (2nd dimension). A+W CAD Designer (Shapes) supports no other dimensions. |
| `sqrt(X)` | Square root of X, X being a number or a surface with a positive sign. The result is a positive square root, i.e. a number or a line. |
| `exp(X)` | Exponent X (eX) of base e, X being a number. The result is also a number. It may be necessary to apply the function `numval` to the result, or convert to standard measure. |
| `ln(X)` | Natural logarithm of X, X being a number with a positive sign. The result is also a number. It may be necessary to apply the function `numval` to the result, or convert to standard measure. |
| `pow(X;Y)` | Exponent Y of base X (X to the Y-th power). Examples: `pow(2;3)=8`, `pow(2;0.5)=sqrt(2)`. X and Y have to be numbers. Only X can be negative as Y is an integer. It may be necessary to apply the function `numval` to the result or to convert to standard measure. |
| `int(X)` | Integer part of X. Example: `int(2.5)=2`, `int(-3.8)= -3`. The result is of the same type as the expression. If the expression is a number with a measure, the number will be converted as described in connection with `numval`. The integer part will be used and converted to the same type as X. |
| `frac(X)` | Non-integer part of X. Example: `frac(1.5)=0.5`, `frac(-2.8)= -0.8`. The result has the same type as the expression. If the expression is a number with a measure, the number will be converted as described in connection with `numval`. The non-integer part will be used and converted to the same type as X. `int` and `frac` are defined as: `X=int(X)+frac(X)`, no matter what the sign. |
| `floor(X)` | Biggest integer part of X, ≤ X. Example: `floor(3.5)=3`, `floor(-2.5)= -3`. The result has the same type as the expression. If the expression is a number with a measure, the number will be converted as described in connection with `numval`. The result will be used and converted to the same type as X. |
| `ceil(X)` | Next bigger integer of X, ≥ X. Example: `ceil(2.2)=3`, `ceil(-1.8)= -1`. The result has the same type as the expression. If the expression is a number with a measure, the number will be converted as described in connection with `numval`. The result will be used and converted to the same type as X. |
| `round(X)` | Round to next integer. Example: `round(1.4)=1`, `round(-1.5)= -2`. The result has the same type as the expression If the expression is a number with a measure, the number will be converted as described in connection with `numval`. The result will be used and converted to the same type as X. |
| `pi()` | Value of Pi (3.1415926...). This expression results in the number Pi. The expression has no argument; the brackets have to be written. |
| `abs(X)` | Absolute value of X (without sign). Example: `abs(4.2)=4.2`, `abs(-3.7)=3.7`. The result has the same type as the expression. If the expression is a number with a measure, the number will be converted as described in connection with `numval`. The result will be used and converted to the same type as X. |
| `sign(X)` | Sign of X. The sign function returns the following values: `sign(X) = 1` if X ≥ 0. 1 stands for all positive numbers and zero. `sign(X) = -1` if X < 0. -1 stands for all negative numbers. The result is a number, notwithstanding the type of expression. `Abs` and `sign` are defined as: `X=sign(X)*abs(X)`. |
| `min(X1;X2;...;Xn)` | Smallest value from a set of Xi. The number of values is unlimited but there have to be two at least. All values have to have the same type. The type is also defined in the result. |
| `max(X1;X2;...;Xn)` | Biggest value of a set of Xi. The number of values is unlimited but there have to be two at least. All values have to have the same type; the type is shown in the result. |
| `rad(X)` | Value of X in arc measure. X has to be an angle. The expression calculates X/180°*pi(). The result is shown without a measure. |
| `deg(X)` | Value X in ° (degrees). X has to be a number without measure, and is used as an arc measure. The expression calculates X/pi()*180°. The result is an angle. |
| `numval(X)` | Numeric value of X. Calculates a number acc. to the following rules: If standard measure is mm: numval shows mm, m2, m3, or mm-1. If standard measure is inch: numval shows inch, sft, cbft, or inverted inch. If using different measures, numval shows a metric value. Simple numbers (without dimension) will not be converted. |
| `thickness(X)` | Thickness of contour X. X has to be a positive integer. `thickness(0)` shows thickness from Global shape data. `thickness(X)` shows the value for PackLayer X. `thickness(2.2)` shows the thickness of contour (lite) 2. |
**Tab. A-4:** Functions that can be used as expressions in the variable editor

> **Results depend on the settings!**
> Contours the variables of which use the expression numval, can change unexpectedly. The reason is that the result of numval depends on the setting of the standard measure with regard to input and display. Contours using numval cannot be simply exchanged between different A+W CAD Designer (Shapes) installations. You should therefore use numval only for short-lived, customized solutions. For contours you want to go on using, you should only use the corresponding basic measures.

- **Value:** Defines the current numerical value of a variable. This value is either calculated from the formula in column Expression or has the same numerical value as in column Expression.
- **Type:** Defines the type of the variable. Valid types are:
    - **Size:** The variable is a measure of length with a measure.
    - **Angle:** The variable is an angle.
    - **Number:** This type is used for numbers without a measure.

**Description of buttons**
- **Save:** When you press this button, A+W CAD Designer (Shapes) checks the syntax of the formula and adds it to the list of variables in alphabetical order. If the variable expression includes other variables that have not been defined yet, A+W CAD Designer (Shapes) will automatically create those.
- **New:** This button will insert a line into the displayed table. This line can be used to define a new variable.
- **Delete:** This function is used to delete a tagged variable from the list.
- **Close:** Press this button to save the values of the variable, and recalculate the sketch accordingly.

**Additional information**
- ⇨ Tools, "Working with variables" on page A-470
- ⇨ Tools, "Create automatic variables" on page A-501

---

## Create a Product

Menu **Product** comprises all functions to enter, create, and design a glass product. This is where you can change the geometry as required.

Select the view you want to use from menu **Product**. A+W CAD Designer (Shapes) automatically shows the valid tools for this view. Menu Product contains the following items:

- **2D import:** Select this view to create a contour from imported 2D data.
- **3D Import:** Select this view to create a contour from imported 3D data.
- **Points:** Choose this view to enter a contour via digitizer and transfer it to A+W CAD Designer (Shapes).
  ⇨ Tutorial, "The Points view" on page A-30
- **Sketch:** This view serves to draw a contour based on a technical drawing or a sketch.
  ⇨ Tutorial, "The Sketch view" on page A-31
- **Geometry:** Use this view to calculate from the data of a previous view a true-to-scale, geometrically correct contour and display it. If this view shows no contour, the data entered in the previous view do not suffice to calculate the contour.
  ⇨ Tutorial, "The Geometry view" on page A-32
- **Revision:** Select this view to amend the technical structure of a contour. The options are:
    - Split segments and add further contour points.
    - Delete contour points and merge segments.
    - Change contours.
    - Smooth out digitized contours.
    ⇨ Tutorial, "The Revision view (for automotive glass only)" on page A-32.
- **Inside contours:** Select this view to align contours, position notches, and define holes to be drilled.
  ⇨ Tutorial, "The Internal contours view" on page A-33
- **Edge processing steps:** Select this view to define processing steps for the edges.
  ⇨ Tutorial, "The Edgework view" on page A-33
- **End product:** This view allows to display the end product with the correct sizes and edgework.
  ⇨ Tutorial, "The End product view" on page A-33

> **Menu entries can be configured.**
> If your system shows other or additional menu items, you are using a customized configuration.

---

## Technology-related Processing

The views in menu **Technology** allow the selection and technology-based processing of the geometry created in view **Product**. This is where restrictions and additional conditions are checked and automatically calculated if necessary. Menu **Technology** is used to edit the created geometry for various processing methods.

The separation of processing and the actual processing machine has two advantages:
- A technology can be used by several machines (drilling for drills and processing machines).
- The user creates the end product (the machine program) step by step in a logical sequence without having to handle too much information at once.

Menu **Technology** mainly comprises the following, glass-related processing steps.

> **Other menu entries are possible!**
> Depending on the configuration, your system can offer more or less menus.

- **Cutting:** Goes to view Cutting.
  ⇨ Tutorial, "The Cutting view" on page A-34
- **MULTICUT:** Goes to view Multicut.
- **Grinding:** Goes to view Grinding.
  ⇨ Tutorial, "The Grinding view" on page A-34
- **Drilling:** Goes to view Drilling.
  ⇨ Tutorial, "The Drilling view" on page A-35
- **Processing:** Goes to view Processing.
  ⇨ Tutorial, "The Processing view" on page A-35
- **Unit:** Goes to view Unit.
  ⇨ Tutorial, "The Unit view" on page A-35
- **Breakout (CNC):** Goes to view Breakout.
  ⇨ Tutorial, "The Breakout view" on page A-35
- **UNICUT:** Goes to view Unicut.
- **Breakout (single, CNC):** Goes to view Breakout.

---

## Machinery Control

Menu **Machine** shows entries if your A+W CAD Designer (Shapes) has been configured to control CNC machinery. The geometrical information displayed in a machine view are used by A+W CAD Designer (Shapes) to create the NC code for machinery control.

Menu **Machine** is a two-step menu. The first level shows different machines (or other functions available through A+W CAD Designer (Shapes)). The second menu level offers:
- An entry for NC creation (start of function).
- The option to go to the appropriate view.

Loading a dialog to enter attributes for the corresponding machine type. Attributes for the individual machines are shown when you select the corresponding segments; their values can be edited.

A+W will configure this when installing A+W CAD Designer (Shapes).

---

## Working with BOMs

If you are working with laminated or IG units, menu **Step** shows entries for which there is a BOM in A+W CAD Designer (Shapes). Select the entries in this menu to display the corresponding BOM step in the individual views.

---

## Transform Contours

The functions in menu **Transformation** allow moving, rotation, reflection, adjusting, and extension in (nearly) all views. First, select the required contours and then a function in menu **Transformation**. The selection of contours will be kept after transformation.

Transformed contours appear transformed in all the following views if no explicit dimensions forbid this. Sizes will always override transformation. Once dimensioned, an inside notch will not be moved even if it is transformed in the Geometry view. Sizes are effective even in the following views. Dimensioned notches will keep their position in all technology views (unless other, new sizes are entered).

Exact alignment of contours cannot be achieved by transformation and is not intended either. Transformation serves for (rough) positioning. It allows to define whether a contour lies within or outside an external contour for instance. The exact position has to be defined by means of sizes.

Transformation offers the following options:

- **Move:** The command **Move** allows to move an existing contour. Prerequisite for moving is that one segment (each) of the object(s) to be moved is tagged.
- **Move to point zero:** With this command, A+W CAD Designer (Shapes) will move the entire contour so that the bottom left corner lies on the zero point (0/0) of the coordinate system.
- **Rotate:** Use this command to rotate any contour by the desired angle. The contour will be rotated around the centre of gravity of the selected contour(s).
- **Rotate by 90°:** This command will rotate the selected object clockwise by 90° around its centre of gravity.
- **Position as in:** This function allows to transform a contour (move, rotate, etc.) in different views. All technology views are available as sub-menus. Select a view to position (transform) the selected contour just like in the present view.
- **Reflect horizontally:** The selected object is reflected horizontally. Left and right will be reversed. Existing, asymmetrical inside contours (e. g. a counter-sunk hole) will not be reflected (turned around). Existing trim will not be reflected either.
- **Reflect vertically:** The selected object is reflected horizontally. Left and right will be reversed. Existing, asymmetrical inside contours (e. g. a counter-sunk hole) will not be reflected (turned around). Existing trim will not be reflected either.
- **Flip horizontally:** The selected object is reflected horizontally. Top and bottom will be reversed. Existing, asymmetrical inside contours (e. g. counter-sunk hole) or trim will be reversed as well.
- **Flip vertically:** The selected object is reflected vertically. Left and right will be reversed. Existing, asymmetrical inside contours (e. g. counter-sunk hole) or trim will be reversed as well.
- **Scale:** The selected object will be adjusted by the defined factors in X and Y direction, i. e. enlarged or reduced true to scale. If you enter a factor below 1, a controlled distortion of the object will be reduced; otherwise, it will be enlarged. Different factors for X (horizontal) and Y (vertical) are possible and will result in the contour. Existing inside contours will be adjusted as well.

> **Adjustment is based on the current position!**
> Please note that the object will be changed, based on its current position. If the object lies diagonally, it will be adjusted this way.

- **Stretch:** The selected object is stretched (or compressed) on both sides. This means that the object is changed by the defined value, left and right (in X direction) or top and bottom (in Y direction). Different entries for X (horizontal) and Y (vertical) are valid and will result in a controlled distortion of the contour. Existing inside contours will be stretched as well. Enter the required values in the input field.

> **Stretching is based on the current position!**
> Please note that the object will be changed, based on its current position. If the object lies diagonally, it will be stretched this way.

- **Grouping:** This function is for grouping.
  ⇨ Tools, "Working with groups" on page A-432
- **Replace group:** This function serves to replace an existing (and tagged) group by another group (in a separate SN file). The alignment applied to the existing group will be applied to the new group as well.
  ⇨ Tools, "Creating a door and positioning the cut-outs" on page A-460
- **Freezing:** This function is available if your A+W CAD Designer (Shapes) has been configured for the manual input of trim. To prevent following processes (e.g. grinding, arrissing, polishing, ... in A+W Production) from recalculating and overriding a manually defined trim, you can fix (freeze) the manually defined trim with this function. The following processes cannot override this value.
- **Remove freezing:** This function will release all frozen trim of a contour. Automatic calculation of trim in the following processes will override the manually defined trim.

---

## Views

This includes all functions that change the layout of the A+W CAD Designer (Shapes) screen or the visibility of certain elements.

This menu also offers functions that allow to change the display of information. You can switch between sizes in inch or mm, or you can update the current sketch after re-dimensioning.

Menu **View** offers the following functions:

- **Show sizes:** Function **Show sizes** offers the following options:
    - **Show all dimensions**
    - **Show dimensions from this view:** Shows only the dimensions defined in the current view. The **Edgework** view only shows the text entered there. View **Inside contours** will only show the dimensions between contours. Sizes from the Sketch view will be missing, which makes work easier if there are many inside contours to be dimensioned.
    - **Show essential dimensions only:** This function omits obvious dimensions that were required for dimensioning. Obvious dimensions are for example information on parallel contours or segments, or right angles between those, as well as distances between contours with a value of 0 (necessary entry for aligning two contours, e.g. for notches). If there are several identical sizes, only one will be shown.
    - **Show no dimensions**
    As the first and last function are self-explanatory, we are going to describe only the second and third option.
- **Check dimensions:** This function is available in all views in which contours can be positioned (e.g. internal contours). This function allows to check whether the sizes defined for the positioned contours are sufficient, contradictory, or clear. A+W CAD Designer (Shapes) also checks if there is cyclic dimensioning, and issues a warning in this case. Incorrect sizes are shown in colour.
> **Avoid waiting periods.**
> Use this function if you have entered extensive dimensions, or if you go to another view. This will help to avoid long waits in which A+W CAD Designer (Shapes) tries to solve mathematical conflicts.
- **Show selection:** This function shows the tagged objects in the optimum size. This allows to view a small segment in maximum size and edit it, e.g. to move a point in view Revision.
  ⇨ Tools, "Smoothing the contour" on page A-233
  If no segment has been tagged, all objects on the drawing board will be combined and shown in maximum size.
- **Show all:** This function shows your sketch(es) in optimum size. This is useful if you have zoomed your sketch in and out several times, and want to return to the overall view.
- **New sketch:** Use this function to make A+W CAD Designer (Shapes) reorganize the drawing board. All entered dimensions will be analyzed; the contours will be adapted and positioned accordingly. In the Sketch view, this menu will tell you whether your contour is sufficiently dimensioned.
  ⇨ Tools, "Creating and dimensioning of sketches" on page A-229
- **Update BOM:** If you add more contours (e.g. drilled holes) to a SN file with a BOM, A+W CAD Designer (Shapes) will update the BOM only if necessary. Use this function if you need an updated BOM of the file. This function will be automatically performed when you save the file, or return to a linked order processing system.
- **Internal contours:** Use this function to show or hide inside contours.
- **Execute corners when cutting:** This function allows you to suppress the execution of corner rounding and corner cut-offs in the cutting process for each shape. If a glass purchase order is placed and corner rounding/corner cut-offs are subsequently produced internally on the product, this is taken into account when generating SN files. In this case, the cutting view may be used to determine the geometry of the purchased part. Therefore, corner rounding and corner cut-offs are not carried out in the cutting process. When creating SN files from OrderXML, this information is stored in the SN file.
- **Settings:** This menu serves to define settings that may change in the course of the program. Basic settings that will not change while working with A+W CAD Designer (Shapes) are made in the configuration file sn.ini. All menu items except the last offer sub-menus.
  ⇨ Tools, "Select measure" on page A-509
  ⇨ Tools, "Show critical points" on page A-510
  ⇨ Tools, "Show measuring points" on page A-511
  ⇨ Tools, "Enter segments" on page A-512
  ⇨ Tools, "Show critical points" on page A-510
- **Tools:** The entries in sub-menu **Tools** allow to show and hide the different tool dialogs.
  ⇨ "Tool bar" on page A-199

### Tool bar
**View > Tools > Tool bar**

**Fig. A-156:** Tool bar

The tool bar offers the most frequently used functions from menus **File** and **Edit** as well as the zoom tools and the call for program information.

### Tools
**View > Tools > Tools**

**Fig. A-157:** Tools

Depending on which view you are in, A+W CAD Designer (Shapes) shows the useful (and configured) tools. For a description of tools, see:

**Additional information**
- ⇨ Tools, "Tools for contour input" on page A-213
- ⇨ Tools, "The Use of Tools" on page A-212

### Select edge
**View Edgework > tool Special edge > Click on a segment > [OK]**

**Fig. A-158:** Select edge

If your installation allows to use different special edges, you can use this dialog to define the special edge to be applied to the tagged segment of the contour.
