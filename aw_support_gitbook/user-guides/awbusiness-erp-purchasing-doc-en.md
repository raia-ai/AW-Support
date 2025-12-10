---
description: "EN_AWBusiness_Purchasing_3_30_2-3"
---


---
## Electronic document exchange

### Document exchange

Order confirmations and invoices can be exported and imported in openTRANS format. This format has been extended for A+W Business. Documents can also be imported in standard format and XML files however.

Exchanging data in openTRANS format requires that the customer/supplier has the same A+W Business versions installed as you have, at least A+W Business 5. The parameters in the interface management have to be defined in the same way at the customer/supplier as in your A+W Business system.

### Document export

The export of order confirmations and invoices are configured separately for each customer/supplier in the module **Master data > B2B**. You have to define whether and which documents are to be exported, and which mode is to be used.

*(Fig. D-95: Settings for electronic data exchange)*
*   **A Export mode:** Selection of export to a file or via email.
*   **B Export format:** Standard (based on openTRANS).
*   **C Selection of documents:** Checkboxes to enable export for order confirmations, invoices, and dispatch notifications.
*   **D Settings for email mode:** Options to use special email addresses for different document types.

**Export mode (A):**

*   **Automatic email dispatch:**
    There has to be an email server in the network for this purpose. The email address defined in customer/supplier master data will be used by default. Different email addresses can be defined for order confirmations and invoices.

*   **Saving in a certain directory (on the server):**
    These files can be transferred manually afterwards.

Whenever an order confirmation or an invoice is printed, the program checks whether there are documents with the code for the export flag. The actual export is performed at regular intervals by a service in the background. The corresponding documents are shown in the Export dialog for control purposes. The following files are created as part of the export process:

*   `RESPONSExxxx.awotres` for order confirmations.
*   `DISPATCHxxxx.awotdis` for a delivery notification.
*   `INVOICExxxx.awotinv` for invoices.

File names are case sensitive.

### Document references

Document references on item level are necessary for the automatic allocation (reference) of order items and the corresponding P.O. items (referencing). At manual order entry, these document references are automatically created from the fields **P.O. text1** in the order header and **Customer item** at item entry.

*(Fig. D-96: Reference for data exchange)*
*   **A Header data - Document:** P.O. text field.
*   **B Items - Item tab:** Customer item and Reference fields.

Plus, this requires that the option **Adopt P.O. text1 and customer item for document references** is active in company data in the Parameters tab.

*(Fig. D-97: Company data – Parameters showing the option 'Adopt PO text 1 and customer item for document references'.)*

### Document import

Order confirmations and invoices in openTRANS format are imported by means of the A+W openTRANS ImportTool. It is installed on the A+W Business client by default.

This is why there are different import options:
*   Double-click on the saved file.
*   Double-click on the file sent as an email attachment.

Double clicking imports the data into the database where it can be displayed in A+W Business's import dialogs.

If the files are stored on the hard disk, you can use the context menu to start the option **Display** and display a generic view of the document.

### XML files

XML files cannot be imported directly from the email client. These files have to be saved first. After that, they can be imported by means of the context menu, or displayed as a generic view.

When a document has been successfully imported, it is available in the **Electr. price control** or **Electr. invoice control** dialog.

### Document check

The **Price control** and **Invoice control** dialogs have the same structure.

*(Fig. D-98: Electronic invoice control dialog)*
*   **A Imported document:** The list of imported documents (invoices).
*   **B Display and filter settings:** Options to filter the displayed documents.
*   **C Status:** Information about the referencing status (e.g., missing items, price/quantity differences).
*   **D Referenced documents:** The list of P.O.s linked to the selected imported document.

In both dialogs, all documents (D) that are linked with the imported document (A) are shown – including possible partial deliveries. For every purchase order, there is an optical signal (C) which tells you whether the links between the purchase order and imported document are complete. Only completely referenced documents can be accepted.

When the imported document has been accepted, the status of the reference purchase orders is changed accordingly. Price or invoice control cannot be run again afterwards.

**Booking types**

When you check the imported documents, the options **Accept**, **Create partial delivery**, and **Reject** are offered depending on the status.

Booking type **Accept** is only available if an imported document is complete and correctly referenced. If only the ordered quantities are not fully referenced while the document is otherwise complete, a partial delivery can be automatically created with this booking type.

### Item allocation

If the P.O. references are incorrect or missing from an openTRANS document, the system cannot automatically link document and P.O. items. These (unlinked) items are marked on the item list and have to be linked manually.

