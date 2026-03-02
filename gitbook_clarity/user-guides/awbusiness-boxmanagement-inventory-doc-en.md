---
description: "EN_AWBusiness_Box_Management_1_2"
---


# Software Reference

---
## Stock P.O.

### Target number area

- **Client**: If you have set up separate number areas for your clients you can select the requested client here.
- **Production preparation**: If you work with production preparations, you can allocate the purchase order to a certain order area.

## Receipt and Shipping of Boxes

You will find the complete descriptions of goods receipt and shipping of goods in the Production and Purchasing sections.

This section provides information on the following subjects:
- "Receipt of Goods (Boxes)" on page K-102
- "Settings (ID)" on page K-113
- "Shipping of Boxes" on page K-114

### Receipt of Goods (Boxes)

**Documents > P.O. > Receipt of goods > Receipt of goods**

This dialog serves to enter the goods received for individual purchase orders or for the purchase orders in a Number Manager.

For booking stock on hand, you can define ID numbers to be automatically assigned if the stock P.O. includes items with a quantity of larger than 1. The ID numbers are assigned for boxes and glass (stockplates).

> **Prerequisite**
> The checkbox for the virtual assignment of item numbers must be ticked in company data.
> ⇨ "Company Data" on page K-18

This dialog offers the following tabs:
- "Receipt of Goods – Selection" on page K-103
- "Receipt of Goods -Complete" on page K-105
- "Receipt of Goods – by Item" on page K-107
- "Receipt of Goods – ID Numbers" on page K-110
- "Receipt of Goods – Protocol (ID Numbers)" on page K-112

### Receipt of Goods – Selection

**Documents > P.O. > Receipt of goods > Receipt of goods > Selection tab**

This tab is used to filter the selection and display of documents for which receipt of goods shall be checked and/or entered.
⇨ Tutorial, "Receipt of goods" on page D-118

#### Selection
By choosing the option, you define how the purchase orders shall be filtered. Open purchase orders are displayed after the search in the Complete tab so that receipt of goods can be booked.

- **By P.O. number**: The input field for the P.O. number can be accessed. Tab Complete shows the required purchase order and all reference orders.
- **By order number**: The input field for the order number is released. The Complete tab shows all purchase orders issued for the defined order number.
- **By supplier**: The input field for the supplier number is accessible. Tab Complete shows all purchase orders placed with the selected supplier.
- **By delivery note number/notification, total quantity delivered**: The input field for the delivery note number or notification number and the field for entering the total quantity can be accessed. If a dispatch notification has been imported, the actually received quantities must be entered.
- **By supplier delivery date**: The input field for the delivery date is accessible. Tab Complete shows all purchase orders to be delivered on the selected date.
- **By number manager**: The combo box for selecting the number manager is accessible. Tab Complete shows all purchase orders in the selected number manager.
- **By scanner / document**: The fields for the barcode of the P.O. number or a P.O. item are released.

#### Target Number Manager
Target Number Manager: After booking the receipt of goods, the stock P.O.s can be automatically transferred to a different Number Manager.
- If ticked: The fields in the Target number manager section are accessible. The orders are moved to the selected number manager.
- If not ticked: The stock P.O.s are not moved to a different Number Manager.

- **Employee**: Name of the employee allocated to the target Number Manager.
- **Number Manager**: Number Manager to which the stock P.O.s with (complete) receipt of goods should be moved.

### Receipt of Goods –Complete

**Documents > P.O.> Receipt of goods > Receipt of goods > Complete tab**

This tab shows all purchase orders matching the search criteria. Select a purchase order to list all reference orders.
⇨Tutorial, "Enter receipt of goods" on page D-125

#### Delivery date
- **Supplier's delivery date**: Shows the current date. You can change it to enter a delivery received before that date. The date will be adopted only for the documents selected in the list.
- **OC supplier**: You can also enter the supplier's order confirmation number for the goods received.

#### Documents
You can use the selection buttons to select some documents or cancel the selection.
The list shows all purchase orders matching the search criteria on the Selection tab. Complete receipt of goods is entered for the documents for which the Book Complete checkbox is ticked.

