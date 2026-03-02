---
description: "EN-UM-AWBusiness_2"
---


# Tutorial 1: Customer Data

---
## Address Data

### Objectives
- Going through the Partner management dialog
- Defining and allocating customer groups
- Defining and allocating routes and delivery terms

### Benefit
- Customer master data are centrally entered and maintained. New orders are therefore always based on up-to-date master data.
- Address data are used for dispatch and invoicing. Alternative addresses can be entered if required.

### Note

**Partner management**
Dialog Partner management serves to enter the master data for every customer which apply just for this partner.

**Address**
A main address is entered for every partner which is generally used for shipments and invoicing.

**Line of business**
The line of business is an additional analysis and sorting criterion for statistics.

**Language**
Documents are printed on the forms that fit the customer's language and customs.

**Groups**
Customers can be assigned to a customer group, e.g. for collective maintenance of prices or discounts.

**Route**
Routes are the basis for dispatch planning and control. The shipping date is determined by means of the delivery time and the delivery date.

## Address Settings

Tab Address serves to enter the data for the address, communication, and dispatch.

**Fig. B-9**: Dialog Partner management – tab Address
- **A**: Address date for the order header
- **B**: Contact data are completed by the settings on tab Order > Document dispatch
- **C**: Section Specifications: Selection and input of the appropriate details

We are going to explain the settings on this tab in closer detail in the following paragraphs.

### Lines of Business
Every customer and supplier can be allocated to a line of business, e. g. glass dealer, window manufacturer, joiner. If a new customer belongs to a line of business which has not been defined before, you can use the file icon to go to dialog Lines of business to enter the new line of business.
The line of business is an additional analysis and sorting criterion for statistics.

### Language
Every customer is allocated the language in which documents and forms shall be printed. The appropriate forms will be selected based on this code.
If you define additional languages you should also translate the price units and quantity units.

### Groups
Partners can be united in groups. Every customer can be allocated to a customer group and every supplier, to a supplier group.
When you enter e. g. discounts or prices for a group, these terms will apply to all members of the group. This makes the maintenance of terms easier.
When you enter a document, the settings which are based on the allocated group, can be changed in the individual fields.

**Examples for the use of groups**

| Category | Use Cases |
| --- | --- |
| **Customer group** | - Marginal income limits<br>- Prices<br>- Discounts<br>- Rounding<br>- Surcharges<br>- as a sorting criterion in customer sales statistics |
| **Supplier group** | - Prices<br>- Discounts<br>- Rounding<br>- Surcharges<br>- as a sorting criterion in supplier sales statistics |

The groups for partners are entered in Partners > General > Partner groups, customer groups, supplier groups. Proceed as described in connection with Basic tables.
⇨ "Extending basic tables" on page B-93

When you have defined the groups you can allocate them to the customer or supplier in Partner management > tab Address.

**Fig. B-10**: Partner management - Group allocation

Calculation or orders (or purchase orders) takes the terms into account in the following sequence:
- Details from the document
- Definitions from partner master data
- Group-specific terms

If no agreements/terms are found, the generally applicable prices, surcharges, and rounding are valid.

### Different Customer/Supplier Groups
If a customer shall get other terms for certain product groups, he can be allocated to another customer group.

**Example**
Among others, you have defined the customer groups Produces and Dealers.
Customer A belongs to customer group Dealers. If an order is entered for this customer with an item that belongs to product group Heat protection IG, the terms of customer group Producer shall apply.
These exceptions are defined in dialog Different customer groups.

**Fig. B-11**: Allocation to a different customer group
- **A**: Allocated customer
- **B**: Product group
- **C**: Customer group

A customer can also be allocated to a different customer group if he is not allocated to any (common) customer group. The terms for the other customer group only refer to the defined product group. All other terms defined for this customer will be kept as they are.
Different allocations for supplier groups can be made in the same way.
If partner groups have been specified in close detail you can even define several differences per partner. If you order e.g. fittings from a supplier he can belong to the group Dealers while also belonging to the Producers group as he also provides you with tempered glass lites.

### Routes and Delivery Terms
Together with customer data and order dates, routes are the basis for dispatch planning and control. Delivery time and delivery date are used for determining the shipping date, i.e. the date on which the goods have to be handed over to the driver.
The delivery time is described in a separate session.

**Fig. B-12**: Routes

The week days for every single route are defined in master data. A route from Manchester to Birmingham for example can be done every Monday and Thursday for example. This route shall serve all customers along the road, within a radius of 30 miles.
You can also enter freight costs which can be used to check whether the shipping of a single order is worthwhile. The type of delivery is set as a delivery term, e. g. Truck or Forwarder.
For your local customers you should also define a route called Collection for which no freight costs must be charged.
Every customer is allocated a suitable route and rank. The rank is defined on tab Order.
The rank defines the sequence in which the customers are served on the route.

**Example**
Customer A and customer B belong to the southern route. Customer A has rank 1 for this route while B's rank is 2.
Customer A is therefore served before customer B.

The settings from master data are adopted for the order. This setting can be changed by order. The system automatically checks whether the defined delivery date matches the route days defined for the customer. A message will be displayed in case of differences. Different dates can be saved. They will be adopted for route planning.

#### Customs routes
The routes for cross-border deliveries are entered in Master data > Dispatch > Customs routes. You can specify border crossings or the name of the route.
Customs routes are required for dispatch planning. They cannot be allocated in partner master data.
Routes and route planning are described in detail in section Production.

### Route Definition
You can change the defined routes or replace them by new routes. To calculate freight charges for example you have to enter the mileage rate per route.

#### How to define a route
1. Go to menu Master Data > Dispatch > Routes.
2. Go to the menu Start > New to switch to the input mode.

**Fig. B-13**: Line for new routes is accessible
- **A**: Number (ID) can be chosen at random
- **B**: Name of the route
- **C**: Check the weekdays on which this route is run.

⇨ Master data, "Routes” on page B-894
3. Enter the number (A) and name (B).
Both can be chosen at random.
4. Check the checkboxes (C) for the days on which the route is usually run.
At order entry, these details will be compared with the defined delivery date. The program will issue a message if date and route day do not match.
5. Move (scroll) the view to the right to specify further details. You can also use the <Tab> key to pass from field to field.

**Fig. B-14**: Define shipping routes - departure time
- **A**: Departure time per weekday
- **B**: Mileage (freight costs)

You do not have to enter all the data. If you do not work in shifts for example or do not have your own shipping department, you can skip the fields in question.
6. Move the view further to the right to enter e. g. the freight costs per kilometer (B).

> **Do not charge shipping fees for collection**
> For the route Collection for which no shipping fee must be charged, you have to check the checkbox w/o shipping fee. For the route Collection for which no shipping fee must be charged, you have to check the checkbox w/o shipping fee.

7. Select in the menu Start > Save to save the data.
The data will be saved.
8. If necessary, repeat the steps 2 to 7 for further routes.

### Input of Partner Master Data
The dialogs for entering customer-, supplier-, and partner data are quite similar and are therefore described as one. In the following example, dialog Partner management is opened for customers. The steps are the same for Suppliers and Partners.

> **Potential customers or suppliers**
> You can enter data in the 'general partners' section at first. Using the copy function, you can save these data later in 'customers' or 'suppliers'.

You can view the free numbers in dialog Partner management by clicking on the [Zoom] icon next to the input field for the number.

**Fig. B-15**: Display and selection of free numbers
- **A**: Free numbers
- **B**: Number to be adopted.

An appropriate dialog for entering product data is also available.

#### How to enter customer data
1. Go to menu Master data > Partners > Customer > Customers.
Dialog Partner management appears with the tab Address.
2. Go to the menu Start > New to switch to the input mode.

**Fig. B-16**: Fields for new partner are accessible
- **A**: Mandatory fields
- **B**: Standard shipping and invoicing address
- **C**: Communication data
- **D**: Customer's language
- **E**: Shipping details

3. If several clients have been defined, choose the client now.
4. Enter the number and the matchcode in the mandatory fields (A).
You can choose the numbers for your customers, suppliers, and other business partners at random; every number must however be assigned just once. You can view the free numbers by clicking on the [Zoom] icon.
5. Enter the address data (B).
If the required data cannot be found in the combo box yet, you can click on the file symbol to open the corresponding dialog and add the data.
6. Enter the communication data (C).
7. Choose the main route (route 1), an alternative route (route 2) (E), and the delivery terms.
If you communicate in another language (D) with your new customer, please select this language. The corresponding language key will be used in the documents so that e.g. the product names are printed in the defined language.
For a description of multi-lingual operation please refer to the Software Reference.
8. Select in the menu Start > Save to save the data.

With this you have entered the main data for identifying a customer. You can now add the invoicing data on tab Order.
⇨ "How to complete the data for customer documents" on page B-118

## Order and Sales Invoice

### Objectives
- Defining the priority of orders
- Knowing the settings for invoices, monthly invoices, and collective invoices
- Knowing the settings for partial shipments and partial invoicing

### Benefit
- Settings from customer master data are applied to the order and do not have to be entered again.
- Most settings from master data can be adapted in the order.

### Note

**Priority**
The order priority defines the urgency for producing a certain order. It is transferred to capacity planning and thus to production.

**Invoice**
Settings for invoices can be made by customer:
- Standard rounding
- Minimum invoice value
- Invoice printing (single, collective)

**Standard rounding**
The glass surface is rounded for pricing purposes. This rounding is not valid for production purposes.

