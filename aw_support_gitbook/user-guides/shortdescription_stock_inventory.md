---
title: "ShortDescription Stock Inventory"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["ShortDescription_Stock_Inventory"]
version: "1.0"
last_updated: "2025-12-10"
description: "A+W Business / ALFAK  Short Description Stock & Inventory                                           English Revision Overview  Part                                      Version / Date                       Changes  Short Guide                               1.0 / 13.06.2013                     Initial Version   Notes on this Document  This document is intended for end users of A+W Business. This documentation and the software it describes are issued only in connection with licenses and must be u"
source_file: "ShortDescription_Stock_Inventory.pdf"
---


# ShortDescription Stock Inventory

A+W Business / ALFAK

Short Description Stock & Inventory




                                      English
Revision Overview
 Part                                      Version / Date                       Changes
 Short Guide                               1.0 / 13.06.2013                     Initial Version


Notes on this Document

This document is intended for end users of A+W Business.
This documentation and the software it describes are issued only in connection with licenses and must be used
and copied only accordance with this license. The contents of the documentation are only informative and are
subject to changes without prior notice. Text and illustrations were compiled with utmost care. Still, errors cannot
be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be at-
tributed to willful or grossly negligent action. This document describes the full scope of A+W Business in connec-
tion with A+W Production.

A+W Software GmbH cannot be held liable for data errors resulting from the basics of the standard functions pro-
vided by other software providers (e.g. functions of operating systems and / or data base systems)..


Copyrights

© 2013, A+W Software GmbH, all rights reserved, including the right of reprint, production of copies, and transla-
tion. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any
other form only in accordance with our license agreement. Without the prior, written consent of A+W Software
GmbH, the documentation must not be transferred, neither electronically, mechanically, by recording, or in any
other way.

Trademarks

All hardware and software names mentioned in this documentation can also be registered trademarks, and should
be considered as such. Third party copyrights have to be obeyed.




                          A+W Software GmbH  Konrad-Adenauer-Straße 15
                          35440 Linden  Germany
                          Tel. +49 6403 970-0  Fax +49 6403 64390
                          www.a-w.com  zentrale@a-w.com
                          © A+W Software GmbH
Contents
Revision Overview                                                    2
   Notes on this Document                                             2
   Copyrights                                                         2
   Trademarks                                                         2

Default Settings in Master Data                                      5
   Stock Definition                                                  5
   Settings in the Company Table                                     6
   Status Changes Based on Additions to and Withdrawals from Stock   7

Definitions in Product Master Data                                    9
   Products as Stock Articles                                         9
   Stock Sizes                                                       10
   Purchase Prices and Average Purchase Price                        12

The Stock Management Module                                          13
   Defining Stock Articles in Stock Management                       14
   Stock Movement                                                    17
   Queries 18
   Stock Statistics                                                  21
   Stock Search                                                      22

Order Entry of Stock Articles                                        23

Stock keeping on BOM Level                                           26

Stock P.O.s                                                          28

Stocktaking                                                          29
   Inventory List                                                    29
   Target Stock Calculation                                          29
   Block Entry                                                       30
   Inventory Management                                              30
   Closing Inventory                                                 30
   Supplementary Stocktaking                                         30

Annex                                                                31
   Opening Inventory for Using the Stock Module                      31
   Stock Modes and Procurement Types                                 31
   Purchase Price Selection for Orders                               32
                                                                              A+W Discovery – Short Description Stock & Inventory




Revision Overview                                                         3
Default Settings in Master Data
In master data, the basic settings for using the inventory management have to be defined in both the stock
catalogue and in the company table.


Stock Definition
The available storage places are entered in Master data - Stock. On catalogue
levels 1 to 4 you can define up to four levels of differentiation, distinguishing
e.g. different warehouses, aisles, shelves, and slots.




Allocation of the levels to each other - and therefore the actual definition of storing places - is done in Stock
Definition.




                                                                                                                        A+W Discovery – Short Description Stock & Inventory




Here you can define whether the storage place in question is e.g. a pure raw material stock etc. (section
Parameters). At present, these fields only serve for information and have no further effects (exception:
printing of the inventory list).




Default Settings in Master Data                                                                                     5
The individual stock levels are named by means of the function
Definition/Stock levels.




You can also define stock categories which
permit the grouping of stock products.



These stock categories can be freely defined and are allocated to the stock products in Stock Management.
Similar to the product types, stock categories are the basis for a detailed search for stock articles in Stock
Search.