- **P.O. no.**: Purchase order number.
- **Book as complete**: A purchase order can be booked as complete when all items were delivered.
    - ☐ Receipt of goods is incomplete. Some deliveries have yet to be made.
    - ☑ Receipt of goods is incomplete; the purchase order will be booked as complete.
- **Status**: Current status. The status is changed after receipt of goods has been entered.
- **Supplier**: Supplier number and name.
- **Supplier's delivery date**: Delivery date stated by the supplier. This date is adopted from the purchase order or order confirmation. When you have entered the receipt of goods, the date is changed to the present date or to the date you have selected.
- **Contains boxes**: Shows the purchase orders which include boxes. This checkbox cannot be selected.

#### Appended orders
This list shows only the reference orders for the selected purchase order. If several purchase orders are selected, this list remains empty.
- **Delivery at the customer's site**: This date is adopted from the reference order. You can change it if the originally scheduled date cannot be adhered to.

### Receipt of Goods – by Item

**Documents > P.O. > Receipt of goods > Receipt of boxes > By item tab**

This tab serves to enter the receipt of goods by item for a purchase order selected on the Complete tab.

#### Goods received/issued
- **Quantity received**: Quantity already delivered for the selected item.
- **Quantity ordered, already delivered, quantity announced**: These fields show the corresponding quantities for the item selected. The fields are updated after input.
- **Storage location**: You can select a storage place for the item, for booking the stock article to. Please note that stock articles can also be booked to storage place <n.e.>. The storage location from the purchase order can be shown via the Options menu.
- **Accept surplus or shortfall**: The quantity delivered can differ from the quantity ordered. You can accept deviating quantities and thus declare delivery of the item as complete.
    - ☐ Do not accept surplus or shortfall.
    - ☑ The quantity entered is accepted; the item is booked as complete. If a stock article has been delivered, the stock on hand is updated based on the quantity delivered. The changed quantity is saved in the purchase order.

#### Confirmation
- **OC supplier**: Supplier's order confirmation number for the selected item.
- **OC delivery date**: Delivery date for the item.

#### Items
List of items included in the selected purchase order.

- **Item**: P.O. item number.
- **Book as complete**: An item can be booked as complete when the entire quantity has been delivered.
    - ☐ Receipt of goods is incomplete.
    - ☑ The item is to be booked as complete.
- **Order no.**: Order number.
- **Article**: Name of the ordered product.
- **Color**: (Color) variations that have been defined for the selected product.
- **Width / Height**: Dimensions of the ordered item.
- **Ordered**: Quantity ordered for this item.
- **Announced**: Quantity announced for the item.
- **Delivered**: Quantity already delivered for this item. For partial deliveries, this is the total of the quantities delivered so far for this purchase order.
- **Receipt**: Quantity already delivered for the selected item.
- **Accept**: If the quantity delivered is higher or lower than the quantity ordered, this quantity can be accepted. Lites that have not been ordered will only be booked on stock if they are stock articles ordered by means of a stock P.O. If the purchase order was created from an order, the stock on hand will not be updated.
    - ☐ The quantity delivered matches the quantity ordered and does not have to be marked in a special way.
    - ☑ The quantity delivered is lower or higher than the quantity ordered and is accepted. The quantity delivered is saved in the purchase order. The reference order will not be changed. Excess lites can be booked as stock on hand if required.
- **Contains boxes**: Shows the purchase orders which include boxes. This checkbox cannot be selected.
- **OC supplier**: Supplier's order confirmation number.
- **OC delivery date**: Delivery date as per the supplier's order confirmation.
- **Storage place**: Standard storage place for this stock article. Please note that articles can also be booked to storage location <n.e.>.
- **Article description 2 + 3**: Descriptions of the ordered product that are stored in the master data. For float glass, usually only description 1 is stored, which is displayed in the Article column.

#### Appended orders
The list shows the reference orders for the items. The fields are explained in connection with the Complete tab.
⇨ "Receipt of Goods -Complete" on page K-105