**Type of invoice**
Collective invoices, monthly invoices, or partial invoices can be issued only if these have been set as valid types in customer master data.

### Order Settings
Tab Orders serves to enter details for invoicing and shipping.

**Fig. B-17**: Partner management – Order
- **A**: Standard rounding of height and width
- **B**: Invoicing details
- **C**: Priority of orders
- **D**: Invoice details

The invoice details (A, B, D) and priority (C) can be changed in the order. These settings will be described in detail below.

#### Priority of orders
The order priority defines the urgency for producing a certain order. It is transferred to capacity planning and thus to production.
- **Express**: These orders are produced with top priority.
- **Normal**: These orders are fitted into the usual schedule.
- **Extra**: The order shall be produced from residue (plates) left over from cutting other orders.
- **On call**: Orders are produced on call.

### Invoice Settings
Settings for invoices can be made by customer:
- Standard rounding
- Minimum invoice value
- Invoice printing (single, collective)

**Fig. B-18**: Customer master data - tab Order
- **A**: Size rounding for pricing purposes
- **B**: Surcharge for minimum invoice value
- **C**: Minimum value (amount)
- **D**: Code for collective invoice
- **E**: Printing of invoice and prices
- **F**: Partial shipment and partial invoice
- **G**: Application of standard surcharges
- **H**: Monthly invoice

#### Standard rounding
The glass surface is rounded for pricing purposes (A). In Germany, pricing is based on rounding to thirty. This means that calculation is based on the next value that can be divided by 30. For a lite of 1000 mm x 1000 mm, pricing will be based on a surface of 1.04 sqm (= 1020 x 1020). This means that calculation is based on the next value that can be divided by 30. For a lite of 1000 mm x 1000 mm, pricing will be based on a surface of 1.04 sqm (= 1020 x 1020). French companies e.g round the glass surface in steps of ten.
This rounding is not valid for production purposes.

The size rounding defined in partner data can be overruled by other settings. A+W Business will search for the settings in the following sequence: Unit prices > Discounts > Prices > Partner master data. Detailed training on pricing will be provided in connection with the Sales module.

#### Invoicing surcharge
The invoicing surcharge (G) must be defined as a Miscellaneous surcharge. These surcharges will be introduced in the corresponding training session.
- **For every first invoice of the month**: The surcharge will be applied only to the first invoice of the month. For all other invoices of the current month, this surcharge will be omitted.
- **For every invoice**: The invoicing surcharge will be applied to every invoice.

#### Min. order value
You can enter a minimum value (C) per order. The difference from the minimum order value can be shown in two ways in an order:
- **As a separate item**: If the order value lies below the defined minimum order value, the surcharge item Minimum order value will be added automatically, showing the difference.
- **Split to all items**: The difference is split to all items.

There are two calculation options:
- You can define a surcharge to be applied to the order if the minimum value is not reached.
- The minimum value will be automatically calculated if the order value falls below the defined limit.

#### Monthly invoice
Invoices can be printed and sent off individually, collectively, or as a monthly invoice (H), e.g. every month or every two weeks. When printing delivery notes for this customers, orders will automatically be marked as Monthly invoice based on which you can select the maturity for invoicing.
The appropriate print point and status point have to be entered on tab Print in company data for this purpose.

**Fig. B-19**: Company data - Printing

#### Collective invoice
If a customer does not want to receive individual invoices, all of his orders will be marked for collective invoicing (D). This code can be used to select the invoices due.
The following criteria have to be same in all orders of the corresponding customer so that they can be combined in a collective invoice:
- Customer number
- Code 'print collective invoice' in the order
- Payment terms and due date
- Currency
- VAT code 1 and 2
- Automatic surcharges: Invoicing surcharge.
- Order area
- Invoice address (name 1)
- Delivery date

If one of these criteria differs in an order, printing of the collective invoice will stop at this order. This order and all those following in the number manager, will automatically get a new invoice number. This means that two invoices will be issued in this case. Another invoice number will be assigned should further differences surface.

#### Partial Shipment, Partial Invoice
If partial shipments have been agreed with a customer (F) you have to decide whether or not the partial shipment shall be accompanied by a partial invoice.
Partial invoicing means that the customer will get an invoice for every partial shipment. The amount and quantity of this partial invoice will be deducted from the original order.
If partial invoicing is not permitted, the original order is blocked for invoicing until the last partial shipment has been made.

> **Partial shipment in an order**
> You can create a partial shipment from an order only if the checkbox Partial shipment has been checked in this customer's master data.

### Editing the Settings for the Customer's Order
The following instructions are based on the steps described in the previous session.

#### How to complete the data for customer documents
1. Select menu Master Data > Partners > Customer > Customers > Orders tab.

**Fig. B-20**: Addresses and shipping data
- **A**: Standard size rounding
- **B**: Invoicing
- **C**: Document dispatch
- **D**: Partial shipment, partial invoice
- **E**: Route hierarchy

2. Check whether the values for the size rounding (A) have been entered correctly.
3. Define the invoicing mode (B)
4. Select the buttons (C) for fax and email dispatch of documents.
This function can be enabled separately for the following documents:
    - Order confirmation (OC)
    - Quotation (Qu)
    - Invoice (In)
    - Credit note (Cr)
Please remember to enter the corresponding fax numbers and email addresses on tab Address.
5. Define whether partial shipments and partial invoices are permitted for this customer (D).
6. Check whether the number for route hierarchy (E) and the priority have been set correctly.
7. Select in the menu Start > Save to save the data.
The data will be saved. You can now add subsidiaries and employees for this customer.
⇨ "How to enter a subsidiary" on page B-124
⇨ "How to enter details on your partner's employees" on page B-126

## Employees and Subsidiaries

### Objectives
- Using subsidiaries as additional shipping addresses.
- Introducing transactions.

### Benefit
- Subsidiaries can serve as additional shipping addresses if e.g. the customer has got several warehouses. The applicable shipping address can be selected in the order.
- Further details on employees serve for improving customer relations so that the persons in charge can be addressed directly.

### Note

**Subsidiaries**
For your partner's subsidiaries, the same data will be entered as for the headquarters.

**Employees**
The data on your customer's employees serve for information only.

**Transaction**
Transactions can be used to trace certain customer contacts.

### Customer's Subsidiaries
For your partner's subsidiaries, the same data will be entered as for the headquarters. The latter will be preset in the corresponding fields and can be adjusted as required.

**Fig. B-21**: Subsidiary

#### Defining the standard shipping address as a subsidiary
Apart from the company address you can enter further addresses for shipping and invoicing. These addresses are entered as subsidiaries. The checkbox Standard has to be checked on tab Address in section Address for the subsidiary that is to be used as the standard shipping address.

### Customer's Employees
You can enter the names of your customer's employees for information.

**Fig. B-22**: Employees

You can add further details like his department, his position, and his extension. You can define whether this person is the sole contact in questions regarding orders and/or sales.
These details can be used for analysis via ODBC interface.

### Transaction
So-called transactions can e.g. be used to note which employee of the customer has called asking for information, and when.
At the same time you can note when this transaction was completed, and by whom.

**Fig. B-23**: Transactions

### Add Subsidiaries
Choose the subsidiary number so that the connection with its headquarters becomes evident, e.g. 10000 for the customer, 10100, 10200, ... for the subsidiaries.

#### How to enter a subsidiary

> **Open partner management**
> Dialog Partner management can be opened for partners, customers, and suppliers. In the following example, dialog Partner management is opened for customers. The steps are the same for Suppliers and Partners.

1. Go to menu Master data > Partner > Customer > Customers.
The Partner management dialog pops up.
2. Search the record of the partner required.
3. Go to menu Functions > Details group > Subsidiary.

**Fig. B-24**: Fields for the new subsidiary are accessible
- **A**: Standard shipping address
- **B**: Close subsidiary and show main company
- **C**: Independent subsidiary

⇨ Software Reference, "Partner Management - Address" on page B-809
4. Enter at least the address and communication data.
You can add further data on the tabs as described in the instructions for entering customer data.
⇨ "How to edit the data for invoicing" on page B-162
5. Select in the menu Start > Save to save the data.
The data will be saved. On tab Address, the checkbox Standard (A) and the button [back to main company] (B) are accessible.
6. Amend the subsidiary's data, e. g. the routes. Please obey the following settings:
    - Check the checkbox Standard (A) if this subsidiary is the standard shipping address.
    - Check the checkbox Independent subsidiary (C) if this subsidiary can place its own orders.
7. Select in the menu Start > Save to save the data.
The data will be saved.
8. Click on button (B) to close the dialog.
The main company's data appear again.

### Add Employees
You can define the area for which the employees of your partners are responsible. This detail only serves for information.

#### How to enter details on your partner's employees

> **Open partner management**
> Dialog Partner management can be opened for partners, customers, and suppliers. In the following example, dialog Partner management is opened for customers. The steps are the same for Suppliers and Partners.

1. Go to menu Master data > Partners > Customer > Customers.
The Partner management dialog pops up.
2. Search the record of the partner required.
3. Go to menu Functions > Details group > Employee.

**Fig. B-25**: Fields for new employees are accessible
- **A**: Name of customer's employee
- **B**: Employee's position (for information only)
- **C**: Communication data
- **D**: Release fields