Settings in the Company Table
On the one hand, the company table defines whether the average purchase price shall be determined or if
the last entered purchase price shall always be used in connection with the stock (section Purchasing). On
the other hand, you can define whether the reservation of stock articles shall result in the updating of stock,
i.e. automatic withdrawal after shipping (depending on the allocated status) (section Stockkeeping mode).


Moreover, you can enable the stockkeeping on BOM
level in the company table (see chapter Stockkeeping
on BOM Level).




                                                                                                                      A+W Discovery – Short Description Stock & Inventory




The individual options have the following meanings:
Ignore combined stock articles without sizes:
         • When determining the evaluated average purchase price, this option will ignore the (often
            negative) stock of 0 x 0 (or sqm) records on stock.
         • Combined stock articles usually serve to handle both articles for which sizes have been defined
            as well as those without sizes, i.e. based on the reports from production, quantities reserved
Default Settings in Master Data                                                                                   6
             by the 0 x 0 record will be deleted, and the corresponding stockplates will be withdrawn. If the
             user does not get any report from production, the stock of sqm articles will soon become
             negative, distorting the costs.
        •    This option will therefore only be used to calculate the average cost of the stock sizes.


Execute stock booking before printing the forms:
        • This option permits to reverse the sequence of stock booking and printing of forms. If this
             option is active, the stock booking will be made before the form is printed. If stock withdrawal
             causes a problem, the order will be removed from the list of documents to be printed. It will
             not be printed.
        • Attention: When enabling this option please make sure to check the status allocation for stock
             withdrawals. The minimum-, allocation- and lock status has to be defined in such a way to
             permit stock withdrawal before printing. If this is neglected, the stock withdrawal may not be
             made at all!


Stock control even without document type Stock P.O.:
        •    Partial P.O./delivery is now possible for stock P.O.s. The above-mentioned option must be en-
             abled for this purpose. Setting this switch is prerequisite for the partial purchasing of stock
             articles because the document type Partial Delivery clashes with the document type Stock P.O.
             The quantity delivered for a stock P.O. is adopted for the partial P.O. if part of the goods have
             been booked as received.
        •    If the switch Stock management without document type Stock P.O. is set, this product will be
             kept on stock even without setting the document type.



Status Changes Based on Additions to and Withdrawals from Stock
Withdrawals and additions to stock can change the status of documents and thus lead to a change of stock
on hand. Based on the status management, the order status is automatically set to <72-Withdrawal> when
the delivery note is printed. At the same time, the stock quantities reserved at order entry will be deducted
from the actual stock on hand.




                                                                                                                     A+W Discovery – Short Description Stock & Inventory




Default Settings in Master Data                                                                                  7
Stock withdrawals can only be made in connection with the printing of the delivery note (status point 71) or
printing of the invoice (95). No other status point is valid at present. The reporting of optimised stock plates
is an exception.

The procedure is similar to that of the receipt of goods. When the received goods of a stock purchase order
are booked, the status of the purchase order will be increased and the received goods will be added to the
inventory. For referenced purchase orders, the status of the related order can be changed as well.

Status management also permits to define individual statuses for partial receipt of goods for orders and
purchase orders. The same applies for order confirmations received from suppliers.

For the following status points, an identical minimum status must be defined (up to version 2007):

    •    31 - Supplier's OC partially / order
    •    32 - Supplier's OC complete / order
    •    33 - Partial receipt of goods / order
    •    32 - Complete receipt of goods / order
    •    59 - Partial receipt of goods / P.O.
    •    60 - Complete receipt of goods / P.O.
                                                                                                                       A+W Discovery – Short Description Stock & Inventory




    •    62 - Supplier's OC partially / P.O.
    •    63 - Supplier's OC complete / P.O.
    •    75 - Receipt of goods on stock

Otherwise, the program will issue the error report "Failed to reach minimum status".




Default Settings in Master Data                                                                                    8
Definitions in Product Master Data
Products as Stock Articles
In A+W Business, products can be defined as production, purchase article, or stock article. The definition is
made in menu Products on tab Stock/Purchasing.




Glass stock articles are distinguished by size-related and non size-related stock articles.


Glass is defined as size-related if it is to be kept on stock as a single article with its stock sizes. Each stock
size is a separate article in this case. The quantity unit in product master data is still "sqm".

