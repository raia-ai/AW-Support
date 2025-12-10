---
title: "EN_AWBusiness_Sales_4_1-3"
source: "EN_AWBusiness_Sales_4_1-3.pdf"
tags: ["A+W Business Sales", "order entry", "document management", "tutorial", "ERP", "item management", "BOM", "CAD integration", "pattern entry", "feasibility checks"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial section from the A+W Business Sales manual covering comprehensive document entry. It details procedures for deleting orders, entering and formatting text, attaching documents, and managing order items, including bills of material, shapes, and patterns."
long_description: "This document is a detailed tutorial from the A+W Business Sales software manual, focusing on the 'Comprehensive Document Entry up to the Invoicing Stage.' It provides step-by-step instructions for various document and order management tasks. The guide begins with searching for and deleting orders, outlining the conditions and user rights required. It then moves to text entry, explaining how to add standard or new text to order headers, format it, and complete it with hyperlinks, images, or tables. The document also covers attaching external files to orders. A significant portion is dedicated to 'Order Items,' detailing objectives, benefits, and procedures for item entry. This includes an overview of the item entry dialog, feasibility checks, and the use of icons and buttons for various functions like BOM management, price calculation, and CAD integration. The tutorial explains how to manage products within an order item, including bills of material (BOM), fixed articles, shapes, grill patterns, and applying visual patterns to sheets. It provides instructions on integrating with A+W CAD Designer for custom grill patterns and describes the dialog structure for pattern entry."
---

# Tutorial: Comprehensive Document Entry up to the Invoicing Stage

4.  To start the search, select **Search** in the menu **Start > Search**.
    If you are searching by means of the customer number, the system will list all orders of this customer in the **Documents list (C)**.
5.  Select the order you were looking for.
    If you have been searching for the order by means of the order number, it will be directly displayed in the **Document** tab.
    You can now edit or copy the document.

---
## Delete order

You can delete an order and its items only if the order status is over **990** (released for deletion). Usually, it will have already been transferred to archives and statistics by this point.

The right for deletion can be taken away via the user rights. These settings can only be defined by an administrator.

> **Automatic deletion**
> Documents can be automatically deleted after archiving. This function is described in the Master data section.
>
> ⇨ Master Data, "Company Data > Archives" on page B-962

If the order cannot be deleted, its status must be manually set to **Released for deletion**.

### ■ How to delete an order

1.  Open the order you want to delete.
2.  Check its status and set it to 'released for deletion' if necessary.
3.  Go to the menu **Start > Delete**.
    The document will be deleted.

## Enter text

Use this function to enter text for a document. You can enter new text or add standard text and complete it.

Go to **Master data > Forms > Management of forms** to exclude text from being printed on certain forms.

### ■ How to enter standard text in the order header

1.  Open the order for which you want to enter text, and go to the tab **Text/Attachments**.
    
    *(Fig. C-13: Enabled fields for text shows a user interface with sections for A: Insert text, B: Text number, C: Format text, and D: Edit text.)*

2.  Click on the button **(A)** to insert text.
3.  Select the required standard text from field **Number (B)**.
    The text is displayed in the **Text block (D)** section.
4.  You can change or complete the text as required, e.g. a validity date.
    > **Note:** Changes apply to the current order only. They are not saved in the standard text.
5.  Repeat the steps 3 and 4 to add more text.
6.  Go to the menu **Start > Save** to save the text.
    The text will be saved.

> **Fonts and type size**
> You can change the fonts and type size (C). These settings only apply to the current document.

### How to enter new text in the order header

1.  Open the order for which you want to enter text, and go to the tab **Text/Attachments**.
2.  Click on the button to insert text.
    The fields will be enabled.
3.  Enter the number **0** in the **Number** field.
4.  If required, you can adjust the text code if the text is only to be printed on certain forms.
5.  Enter the text in the **Text block** section.
    This text will only be used for this order. If you need the same text frequently, you should create it as a standard text.
6.  If required, format the text as described in the next activity sequence.
7.  Repeat the steps 3 to 5 to insert more text.
    You can allocate a different text code to each text, depending on the documents on which the text is to be printed.
8.  Go to the menu **Start > Save** to save the text.
    The text will be saved.

> **Text per item**
> You can enter text in the same way for every order item at item entry.

### How to complete and format a text

1.  Open the order for which you want to enter text.

The following steps apply in the same way to all texts that you insert in a document or in the **Master data** module as standard texts, in the partner master data or in the product master data.

We assume that you are familiar with changing fonts, font style and size (formatting). The buttons for these changes correspond to those of common text processing systems.

In addition, A+W Business offers the following buttons:

*(Fig. C-14: Text tools shows icons for A: Insert hyperlink, B: Remove hyperlink, C: Insert image, D: Insert table.)*

Please note the following:

*   **Hyperlink:**
    Mark the word with which you want to link and click on the button **(A)** and enter the path.
    You can copy and enter the path to an external file from the address bar of Windows Explorer.
*   **Image:**
    Click on the button **(C)** and select the file.
*   **Table:**
    First, enter the complete text and leave an empty line for the table. Then insert the table here.

## Attaching documents

In the order header and at item entry, files of any format can be saved, e.g. the scanned original order. These files can be opened in the corresponding dialog. Prerequisite is that the appropriate program has been installed, e.g. Acrobat Reader for reading PDF files.

### How to add an attachment

1.  Open the order to which the file shall be attached, and go to the **Attachments** tab.
2.  Open Windows Explorer up to the directory in which the file you want to attach is saved, e. g. customized price agreements.
3.  Select the file in Windows Explorer and move it by Drag & Drop (hold down the mouse button) to the order.

    *(Fig. C-15: File attached shows an interface with a file path C:\temp\2013\Order\20287\prices_2013.csv listed under the Attachments tab.)*

4.  A copy of the file is saved in a separate directory, e. g. with the customer or supplier number.

> **File per item**
> You can attach a file in the same way to every order item at order entry.

## Exercises

**Enter order header**
*   Open an order header.
*   Enable the option Adopt customer and enter an order for this customer.

**Enter order header for a second customer**
*   Disable this option and enter a completely new order header.

**Edit order header**
*   Open the order and change the following details:
    *   Enter a new shipping address.
    *   Enter a different invoicing address.
    *   Permit partial shipment and partial invoicing.
    *   Choose a different route.
    *   Enter standard text.

**Additional information**
*   ⇨ Software Reference, "Document - Header Data" on page C-413
*   ⇨ Software Reference, "Dates" on page C-416
*   ⇨ Software Reference, "Header data - Different addresses" on page C-420
*   ⇨ Master Data, "Status Allocation" on page B-886
*   ⇨ Master Data, "Company Data > Financial Accounting" on page B-923
*   ⇨ Master Data, "Raise status when credit limit is exceeded" on page B-935

## Order Items

### Objectives

*   Getting familiar with the dialog for item entry.
*   Getting familiar with details on items.
*   Checking the availability of products.
*   Getting familiar with the BOM structure.
*   Entering grills, shapes, processing steps, motifs and services.
*   Getting familiar with various methods of item entry.
*   Getting familiar with the rules of quick entry.
*   Answering quick inquiries.

### Benefits

*   You can add order items quickly and safely, avoiding incorrect input.
*   You can adapt the products defined in the master data to the customer's requirements in the order item, e. g. by adding grills, shapes, processing steps or motifs.
*   By means of quick entry via numerical entries, an identical product structure can be entered faster than by means of selection and input fields.
*   You can answer telephone inquiries immediately, without having to close the current item entry dialog. Once you have finished the quick inquiry, you can simply continue working on the previous order.

### Please note:

| Term | Description |
| :--- | :--- |
| **Dialog structure** | Item entry is the same for all document types. |
| **Save document** | You can enter an item only if the document header has been filled out and saved. |
| **Product master data** | Item entry requires that products have been defined in master data. |
| **Main product** | Every product which is entered in the input line is called a main product. Bills of material can be attached to a main product. |
| **Item** | All products defined in the master data can be entered as order items and modified if required. |
| **Quick entry** | Order items can be entered with all details on glass replacements, grills, processing steps and shapes in numerical order. |
| **Dynamic input field** | This product data is entered according to defined rules. If you are using quick entry, you should also enable the option Dynamic product field. |
| **Quick inquiry** | While you are entering order items, inquiries from another customer regarding products and prices can be answered by means of quick inquiries, without having to close the item entry dialog for the first customer. Items entered via quick inquiry can be directly saved as a new order. |
| **Default settings** | Company data: <ul><li>Parameters tab</li></ul> |

## Controls in the item entry

The order item entry dialog offers the following elements:

*(Fig. C-16: Item entry dialog shows a complex user interface with multiple sections.)*

*   **A** Details of BOM
*   **B** Display of BOM
*   **C** Purchase prices per item
*   **D** Sales prices per item
*   **E** Price code
*   **F** List of order items
*   **G** Discount per piece
*   **H** Prices per piece
*   **I** Product search button
*   **J** Diagram of pane structure
*   **K** Symbol for saved text

### Menu bar

You can set checks and filters via the **Options** menu.

You can define for example the field on which the cursor shall be positioned when you open the dialog Document management. This option is useful if you have defined at the same time that the data of the last order entered for this customer is automatically entered.

Depending on your choice of options, the fields will be preset with certain data. These basic functions are described in the Quick Guide.

⇨ "User Interface" on page 1-6

### Quick help

In addition to the online help, a quick help is available at some points in item entry.

*(Fig. C-17: Quick help shows a tooltip labeled 'Min. calculation'.)*

*   **A** Tool tip

Access the online help using `<F1>`. For information on the online help, please refer to the Overview section:
⇨ Tutorial, "Online Help" on page A-57

### Item entry

In the item entry mode, all data can be entered using the number pad on the keyboard:

*   **Input mode:**
    *   The input mode for new items is automatically enabled when you open item entry for a new order.
    *   The input mode has to be started specifically once item entry has been closed: **Menu Edit > New**.
*   **Data input using the number pad:**
    *   `<+>` represents the `<Tab>` key.
    *   `<Enter>` creates a new line, using the data of the previous item.

You can also define the tab that shall be opened in item entry after the most important data has been entered. This selection is made in the menu **Options > Automatically go to tab**.
⇨ Software Reference, "Options menu" on page C-441

> **Fields in the list of items**
> You can select which fields are displayed and in which order. If you are using quick input, you should also enlarge the width of the Product column.

## Enabling the feasibility checks

A+W Business offers a number of feasibility checks; not all of them are automatically activated however. This would affect the data processing speed considerably. You should enable those however that help to avoid input errors in connection with complex orders.

For item entry, this includes the following checks:
*   Pricing errors
*   Missing sizes
*   Processing parameters

*(Fig. C-18: Feasibility checks shows a settings window with options grouped under A: Pricing errors, B: Sizes of panes, and C: Processing parameters.)*

## Icons for item entry

The item entry dialog offers the following icons:

| Icon | Meaning |
| :--- | :--- |
| **[Sun Icon]** | Outside referring to the sheet or unit displayed below |
| **[Sheet Structure Icon]** | **Sheet structure:** This image shows the schematic structure of a triple IG sheet with laminated glass on the outside, a patterned glass sheet in the middle, and a tempered glass sheet on the inside. The spacers are shown in between these sheets. This picture neither shows the glass thickness nor the spacer thickness. |
| **[Float Glass Icon]** | Float glass |
| **[Coated Float Glass Icon]** | Coated float glass |
| **[Tempered Glass Icon]** | Tempered glass |
| **[Laminated Glass Icon]** | Laminated glass |
| **[Patterned Glass Icon]** | Patterned glass |
| **[Text Icon]** | Text has been entered in the master data for this product. This text can be displayed at item entry in the Text tab. |

## Buttons at item entry

| Button | Function |
| :--- | :--- |
| **[Sense of Pattern Button]** | Changes the level of the pattern side or coating side. Level 1 is on the outside. |
| **[Sense of Pattern Button 2]** | Changes the sense of pattern. |
| **MIOSCF** | Enables or disables the corresponding price calculation: <ul><li>M: Minimum calculation</li><li>I: Individual price</li><li>O: Other surcharge</li><li>S: Stock size</li><li>C: Cost and surcharge calculation</li><li>F: Formula price</li><li>P: Production BOM explosion</li></ul> |
| **[Stock Info Button]** | Opens the Stock info dialog. |
| **[Insurance Prices Button]** | Opens the Insurance dialog. |
| **SN Editor** | Creates an SN file and starts the editor CAD Designer (Shapes). |
| **[Insert Text Button]** | Inserts text. The button is also available in Document management. |
| **[Delete Text Button]** | Deletes text. The button is also available in Document management. |

## Buttons in the Processing dialog

To define processing for a shape, you can use buttons to restrict the product selection to a certain product type. For every processing step, the system shows the fields in which the relevant parameters have to be entered.

| Button | Function |
| :--- | :--- |
| **< >** | Scrolls ahead and back in the catalog. |
| **[Shape Icon]** | Opens the selection dialog for the product group Shape. ⇨ "Shapes" on page C-69 |
| **[Stepping Icon]** | Opens the selection dialog for the product group Stepping. ⇨ "Enter Shape" on page C-110 |
| **[Edges Icon]** | Opens the selection dialog for the product group Edges. |
| **[Drilling Icon]** | Opens the selection dialog for the product group Drilling. |
| **[Rounded Corners Icon]** | Opens the selection dialog for the product group Rounded corners. |
| **[Notched Corners Icon]** | Opens the selection dialog for the product group Notched corners. |
| **[Slanted Corner Icon]** | Opens the selection dialog for the product group Slanted corner. |
| **[Edge Notches Icon]** | Opens the selection dialog for the product group Edge notches. |
| **[Inside Cut-outs Icon]** | Opens the selection dialog for the product group Inside cut-outs. |
| **[Speech Holes Icon]** | Opens the selection dialog for the product group Speech holes. |
| **[Handles Icon]** | Opens the selection dialog for the product group Handles. |
| **[Coating Icon]** | Opens the selection dialog for the product group Coating. |
| **[Frosting Icon]** | Opens the selection dialog for the product group Frosting. |
| **[Edge Stripping Icon]** | Opens the selection dialog for the product group Edge stripping. |
| **[Gluing Icon]** | Opens the selection dialog for the product group Gluing. |
| **[Screen Printing Icon]** | Opens the selection dialog for the product group Screen printing. |
| **[Bending Icon]** | Opens the selection dialog for the product group Bending. |
| **[Fluted Beveling Icon]** | Opens the selection dialog for the product group Fluted beveling. |
| **[Counter-sinking Icon]** | Opens the selection dialog for the product group Counter-sinking. |
| **[Regrinding Icon]** | Opens the selection dialog for the product group Regrinding. |
| **[Logo Icon]** | Opens the selection dialog for the product group Logo. |
| **[Edge Protection Icon]** | Opens the selection dialog for the product group Edge protection. |
| **[Macro (corner) Icon]** | Opens the selection dialog for the product group Macro (corner). |
| **[Macro (edge) Icon]** | Opens the selection dialog for the product group Macro (edge). |
| **[Enamel Icon]** | Opens the selection dialog for the product group Enamel. |
| **[Stepped Drilling Icon]** | Opens the selection dialog for the product group Stepped drilling. |
| **[Arch-shaped Notch Icon]** | Opens the selection dialog for the product group Arch-shaped notch. |
| **[Surface Enamel Icon]** | Opens the selection dialog for the product group Surface enamel. |
| **[Alarm Wire Icon]** | Opens the selection dialog for the product group Alarm wire. |
| **[Leaded Design Icon]** | Opens the selection dialog for the product group Leaded design. |
| **[Curved Glass Icon]** | Opens the selection dialog for the product group Curved glass. |
| **[Masking Icon]** | Opens the selection dialog for the product group Masking. |
| **[Decoating Icon]** | Opens the selection dialog for the product group Decoating. |
| **[Coloring Icon]** | Opens the selection dialog for the product group Coloring. |
| **[Edge Screen Printing Icon]** | Opens the selection dialog for the product group Edge screen printing. |
| **[Sand Blasting Icon]** | Opens the selection dialog for the product group Sand blasting. |
| **[Stamp Icon]** | Opens the selection dialog for the product group Stamp. |
| **[Macro (inside) Icon]** | Opens the selection dialog for the product group Macro (inside). |
| **[Parameterizable Macro (inside) Icon]** | Opens the selection dialog for the product group Parameterizable macro (inside). |
| **[Parameterizable Macro (edge) Icon]** | Opens the selection dialog for the product group Parameterizable macro (edge). |
| **[Heat Soak Icon]** | Opens the selection dialog for the product group Heat soak. |
| **[Article Icon]** | Opens the selection dialog for the product group Article. |
| **[Formula Text Icon]** | Opens a dialog for editing text in progress (formula). |

## Products in an order item

You enter items in quotations, orders and credit notes via the products that are defined in the master data. You can add order-specific details to the entered products, e. g. sizes, quantities, processing steps. You can also allocate spacer text.

*(Fig. C-19: Product structure changed in the order shows a comparison between a standard BOM from Master data (A) and a modified BOM in an Order item (B), where a spacer has been changed.)*

You can enter text for every order item. If you are using several clients, this is a means of conveying special information on this item. The text is added at item entry in the **Text** tab. This procedure has already been introduced in the module on the order header.
⇨ "Enter text" on page C-52

### Quantity

The entry in field **Qty.** refers to the following measures:
*   For glass: surface/pc.
*   For linear meter products: LM/pc.

This entry will be taken into account for pricing.

The quantity cannot be edited in the input line. This field is only enabled if you have activated the menu item **Options > Enter quantity for current item**.

## Bills of material

The actual product structure including processing steps is shown in the shape of a bill of material. You can replace, add or remove components and edit the production BOM. All production-relevant data will be transferred to production.

To define the product, open the corresponding dialogs by means of the icons and select the basic patterns for grills and shapes from the offered catalogs. Once you have entered the size, a product sketch will be displayed. You can see immediately whether your entries have created the required result. You can print sketches of the grill pattern as well as of the shapes.

You can enter processing steps and services for every item.

If you enter formulas in the size fields of the main product, these will be used to calculate the actual sizes in the order.

### Fixed articles

Frequently used product structures can be fixed at item entry. The following entries are possible:
*   Alpha-numerical, customized article number and name
*   Price and discount
*   Printing the customized article name

Fixed articles cannot be edited, except for the prices and discounts.

At item entry, the search via customized article number is applied only to the main article number, not to the BOM elements or replacement sheets.

## Shapes

In addition to the standard shapes, you can save individual shapes as SN files for CAD Designer (Shapes). These can be created directly from an order item, or you can enter them independently of any actual order.

Working with SN files will be introduced to you in a separate module:
⇨ "SN File and Template" on page C-167

You can change every order item, e. g. replace the sheets of an IG unit, add or remove grills, etc.

Shapes and grills are entered in separate tabs which can be accessed from item entry. The shape catalog offers a selection of standardized shapes; you only need to enter the required data.

In addition to grills and shapes, A+W Business allows you to enter processing steps, services, leaded designs and curved glass.

Numerous checks will be run at order item input so that incorrect or incomplete orders are virtually impossible.

By activating different options in item entry, you determine which check values are relevant to individual documents, e. g. check for sizes, quantities, consignment.

By default, it is impossible, for example, to save an order item if you have failed to enter sizes for a shape.

## Grill pattern

Grill grids can be entered in the first and second airspace of a triple IG unit. The position of the grill grid is freely selectable.

The number of vertical and horizontal grills can be entered as required. You can also enter diagonal bars and check them on the sketch.

Drilled hole sizes and the grill pattern will be checked automatically so that you cannot save incorrect patterns.

Sketches of the structure are automatically updated after every change so that the result can be checked during input.

## Integration of A+W CAD Designer (Bars)

The program A+W CAD Designer (Bars) offers the integrated entry of template grills which can be edited at item entry.

A+W CAD Designer (Bars) can be used to define free grill grid patterns and print them on A+W Business forms. The entered grills are transferred to production via the OrderXML interface where they can be integrated in the production process. Elements that are relevant for pricing will be recognized and calculated during the input:
*   Bar lengths
*   Fields
*   Edge connections
*   Connections (X, Y, L, T)
*   Sun and star pattern

The settings can be saved as macros and loaded if required.

### Calculation type for grill pattern

Grills can be entered symmetrically or asymmetrically with reference to the fields or drill points. You can enter individual sizes for the grill pattern so that drilled holes or fields are arranged asymmetrically.

In case of automatic calculation, you can define whether the symmetry shall be related to the drilled holes or to the fields.

**Example**

*(Fig. C-20: Symmetrical calculation of grill pattern shows two diagrams, one for "Drill hole-symmetrical" and one for "Field-symmetrical", illustrating the difference in measurements.)*

An edge length of 1000 mm and a grill width of 26 mm will produce the following values (without cutback):
*   **Drill hole-symmetrical:** Each of the drilled holes lies 333.3 mm away from the edges. The edge length of the outside fields is 307.3 mm while the central field has an edge length of 320.2 mm.
*   **Field-symmetrical:** Each of the drilled holes is 329.0 mm away from the edges, with a central distance of 342.0 mm. The edge length of the three fields is 316.0 mm.

## Grillpattern types

For the processing of windows with several fields, the connection between the grills is defined in addition to the edge stoppers. The following pattern types are defined by default:

| Type | Image | Description |
| :--- | :--- | :--- |
| **Type 1** | **[+]** | Grill with double miter at the crossing points |
| **Type 2** | **[+]** | Crossbars, horizontal and vertical grills have blunt connections to the crosspieces. |
| **Type 3** | **[+]** | Vertical grill continuous, horizontal grill with overreaching miter |
| **Type 4** | **[+]** | Horizontal continuous grill, vertical grill with overreaching miter |
| **Type 5** | **[+]** | Vertical grill continuous, horizontal grills with blunt connections to the vertical grills. |
| **Type 6** | **[+]** | Horizontal grill continuous, vertical grills have blunt connections to the horizontal ones. |
| **Type 7** | **[Isometric Grill]** | Horizontal and vertical grills are continuous. |

*(Tab. C-4: Grill pattern type)*

## Patterns

You can apply patterns to sheets in the item entry. A pattern is an image, e.g. a Formula 1 vehicle, which is applied to the sheet with a processing.

Patterns can be entered in the following product groups:

| Icon | Product Group |
| :--- | :--- |
| **[Coating Icon]** | Coating |
| **[Frosting Icon]** | Frosting |
| **[Screen Printing Icon]** | Screen printing |
| **[Surface Enameling Icon]** | Surface enameling |
| **[Sandblasting Icon]** | Sandblasting |
| **[Coloring Icon]** | Coloring |

*(Tab. C-5: Product groups for pattern entry)*

In order to enter a pattern, a pattern file must be saved in a directory that you can access. The file must be in one of the following formats: bmp, tif, png, gif, jpg or emf.

Patterns can be created in the product master data. There, the pattern is assigned various parameters, such as the screen number, the path to the directory in which the pattern file is saved, the maximum dimensions, and if necessary, a name.

Patterns with screen number and patterns without screen number differ as follows:
*   A pattern with screen number has a fixed size and is inserted using the screen number. It must be created in the product master data. The file path and maximum dimensions of the pattern are taken over from the master data. The size of the pattern can only be adjusted within the maximum dimensions. The pattern will not be scaled.
*   A pattern without screen number must be inserted via the file path. The size of the pattern can be specified freely. The pattern can be scaled proportionally.

## Dialog structure for pattern entry

*(Fig. C-21: Pattern entry - Dialog structure shows the user interface for applying patterns.)*
*   **A** Product structure
*   **B** Selection of the product group for the processing
*   **C** Parameters for the selected processing
*   **D** Front view of the sheet
*   **E** Side view of the sheet
*   **F** Preview

The product structure including the processings is displayed in the form of a BOM **(A)**. If a product consists of several sheets, you can choose to which sheet the pattern should be applied.

In the **Processing** area **(B)** select one of the above-mentioned product groups in order to enter the pattern.

In the **Parameter** area **(C)** you specify the pattern, size, and position of the pattern and assign a processed side to the pattern.

The preview window **(F)** displays a graphic view of the sheet as front view **(D)** and side view **(E)**. The graphic display with the pattern is updated on the preview window with each change of the parameters, so that you can check the result on entry.

## Entering a pattern

You can enter patterns in two ways:
*   With screen number
*   Without screen number

Patterns with specification of screen number are entered by entering the screen number of the pattern from the master data in the **Number** field. The **Pattern** field is automatically filled with the path of the pattern field that is stored in the master data.

Patterns without screen number are entered by entering the path of the pattern file in the **Pattern** field. The **Number** remains empty.

### Processed side for the pattern

*(Fig. C-22: BOM using the example of a triple IG sheet shows the BOM structure for a multi-layered product.)*
*   **A** Bill of materials (BOM)
*   **B** Product number
*   **C** Main product
*   **D** New BOM
*   **E** Sheet
*   **F** Processing

You can attach the pattern to the main product **(C)** or a sheet of the main product **(E)** by clicking on the corresponding BOM element. If you assign the new BOM element **(D)** a product number **(B)**, the symbol of the BOM element is adjusted, e.g. the symbol for a processing **(F)** is displayed if you select one of the product groups for the pattern entry.

In the **Parameters** area, on the **Processed side** combo box **(B)**, you can select whether the pattern should be applied on the outside or inside of the sheet. Here, a distinction is made between processings that are attached to a single sheet and processings that are attached to the main product as follows:

*(Fig. C-23: Processing (attached to sheet) shows an interface with a preview of a sheet with two different patterns applied.)*
*   **A** Processing (attached to sheet)
*   **B** Level to which the pattern is applied
*   **C** Screen printing on the outside of the float sheet
*   **D** Coating on the inside of the thermo sheet

If the processing **(A)** is attached to a single sheet of the main product, you can select whether the pattern should be applied on the outside or inside of the marked sheet:
*   **Level 1:** The pattern is applied to the outside of the selected sheet
*   **Level 2:** The pattern is applied to the inside of the selected sheet.