⇨ Software Reference, "Employee" on page B-840
if customer's employees have already been entered, the appropriate data are shown.
4. Click on [New] (D) to release the fields.
If the customer's employees have already been entered you can change the data.
5. Enter at least the name (A) and the phone number (C).
6. Add further details if these are important for communicating with this employee, e. g. the employee's function (B).
With that you have entered the main data.

**Fig. B-26**: Fields for new employees are accessible
- **A**: Save employee's data

7. Click on [New] (A) to save the data.
The data will be saved. You can now enter details of other employees by repeating the steps 5 to 7.
8. Click on [End] to close the dialog.
Dialog Partner Management reappears in the foreground. Tab Empl./Subsid./Settings shows the employees.

## Text

### Objectives
- Entering customized text.
- Introducing text codes.

### Benefit
Text provides information on certain facts, e. g. special requests in connection with production.

### Note

**Customised text**
Text which is used just for a single customer can be entered in customer master data, to be automatically added to the document.

**General text**
Frequently used text can be entered as 'general text' which can be automatically inserted in a document by means of customer master data.

**Text codes**
Text codes serve to define the documents in which the text shall be printed, e. g. order confirmations, delivery notes.

### Text and Text Codes
Recurring text can be saved, e.g. to be included in the document automatically. We distinguish system-, default-, and spacer text.
Standard text is distinguished by means of text codes, e. g. text code Q for quotations, P for production, D for delivery note. Text codes can be entered according to your company's requirements.

**Examples**
- **Info text (text code /):**
Shall be printed on all documents, e.g. to announce company holidays.
- **Delivery note text (text code D):**
To be printed only on delivery notes, e.g. deadlines for complaints.
- **Quotation text (text code Q):**
To be printed only on quotations, e.g. the validity of the quote.

Text codes are not only used for grouping your standard text. Text codes can also serve to define when text shall be printed.

**Example**
Production text (text code P) shall not be printed on delivery notes. In management of forms you can define - for every form - the text codes that shall not be printed.

You can enter special spacer text for every IG unit, and allocate them to the product.
In partner and product master data you can enter text that shall always be used in documents. This can be standard text or text which is entered just for the partner or the product.

> **Detailed description of text**
> Text modules are described in detail in Tutorial 2.
> Tutorial 2, "Text" on page B-534

### Entering Text in Customer Master Data
This example describes a text module in customer master data. Text for suppliers or products can be entered in the same way.
There are the following instructions on this subject.
- "How to allocate standard text" on page B-130
- "How to enter customised text" on page B-132

> **Fonts and type size**
> The settings for the fonts and the type size only apply to the display on screen. They will not be used for printing.

#### How to allocate standard text
1. Go to menu Master data > Partners > Customer > Customers > tab Text.

**Fig. B-27**: Release the fields for new text
- **A**: Release fields
- **B**: Number of the standard text
- **C**: Check the text code

2. Click on the (A) icon to release the input fields.
3. Enter the number (B) of the desired standard text or select it using the magnifier symbol.
If you enter the text number directly you have to press the <Tab> key to go to the next field to make sure that the text is loaded.

**Fig. B-28**: Allocated standard text
- **A**: List of allocated text modules
- **B**: Editing field

The standard text appears in the editing field (B). You can edit it and change it as required for the customer in question.
4. Select in the menu Start > Save to save the data.
According to the text code, the standard text will be printed on the appropriate forms or is transferred to production.
Enter the spacer text in the same way.

#### How to enter customised text
1. Go to menu Master data > Partners > Customer > Customers > Text tab.

**Fig. B-29**: Text input
- **A**: Release fields
- **B**: Text Number
- **C**: Select text code
- **D**: Text input

2. Click on the (A) icon to release the input fields.
3. Choose a text code (C), e. g. I Information text.
The text code defines how the text shall be used. If the text shall be transferred to production for example, choose text code P. If no text code is entered, the text will not be transferred.
Keep the entry 0 in the Number (B) field.
4. Enter the desired text in the input field (D).

**Fig. B-30**: Customised text

5. Select in the menu Start > Save to save the data.
The data will be saved and will be used only for this customer acc. to the text code.
In the same way, you can enter text for individual suppliers, partners, or products.

## Classifiers

### Objectives
- Defining classifiers.
- Allocating classifier values.

### Benefit
Classifiers serve as filters for additional analyses, e. g. sales.

### Note

**Classifiers**
Classifiers are defined for all partners, or just for customers, suppliers, or partners.

**Classifier values**
Classifier values can be numerical, alpha-numerical, or dates.

### Classifier and Classifier Value
Classifiers are defined in order to use them as filters for additional analyses, e. g. sales, birthday, hobbies. You can also define whether the entry is numerical, alpha-numerical, or a date. Classifiers which are no longer required can be deleted.
Working with classifiers is based on two steps:
- Define a classifier.
- Enter a name for the classifier and define the values it can adopt.
- Allocate a classifier value.

### Enter a Classifier
Classifiers for customers, suppliers, or partners can be entered in the corresponding partner management.

#### How to enter a classifier
1. Go to Master data > Partners > Customer > Customer > menu Functions > Classifier group > Classifier definition.

**Fig. B-31**: Enter a Classifier
- **A**: Tab defining the validity
- **B**: Release fields

⇨ Software Reference, "Classifiers" on page B-803
Classifiers entered in tab Common are valid for all partners. The other three tabs serve to define classifiers that apply to the corresponding group only.
2. Select the required tab, e. g. Common.
On this tab, enter a classifier that is valid for all partners.
3. Click on [New] (B) to get access to the next line.

**Fig. B-32**: Fields for new classifier are accessible
- **A**: Name can be chosen at random
- **B**: Comments, e.g. regarding the use
- **C**: Classifier type: N: numerical, A: alpha-numerical, D: date

4. Make your entries:
    - In field Name (A) e. g. group sales.
    - In field Comment (B) e. g. ABC classification.
5. Check one of the checkboxes (C) to define if the entry has to be numerical, alpha-numerical, or a date.
This defines the way in which the classifier values can be entered in partner management, and how they will be analysed.
6. Click on [New] to save the data.
The data will be saved. All classifiers on tab Common are listed for all partners in partner management on tab Classifiers. All other classifiers will only be listed for the corresponding partners.

### Allocate Classifier Value
Classifier definition determines the type of values a classifier can have. This definition determines the way in which the value is allocated.
⇨ "Enter a Classifier" on page B-135
There are the following instructions on this subject.
- "How to allocate an alpha-numerical value" on page B-137
- "How to allocate a numerical value" on page B-139

> **Open partner management**
> Dialog Partner management can be opened for partners, customers, and suppliers. In the following example, dialog Partner management is opened for customers. The steps are the same for Suppliers and Partners.

#### How to allocate an alpha-numerical value
1. Go to menu Master data > Partners > Customer > Customers > tab Classifiers.

**Fig. B-33**: Allocate classifier value
- **A**: Classifier type
- **B**: Allocated value

⇨ Software Reference, "Partner Management - Classifiers" on page B-821
2. Mark a classifier (A) with code A (alpha-numerical).
The entire line is selected.
3. Go to menu Functions > Classifiers group > Classifier values.
You can also double-click on the Value (B) field of the selected classifier. Dialog Classifier value allocation appears.

**Fig. B-34**: Enter a classifier value
- **A**: Input line
- **B**: Release input line
- **C**: Adopt the value

4. Click on [New] (B) to get access to the next line.
The next line is released. Enter the new value, e. g.
⇨ Software Reference, "Classifier Value Allocation" on page B-843
5. Area South 1 for an alpha-numerical classifier for the sales.
6. Click on [OK] to save the data.
The data will be saved. You can enter further classifiers by repeating the steps 4 to 6. These classifier values will not be automatically adopted for the current partner.
7. Select the line with this value and click on [Adopt] (B) to assign this value to the partner.
Dialog Classifier value allocation is closed and dialog Partner management reappears in the foreground.

**Fig. B-35**: Adopted classifier value

If you have adopted the value, it will be listed in section Classifiers.
8. Select in the menu Start > Save to save the data.
The data will be saved. They can be used now for analysis.

#### How to allocate a numerical value
1. Go to menu Master data > Partners > Customer > Customers > tab Classifiers.
2. Position the cursor in section Classifiers on the field Value for an entry with code N (numerical) or D (Date).
3. In the context menu, select Insert.
Open the context menu with the right mouse key.
4. Enter the values as defined:
    - N (numerical), e.g. 600000 (sales)
    - D (date), e. g. 23.02.2012 (birthday gift for the head of department)
Use <Tab> to go to the next line to enter another value.

**Fig. B-36**: Numerical value.
5. Select in the menu Start > Save to save the data.
The data will be saved.

### Exercises
The exercises are based on each other. The data you have entered for exercise purposes will therefore be needed again. Mark these data so that they are easy to distinguish, e. g. by the supplement 'training' or 'demo'.
- Enter at least one new customer.
- Enter routes for your district, for collection, and for a forwarder.
- Enter a customer group called Training.
- Allocate your customer to one of the groups.
- Allocate the customer to another customer group when a tempered glass order is entered for him.
- Standard rounding
- Invoicing mode
- Partial shipment and partial invoice permitted
- Enter an alternative invoice address.
- Define one of the addresses as the standard shipping address.
- Enter text for your training customer which is valid only for him, and shall be printed on production papers.
- Enter three classifiers with different properties (numerical, alpha-numerical, date).
- Allocate to your training customer a value for each of the classifiers.