Only real stock sizes will be booked in this case. This has no effect on cutting. Valid procurement types in
orders for these stock articles are only stock withdrawal and cutting.

Non size-related stock articles are generally kept on stock by the quantity unit defined for the article in
product master data, e.g. kg articles in kg (e.g. lead) and units for single articles (e.g. fittings). If glass is to be
kept on stock only by sqm irrespective of the number of stock sizes, it has to be defined as 'non size-
related'. If those are entered including sizes e.g. at stocktaking, the glass will be converted and shown as
sqm in the closing inventory.

The combined stockkeeping mode allows stockkeeping on sqm and unit basis, with reports on the cut sizes.
This additional XOPT/XTV report (via Interface Service) even permits to withdraw cut sizes automatically
                                                                                                                               A+W Discovery – Short Description Stock & Inventory




from stock (instead of just the amount of sqm).
In the orders, the stock sizes will get the procurement type "Stock withdrawal" and cut sizes, the pro-
curement type "Stock withdrawal and cutting".

You may have to enter a different product number must be entered on tab 2. Production in field <Opti-
misation key>.
If the delivery note is printed before the XOPT report is made, the appropriate amount of sqm will be
withdrawn first. When the XOPT is made later on, this sqm booking will be corrected, and the actual
amount of stock sizes will be withdrawn.

In "Product codes", these codes can be defined individually by client or area. Stock keeping is also possible
on BOM level.

Definitions in Product Master Data                                                                                         9
Stock Sizes
In the stock size table, stock sizes and boxes can be entered which exist for certain sheets. For these stock
sizes/boxes, different product groups and price codes for sales and purchasing can be defined as well. Even
a different name can be defined which will be shown automatically when the dimensions of a stock size are
entered at order entry.




                                                                                                                A+W Discovery – Short Description Stock & Inventory




Except for one special case, the stock size table is NOT linked with the stock but will only be used for
showing differences in price and for statistics!

Stock sizes to be kept on stock as real stock articles therefore have to be defined accordingly in stock
management. Certain functions can be used to switch directly to stock management. When a new stock size


Definitions in Product Master Data                                                                         10
is entered which is also a stock article, the program will also want to know if this stock size shall be defined
as a stock article. If this is the case, the program automatically switches to stock management.

This special case refers to <Non size-related stock articles> for which a stock size has been entered in the
stock size table.

No waste will be reserved for this non size-related stock article, and there will be no transfer to production
if this size exists in the stock size table.

In practice this means that for a float 4 mm item of 500 x 500 mm with 10% of waste, 0.275 sqm (or 0.28
sqm rounded) will be reserved on stock and that the item is transferred to production if no stock size has
been defined. If a stock of 500 x 500 is defined in the product stock size table, just 0.25 sqm will be re-
served; no transfer to production is made.




                                                                                                                   A+W Discovery – Short Description Stock & Inventory




Definitions in Product Master Data                                                                            11
Purchase Prices and Average Purchase Price
Purchase prices are defined in price master data in the same way as sales prices. Basically, just one price key
is entered for the PP but you can use several PP price keys. These have to be defined as combinations of
rates as well. In practice, supplier-related prices usually have a price key.




The average PP is determined by means of stock additions and is shown in stock management. It will be
calculated for stock products only if the corresponding settings have been made in company data. In stock
management, a radio button can be used to set the view for the average prices of stock articles. The mode
"This article only" shows the PP history for the current article plus the resulting average price for this article.
When you switch to the "All sizes" mode, the table shows the average price for all sizes of this article plus
the resulting average price for all sizes.

To render the function for calculating the average costs even more flexible, and to offer the old functions
                                                                                                                      A+W Discovery – Short Description Stock & Inventory




again, an additional code has been implemented in stock management and in product stock sizes. The code
in product stock sizes defines whether or not the average costs of this article are calculated from stock. The
stock management code defines whether or not the corresponding article shall be considered for
calculating the overall average price for all variants of this article.

Pricing first checks the product stock sizes as to whether the article exists in just this variant. If so, the
average price of the stock article will or will not be calculated, depending on the code "Include". If the code
is inactive, the system will search for the price in the standard purchase price rate. If a different purchase
price code has been entered, this will override the standard rate allocated. If the article cannot be found in
product stock sizes, the system goes on searching for the average price in inventory.