In an invoice, the reference with an item can be missing or incorrect for instance. Based on the product names, you can set these references in the **Manual item allocation** dialog.

### Footer surcharges/discounts

Footer surcharges or discounts are usually not entered in the purchase order. They do appear on the order confirmation or on the invoice however. To perform invoice control, these items have to be subsequently added to the purchase orders. P.O. entry can be accessed from the Invoice control dialog for this purpose. After the surcharge has been entered in the P.O., it has to be allocated in the invoice.

If your supplier has collected several purchase orders in one invoice in which the footer surcharge/discount appears just once, this item can be distributed to all linked purchase orders. Based on the surcharge basis, the program tries to find - and suggests – reasonable values for the proportional amounts. These values can be changed.

Based on the product number, the footer surcharges/discounts can also be allocated automatically for this supplier. The allocation of the supplier's product number to your own product number will be saved.

### Collective invoices in A+W Business

If collective invoices are issued in A+W Business, the footer surcharges/discounts are shown as individual items for every order. Since direct manual allocation is often difficult, you can collect several document items in this case, and allocate them to the P.O. items. In the item overview, it is then only listed as a combined document item.

### Differing amounts

You can usually accept an invoice only if no differences are found. If you (are to) expect different amounts from a supplier, you can handle this in various ways:

*   You can reject the invoice and inform the supplier of the discrepancies (by phone).
*   Different amounts can also be caused by different rounding methods. Option **Accept different amounts** allows for invoice control to be performed despite such discrepancies. The difference may only be a matter of cents. You should use the option **Notification of price difference/balancing item** to be made aware of this.
*   Rounding differences in the scope of cents can be accepted automatically. You have to create a so-called **balancing product** to which the difference can be booked.
*   The function **Prod.no. for balancing item** can be used to select a product to which the rounding differences (if they are just a matter of cents) are to be booked.

### Check the services

The following services must be installed and running:

*   **A+W Business 6 Interface Service**
    This service is usually installed on a separate computer. When it is installed by a member of the A+W Software GmbH service team, the function **Interface Service handles B2B documents** must be enabled.
*   **AWProtocolService**
    This service can be found in **System control > Management > Services**.
*   **ERP-WebService**
    This service is found in **System control > Computer management > Services and applications > Sites > Default web site**.

*(Fig. D-99: Check ERP service in Computer Management)*

The services are usually installed together with A+W Business. They are set to the start mode **Automatically**. They should start automatically when you turn on your computer.

If the data exchange does not work, you should check the services and start them manually if necessary. Instructions for this can be found in the operating system's online help.

You will also need the **A+W openTRANS ImportTool** which is automatically installed by the A+W Business setup.

### Status allocation

The status of the documents is also changed during import and export. For this, the following status points need to be assigned.

| Status Points for import | Status Points for export |
| :--- | :--- |
| 61 - Do not accept order confirmation | 830 - Invoice export |
| 64 - Do not accept invoice | 840 - Export of order confirmations |

During import, the status is changed manually and during export it is changed automatically.

The status points and status allocations are described in detail in the Master data section. This unit therefore only deals with the peculiarities you have to consider in connection with the electronic exchange of documents.

### Check the default settings for data exchange

> **Reboot A+W Business**
> After changing company data, reboot A+W Business.

The settings for exchanging product data have to be made correctly in company data. Documents can be imported correctly only if the corresponding product data has been entered and allocated.

**How to check company data**

1.  Select the menu **Master data > Company > Company data** and go to the **Parameters** tab.
    *(Fig. D-100: Company data – Parameters tab)*
2.  Tick the checkbox **Adopt P.O. text1 and customer item into document references**.
3.  Go to the menu **Start > Save** to save the changes. The data is saved.

### Check the currency settings

The international currency code must be stored for the currencies used in the orders and purchase orders. You have to check the settings if you are using several currencies.

**How to check currency settings**

1.  Select **Master data > Finances > Currency**.
    *(Fig. D-101: International currency code settings)*
2.  Every currency has to be assigned an international currency code (B).
3.  Select the line of the currency that you want to assign the code to.
4.  Open the combo box in the column **Internat. code** and select the appropriate code from the list.
5.  Check each exchange rate (A) entered and update them if required.
6.  Go to the menu **Start > Save** to save the changes. The data is saved.

### Check status definitions

Status points 61, 64, 830, 840 must be defined and assigned in order to process electronic documents. These status points are required for the following actions:

*   Import and export of documents.
*   Rejecting or accepting an imported document.