> **Locking of demo data**
> If you do your exercises during actual operation you should lock the demo data for further use as soon as you have made your tests.

## Finances and Balance

### Objectives
- Knowing the terms for invoices and payments.
- Defining a calendar and a change of payment date.
- Setting the credit limit check.

### Benefit
- Customer invoices are issued based on the settings made in customer master data.
- Balance and credit limit are shown at order entry so that the actual orders and receivables can be taken into account.

### Note

**Due date**
Due dates are calculated automatically. Enter the required mode and the invoicing dates:

**Credit term**
The document date and the invoicing date form the first reference date. This is the basis for calculating the credit term.

**Payment day postponement**
To make sure that no invoices are due for payment during the customer's company holidays you can define the period in question in the customer's calendar.

**Payment terms**
Each payment term can take into account several levels of due dates and percentages for the cash discount.

**Acct. No.**
The customer number is used as the main account and is transferred to financial accounting. The customer number of one of the customer's subsidiaries can be used as the main debtor to whom invoices and credit notes are addressed.

**Credit limit**
You can define the insured credit limit and the internal (uninsured) credit limit for every customer. The credit limit can be automatically checked when new orders are entered.

**Taxes**
Taxes can be calculated only if they have been defined as tax rates and allocated to the customer.

**Currencies**
Prices can be kept in different currencies. Orders can be entered in national currency or foreign currency. The national currency will always be used for statistical purposes. A+W Business will convert the amounts accordingly.

### Payment Settings
Invoice settings can be made for every customer on tab Finances.

**Fig. B-37**: Customer master data - tab Finances
- **A**: Bank account
- **B**: Due date calculation
- **C**: Invoicing
- **D**: Payment termss
- **E**: Main account or alternative invoice address
- **F**: Valid tax rate

The customer's bank details (A) are entered e.g. in order to use them for credit notes or printing receipts.

For the customer invoices, enter:
- Due day calculation mode (B)
- Accounting date (C)
- Payment terms (D)
- Valid tax rate (F): You can enable up to five different tax rates.

The tax rates are defined in Finances > Tax. You can also enter (in company data) whether the tax shall be calculated per item or per BOM element. This entry is valid for all customers. The settings in company data are described in the software reference.

### Due Date Calculation
Due dates are calculated automatically. Enter the required mode and the invoicing dates:
- Accounting date, e. g. if the invoice date is not decisive.
- Due days (gross days)
- Payment days

| Mode | Text |
| --- | --- |
| 0 | 1st Reference date |
| 1 | 1st Reference date + Days gross |
| 2 | 1st Reference date + Days gross + Rounding up to 1st day of settlement or end of month |
| 3 | 1st Reference date + Days gross + Rounding up to the 15th or end of month |
| 4 | 1st Reference date + Days gross + Rounding up to the 10th, 20th or end of month |
| 5 | 1. Reference date rounded to end of month + gross days (0/30/60/90). The calculated term of payment is always rounded to the month's end. Attention: For flag 5 and 6, the entry in field Gross days must be divisible by 30. 30 days = 1 month, 60 days = 2 months, 90 days = 3 months by which the first reference date is increased. |
| 6 | 1. Reference date is rounded to the month's end + gross days (0/30/60/90) + date of settlement |
| 7 | 1st Reference date + Days gross + rounded up to 1st, 2nd or 3rd day of settlement |
| 8 | 1st Reference date + Days gross + rounded up to 1. Or 3rd day of settlement in dependence on 2nd day of settlement |
| 11 | Maturity date = shipping date + payment term |

Examples for calculating due dates are available in section Sales.
⇨ Sales, "Due date calculation" on page C-1330

### Accounting
The document date and the accounting date form the first reference date. This is the basis for calculating the payment term.
- **Accounting date = 0:** The first reference date matches the document date.
- **Accounting date ≠ 0:** The document date is rounded to the accounting date and forms the first reference date.

**Examples**

| Document date | ACD | 1st reference date | Note |
| --- | --- | --- | --- |
| 13.03. | 0 | 13.03. | 1st Reference date = Document date |
| 13.03. | 25 | 25.03. | The document date is rounded to the 25th of the same month |
| 27.03. | 25 | 25.04. | Since the invoicing date is less than the document date, the document date is rounded to the 25th of the following month |
*ACD = accounting date*

### Payment Day Postponement
You can define that the calculation of the payment date shall be postponed, e. g. to make sure that invoices do not become due during the customer's works holidays. The time of the postponement is set in the customer calendar.
Calculation always refers to the entries in the customer calendar. The type of postponement is valid irrespective of the days defined in the customer calendar.
⇨ "Editing Customer's Calendars" on page B-165

| Option | Type of postponement |
| --- | --- |
| 0 | No postponement |
| 1 | 50:50 split - due dates are split into half: One half of the amount becomes due within a certain period before the original due date. The other half is due within a certain period after the original due date. |
| 2 | Shift by period – due dates will be postponed by a certain period. |
| 3 | Same as option 2 plus surcharge. An appropriate surcharge must have been defined if you choose this option. |

#### Examples
**Starting position:**
- Invoice amount: 300 Euros
- Invoice date: 10.07.
- Customer accepts no due dates in August (01.08. - 31.08.)

**Example 1**
Credit term 30 days = Due date 10.08.
- **Option 1: 50:50 split**
  - Due date 1: 10.07. = 150 €
  - Due date 2: 10.09. = 150 €
  - Half of the invoice amount is due before the company holidays and the other half, afterwards.
- **Option 2: Postponement by period**
  - Due date: 10.09. = 300 €
  - The entire amount becomes due after the company holidays.
- **Option 3: Like option 2 + surcharge**
  - Due date: 10.09. = 303 € (300 € + 1 %)
  - The entire amount is due after the company holidays. An additional surcharge will be applied.

**Example 2**
Credit terms 30, 60 days
- Due date 1: 10.08. = 150 €
- Due date 2: 10.09. = 150 €
- **Option 1: 50:50 split**
  - Due date 1: 10.07. = 75 €
  - Due date 2: 10.09. = 225 €
  - 150 € are due on the first due date. This amount will be split into halves so that 75 € are due on the moved up first due date.
  - The remaining 75 € are due on the second due date so that 15 € + 75 € are due at that time.
- **Option 2: Postponement by period**
  - Due date: 10.09. = 300 €
  - 50 € are due on the first due date. This amount is due on the second due date so that at that time, 300 € are due.
- **Option 3: Like option 2 + surcharge**
  - Due date: 10.09. = 303 € (300 € + 1 %)
  - The whole invoice amount is moved to the second due date. An additional surcharge is applied.

**Example 3**
Credit terms 30, 60, 90 days
- Due date 1: 10.08. = 100 €
- Due date 2: 10.09. = 100 €
- Due date 3: 10.10. = 100 €
- **Option 1: 50:50 split**
  - Due date 1: 10.07. = 50 €
  - Due date 2: 10.09. = 150 €
  - Due date 3: 10.10. = 100 €
  - In this example, only the first due date is affected at which point 100 € would be due.
  - This amount is split so that the first half (50 €) is due before the original date. The second half is due on the second due date together with the original (third) amount (50 €+100 €).
- **Option 2: Postponement by period**
  - Due date 1: 10.09. = 200 €
  - Due date 2: 10.10. = 100 €
  - In this example, the amount is moved from the first due date to the second.
- **Option 3: Like option 2 + surcharge**
  - Due date 1: 10.09. = 201 € (200 € + 1 %)
  - Due date 2: 10.10. = 100 € (100 €)
  - In this example, the amount is moved from the first due date to the second, and a surcharge is applied to the postponed amount.

The customer calendar is described in a separate session.
⇨ "Editing Customer's Calendars" on page B-165

### Calendar
The current year must be defined in the general calendar in order to enter documents. Daily working hours have to be defined so that dates can be calculated at order entry, e.g. delivery dates. Weekends and public holidays (without working hours) have to be entered for these calculations.
You can also enter the company holidays by setting the daily working hours to zero for that time. These days will be taken into account when determining delivery dates.

**Fig. B-38**: General calendar
- **A**: Number of operating hours
- **B**: Accept changes

The customer calendar is based on the general calendar. It mainly serves to enter the days for the due date postponement for every customer.
⇨ "Editing Customer's Calendars" on page B-165

### Payment Terms
The payment terms for every customer are entered in customer master data on tab Finances. In the order header, the payment terms are loaded from customer data and can be changed if required. The settings for calculating the cash discount are made in dialog Payment terms.

**Fig. B-39**: Payment terms
- **A**: Cash discount definition
- **B**: Credit term definition

You can set up several steps for a payment term, in complete records of up to five credit terms (B) and three percentages (A) for cash discount. Moreover, you can enter any number of conditions which only refer to the cash discount.

**Example**

| | Rate 1 | Days 1 | Rate 2 | Days 2 | Due days 1 |
| --- | --- | --- | --- | --- | --- |
| Cash discount | 3.00% | 10 | 1.5% | 20 | 30 |

This example shows that the customer can deduct a cash discount of 3% within the first 10 days but only 1.5% within the following 10 days. After 30 days, the invoice is due without deductions.

### Payment Modes, Solvency
Payment modes and solvency serve for information only. These entries are made in simple, basic tables. They can be extended at random.

**Fig. B-40**: Payment Modes, Solvency