Definitions in Product Master Data                                                                               12
If the average price is calculated based on stock, the exact stock article is defined first. If the article exists,
the defined price will be used. If the article does not exist, the assessed average price for all products of this
article number with an active code will be calculated. If the calculated price is 0, the system will search for
the price in the standard purchase price allocation. If the price code is entered manually at order entry, the
price is calculated only from the rate allocated to the selected price key, without searching for an average
price.

The codes do not influence the saving of costs for the corresponding stock article.




The Stock Management Module
The stock management module consists of the following elements:
•   Stocktaking:
    This is where inventory lists are compiled, the results of counting
    are entered, and the new values are transferred to stock
    management by means of the closing inventory.
•   Stock management:
    In stock management, new stock articles are entered defining the
    minimum stock, maximum stock, etc. plus possible reservations
    for certain customers.
•   Stock movement:
    This is where manual additions to and withdrawals from stock
    can be entered.
•   Queries:
    This button is used to display the booking journal, stock history,
    stock statistics, and to calculate the stock value.
•   Search:
    This module matches the search for stock articles at order entry.
•   Stock P.O.:
    Stock articles the amount of which falls below the defined
    minimum will be directly transferred to the P.O. pool for stock
    P.O.s.



                                                                                                                      A+W Discovery – Short Description Stock & Inventory




The Stock Management Module                                                                                      13
Defining Stock Articles in Stock Management
New stock articles are entered in stock management. By defining the storage place, the stock ID (for boxes),
and the different details on the stock on hand, you provide A+W Business with all necessary information for
making reservations, withdrawals, and additions to stock.




Field <Main article> allows linking several stock sizes. This means that the minimum stock has to be defined
only for the main article; the stock on hand will be checked against this.

The option <Stocktaking> defines that the minimum quantity and the purchase quantity have to be entered
for every storage place. This means that the purchase suggestion is only created for the required storage
place.

Tab 2. Prices shows the minimum, maximum, last, and average price. By multiplying this with the current
                                                                                                               A+W Discovery – Short Description Stock & Inventory




stock on hand you will get the stock value for all price types.




The Stock Management Module                                                                               14
The average price takes into account the additions in the stock module as well as the goods received
bookings.

The average PP is calculated in the following way:

         Stock on hand: 100 pcs at 15.00 € =        1500.00 €
         Stock addition: 40 pcs at 18.00 € =         720.00 €
         Stock value                         =      2220.00 €
         ÷ act. qty. on stock (100+40) _____ ÷ 140.00 pcs.
         average purchase price             =         15.86 €


New average purchase price for stock articles from 4.2.435:

With this stock management patch, the second tab offers a new table. It shows quite clearly how the
                                                                                                                      A+W Discovery – Short Description Stock & Inventory




average price is calculated. It always shows the first, initial record plus a quantity and the original price. This
is followed by withdrawals and additions (marked by the appropriate signs). If the addition is based on a
stock P.O. you will also see the P.O. number and the P.O. item.

The average price is calculated as follows:
Average price = (initial quantity * initial price) + (quantity added * price of added articles) / (initial quantity
+ price of added articles)

This calculation is made for every record of the table except for the goods withdrawn which are only used
for reducing the stock on hand.



The Stock Management Module                                                                                      15
Let us assume you have got 100 sqm at a price of 10 EUR/sqm. If 20 sqm at 6 EUR/sqm are added, the
calculation looks as follows:

Average price = ( 100 * 10 ) + ( 20 * 6 ) / ( 100 + 20 ) = 9.33 EUR/sqm

This table grows as the number of bookings increases. This way, any changes in the purchase orders can be
correctly included in the average price. Automatic surcharges which may occur in the purchase orders, will
also be proportionally included in the price. This means that you may see the P.O. number and P.O. item
plus the ordered quantity - only the price is slightly higher. This is due to the proportional surcharge (e.g.
energy or transport surcharge).

To prevent the table from growing indefinitely, its size will be reduced by archiving or when invoices are
checked. The system assumes that after the invoice check has been made, the purchase order will not be
changed. Any further changes will not be included in the average price.

This table update appears as "Initialisation". In addition to archiving and invoice checks, this booking type
will also be used if the PP is changed by hand in stock management and also for stock initialisation (start-up
of stock).

The switch "Include in total PP" has two effects: On the one hand, this stock article is included in the
calculation of the average price for all sizes while on the other hand, the PP defined in stock management
will be used as Order PP for products for which this code is active (additional condition in this case: active
code in stock sizes). If this switch is not set, the price will be loaded from the price tables.