For instructions on this subject, please see:
*   "How to check the status points" on page D-161
*   "How to check the status management" on page D-161
*   "How to check the status allocation" on page D-163

**How to check the status points**

1.  Select the menu **Master data > Order > Status points**.
    *(Fig. D-102: Status points dialog)*
2.  Check whether status points 61, 64, 830 and 840 exist. The numbers of the status points are stated in the **Code** column.
3.  Status points are normally created during installation. They always have to be allocated manually.
4.  If not all of these status points exist, enter the missing ones.
5.  Go to the menu **Start > Save** to save the changes. The data is saved. The status points must be assigned a corresponding user status.

**How to check the status management**

1.  Select the menu **Master Data > Order > Status management**.
    *(Fig. D-103: Status management dialog)*
2.  If the user status for 61/64 and 830/840 do not exist in full, enter the missing ones.
3.  Go to the menu **Start > Save** to save the changes.
4.  Then check whether all allocations are available and complete.

**How to check the status allocation**

1.  Select the menu **Master data > Order > Status allocation**.
    *(Fig. D-104: Status allocation dialog)*
    *   **A Status point:** The selected status point from the list.
    *   **B Document type:** The document type the status applies to.
    *   **C Allocated user status:** The user-defined status linked to the system status point.
2.  Check whether status points 61, 64, 830 and 840 are allocated. If you select a status point in the **Status allocation table**, the status allocation must at least show the user status (C).
3.  If these status points have not been allocated in full, catch up on the allocations.
4.  Go to the menu **Start > New** to switch to the input mode.
5.  Select the appropriate entries in the fields **Status point**, **Document type**, and **User status**.
6.  Go to the menu **Start > Save** to save the changes. The data is saved.

### Set the data export via openTRANS

You must define how data should be exchanged in the module **Master data >B2B**.

**How to define the export type for openTRANS**

1.  Go to **Master Data > B2B > Customer > Document export**. The openTRANS document export dialog opens with the **Selection** tab.
2.  Go to the menu **Start > Search** to import the customers. The customers are listed in the **Table** tab.
3.  Select the customer (C) with whom documents shall be exchanged in openTRANS format.
4.  Go to the **Selection** tab.
    *   If the information for the customer is correct, you can proceed to the next customer.
    *   If there is no information, you must enter it.
    *(Fig. D-105: openTRANS document export dialog)*
5.  Go to the field **Type (B)** and select the entry **Standard (openTRANS-based)**. With this setting, documents intended for this customer will automatically obtain the code for openTRANS exchange.
6.  Go to the field **Export type (A)** and define how the files shall be exchanged.
    *   **Export to a file:** This setting means that the data will be saved in a file. The fields for the target path are released. You can select a directory or enter the path manually.
    *   **Export via email:** This setting means that the data will be attached to an email. You have to check whether the email address has been defined correctly in the customer master data.
7.  Define whether order confirmations and/or invoices (D) shall be exported.
8.  If the data is sent by email, different email addresses (E) can be entered for order confirmations, invoices and/or delivery notifications.
9.  Go to the menu **Start > Save** to save the changes. The data is saved.
10. Repeat the steps 3 to 9 for all customers with whom you exchange data.

No additional settings are required for importing order confirmations and invoices from your suppliers.

### Check Partner Master Data

The communication details must be correctly defined in supplier/customer master data to make sure that documents can be directly dispatched from A+W Business.

**How to check supplier/customer data**

1.  Go to the menu **Master data > Market partners > Supplier, customer > Suppliers, customers**.
    *(Fig. D-106: Partner data - address tab showing email address)*
2.  Check whether the email address of the supplier/customer is correct. If your supplier or customer has more than one email address, you can enter alternative email addresses in the document exchange settings. (See "Set the data export via openTRANS" on page D-164)
3.  Go to the **Order** tab and check whether the external number has been entered.
    *(Fig. D-107: Partner data - order tab showing external number)*
    This number has the following meaning in the customer and supplier data:
    *   **Supplier data:** You can get the external customer number from your supplier. It has to be entered even if it is the same as your internal number.
    *   **Customer data:** In the customer master data, this field must show the number your customer uses for you as a supplier.
4.  Go to the menu **Start > Save** to save the changes.

### Import of electronic documents

You can receive electronic documents in two different formats: as an openTRANS file or as an XML file. Depending on the settings in your company, these files are saved in a certain directory on the server or are available as an email attachment.

**How to import an openTRANS document**