### Main Account or Alternative Invoice Address
You can enter the customer number of the main debtor (subsidiary) who shall receive invoices and credit notes. Prerequisite is that this has been defined as a subsidiary of the customer. The main account is thus the main debtor's customer number. If this field is blank, the number of the current customer will be automatically used as the main account.

### Banks
Enter the bank data for payments from and to your customers and suppliers.

**Fig. B-41**: Bank data
- **A**: Bank code necessary for IBAN
- **B**: BIC for international payments
- **C**: Country code necessary for IBAN

Banks are allocated to the partners in partner management, tab Finances. In partner management, you can have the IBAN determined by the system if at least the following data have been entered for the bank: bank code (A), country code (C), and account number (in customer master data). This function is started in partner management via menu Functions.

> **Bank for the company and clients**
> The bank accounts for your company and clients are entered in menu Master data > Company > Banks. You also access the bank data entered in Finances.

### Credit Limit for Customers
You can enter two different values for the credit limit for every customer, which can be automatically checked when a new order is entered. Credit limit 2 can be used as an internal, uninsured credit limit.

To check the credit limit you have to make the following decisions:
- **Define the credit limit for every customer in customer data.**
  - **Credit limit 1:** This entry defines the insured credit limit.
  - **Credit limit 2:** This entry is an internal (uninsured) credit limit granted to the customer because of his credit standing.
- **Define the reaction in case the credit limit is exceeded:**
  - Normally, the status will be raised. If the credit limit is exceeded, new orders will be set to a defined status and will be locked for processing. This status can be reset by hand to release the orders for processing.
  - New orders can be entered and saved. There is a message however pointing out that the credit limit is overdrawn. It is up to the user to decide whether the order shall be processed or rejected.

#### Type of check
The appropriate code for every customer or subsidiary is set in partner management.
- No credit limit check
- Limit 1 + Message Limit 2
- Limit 2 + Message Limit 1
- Check of credit limit 1
- Check limit 1 and 2
- Check credit limit 2
- Advance payment

If you are working with subsidiaries, the credit limit can be checked on two levels:
- Checking the site's credit limit.
- Check the main customer's credit limit:
  - Check via subsidiary code
  - Check via input in field Main account: The subsidiary's credit limit will be ignored.

**Fig. B-42**: Partner management - Settings for checking the credit limit
- **A**: Settings for customers with subsidiaries
- **B**: Type of check

### Show current order volume
The order header shows the credit limit and the receivables. This allows to check every order and discuss with the customer whether a new order can be accepted. In this area, data will be updated after transfer to accounting and after every report.

**Fig. B-43**: Credit limit and balance
- **A**: Credit limit
- **B**: Balance

#### No credit limit check
If the credit limit is not checked, the actual amounts will only be displayed. When the credit limit is exceeded and in case of cash in advance, orders can generally be processed. Quotations can be entered irrespective of the credit limit and possible locks.

#### Receivables Reports
In connection with a financial accounting program (FinAcc) which reports the receivables, you will get an expressive overview of the customer's present financial status. If you do not use receivables reports, the check will include all orders which have not been transferred to financial accounting yet.
If the function Individual receivables report is active in company data, receivables can be checked for the corresponding customer at order entry and in customer management. All open invoices will be shown.
Customers whose balance has been settled after the last receivables report will be updated in customer management with a balance of 0.

#### Overdrawn credit limit
The settings in company data and the status allocation define how A+W Business is going to act in case the credit limit is overdrawn:
- A lock status is defined in status allocation beyond which further entries are impossible.
- The status will be raised only if the option Raise status if credit limit is overdrawn is active in company master data.

If these two settings are combined, new orders cannot be entered once the credit limit is reached or overdrawn.
The message `Credit limit exceeded, customer locked` also appears before the document is copied. Copying will not take place. The credit limit will be checked even if the customer is changed in an existing order.
To process a new order even if the credit limit has been exceeded, the order status has to be reduced manually. After that, the status will not be raised again automatically. The change of status is described in detail in section Sales.
Customer orders can be transferred via EDI interface (electronically). If the credit limit is overdrawn by an order, it gets the status `Order locked due to credit limit`. It will be booked in capacity planning despite the lock status. This order has to be released manually by reducing the status. After that, it will be automatically transferred to production.
The status-raising functions will be explained in detail in a separate session.
⇨ Tutorial 2, "Status administration" on page B-492

### The Process of Checking

**Fig. B-44**: Checking the credit limit

This process can be described as follows:
1.  **Enter order header.** This links to the customer's credit limit data.
2.  **Is the check activated?**
    *   **No**: The process flows to "Enter order".
    *   **Yes**: Proceed to the next step.
3.  **Is the limit overdrawn?**
    *   **No**: The process flows to "Enter order".
    *   **Yes**: Proceed to the next step.
4.  **Change status.**
5.  **Is there a lock?**
    *   **No**: A "Message" is displayed, and the process flows to "Enter order".
    *   **Yes**: Proceed to the next step.
6.  **Reset status manually?**
    *   **No**: Do not save the order. The process ends.
    *   **Yes**: Proceed to the next step.
7.  **Enter order.**
8.  From here, the process can lead to "Transfer invoice to financial accounting", which in turn feeds into a "Receivables report".

The manual change of status can be prevented e.g. by the appropriate settings in the user rights.

### Credit Limit Analysis
Credit limit analysis can be used for evaluating the development of certain financial data for a customer or customer group within a defined period.
The system will analyse the credit limit, receivables, liability, balance 1, balance 2, and the orders on hand.

The hierarchy is:
1. Undelivered orders
2. Orders shipped but not yet invoiced
3. Invoiced orders that have not been transferred to financial accounting yet
4. Totals of 1-3

**Fig. B-45**: Credit limit snapshot for a customer

The credit limit snapshot is created by a daily task analysing the financial data.
If you are going to work with formulas, please contact a member of the service team of A+W Software GmbH.

### Currencies
Prices can be shown in the orders in the currency allocated to the customer. Prerequisite for this is that currencies and exchange rates are entered and maintained accordingly.
For order entry, A+W Business can use two different currency settings:
- **National (home) currency:** The currency of the country in which headquarters are located. In Europe, this is usually Euro.
- **Foreign currency:** The currency that differs from the home currency, e.g. the currency in which prices are shown in orders for foreign customers.

For statistical comparison, your home currency will be used always. A+W Business will convert the amounts accordingly.
The options for price management and calculation in the orders are:
- Price lists and orders are kept in national currency.
- Price lists are kept in national currency; for foreign customers, the amounts can be shown either in national or foreign currency. For this, you have to enter and update the exchange rates for the foreign currencies.
- Price lists are kept in foreign currency; the amounts in the orders can be shown in national or foreign currency. The exchange rate is defined for internal purposes.

The currency to be used as a basis for calculation as well as the currency in which orders are entered are both defined in company data.

**Fig. B-46**: Company data – tab tax, currency settings
- **A**: Currency used by A+W Business for calculation
- **B**: Default settings for order entry
- **C**: Currency for displaying prices in the order

This example shows that the national currency (A) is Euro. The national currency is usually selected as the standard setting (B) for order entry. If you are using price lists in another than the national currency, select the setting Euro for displaying prices (C) at order entry.

### Pricing in connection with foreign currency
You can maintain sales and purchase prices in A+W Business even if they occur in different currencies.
Price calculation with foreign currencies can produce different results if prices for quantities are calculated on different levels. This setting is made in company data.
⇨ Software Reference, "Calculate foreign currency amount from unit price x quantity" on page B-974

If the foreign currency amount shall result from the BOM and the quantity, the amounts can be calculated in the following ways.

- **The item price is the item price in national currency:**

| Calculation | Operation | Result |
| --- | --- | --- |
| HC price/PU | x factor | = FC price/PU |
| HC gross price/pc. | x factor | = FC gross price/pc. |
| HC net price/pc. | x factor | = FC net price/pc. |
| HC item price | x factor | = FC item price |
*Note: NC = national currency, PU = price unit, FC = foreign currency*

- **The item price is created from the net price in foreign currency:**

| Calculation | Operation | Result |
| --- | --- | --- |
| NC price/PU | x factor | = FC price/PU |
| NC gross price/pc. | x factor | = FC gross price/pc. |
| NC net price/pc. | x factor | = FC net price/pc. |
| FC net price/pc. | x qty. | = FC item price |
*Note: NC = national currency, PU = price unit, FC = foreign currency*

### Cash Discount
A+W Business distinguishes three calculation types for cash discount which are described in the following examples.

- **On gross amount:**

| Calculation | Calculation/basis | Value |
| --- | --- | --- |
| Net 100.00 | 100.00 | 100.00 |
| VAT 19% | | 19.00 |
| Gross | 119.00 | 119.00 |
| Cash discount 2% | | 2.38 |

- **On net amount (gross minus cash discount):**

| Calculation | Calculation/basis | Value |
| --- | --- | --- |
| Net 100,00 | 100.00 | |
| Cash discount 2% | 2.00 | 98.00 |
| VAT 19% | 98.00 | 18.62 |
| Gross | | 116.62 |

- **On net amount:**

| Calculation | Calculation/basis | Value |
| --- | --- | --- |
| Net 100,00 | 100.00 | 100.00 |
| Cash discount 2% | 2.00 | |
| VAT 19% | 98.00 | 18.62 |
| Gross | | 118.62 |

### Settings in Company Data
If the status shall be changed when the credit limit is overdrawn, checkbox (A) must be checked in company data, tab Parameters.