If the setting "Last PP" is made in company data, the last PP on tab 2. "Prices" will also be updated up to the
invoice check. If the price is changed in the P.O. by hand, this update will be made when receipt of goods is
booked.




                                                                                                                  A+W Discovery – Short Description Stock & Inventory




The Stock Management Module                                                                                  16
Stock Movement
In stock movements, stock additions to and withdrawals can be booked by hand.




When you enter the product number, the table shows all stock articles/storage places for this product.
After selecting the required stock article you can enter the quantity and evaluation price. If the appropriate
code has been set in the company table, the new average PP will be calculated right away.
Receipts of boxes with an ID have to be defined in stock management because every new ID will result in
the creation of a new stock article. Stock movement only permits withdrawals with an ID.



                                                                                                                 A+W Discovery – Short Description Stock & Inventory




The Stock Management Module                                                                                 17
Queries
The Queries module unites various lists which show the stock management bookings in chronological order:

The Booking journal automatically lists all bookings resulting from orders and purchase orders (reserved,
shipped, ordered, and received). Orders will be displayed only until they are removed from the main
database.




Stock history lists all manual and automatic bookings as well as new entries, corrections, and transferred
entries from stocktaking.




                                                                                                             A+W Discovery – Short Description Stock & Inventory




The Stock Management Module                                                                             18
The booking types have the following meanings:
•    (No entry):
     If no booking type is entered, all articles will be displayed.
•    Reserved:
     Only the reserved articles will be displayed. An article will remain reserved until the delivery note or
     invoice is issued.
•    Shipped:
     Only shipped stock articles will be shown. An article is marked as shipped when the delivery note or
     invoice has been issued.
•    Cut stock size:
     This booking type is used by the XOPT/XTV report if an item has been cut from a stock size. The
     number of stock sizes will be analysed.
•    Ordered:
     Only ordered stock articles will be displayed. The code is set by a stock P.O.
•    Received:
                                                                                                                     A+W Discovery – Short Description Stock & Inventory




     Only stock articles received will be displayed. An article is considered delivered and received once its
     receipt has been booked.
•    Manual stock addition/withdrawal:
     Only manually booked stock additions or withdrawals will be displayed.
•    Stock transfer:
     Only stock transfers will be shown.
•    New entry:
     Only articles newly added to stock will be displayed. The data may have been entered during
     stocktaking or manually. The system will consider all new articles entered after the latest archiving.
•    Correction:
     Only articles will be displayed the stock of which has been considered for stocktaking. The system will
     take into account all corrections starting from the latest archiving.

The Stock Management Module                                                                                     19
•    Transfer to waste, retrieval from waste, deleted from stock:
     Internal booking types


Dialogue "Reserved stock articles" allows displaying the products reserved on stock for the orders selected
from the number manager:




                                                                                                              A+W Discovery – Short Description Stock & Inventory




The Stock Management Module                                                                              20
Stock Statistics
Inventory management now offers a supplement which allows printing stock statistics which show the
average storage time and the average stock on hand for a product.
Selection can be made for a certain period and/or certain products.




Selection produces the following results:




                                                                                                     A+W Discovery – Short Description Stock & Inventory




The Stock Management Module                                                                     21
Calculation of the average values is based on the following formulas:
 Stock on hand:          (initial stock+final stock)/2

  Stock on hand:        Initial stock+(n*final stock)
                                     n+1
                          n=number of months

 Storage time:           accounting period in days/ turnover rate. This represents the number of days
                          required to use of the current final stockat the actual withdrawal rate.

Turnover rate:            Stock withdrawals/average stock on hand. The higher this value, the shorter the
                          dwelling time of the products on stock.



Stock Search
The stock search in stock management is identical with the F3 button at item entry. It can be used to show
all stored products including their sizes and storage places.




                                                                                                              A+W Discovery – Short Description Stock & Inventory




The values listed are based on the defined filter which can be selected from the filter options.

Click the right mouse key on a line to list all orders for which this stock article has been reserved.
Column "Available" is determined as follows for boxes which have no ID number. The system checks the
number of boxes of the defined size (no matter whether or not they have an ID number). After that, the
system checks how many of them have been reserved. Both values are shown in brackets in this column,
and will be subtracted. The result appears in front of the brackets and shows the available number of those
boxes.

The Stock Management Module                                                                              22
The second tab shows the future stock on hand.