1.  Open the directory with the sent files or the email to which the file had been attached. An openTRANS file has the suffix `*.awotdis`, `*.awotres` or `*.awotinv`.
2.  Double-click on the file to start the import. The data will be loaded and will appear in the dialogs for electronic price or invoice control.

**How to import an XML document**

1.  Open the directory with the sent files or the email to which the file had been attached.
2.  Save the XML file on your computer.
3.  Select the file in the Explorer and open the context menu.
4.  Select the option **Import as openTRANS document**. The data will be loaded and will appear in the dialogs for electronic price or invoice control.

### Check the electronic document

In documents imported from your suppliers, you can check the prices in both the order confirmation and in the invoice. Two dialogs are available for this purpose which are identical in structure and function:
*   Electronic price control
*   Electronic invoice control

We are going to describe the steps now, using electronic invoice control as an example.

**How to check and accept an imported supplier's invoice**

1.  Go to the menu **Documents > P.O.s > Invoice > Electr. invoice control**.
    *(Fig. D-108: Electronic invoice control – Document import)*
    *   **A Options for the booking type:** Reject, Accept, Create partial delivery.
    *   **B Restriction of the display:** e.g., Only open documents.
    *   **C Status of the selected document:** Information on discrepancies.
    *   **D Information on discrepancies:** List of issues found.
    *   **E Filtering the shown documents:** Button to open filter settings.
    *   **F Referenced documents:** List of P.O.s.
2.  Restrict the view if too many documents are shown:
    *   Select the entry (B) to view **Only open documents**.
    *   Click on the (E) button and set the desired filters. From the **Filter settings** dialog you can select several suppliers and accept them by pressing [OK].
3.  Select one of the displayed invoices.
4.  The list **P.O.s/partial deliveries (F)** shows all purchase orders which belong to this invoice. The section **Document status (C)** tells you whether references are missing and/or if there are differences in price or quantity.
    *   If you are not going to accept price differences, select the option **Do not accept (A)** and return the invoice to the sender. The document will be marked as rejected and can be archived.
    *   The following steps explain how to correct differences.
    *   Establish the missing references. (See "How to allocate items in an imported invoice" on page D-171)
5.  Go to the **Item overview** tab if required in order to check the differences in the purchase prices of individual items.
    *(Fig. D-109: Electronic invoice control - Item overview)*
    If there are divergences due to different rounding methods, you can accept them in general via the menu **Options > Accept different amounts**. In this case, you can choose the booking type **Select** or **Reject**.
    You cannot correct the item prices and quantities directly.
6.  Select the item you want to correct.
7.  Select the menu **Functions > Open P.O. creation** and correct the quantity. When you close a P.O. entry after correcting and saving the differences, the new values will appear in the electronic invoice control.
8.  You do not need to correct price differences manually. You can just accept the document despite these differences. The program will make the necessary corrections automatically.
9.  When all errors have been corrected, select the option **Accept**.
10. Go to the menu **Start > Save** to close the invoice control. The data is saved, and the status of the purchase order(s) changed. Invoice control cannot be run again for this document after that.

### Create a partial delivery from an electronic document

You can create a partial delivery if the imported document includes only part of the P.O. items or of the ordered quantities.

**How to create a partial delivery for an imported supplier's invoice**

1.  Go to the menu **Documents > P.O.s > Invoice > Electr. invoice control**.
2.  Select the invoice for which you want to create a partial delivery. You can create a partial delivery if the document status does not show any other errors except quantity differences. The option **Create partial delivery** is available only if this is the case. The process of creating missing references is described in "How to allocate items in an imported invoice" on page D-171.
3.  Select the option **Create partial delivery**.
4.  Go to the menu **Start > Execute** to generate the partial delivery. This creates a partial delivery with the invoice number, the delivered quantity and the prices from the imported document. The status of the original purchase order is changed accordingly.
5.  The original purchase order can be reallocated until all items have been delivered in full and referenced.

### Allocate items in electronic documents

The item cannot be allocated if the references in the electronic document are not clear. You can make up for this allocation when checking the document.

If an item is completely missing from the purchase order, e.g. an energy surcharge, you have to enter this item in the corresponding purchase order first. You can open the purchase order from price/invoice control for this purpose. When you have entered and saved the item, proceed with invoice control.

**How to allocate items in an imported invoice**

1.  Go to the menu **Documents > P.O.s > Invoice > Electr. invoice control**. The (Electr.) Invoice control dialog opens and the imported invoices are displayed.
2.  Mark the invoice for which you would like to allocate items.
3.  Go to the **Item overview** tab. You can add an item to the purchase order at a later stage by opening the document via the menu **Functions > Open P.O. entry**. When you have entered and saved the item, proceed with the invoice control, step 4.
    *(Fig. D-110: Electronic invoice control - Item overview)*