**Fig. B-47**: Company data > Parameters
- **A**: Raise status for credit limit
- **B**: Tax calculation

You have to define in status allocation whether order entry shall be locked when the status is raised. Status allocations are described in a separate session.
⇨ Tutorial 2, "Status administration" on page B-492

### Receivables
For receivables reports, you have to check the financial accounting program as well as the settings for updating in company data.

**Fig. B-48**: Company data – tab FinAcc
- **A**: Selection of FinAcc interfaces
- **B**: Path for reports
- **C**: Update after receivables report
- **D**: Individual check by customer

### Editing the Customer's Financial Data
The following instructions are based on the steps described in the previous session.

#### How to edit the data for invoicing
1. Go to menu Master data > Partners > Customer > Customers > tab Finances.

**Fig. B-49**: Partner management - Payment terms
- **A**: Due date calculation mode
- **B**: Activate tax calculation
- **C**: Select tax rate
- **D**: Lock customers

2. Check the settings for the lock code (D).
If the new partner data shall be used at once, you have to choose the setting `not locked`.
You should lock the date if e. g. price and payment agreements have not been finalised with the new partner. In this case, you cannot enter any documents for him, i. e. orders of purchase orders.
3. Enter the settings for the due dates (A) agreed with this partner.
4. Activate tax calculation (B) and choose the tax rate (C).
5. Select in the menu Start > Save to save the data.
The data will be saved. You can now add the data for sales representatives or for production.
⇨ "How to enter a subsidiary" on page B-124
⇨ "How to enter details on your partner's employees" on page B-126

### Drawing up a General Calendar
You have to enter the public holidays and company holidays for every new calendar year so that these will be recognised at order entry and taken into account for scheduling. If you enter the date of a public holiday in a document, the system will inform you that the selected date is no working day.

#### How to enter a new calendar
1. Go to menu Master data > General > Calendar.

**Fig. B-50**: Data for the current calendar year
- **A**: Adopt weekdays
- **B**: Number of operating hours
- **C**: Year

⇨ Software Reference, "Calendar" on page B-639
2. Check the checkboxes (A) for the weekdays.
3. Enter the regular working hours for every weekday (B), e. g. Monday to Thursday 8 hours each, Friday 6 hours.
4. Enter the new year in field Year (C).

**Fig. B-51**: Data for the new calendar year

5. Select in the menu Start > Save to save the data.
The year is entered and displayed in field Overview. Weekends are shown in red.
Next you should enter your national holidays and company holidays.

**Fig. B-52**: Data for the current calendar year
- **A**: Operating hours on a holiday
- **B**: Calendar year, overview
- **C**: Apply changes to the entire calendar week
- **D**: Select calendar week
- **E**: Holiday without working hours

6. Choose the calendar week in field Week (D), e. g. week 40.
7. Select from the overview (B) the day you want to define as a holiday, e. g. 03.10.
8. Check the checkbox (E) of the corresponding weekday.
9. Enter 0 in field Hours (A).
10. Click on [apply to week] (C).
The working hours for this weekday are shown on the list as 0 hours.
11. Repeat the steps 6 to 10 for all public holidays and for your company holidays.
12. Select in the menu Start > Save to save the data.
With that, the general calendar has been drawn up completely. You can now edit your customer calendars.
⇨ "Editing Customer's Calendars" on page B-165

### Editing Customer's Calendars
Dialog Calendar is used to enter the holidays per customer and year, i.e. the times to be omitted from due date calculation.
Calculation has already been introduced in the session on Due date postponement.
⇨ "Payment Day Postponement" on page B-145

> **Prerequisite**
> A calendar year must be entered in the general calendar before you can draw up or edit the customer calendar for a new year.

There are the following instructions on this subject.
- "How to set up a customer calendar including holidays" on page B-166
- "How to enter holidays" on page B-167
- "How to delete holidays" on page B-167
- "How to delete a customer calendar" on page B-168
- "How to copy holidays from one customer to another" on page B-169

#### How to set up a customer calendar including holidays
1. Go to Partners > Customer > Calendar.
Dialog Calendar appears.
2. Go to the menu Start > New to switch to the input mode.

**Fig. B-53**: Fields for new customer calendar are accessible
- **A**: Select a customer
- **B**: Select calendar year

⇨ Software Reference, "Calendar (Customer)" on page B-883
3. Choose the customer (A) and the year (B).
If the desired year is not offered for selection you have to enter it in the general calendar first. This is found in Master data > General > Calendar.
⇨ Software Reference, "Calendar" on page B-639
4. Select the days on which no invoices shall be due for payment.
If you do not want to fix certain days for the postponement, just select a random date, e.g. a Sunday.

**Fig. B-54**: Holidays for customers
- **A**: (Company) holidays
- **B**: Check the calendar year

5. Select in the menu Start > Save to save the data.
The data will be saved. You can enter further holidays or create a new customer calendar.

#### How to enter holidays
1. Go to Partners > Customer > Calendar.
2. Select the customer whose holidays you want to enter.
Calendars from the previous year can be deleted to keep the size of the list at bay. A description of how to delete these can be found in the next process.
3. Check whether the right year has been set.
4. Select the company holidays for this customer.
These days shall be omitted from credit term calculation.
5. Select in the menu Start > Save to save the data.
The data will be saved. The days for which no due dates must be calculated are marked.

#### How to delete holidays
1. Go to Partners > Customer > Calendar.
The table lists all customers for whom holidays have been entered, per year.
2. Select the required customer and search the days on the list for which you want to remove the check.
3. Untick the days in question.
The checkboxes have been unticked.
4. Select in the menu Start > Save to save the data.
The data will be saved.

#### How to delete a customer calendar
1. Go to Partners > Customer > Calendar.
The table lists all customers for whom holidays have been entered, per year.
2. Select the required customer.
3. Go to the menu Start > Delete.
A security query appears.
4. Answer the security check by [Yes].
The data will be deleted. The old customer calendar has disappeared from the list.

#### How to copy holidays from one customer to another
1. Go to Partners > Customer > Calendar.
The table shows all customers for whom a calendar has been drawn up, per year.
2. Select the required customer and search the list for the days you want to copy.
Only the selected calendar days will be copied. To copy the entire calendar, select all days.

**Fig. B-55**: Data transfer

3. Choose the days you want to copy by selecting the entire line.
Keep pressing the <Ctrl> key to select several days in a row.
4. Go to menu Functions > Transfer dates.
Dialog Transfer calendar data appears.

**Fig. B-56**: Select customer
- **A**: Adopt selected holidays
- **B**: Target customer

5. Select the target customer (B) to which the holidays shall be transferred.
6. Remember to check the checkbox Omit payment (A) so that the holidays can be transferred.
7. Click on [OK] to start the transfer.

**Fig. B-57**: Holidays of the target customer

The selected days will be transferred to the target customer's calendar. At the same time, a calendar is drawn up for the target customer if necessary. Dialog Calendar pops up.

## Sales Representatives

### Objectives
- Defining a sales territory
- Allocating a sales representative
- Introducing the different ways of calculating commissions

### Benefit
The commission will be calculated automatically if the order states the salesman in charge and the applicable commission.

### Note

**Salesman**
Only employees who have been allocated a sales territory are offered for selection.

**Sales territories**
Sales territories have the following functions:
- Calculation of commission (sales commission)
- Sorting criterion in A+W Business sales statistics.

**Commission**
Details on the commission and its calculation are entered in dialog Sales commission.

### Sales representatives
Commissions for your sales representatives can be calculated according to different settings. The assigned territories, product groups, and the orders received are possible criteria. The document must state the salesman in charge.
Sales representatives are entered as employees. To define an employee as a sales representative, he is assigned a sales territory.

### Sales territories and salesmen
Sales territories have the following functions:
- Calculation of commission (sales commission)
- Sorting criterion in A+W Business sales statistics.

Only employees who have been assigned a sales territory are offered for selection in the documents.

**Fig. B-58**: Sales territories
- **A**: Employees working as sales representatives
- **B**: Area of responsibility
- **C**: Area codes, e.g. for minor customers
- **D**: Type for commission splitting

All details except the name (A) are not mandatory. If you do not require evaluations by territory, just leave these fields blank.
Sales territories can be assigned by post code (B) or area code (C). These details will be analysed when evaluating the orders for calculating the commission.
The type (D) defines the percentage from the document to be used for commission splitting.
Details on the commission and its calculation are entered in dialog Sales commission. These are described in a separate session.
⇨ "Sales Commission" on page B-447

### Allocating a sales representative
The sales representative assigned to a customer will be suggested by default when an order is entered for the customer. These settings can be changed per order.

#### How to allocate a salesman to a customer
1. Go to menu Master data > Partners > Customer > Customers > Sales tab.

**Fig. B-59**: Preset sales representatives in partner data
- **A**: Salesman 1 and 2
- **B**: Share of commission for salesman 2
- **C**: List of quotations
- **D**: List of orders

2. Choose the salesmen (A) in charge of this customer.
If you select a salesman in both fields you should also define how the commission is going to be split (B).
If no sales representatives are offered for selection, you can enter the appropriate data.
3. Click on the file symbol to open the dialog Sales representatives.
4. Click on [New] to get access to the next line.

**Fig. B-60**: Sales representatives