### Receipt of Goods – ID Numbers

**Documents > P.O.> Receipt of goods > Receipt of goods > ID numbers tab**

This tab shows the items belonging to a purchase order that includes boxes. For every box in a P.O. item, a sub-item (virtual item number) is created which can be assigned a box with a special ID number (identification number). You can define the default for the ID.
⇨ "Settings (ID)" on page K-113

> **Prerequisite**
> The checkbox for assigning virtual item numbers must be ticked in the company data.
> ⇨ Master Data, "Use virtual item numbers" on page B-940

#### Box data
- **Supplier ID number**: Box ID assigned to the delivery item by the supplier. When you enter the number, the ID numbers field shows the automatic box ID.
- **ID numbers**: The automatic box ID appears when you enter the supplier ID. For every box in a P.O. item, a separate box ID is created when you enter the receipt of goods. If e.g. 5 boxes of Float 5, size 1200 x 800 mm have been ordered and delivered, the IDs XXXX00001, XXXX00002, ..., XXXX00005 will be assigned. You can define the presetting for XXXX. ⇨ "Settings (ID)" on page K-113
- **Storage location**: Each item can be assigned a separate storage location. Please note you can also assign storage location <n.s.>.
- **Remark**: Comments can be entered here in case of peculiarities, e.g. regarding the allocation of storage locations or in connection with reservations.
- **Content**: Contents of the box selected in the list. This entry can be changed if required.
- **Prod. date**: Date by which the production of the ordered goods should be finished. This date is important for the stock withdrawal in accordance with the FiFo principle, e.g. for coated glass.
- **PP / QU**: Purchase price and price unit of the ordered item. If you change the price, the amendment will be saved in the purchase order.

#### Box items
- **Item**: Item number stated in the purchase order. An item sub-number is automatically assigned at booking if the quantity of the P.O. item is higher than 1, e.g. 1.1, 1.2, etc.
- **Description**: Description shown in the purchase order.
- **Width / height**: Stock sizes of the lites in the box.
- **Supplier ID**: Supplier's box ID as entered in the Box data section.
- **Contents**: Contents of the box as defined in the Box data section.
- **ID number**: (Automatic) ID as defined in the Box data section.
- **Storage location**: Storage location as defined in the Box data section.
- **Prod. date**: Production date as defined in section Box data.
- **Pr./QU**: Purchase price per quantity unit as defined in the Box data section.
- **Pr. unit**: Price unit that applies to the displayed price.

### Receipt of Goods – Protocol (ID Numbers)

**Documents > P.O.> Receipt of goods > Receipt of goods > Protocol tab (ID numbers)**

This tab gives you an overview of the allocated box IDs.

### Settings (ID)

**Documents > P.O. > Receipt of goods > Receipt of goods > Options menu > ID allocation group > Settings**

This dialog is used to define the ID numbers for boxes. This setting is necessary to automatically allocate individual box IDs.

If a delivery includes, e.g. an item with 5 boxes, 5 (virtual) sub-numbers will be assigned when you enter the receipt of goods. These numbers must be given a code so that, e.g. instead of the scanned box number 12345, the sub-numbers SupplierA00001, SupplierA00002, ..., SupplierA00005 are assigned.
⇨Tutorial, "Dealing with boxes" on page D-134

> **Prerequisite**
> The checkbox for the virtual assignment of item numbers must be ticked in company data.
> ⇨ Master Data, "Use virtual item numbers" on page B-940

#### Stock ID number
- **Default**: You can enter text (or numbers) of max. 15 characters which is completed by XXXXX. XXXXX represents the automatically assigned number. The text is retained until you change it. If you buy boxes from different suppliers and want to mark them separately, you have to amend the default before entering the receipt of goods.

## Shipping of Boxes

**Production > Logistics > Shipping boxes > ID tab**

This tab can be used to reserve a box or withdraw it from stock. You can only reserve boxes which were added to stock with a box ID.
⇨ Tutorial, "Issue of Boxes" on page E-146