If you select a line on the first tab then switch to tab "2. Future stock on hand", you will see the future stock
on hand for all days on which goods are to be withdrawn.
The future stock on hand can be displayed on a daily basis (one line per day), by order (one line per order
plus the total quantities of this product), or by item (one line per relevant item).

A double click opens the document view.



Order Entry of Stock Articles
When stock articles are entered at order entry, all stock sizes and/or storage places can be listed by
pressing the F3 button. It is identical with the stock search in stock management.




                                                                                                                     A+W Discovery – Short Description Stock & Inventory




To view e.g. only the stock sizes in the stock size table, just disable the option "Stored goods" in the filter to
see only the stock sizes defined in the stock size table no matter whether or not these are genuine stock
products.

The desired dimensions and/or the desired storage place can be selected by means of a mouse-click. The
size will be automatically applied to the item; the quantity will be reserved when you confirm the item.




Order Entry of Stock Articles                                                                                   23
When the item has been entered and acknowledged, the stock articles are reserved.




Withdrawal of goods from stock - based on status management - is usually booked when the delivery note
is printed. In order history, this looks like that:
                                                                                                         A+W Discovery – Short Description Stock & Inventory




Order Entry of Stock Articles                                                                       24
The booking journal shows the booking type <reserved> only until the withdrawal of goods is booked.




What happens to the stock on hand if orders for which the withdrawal of goods has already been booked,
are changed later (example: withdrawal of goods upon printing of delivery note)?

1.   The status is reduced, no change of items: A reprint of the initial delivery will not result in the with-
                                                                                                                 A+W Discovery – Short Description Stock & Inventory




     drawal of goods from stock.
2.   An item is removed (status is already 72 and is not changed): The system will want to know whether
     the stock on hand shall be corrected.
3.   An item is added: The system will want to know if the stock on hand shall be corrected.
4.   The quantity is changed afterwards: The stock will be corrected automatically, without a message.




Order Entry of Stock Articles                                                                               25
Stock keeping on BOM Level
Prerequisite for this stock keeping mode is that the appropriate checkbox in company data is ticked.




The stock/purchasing code can be defined in the BOM for every element in product master data.




This definition can be made on any BOM level. If the main article has already been defined as a stock article
however, the BOM elements can still be changed if required. When you enter such a BOM article in the
order, every element defined as a stock article will appear in the stock search.
                                                                                                                A+W Discovery – Short Description Stock & Inventory




Stock keeping on BOM Level                                                                                 26
When you acknowledge the item, all BOM elements defined as stock articles will be reserved on stock.




                                                                                                            A+W Discovery – Short Description Stock & Inventory




Stock keeping on BOM Level                                                                             27
Stock P.O.s
To issue stock POs and automatically add the goods received to stock, you have to enter the document type
"Stock P.O." in the P.O. header.




Since the new document will always show the last defined document type (in this case, P.O.), you should
check the pre-set document type before saving. When the goods are received, the quantity can be booked
in module Goods Received. The quantity will be booked as stock receipt.




                                                                                                            A+W Discovery – Short Description Stock & Inventory




The booking journal offers the following evaluation:




Stock P.O.s                                                                                            28
Stocktaking
Inventory List
The inventory list is the count list which can be printed for stocktaking purposes. Articles can be
preselected; individual articles can appear as fixed sizes as well as stock sizes if stock sizes have been
entered.
If you click on "all articles", all articles will be selected for the inventory list. If you choose the code "List
current stock on hand only", the list will comprise only the articles defined as stock articles in stock man-
agement. Another, new option is "only articles with stock code". For stock sizes, the program will
automatically use "units" as a quantity unit.
Purchase price and price unit are loaded from stock management. Column "Target stock" shows an entry
only if the target stock have been enabled before in <Target stock calculation>.
The printout can be sorted by warehouse, aisle, shelf, and slot.
Purchase prices can be omitted from printing (after selecting "Print", a window appears in which the
printing of purchase prices can be disabled).
The primary key for those lists is the stocktaking date. This is the reason why a combo box exists here from
which the inventory lists can be selected.




Target Stock Calculation
                                                                                                                     A+W Discovery – Short Description Stock & Inventory