5. Choose the salesman in charge of this customer.
You can also define whether he shall be considered as Salesman 1 or Salesman 2 by default.
6. Click on [New] to save the data.
The data will be saved. The dialog is closed and you will find yourself back in partner management. You can select the new salesman in one of the fields now.
7. Enter the share in sales (B) for Salesman 2.
Based on this share, the commission is calculated.
8. Select in the menu Start > Save to save the data.
The data will be saved. The commission will be calculated at archiving according to the settings.

## Production

### Objectives
- Definition of customized production settings

### Benefit
- Standard settings for producing certain lites made in customer master data can be adopted for orders. They do not have to be entered all over again.

### Note

**Production settings**
Settings for grills and spacers are automatically adopted for the order if the corresponding product is entered for the customer. The entries can be adjusted in the order.

**Distance**
The distance is used for calculating the travel costs. A distance fee has to be entered for the route for this purpose.

**Capacity areas**
Capacity areas can be entered for the three main product types (IG, laminated glass, tempered glass), shares of which can be reserved for the main customers (key customers).

### Production Settings
You can enter default settings for production in every customer's master data. These settings will be used as default settings for orders entered for the customer, e.g. a certain grill type.

**Fig. B-61**: Partner management - Production settings
- **A**: Production capacities
- **B**: Settings for the customer logo
- **C**: Spacer settings
- **D**: Grill settings
- **E**: Number of kilometers to the delivery address

A logo can be applied to the lite. The details for the logo (B) also have to be entered in management of forms.
Settings for grills (D) and spacers (C) are automatically adopted for the order when the corresponding product is entered for the customer. The entries can be adjusted in the order. grills and spacers will be described in detail in the session on product management. The entries can be adjusted in the order. grills and spacers will be described in detail in the session on product management.
The distance (E) is used for calculating the travel costs. A distance fee has to be entered for the route for this purpose.

### Capacity area
You can define total capacities for the three main product types (IG, toughened, laminated glass). Shares of these total capacities can be reserved for the main customers (key accounts). These shares are defined in customer master data. Customers for whom no capacities have been defined, will be collected in a group to which the remaining capacity is allocated.
These details are analysed by module Customer-based capacity information system.

**Fig. B-62**: Capacity information system

At order entry you can use the function Capacity info by customer to check the capacity left for production. This information is just a rough indicator as to whether the date requested for an order is actually feasible.

> **Capacities have not been scheduled**
> This display does not show the current capacity planning. To check the use of machinery you have to start capacity planning and schedule the orders.

### Editing Data for Production
The following instructions are based on the steps described in the previous session.

#### How to enter customer settings for production
1. Go to menu Master data > Partners > Customer > Customers > tab Production.

**Fig. B-63**: Partner management – Production
- **A**: Layout and product number of the customer logo
- **B**: Spacer settings
- **C**: Grill settings
- **D**: Distance

2. Enter the distance to the delivery address (D).
3. Make the standard setting for the spacer (B) and the grills (C).
4. Select in the menu Start > Save to save the data.
The data will be saved.

### Exercises
- Enter a credit limit for your customer. At order entry, you will see how the data are displayed.
- Skip these exercises if you are not going to use credit limits in your installation.
- Enter a new, general calendar.
- Draw up a customer calendar including holidays for your customer. Choose days in the near future so that you can check the postponement of invoicing.
- Assign two salesmen to your training customer. Enter a new Salesman 2 for this purpose.
- Check whether the following entries exist for one of your training customers and complete the data if necessary:
  - The customer has a subsidiary and two employees.
  - The invoice address matches the shipping address.
  - The customer is part of the North route. Enter the distance between your shipping stock and the destination.
  - Enter the communication paths (document dispatch).
  - Enter the payment terms and tax rates.
  - Enter another customer and two suppliers; this will give you more details to choose from and more possibilities for comparison in the following exercises.

## Additional Data for Partners

### Objectives
- Defining the customized price view.
- Defining customized (different) roundings.
- Calculating and setting the delivery time.
- Defining and allocating projects.

### Benefit
- Partner-specific settings make document input easier.
- Documents for customers and suppliers can refer to the same (building) project.

### Note

**Parameters**
You can define how prices of certain products or product groups are going to be shown in an order.

**Delivery Time**
The delivery time is the time it takes the lorry to get from your plant to the customer. It is defined by route and customer.
The delivery time defined will be considered at order entry to determine the production date.

**Rounding**
Two different values are used for calculating the rounding:
- The number of digits and the rounding type, e.g. upwards or downwards.
- The rounding point defines what is going to be rounded, e.g. the surcharge.

**Projects**
Projects are actual construction sites involving customers and/or suppliers.
Projects can be connected with certain terms, e.g. special prices or discounts which are automatically used for pricing if the project is allocated.

### Order Parameters
For order input you can define how prices are going to be displayed if a certain product or a certain product group is selected. These settings apply to a customer or a customer group.

**Fig. B-64**: Customer - Order parameters
- **A**: Customer group
- **B**: Product group
- **C**: Cursor position
- **D**: Price view

This example shows that prices for the selected customer group (A) will always be shown explicitly (D) when a product of the selected product groups (B) is entered.
The appropriate settings for entering purchase orders are made in Supplier > Parameters.

### Delivery Time
The delivery time is defined by route. A route usually takes one day. Special routes can be defined if the journey is longer. The delivery time defined will be considered at order entry to determine the production date.

**Example**
- Shipping date: Date on which the goods are passed on to the driver
- Delivery: Delivery date = arrival of goods at the customer's
- Delivery time: 3 days

*In this example, the order must be reported completed on 18.05.*

The delivery time is entered in dialog Delivery time.

**Fig. B-65**: Delivery time for customer
- **A**: Route
- **B**: Priority
- **C**: Delivery Time

This example shows that the same route (A) covers several customers. The delivery time (B) is the same for these customers but the sequence of delivery is different (C).

### Roundings
Calculated values for prices, tax, and surfaces are usually rounded. Rounding is managed in two ways:
- Standard allocations
- Different rounding for certain products for customer/supplier or customer group/supplier group

**Fig. B-66**: Rounding for customers

This example shows that the glass price for IG lites shall be rounded for a certain customer.
Two different values are used to calculate the rounding. First, the rounding itself, i.e. the number of digits and the rounding type. Secondly, the rounding point, i.e. the object of the rounding.
The following settings are used for calculating the rounding:
- Master data > Order > Rounding = rounding value, digits, and rounding type
- Master data > Order > Rounding allocation = calculation size that can be rounded
- Master data > Order > Rounding allocation = rounding points and the rounding used

These settings will be dealt with in detail in Tutorial 2.
⇨Tutorial 2, "Roundings" on page B-515

### Projects
Projects are actual construction sites involving customers and/or suppliers. A+W Business can handle a variety of project information. This includes special terms, e.g. special prices or discounts which are automatically used for pricing if the project is allocated.

> **Prerequisite**
> A+W Business offers different modes for project and invoice management. Projects can only be defined and edited in one of the project management modes. These modes are described in detail in Tutorial 2.
> ⇨ Tutorial 2, "Project/invoice management" on page B-568

You define the general conditions for the project, e.g. time limits. After this time has elapsed, the project can no longer be allocated in a document.
The values for estimated order totals or quantities will not be checked. You can use the specific customer and supplier overviews to display the allocated orders, purchase orders, and quantities in order to keep track of the quantities sold.

**Fig. B-67**: Allocating projects to partners
This diagram shows how different customer and supplier projects relate to central project definitions.
- **Project A (e.g., city hall)** is linked to:
  - **Customer A:** Valid until 31.12., Max. surface 150 sqm, with a standard price list and project-related discounts.
  - **Supplier A:** Valid until 01.11., Max. surface 50 sqm, with a purchase price table and project-related discounts.
- **Project B (e.g., convention hall)** is linked to:
  - **Customer B:** Valid until 01.01., Max. quantity 400 pcs., with a project-related price table and standard discounts.
  - **Supplier B:** Valid until a certain date, Max. surface 50 sqm, with a project-related price table.
- **Project C (e.g., hospital)** is linked to:
  - **Customer B:** Valid until 01.03., Max. quantity 400 pcs., with a standard price table and project-related discounts.

These examples show how the settings and terms for customer and supplier projects can differ.

### Definition and Allocation of Projects
For a detailed description please refer to the session on Invoice management.
⇨ Tutorial 2, "Project/invoice management" on page B-568

Working with projects requires three steps:
- The right mode for project management must be set in company data.
- Projects are first entered in simple basic tables as described in the session on basic tables. This dialog is found in Partners > General > Projects.
⇨ "Extending basic tables" on page B-93
- Allocating a project to customers and/or suppliers. A project can be allocated to one or several customer(s) or supplier(s). For every customer, enter the maximum amount, surface, and pieces. You can also enter project-related prices and terms.

> **Prerequisite**
> A+W Business offers different modes for project and invoice management. Projects can only be defined and edited in one of the project management modes. These modes are described in detail in Tutorial 2.
> ⇨ Tutorial 2, "Project/invoice management" on page B-568

#### How to check the project management mode
1. Go to menu Master data > Company > Company data
2. Go to tab Documents.

**Fig. B-68**: Activate project management
- **A**: Company data > Documents
- **B**: Project management mode

3. Select the Standard project management mode.
This mode permits to enter and allocate projects.
4. Select in the menu Start > Save to save the data.