4.  Select the item that could not be allocated and go to the menu **Functions > Allocate items manually**.
    *(Fig. D-111: Electronic invoice control - Allocate items dialog)*
    *   **A Item from the invoice:** The list of items from the imported document.
    *   **B Retain allocation of the footer surcharge for the current session:** Checkbox option.
    *   **C Save the allocation of the footer surcharge for all future imports:** Checkbox option.
    *   **D Item in the purchase order:** The list of items from the referenced P.O.
5.  From the left and the right list, select the items (A, D) you want to be allocated.
6.  Click on **[OK]** to save the allocation.
7.  Repeat the process until all items have been allocated. If you have allocated footer surcharges/discounts you can use the checkboxes (B, C) to define whether the allocation shall be maintained for this invoice and/or this supplier. How you distribute a footer surcharge/discount to several purchase orders, is described in: "Allocate surcharges/discounts manually" on page D-172.
8.  Click **[End]** if all allocations are correct. All booking types are available in the **Electr. invoice control** dialog.
9.  Select the desired booking type, e.g. **Accept**.
10. To start the activity, go to the menu **Start > Execute**.
11. Go to the menu **Start > Save** to save the data. The data is saved, and the status of the purchase order(s) changed.

### Allocate surcharges/discounts manually

If an invoice shows just one footer surcharge/discount for several purchase orders, you can distribute it manually to the individual purchase orders and/or P.O. items. The surcharge/discount will be calculated proportionately and saved in the purchase orders.

**How to distribute the footer surcharge/discount to purchase orders**

1.  Go to the menu **Documents > P.O.s > Invoice > Electr. invoice control**. The **Electr. Invoice Control** dialog opens and the imported invoices are displayed.
2.  Select the invoice from which the footer surcharge/discount is to be distributed. The list **P.O.s/Partial deliveries** shows all reference documents.
3.  Go to the menu **Functions > Distribute footer surcharges/discounts to P.O.s**.
4.  Hold down the `<Ctrl>` key and select all of the items which you would like the surcharge/discount to be distributed to.
5.  Click on **[OK]** to save the distribution. The data is saved in the respective purchase orders. The purchase prices in the purchase orders will be updated.
6.  Close the dialog using **[End]** and proceed with invoice control. (See "How to check and accept an imported supplier's invoice" on page D-168)

### Additional information

*   Software Reference, "Electronic price control" on page D-211
*   Software Reference, "Electronic invoice control" on page D-254
*   Software Reference, "Manual allocation of items" on page D-219
*   Master Data, "Handling of Business Processes" on page B-413
*   Master Data, "Company Data – Parameters" on page B-914

## Data export/import (EDI)

**Objectives**
*   Learning about the function of the external interface
*   Learning about the default settings for data exchange via the EDI interface

**Benefits**
*   Thanks to data exchange via EDI interfaces, documents do not have to be entered manually.

**Please note:**
*   **EDI:** EDI = Electronic Data exchange, electronic data exchange via ASCII file
*   **Interfaces:** Interfaces have to be implemented for customers and suppliers.
*   **Default settings:**
    *   Company data: Stock/PP/EDI tab
    *   B2B: Customer, supplier

### Data exchange in ASC format

The EDI interface serves for exchanging quotations, orders, purchase orders, and credit notes. The data is saved in an ASC file (ascii). Define the path for this file for each customer and each supplier.

The data of the file to be transferred are automatically converted to ANSI format by default, e.g. `ä` becomes `ae`.

### Check company data

In company data (in the **Stock/PP/EDI** tab), you have to check the default settings which refer to the conversion.

*(Fig. D-112: Company data – Stock/PP/EDI tab, showing the option 'Disable OEM/ANSI conversion')*

OEM/ANSI conversion should be disabled only if the interface you are using requires this specifically.

### Check the settings

If you exchange orders and purchase orders in the ASC format with your suppliers/customers, you must set the parameters for each individual supplier/customer.

**How to check the settings for data export via EDI**

1.  Select the menu **Master data > B2B > Supplier > Supplier**. For data import via EDI, select **Master data > B2B > Customer > Customer**. The following steps apply likewise.
2.  To start the search, go to the menu **Start > Search**. The list of matches is shown on the **Table** tab.
3.  Select the supplier who shall receive purchase orders via the EDI interface.