The calculation of the target stock is a prerequisite for stocktaking. It has to be made always, preferably
right before the actual count. If the target stock shall appear on the inventory list, it has to be enabled in
this module so that the target stock also appears on the count list.
This is done by simply clicking on the OK button. The stock will be updated, and the target stock will appear
on the inventory lists.
The system will not be locked for booking. The user has to make sure that there are no changes on stock
between the calculation of target stock and the end of the Stock count (not the closing inventory). Stock
additions and withdrawals can be booked in the system (target stock calculation will take care of that) but
must not be included in the counting. During the time between the handing in of counting results and the
closing inventory, the physical stock can be used again. The system will take the differences into account.

Stocktaking                                                                                                     29
The target stock can be calculated just once. Repeating the target stock calculation will not change the
original result.




Block Entry
Currently not used!


Inventory Management
This is where the stocktaking results are entered by means of the inventory list. This list matches the
inventory count list; when a quantity has been entered, the cursor proceeds to the next line in which the
next quantity can be entered.
Conversion of articles counted by unit into square metres: If an article shall be kept on stock in sqm, it must
be defined in product master data as <Non size-related stock article>. If individual sheets in certain sizes are
counted for such a sqm article, these can be entered as units. If the appropriate function is active, the
counted residue plates will be converted into sqm for the closing inventory and will be booked as such on
stock (the closing inventory printouts will show the counted units however). ATTENTION: Just one storage
place is possible for those articles.
Selected articles can also be initialised with a value of 0. To do this, select the lines in the same way as in
the Explorer, and press the right mouse key. The only option "Reset quantity for selected articles to zero"
will set the field "Quantity" to 0 for all selected articles. Newer versions offer a special function for this
purpose.
You should not delete any proofs in inventory management as this might cause problems in the closing
inventory.




Closing Inventory
Stocktaking is closed by booking the results of counting and updating the stock on hand. New stock
products in the inventory will be automatically transferred to the stock management.




       Closing inventory only once per inventory list
The closing inventory can only be made once for each inventory list. If e.g. entry errors are noticed after the
closing inventory has been drawn up, they are to be corrected in stock booking/management, or a new
inventory list must be created.
                                                                                                                   A+W Discovery – Short Description Stock & Inventory




Supplementary Stocktaking
The so-called additional stocktaking allows adding booked stocktaking results to other booked stocktaking
results to print a single stocktaking result for both. The menu "Functions - Add supplementary stocktaking"
in the closing inventory can be used to add other stocktaking results to the selected stocktaking results in
order to print both inventory lists together.




Stocktaking                                                                                                   30
Annex
Opening Inventory for Using the Stock Module
Step 1:
Select to Utilities / Stock initialisation "Delete stock" (stock management will be empty afterwards). Please
do not enter any new orders at this point, and do not change any old orders up to item C (otherwise, the
storage place <n.e.> will be created again in stock management, and will be used by default).
Step 2:
Draw up the inventory list including all stock articles, determine the target stock, select ALL entries in
inventory management, go to Functions and use the right mouse key to set the Quantity to 0 and set the
corresponding Standard storage place. Draw up the closing inventory. Initialise the stock (in Utilities).
Step 3:
Draw up a new inventory list, print the inventory count list for the warehouse staff, and determine the
target stock. From this point on, new orders can be entered and old orders can be changed.
Do not book any stock withdrawals or additions while counting is in progress.
When the warehouse staff has determined the actual stock on hand, please enter the correct quantities,
storage places etc. in inventory management. After the closing inventory, print the list (check the option
"Do not print articles with a stock of 0").
Initialise the stock (in program Utilities). The stock on hand is now correct.




Stock Modes and Procurement Types
                                                                                                     Autom.
                                                                                                     creation of
                                                                                                     sqm
 Stock mode          Stock size            Cutting size                          Res. SS   Res. CS   articles
 not size-related    Stock withdrawal      Stock withdrawal and cutting          sqm       sqm       yes


 size-related        Stock withdrawal      Cutting                               pcs       -         No


 combined            Stock withdrawal      Stock withdrawal and cutting          pcs       sqm       yes
                                                                                                                    A+W Discovery – Short Description Stock & Inventory




Annex                                                                                                          31
Purchase Price Selection for Orders

 Code active in stock   Code active      in   stock
 sizes                  management                         PP in order
                                                       Average purchase
         yes                       yes                       price
          no                       yes                  PP from price list
         yes                        no                  PP from price list
          no                        no                  PP from price list


The PP from price master data will generally be used for purchase orders, irrespective of the settings. This
PP can be updated based on an OC price check or supplier's invoice.




                                                                                                               A+W Discovery – Short Description Stock & Inventory




                                                                                                          32