#### How to allocate a project to a customer
1. Go to menu Master data > Partners > Customer > Projects.
Dialog Projects appears. The display on the tab depends on the active project management.
2. Go to the menu Start > New to switch to the input mode.

**Fig. B-69**: Fields for new project are accessible
- **A**: Project
- **B**: Customer
- **C**: Define the time during which orders can be entered for this project.

In this example, standard project management is active.
⇨ Software Reference, "Projects (Customer, Supplier)" on page B-861
3. Select the project (A) and the customer (B).
4. If required, enter a space of time (C) for the validity.
The validity will be checked at order entry. The project will no longer be offered for selection after the defined time has expired.
Project management is described in a separate session.
⇨ Tutorial 2, "Project/invoice management" on page B-568
5. Select in the menu Start > Save to save the data.
The data will be saved. You can now enter an order for this project for the customer.

### Exercises
- Enter the delivery times for your customers.
- Create a project and allocate it to your customer. If you cannot create projects: Which settings have to be changed?

**Additional information**
- ⇨ Tutorial 2, "Project/invoice management" on page B-568
- ⇨ Software Reference, "Projects" on page B-801
- ⇨ Software Reference, "Delivery Time (Customer, Supplier)" on page B-860
- ⇨ Software Reference, "Projects (Customer, Supplier)" on page B-861
- ⇨ Software Reference, "Projects - Documents" on page B-871
- ⇨ Software Reference, "Claims Calculation" on page B-874
- ⇨ Software Reference, "History of Claims" on page B-875
- ⇨ Software Reference, "Different Customer/Supplier Groups" on page B-878

## Supplier data

This set of topics shows you how to enter master data for suppliers.
Menu Supplier offers the following dialogs for this purpose: Apart from the supplier data described in this set of topics, you have to enter other data for your supplier.
- "Lieferantenspezifische Daten" auf Seite B-229

This includes the following training sessions: Menu Supplier offers the following dialogs for this purpose:
- Supplier discounts
- Parameters
- Delivery Time
- Projects
- Rounding
- Supplier group rounding
- Different supplier groups
These data are entered in just the same way as customer data.
⇨ "Customer Data" on page B-95

### Supplier-Specific Data

#### Objectives
- Introducing special features of supplier data.
- Check supplier file.

#### Benefit
- Purchase orders can be directly sent to the supplier by means of the defined communication channels.
- Standard suppliers are automatically entered in the purchase order. They can be changed however if necessary.
- Based on the delivery time, the dates for purchase orders and reference orders are calculated.

#### Note

**Supplier data**
Supplier master data differ only slightly from customer master data. You can also define and allocate e.g. groups, rounding, and projects.

**Differences from customer master data**
The following details are not required for supplier data:
- Credit standing
- No reminders
- Direct debiting
- Salesman in charge
- Packaging details

**Supplier File**
Products and product groups are allocated to the corresponding suppliers. Based on the delivery times and purchase prices, the most favorable and/or fastest supplier can be chosen when a purchase order is entered.

### Supplier File
The supplier file defines which products or product groups are delivered by the individual suppliers. The supplier file is checked when orders which include purchased articles are directly transferred to purchasing. Since the purchase pool is ignored in this event, defining a standard supplier is essential.

**Fig. B-70**: Supplier File
- **A**: Delivery Time
- **B**: Rank 1 = Standard supplier
- **C**: Allocated products
- **D**: Suppliers of the selected product

This example shows that the current supplier can provide different products (C). Moreover, the selected product can be provided by several suppliers (D). This is why you need to define the supplier who shall be selected by default (B) at transfer to purchasing. All possible suppliers with a hierarchy number of >1 will be offered for selection in dialog Price comparison.
The details from the supplier file will be ignored if an alternative supplier is entered for an item or a BOM element in the document header.
These are described in detail in section Purchasing.
⇨Purchasing, "Supplier file amendment" on page D-1855

### Checking a Supplier's Master Data
This session shows you how to enter the supplier master data. We will only deal with the special features which differ from customer master data.

#### How to edit supplier master data
1. Go to menu Master data > Partners > Suppliers > Suppliers.
2. Search for the supplier the data of whom you want to check.

**Fig. B-71**: Master data - Suppliers
- **A**: Data for correspondence
- **B**: Data for communication

3. Check in the Address tab whether the data for written correspondence and communication are complete and up to date.
The email address can also be used for the exchange of electronic documents, e.g. PDF files. Make sure that the syntax is correct and complete.
4. Go to tab Order and check whether document dispatch has been set correctly.

**Fig. B-72**: Fax and email dispatch (example settings)
- **A**: Fax inquiry
- **B**: Email order confirmation

5. Select in the menu Start > Save to save the data.
The data will be saved.

### Exercises
- Enter at least one supplier.
- Check the existing supplier groups.
- Add a supplier group for training purposes.
- Check whether products or product groups have already been allocated in the supplier file.
- Define your training supplier as the standard supplier for a tempered glass product. If no products are available in your installation yet, do this exercise later, at the end of the training session on products.

**Additional information**
- ⇨ Software Reference, "Partner Management" on page B-808
- ⇨ Software Reference, "Supplier List" on page B-888
- ⇨ Software Reference, "Declaration" on page B-892

## Product data
This section shows you how to enter and maintain the master data for your product range.
This includes the following training sessions:
- "Produktverwaltung" auf Seite B-234
- "Produkt" auf Seite B-239
- "Fertigung" auf Seite B-260
- "Preis und Zuschläge" auf Seite B-267
- "Lager und Einkauf" auf Seite B-272
- "Modell und Stückliste" auf Seite B-277
- "Produkt anlegen" auf Seite B-284
- "Lagermaße und Varianten" auf Seite B-302

### Product Management

#### Objectives
- Introducing the basic data (settings) for product definition.
- Introducing the function of product types and groups.

#### Benefit
- Basic data make product master data definition and maintenance easy.
- Basic data entered for a product can be changed at order entry.

#### Note

**Basic data**
Basic data are allocated to a product, e.g.:
- coating layers or patterns
- colors for distinguishing product variants
- groups for allocating prices and surcharges

**Product type**
Products are distinguished by product type.
The product type determines the data that are necessary for product definition. The corresponding fields are accessible in dialog Product management.

**Product groups**
Product groups unite the products for transfer to production and for internal program purposes.
Each product is allocated to a product group.

**Product master data**
Product master data are used for describing products. This includes the structural description (product structure) and the price.

### Introduction of the Subject 'Products'
A+W Business can handle your individual product structure. A product in A+W Business is something that is listed as an independent order item. These are all standard products which exist in the price list. This means that processing steps, deposits, surcharges or glass door systems are defined as products just like an IG unit or a single annealed lite.

| Glass, third party products | Processing steps | Other services |
| --- | --- | --- |
| Float 4 mm | Ticket window | Down payment |
| IG | Bevelling | Waste glass disposal |
| Shower | Mitre | Freight costs |
| Emergency glazing | Drilled hole | Shipping fee |
| Gas | Edges arrissed | Deficit qty. |
| Leaded designs | Edge stripping | Assembly |
| Fittings | Silk screen printing | Special discount |

These examples also show the so-called third party products which are defined as products but which are just sold on as merchandise, e.g. fittings.
Apart from these third party products there are products which are ordered only by a certain customer, or which are provided by the customer. These have to be marked accordingly in product master data.
A product is entered in an order with the following details:
- **Structural description:** Bill of materials, sizes and measure, quantity and quantity units.
- **Price description:** Price per quantity unit, surcharges, discounts
The structural description includes among others the product type and product group, glass type, and the glass thickness which are entered in basic tables and allocated to the product.

**Fig. B-73**: Interaction of basic data in product management
This diagram illustrates that various basic data components flow into the "Dialog Product Administration".
- **Structure Coating**, **Glass type**, and **Variant** are inputs.
- **Product type**, **Product class**, and **Product Group** are also inputs.
All these elements combine to define a product within the system.

This example shows the interaction of basic data for defining and maintaining partner master data.
In the orders, you can only enter products defined in product master data. This means that products have to be defined also for down payments, processing, surcharges, etc. This makes sure that orders clearly refer to products and can be statistically analysed.

### Product Management Dialog
Product data are entered in A+W Business as product master data in dialog Product management. These master data are used in documents and can be changed there if required. Amendments made in the documents will not be saved in master data.
Product master data include details for production, for structural description (BOM), and prices. These data are entered on the different tabs in the Product management dialog.

**Fig. B-74**: Dialog Product management - tab Product (example)
- **A**: Product name and short description as name 2
- **B**: Allocation of product type and group
- **C**: Measures, details for stock management and pricing

Product master data and bills of material are the basis of pricing and cost calculation, purchasing, materials and time management, technical checks, etc. Production-relevant data are transferred to production. For every product, codes have to be entered for production, pricing, discount calculation, etc.
These codes will be introduced in this session.

### Master Data Dialogs for Products
Menu Products offers the sub-menus General and Articles where you can enter general and product-related data. All these dialogs are described in detail in the software reference.
⇨ Software Reference, "Products" on page B-642
Apart from the data entered in the dialogs in menu Product, further data from the following dialogs can be used for product definition:
- **Prices:** Price list, key, rate, and Price
- **Surcharges:** Other surcharges, exchange surcharges, shape surcharges
- **Finances:** Tax, cost type, cost centers

> **Description of dialogs in other sections**
> Some of these dialogs are described in detail in other sections. These dialogs will not be handled in detail in the master data tutorial.
