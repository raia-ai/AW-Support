---
description: "EN-UM-AWEnterprise_2"
---


# Market Partner

vide information about this. Ex.: if 1:100 (14873) is in the record display. This means that the first 100 entries (the hit quantity) of 14873 are loaded (into the cache). The number of entries to be loaded (into the cache) can be configured.

---
### Buttons for scrolling
Use the |<, <<, >>, and >| buttons to scroll through the hit quantity. Use the >> button to scroll forward (16 entries). Use the << button to scroll backward (16 entries). Use the >| button to jump to the end of the cache (100th entry) and |< to jump to the beginning of the cache (1st entry). To load additional entries, click the [More Data] button. Then the configured quantity of data (in our case, 100 records) is loaded into the cache.

## Description of the search fields

### From no.
Entry of a number from which the search should start.
**Technical info:** numeric field, DB field: mp.mpnr

### Matchcode
Entry of the matchcode as search value. You can enter the whole matchcode or only part of it.
**Technical info:** alphanumeric field, DB field: mp.mpmc

### Type
Display of the market partner type you are searching for. It is pre-populated according to the selection on the market partner dialog and cannot be changed.

### Name
Entry of the name as search value. You can enter the whole name or just a part of it (capitalization is not considered).
**Technical info:** numeric field, DB field: mp.name

### 1st Name
Entry of the first name as search value. You can enter the whole name or only part of it.
**Technical info:** alphanumeric field, DB field: mp.vname

### Street
Entry of the street as search value. You can enter the whole street or only part of it.
**Technical info:** alphanumeric field, DB field: mp.strasse

### Site
Selection and input of the site number/client number as search value. Entry here only makes sense if the extended multi-client system is configured since only then can market partners be assigned to a client.
**Technical info:** numeric field, <F9>, DB field: mp.hausnr

### Cntry
Selection and entry of the country as search value. The appropriate codes can be assigned via the Country (Keys > Market Partner) menu.
**Technical info:** alphabetic field, <F9>, DB field: mp.kfz

### PCd
Selection and entry of the postal code as search value. You can enter the whole postal code or only part of it.
**Technical info:** numeric field, <F9>, DB field: mp.plz

### City
Selection and entry of the city as search value. You can enter the whole city or only part of it.
**Technical info:** alphabetic field, <F9>, DB field: mp.ort

### VAT ID No.
Entry of the VAT identification number as search value. You can enter the whole number or just a part of it (capitalization is considered).
**Technical info:** numeric field, DB field: mp.steuernr

### Type
Selection of the type as search value:
- **active:** Only active market partner are displayed.
- **closed:** Only closed market partners are displayed.
- **all:** All market partners are displayed.
**Technical info:** alphabetic field, <F9>, DB field: mp.still

## Address tab
**Master Data > Market Partner**

*Fig. B-9: Address tab*

On this tab, you enter and/or edit the invoice address for the market partner. The tab is divided into a left and right side. The left side includes the market partner's address data and is present during the entire editing process. The right side displays the data from other tabs and additional options.

Use <F5> to open a dialog on which you can store note texts for the market partner.
⇨ "Market partner - note texts" on page B-106

Use <Shift><F5> to open a dialog on which you can store product note texts for the market partner.
⇨ "Article - notes" on page B-385

Use <Shift><F9> to jump to the Matchcode field.

> **Asian installations**
> Asian installations include additional text fields for the input of addresses.

### Name
Name of the market partner.
**Technical info:** alphabetic field, DB field: mp.name

### 1stName
First name of the market partner.
**Technical info:** alphanumeric field, DB field: mp.vname

### Title
Selection of the title, e.g. Mr. or Mrs. (Master Data > Keys > Market Partner > Titles).
**Technical info:** <F9>, DB field: mp.anrede

### Attn.
For the attention of. Name of the postal recipient for company addresses.
**Technical info:** alphabetic field, DB field: mp.zhd

### Addition
Field for addition, e.g. the industry.
**Technical info:** alphabetic field, DB field: mp.branche

### Street
Street for the address.
**Technical info:** alphanumeric field, DB field: mp.str

### PCd, POB
The postal code corresponding to the post box and the number of the post box.
**Technical info:** alphanumeric field, DB field: mp.pfplz / mp.postfach

### PBox City
The city assigned to the postal code.
**Technical info:** alphanumeric field, DB field: mp.pfplz / mp.pfort

### PCd, City
Postal code corresponding to the city and the city.
**Technical info:** alphanumeric field, DB field: mp.plz / mp.ort

### Country
Country code and the corresponding country.
**Technical info:** alphanumeric field, DB field: mp.kfzcode / mp.land
⇨ "Countries" on page B-203

### Distance
The distance between your company and the market partner in kilometers. Is used in the discount/surcharge calculation (e.g. transport surcharge) as scaling basis.
**Technical info:** numeric field, DB field: mp.kilometer

### Phone
Telephone number of the market partner (land line number).
**Technical info:** numeric field, DB field: mp.telefon

### Mobile
Telephone number of the market partner (land line number).
**Technical info:** numeric field, DB field: mp.mobile

### Fax
Fax number of the market partner. With the toggle field next to this, you control whether the market partner would like to have the documents via fax. Possible values: Y/N. Is evaluated in the form printing and with appropriate configuration, allows the automatic faxing of documents to the market partner.
**Technical info:** numeric field, DB field: mp.faxnr

### E-mail
Market partner's e-mail address. Use <F5> to store several e-mail addresses. Is evaluated in the form printing and with appropriate configuration, allows the automatic sending of documents to the market partner via e-mail.
**Technical info:** alphanumeric field, DB field: mp.email

### Website
Market partner's URL. Start the browser with <F5>.
**Technical info:** alphanumeric field, DB field: mp.website

### Language
Selection of the language in which the customer receives documents, e.g. German or English (Master Data > System > Languages). The texts are generated according to this definition during the document entry and with appropriate configuration, the expressions for market partners are created in the specified language.
**Technical info:** <F9>, DB field: mp.sprkz

### Notes
The texts serve as important information in various parts of the program. This way, the entries can be displayed in the order entry with selection of the customer on the screen. There are two different note texts:
- <F5> starts the dialog for general note texts for the market partner.
- <Shift><F5> starts the dialog for product-related note texts for the market partner.
**Technical info:** DB field: memo.txt

#### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Market partner - note texts
**Master Data > Market Partner > F5**

*Fig. B-10: Market partner - note texts*

On this dialog, you can store texts for market partners; these serve as important information in various parts of the program. At the top of the dialog, you see the market partner number for which the text applies.

> **Multilingual note texts**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Notes. However, this is only possible if you are working with the multilingualism for employees within the internal client separation module.

### Language
Language ID.
**Technical info:** numeric field, DB field: xsprbez.sprkz

Enter the text in the free field and store it with <F3>. Use <Shift><F9> to specify the info location:

- **Master data:** The text is only displayed in the master data.
- **Everywhere:** The text is displayed in the master data and in the sales and purchasing documents.
- **SA-order:** The text is displayed in the sales document.
- **PU-order:** The text is displayed in the purchasing document.

Use <Shift><F10> to specify the priority:

- **high:** The text is displayed automatically in the specified info locations as soon as just one line has the Prio=high.
- **Low:** The text will not be displayed automatically; it has to be loaded via menu at document entry.
**Technical info:** alphanumeric field, DB field: memo.txt

> **Priority of info position master data**
> If you have selected Master data as Info position, the priority low is invalid. The text will always be displayed in the market partner's master data.

## Identification tab
**Master Data > Market Partner > Identification tab**

*Fig. B-11: Market Partner - Identification tab*

On this tab, you enter and/or edit all tax and commission-related data for the market partner.

> **Left side of the dialog**
> During editing of the right side of the dialog, the customer's master data remains visible on the left side of the dialog. If changes are required, these have to be made on the Address tab.

### VAT ID No.
EC tax number, that is, the VAT ID number. With the entry of the VAT ID No., there is a country-specific check. This number is used primarily in the FinAc transfer.
**Technical info:** alphanumeric field, DB field: mp.steuernr

### Taxpay. no.
Specification of the taxpayer number that is used primarily in the FinAc transfer. It is also possible to configure the system so that entry of credits is not possible without Taxpay. No.
**Technical info:** alphanumeric field, DB field: mp.finstrnr

### Company name
Complete company name of the market partner, e.g. Schmidt GmbH & Co. KG.
**Technical info:** alphanumeric field, DB field: mp.firmname

### Ext. supplier no
If the market partner specifies its own supplier number, you can store it here. This field is used primarily in the FinAc transfer.
**Technical info:** alphanumeric field, DB field: mp.exlinr

### Ext. customer no
If the market partner specifies its own customer number, you can store it here. This field is used primarily in the FinAc transfer.
**Technical info:** alphanumeric field, DB field: mp.extkundnr

### Ext. project no.
This field is only active if the market partner is of the type. Then you can store an external project number here.
**Technical info:** alphanumeric field, DB field: mp.extkundnr

### Supplier no.
Selection of the supplier number. If the market partner is a customer that also functions as supplier, then you can assign the supplier number here. This field is used primarily in the FinAc transfer.
**Technical info:** <F9>, DB field: mp.lieflinr

### Matchcode
This field is used in connection with the Supplier No. field and shows you the supplier's matchcode.
**Technical info:** display field

### Misc MP
This is a market partner that orders and is deliverd to just once. In contrast to other customers in the document entry, the address for this customer can be changed:
- **Yes:** This market partner is a miscellaneous market partner.
- **No:** The market partner is kept as a permanent customer.
**Technical info:** toggle field, DB field: mp.divers

### Commission
Selection of the commission code. If the amount of the representative's commission depends on the customer, a numeric commission code has to be entered here. The commission rates for the various code values are stored in the Commission Code menu element (Master Data > Commissions). The field is only available with appopriate system configuration.
**Technical info:** <F9>, DB field: mp.provnr

### Sales repres.
Selection of the relevant sales representative. The respective commission rates for the representative entered here can be booked and they are ready for invoicing. These details can be changed later in the order. Prerequisite for the selection quantity is the function allocation Representative in the employee master data. With expanded internal client separation, this detail can also be entered client-specifically.
**Technical info:** <F9>, DB field: mp.vertrerloe

### Field staff
Selection of the responsible field service employee. These details are taken over in the order entry and if necessary, output on the customer's papers. These details can be changed later in the order.
**Technical info:** <F9>, DB field: mp.aussenmanr

### Intern.repr.
Selection of the responsible internal sales employee. These details are taken over in the order entry and if necessary, output on the customer's papers. These details can be changed later in the order.
**Technical info:** <F9>, DB field: mp.innenmanr

### Handled by
Selection of the employee responsible for the order processing. This employee is taken over in the order and if necessary printed out on the customer's papers. These details can be changed later in the order.
**Technical info:** <F9>, DB field: mp.sachmanr

#### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## References tab
**Master Data > Market Partner > References tab**

*Fig. B-12: Market Partner - References tab*

On this tab, you enter and/or edit all FinAc technical and some of the price-relevant data for the market partner. The right side displays the address information.

### Descriptions of fields

#### FinAc debtor
Selection of the FinAc debtor number. It is a reference to the customer receiving the invoice. That's why the FinAc debtor and customer number should be the same. In case of central invoice management of a company with several locations, the FinAc debtor has to be assigned the customer number of the invoicing office to which the invoices are booked and issued.
**Technical info:** <F9>, DB field: mp.stddebnr

#### Debtor statistics
Selection of the statistics debtor. Regardless of the FinAc debtor, the statistical sales can be cumulated for other statistics debtors. This could be the customer number of an ordering branch office, for example. The statistical data provides information about the sales development of the individual branch offices.
**Technical info:** <F9>, DB field: mp.statdebnr

#### Debtor conditions
Selection of the customer number whose conditions should apply for the documents entered. With extended internal client separation, the debtor conditions can also be assigned client-specifically.
**Technical info:** <F9>, DB field: mp.konddebnr

### Debtor exch./add.
Selection of the customer number. The exchange-addition rules that were stored for the customer that was noted in this field apply analogously in document entry.
**Technical info:** <F9>, DB field: mp.azdebnr

### Debtor
Selection of whether debtor:
- **Yes:** The market partner is a debtor.
- **No:** The market partner is not a debtor.
**Technical info:** <F9>, DB field: mp.debitor

### Debtor site no.
Is only active if the Debtor field has the entry Yes. Then you can assign the debtor a site. These details are only relevant with expanded internal client separation. For more details, see the A+W Enterprise configuration instructions.
**Technical info:** <F9>, DB field: mp.debhausnr

### Cond. branch
Selection of the industry, e.g. carpenter, metal construction, etc. The appropriate conditions are stored on the Industry menu (Master Data > Keys > Market Partner > Industry).
**Technical info:** <F9>, DB field: mp.kbranche

### Economic area
Selection of the economic area in which the market partner is located, e.g. France, Netherlands, Belgium, etc. The economic area is often used in a company's own statistical evaluations.
**Technical info:** <F9>, DB field: mp.kwrtraum

### Area
Selection of the area in which the market partner is located, e.g. Hessia, Lower Saxony, Bavaria, etc. The areas are stored on the Region/States menu (Master Data > Keys > Market Partner > Region/States).
**Technical info:** <F9>, DB field: mp.region

### Cost center
Selection of the market partner's cost center, e.g. insulated glass, TG, racks, etc. Cost centers are logical business areas (departments, groups) incurring calculable costs. The selected cost center can be evaluated later. Cost centers are stored on the Cost Centers menu (Master Data > Cost Master Data > Cost Centers).
**Technical info:** <F9>, DB field: mp.kostenst

### Departm.
Selection of a department, e.g. cutting, shipping, etc.
**Technical info:** <F9>, DB field: mp.abtnr

### Calendar
Selection of a market partner-specific calendar number.
**Technical info:** <F9>, DB field: mp.kalnr

### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Order tab
**Master Data > Market Partner > Order tab**

*Fig. B-13: Market partner - Order tab*

All order-related information for the market partner is stored on this tab. The right side displays the address information.

### Descriptions of fields

#### Edge prot.
Selection of the desired edge protection item that should be applied for IGUs. This way, there is an automatic entry for the customer-exchange-addition rules, which are evaluated during order entry.
**Technical info:** <F9>, DB field: mp.kantschutz

#### Std. glazing
Selection of the desired glazing item that should be applied for IGUs. This way, there is an automatic entry for the customer-exchange-addition rules, which are evaluated during order entry.
**Technical info:** <F9>, DB field: mp.stdverglas

#### Glazing
Selection of where the glazing is displayed:
- Show in item and footer
- Calculate in item
- Show in footer only
**Technical info:** toggle field, DB field: mp.verglasung

### Proj. force
Definition of whether a project must be assigned to the customer in the order:
- **Yes:** A project must always be assigned to the customer in the order.
- **No:** Project assignment is optional.
**Technical info:** toggle field, DB field: mp.objmuss

### Ext.no.req.
Definition of whether a third-party number must be assigned to the customer in the order:
- **Yes:** A third-party number must always be assigned to the customer in the order.
- **No:** The assignment of a third-party number is optional.
**Technical info:** toggle field, DB field: mp.exaufmuss

### Refer. requ.
Definition of whether a commission must be assigned to the customer in the order:
- **Yes:** A commission must always be assigned to the customer in the order.
- **No:** The assignment of a commission is optional.
**Technical info:** toggle field, DB field: mp.kommmuss

### Dimens. unit
Selection of the dimensional unit:
- Metric
- Imperial
The system has to be configured appropriately for the use of the imperial dimensional unit.
**Technical info:** toggle field, DB field: mp.massystem

### Standard AIR
Here you can specify the value for a standard spacer in mm. This value is then used to pre-populate IG items without fixed AIR in the order entry.
If a non-changeable AIR is defined for an IG article, the AIR of the article is used. If, however, the AIR is defined as changeable, the customer-specific AIR is used.
If the AIR is defined as changeable in the article master data, the customer-specific AIR can also be changed in the item entry.
**Technical info:** numeric field, DB field: mp.defszr

### min IG tot thickn.
Here you can specify the minimum thickness of a total IG unit.
**Technical info:** numeric field, DB field: mp.minszr

### max IG tot thickn.
Here you can specify the maximum thickness of a total IG unit.
Minimum and maximum thickness are checked within the restriction check in the order entry. If an order contains items that do not fulfill this restriction, the order can only be entered by authorized employees. For additional information, consult the A+W Enterprise EDP module description.
**Technical info:** numeric field, DB field: mp.maxszr

### Min. order value
Here you can store a minimum order value (customer) or a minimum order value (for suppliers). This value is taken over as a calculation basis in the order. If the order value < minimum value, the minimum value is calculated.
The minimum order value must be specified in the customer currency. Otherwise, with a currency change in the order, there is no conversion of the minimum value.
**Technical info:** numeric field, DB field: mp.relimwert

### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Delivery tab
**Master Data > Market Partner > Delivery tab**

*Fig. B-14: Market Partner - Delivery tab*

All information that relates to the supply of the market partner is stored on this tab. The right side displays the address information.

### Descriptions of fields

#### Stand. route
Selection of the route. For dispatch planning, each customer should be assigned to a route. The route is taken over in the order; if necessary, it can be changed. From there, the route is transmitted to the dispatch control system. The routes are stored in the Routes menu element (Master Data > Keys > System > Dispatch > Routes).
**Technical info:** <F9>, DB field: mp.routenr

#### Route 2-4
Definition of alternative routes that can be used if the standard route does not optimally fit the customer's requested date. For delivery date determination in the order, it is then calculated whether an alternative route is cheaper. The fields Route 2-4 can only be changed if the system is not configured for routes from the address master data.
**Technical info:** <F9>, DB fields: mp.routenr2, routenr3, routenr4

#### Load.Seq.
Definition of the loading sequence. During the composition of a route, order items from different customers are loaded onto a truck. The sequence of the loading can be specified by the Load. Seq. The entry is made freely and displayed in the dispatch control system and can be evaluated on the loading papers. Use <F9> to get an overview of which loading sequences have already been assigned.
With use of the OTR module, the loading sequence is taken over from OTR.
**Technical info:** <F9>, DB field: mp.routeposnr

### Disp.type
Selection of the dispatch type, e.g. truck, transport company, etc. This field has only an informative character for the dispatch department. The dispatch types are created on the Packing Type menu (Master Data > Keys > System > Dispatch > Disp.Type).
**Technical info:** <F9>, DB field: mp.versandart

### Pack.type
Selection of the packing type, e.g. rack, box, pallet cage, etc. This field has only an informative character for the dispatch department. The packing types are created on the Packing Type menu (Master Data > Keys > System > Dispatch > Pack. Type).
**Technical info:** <F9>, DB field: mp.verpackart

### Incoterm
Selection of the delivery condition, e.g. carriage free, self pick-up, etc. This text is intended for output on the customer papers. The delivery types are created on the Packing Type menu (Master Data > Keys > System > Dispatch > Suppliers).
**Technical info:** <F9>, DB field: mp.lieferart

### Collective del. note
Selection of whether or not a collective delivery note is possible for the market partner:
- **Yes:** A collective delivery note is possible.
- **No:** A collective delivery note is not possible.
**Technical info:** toggle field, DB field: mp.lsammel

### Partial shipment
Selection of whether or not the market partner allows partial shipments.
- **Yes:** Partial shipments are allowed.
- **No:** Partial shipments are not allowed.
**Technical info:** toggle field, DB field: mp.teilliefkz

### Handling time
Is the time between the completion of the product and the day of delivery. Such a time can be necessary if the customer makes particular specifications for the picking of its goods. It is entered as a deadline and thus considered by the date and capacity planning. The time can be entered in days or hours (configurable).
**Technical info:** numeric field, DB field: mp.hzeit

### Call before delivery
Selection whether or not the market partner should be contacted by telephone before delivery.
- **Yes:** The market partner would like to be called before delivery.
- **No:** No call is necessary.
**Technical info:** toggle field, DB field: mp.anruf

### Travel time
You can store the travel time to the market partner in days here. This value is then considered during the calculation of the delivery date.
**Technical info:** numeric field, DB field: mp.anfahrt

### Ship via
Selection whether the shipment is via another site. For more details, see the documents about plant logic.
**Technical info:** <F9>, DB field: mp.vsvia

### Type of EDI
If this market partner is an internal customer, it is possible to define here how internal orders are exchanged via EDI. The setting especially affects how the addresses in the POs generated are treated:
- **none:** There is no automatic internal PO transmission.
- **SACoupling:** The parts to be ordered are from the order in the distributor. An order is generated directly in the supplier's system.
- **PU 1:1:** The parts to be ordered are from the order in the distributor. Here, first a corresponding PO is generated at the distributor and from it, an order is generated directly in the supplier's system. For this setting, a PO contains only ordered parts from an order.
- **PU 1:n:** The parts to be ordered are from the order in the distributor. Here, first a corresponding PO is generated at the distributor and from it, an order is generated directly in the supplier's system. Here, a PO can include ordered parts from several orders.
**Technical info:** <F9>, DB field: mp.dfuetyp

### Direct P.O.
Selection for direct PO. The field is only active if the market partner is a supplier. This way, you control whether or not a PO is triggered immediately for this supplier after order release:
- **Yes:** PO is triggered immediately.
- **No:** The PO is not triggered immediately, but instead placed in the PO pool and can be triggered later.
**Technical info:** toggle field, DB field: mp.direktbestkz

### Delivery note transfer
With this checkbox, you control the automatic delivery note transfer:
- [x] The delivery note transfer is done automatically via OpenTRANS.
- [ ] There is no delivery note transfer
**Technical info:** toggle field, DB field: mp.liefdfuekz

### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Invoice tab
**Master Data > Market Partner > Invoice tab**

*Fig. B-15: Market Partner - Invoice tab*

All information that relates to the invoicing of the market partner is stored on this tab. The right side displays the address information.

### Descriptions of fields

#### Account
9-digit account number. With the introduction of the IBAN, this field is no longer evaluated.
**Technical info:** numeric field, DB field: mp.konto

#### Invoice type
Selection of the desired invoice form of the market partner:
- Individual invoice
- Cover invoice
- Collective invoice (weekly, every 14 days, monthly)
**Technical info:** toggle field, DB field: mp.rechnungsart

#### Coll. invoice limit
Here you enter how high the invoice limit for the collective invoices is.
**Technical info:** numeric field, DB field: mp.srechlimit

### Coll. invoice type
Selection of the interval at which the collective invoices are written:
- weekly
- every 14 days
- monthly
**Technical info:** toggle field, DB field: mp.srechart

### FinAc
If the connected financial accounting does not allow the separate transfer of various payment terms, this field can alternatively be provided with any alphanumeric code that is transferred to financial accounting. The concrete usage of this field depends largely on the FinAc system used.
**Technical info:** numeric field, SELO (<F9>), DB field: mp.fibukey

### Invoice transfer
Selection whether the invoice transfer in openTRANS format is possible.
- [x]: Transfer is possible in the openTRANS format.
- [ ]: Transfer is not possible.
**Technical info:** toggle field,

### Calculate racks
Selection of whether or not the market partner allows partial shipments.
- **Yes:** Racks are invoiced.
- **No:** Racks are not invoiced.
**Technical info:** toggle field, DB field: mp.gsfaktura

### Rent-free days
If you leave your customer the racks for a certain number of days when the racks do not cost anything, you can specify this number of days here.
**Technical info:** numeric field, DB field: mp.gsmietfrei

### Additional Information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Customized tab
**Master Data > Market Partner > Customized tab**

*Fig. B-16: Market partner - Customized tab*

The tab is only active if the market partner is an object and is configured appropriately. This tab summarizes all information that relates to the project. The right side displays the address information.

### Descriptions of fields

#### Sales repres.
Each project can be assigned a sales employee who is used as revenue representative for all orders participating in the project and flows into the representative commission.
**Technical info:** <F9>, DB field: mp.vertrerloe

#### Cost center
Whether the cost center should be replaced project-specifically in the order processing depends on the selected cost center procedure. If a project-related cost center assignment is desired, it can be set up by A+W.
**Technical info:** <F9>, DB field: mp.kostenst

#### Proj. force
If the entry in this field is Y, a project must absolutely be entered in the order entry.
**Technical info:** toggle field, DB field: mp.kommmuss

### Limit check
Project-oriented limit check:
- **FinAc Debtor:** Limit check during order entry.
- **MP project:** Project-oriented limit check.
**Technical info:** toggle field, DB field: mp.objlimitpruef

### Cred. limit
This field is only brought to bear if the Cred. Limit field is set to Y. If an order value including the open items and the open orders exceeds the credit limit stored here, a warning is issued.
**Technical info:** numeric field, DB field: mp.firmlimit

### VAT
Selection of the VAT code. The necessary tax codes are stored on the Tax Types menu (Master Data > Keys > System > Taxes).
**Technical info:** <F9>, DB field: mp.mwst

### Discount 1/2
Selection of the cash discount key. The required cash discount codes are stored on the Cash Discount Groups menu (Keys > System > Discount Groups).
**Technical info:** toggle field, DB field: mp.skonto1/2

### Invoice type
Selection of the desired invoice form of the project:
- Individual invoice
- Cover invoice
- Collective invoice (weekly, every 14 days, monthly)
**Technical info:** toggle field, DB field: mp.rechnungsart

### Stand. route
Any project route applies during the order processing and replaces the customer route stored in the customer master data.
**Technical info:** toggle field, DB field: mp.routenr

## Payment tab
**Master Data > Market Partner > Payment tab**

*Fig. B-17: Market Partner - Payment tab*

All information that relates to the market partner's payment options is stored on this tab. The right side displays the address information.

### Descriptions of fields

#### Cash D. 1-3
In the cash discount field, customer-specific cash discounts can be assigned as codes. Up to three scaled cash discounts are possible, whose term and percentage has to vary accordingly. The required cash discount codes are stored on the Cash Discount Groups menu (Codes > System).
**Technical info:** <F9>, DB field: mp.skonto1-3

#### Consider vacation
Selection whether the cash discount period is extended if the invoice recipient is on vacation:
- [x] The cash discount period is extended.
- [ ] The cash discount period is not extended.
Prerequisite is that the calendar for the invoice recipient in question is maintained.
**Technical info:** toggle field, DB field: mp.htag_skonto_rel

#### Pay.term
This refers to the latest possible time of net payment. After expiry of the payment term, the dunning period begins. Entry is made in days.
**Technical info:** numeric field, DB field: mp.zahlziel

### Val.date
The value date in days determines the beginning of the cash discount periods and the payment term starting with the invoice date (including mailing time).
**Technical info:** numeric field, DB field: mp.valuta

### Charact.
With this code, payment characteristics for market partner can be noted (debit, booking, etc.). The codes are stored on the Payment Characteristic menu (Codes > System).
**Technical info:** <F9>, DB field: mp.zahlngmerk

### Bonus
Here you define whether and in what amount within which period of time the customer/project receives a bonus. The bonus is not calculated automatically. This specification serves only a company's own statistical purposes. The bonus codes are stored on the Bonus menu (Codes > System > Market Partner).
**Technical info:** <F9>, DB field: mp.bonus

### Paym. transact.
Selection of the payment transaction:
- Direct debiting
- Prepayment
- On delivery
- By arrangement
- Check
- Bank debit
**Technical info:** toggle field, DB field: mp.azahlkz

> **Payment fields for Market partner type=Project**
> With appropriate system configuration, the fields Cash discount 1-Payment transaction can also be stored for projects. These payment conditions are then taken over in the block in the order insofar as the project is entered. If the fields in question remain empty for project, the information is taken over from the customer master data.

### Reminder
Selection whether in case of delay there should be a reminder.
- [x] The customer will be reminded.
- [ ] The customer will not be reminded.
**Technical info:** toggle field, DB field: mp.mahnkz

### Remind.
For information, it can be noted how many reminders have already been sent to the customer/project. This value can be transmitted to financial accounting if necessary.
**Technical info:** numeric field, DB field: mp.mahnanz

### Last CIC inquiry
Here you can enter the date of the last CIC inquiry.
**Technical info:** date field, DB field: mp.ltzschufa

### Partial invoicing
Selection of whether or not the market partner allows partial invoicing.
- **Yes:** Partial invoices are allowed.
- **No:** Partial invoices are not allowed.
**Technical info:** toggle field, DB field: mp.teilfakkz

### Currency
The multi-currency system is optional. Selection of the currency in which the market partner should be invoiced. The currency codes are stored on the Currency menu (Master Data > Keys > System).
**Technical info:** <F9>, DB field: mp.waehrung

### Calculate in
The multi-currency system is optional. Selection of the current in which orders should be invoiced:
- Own currency
- Customer's foreign currency if the customer currency deviates from the company's own currency, e.g. customer in Switzerland.
**Technical info:** toggle field, DB field: mp.waehrprs

### Print in
If you specified Foreign currency in the Calculate in field, then you control here in which currency the customer papers should be output. Possible values are:
- Calculated currency
- Foreign currency in the footer
- Foreign currency in item and footer
- Calc. currency + Euro in footer
- Calc. currency + Euro in item and footer
- Foreign currency + in footer
- Foreign currency + Euro in item and footer
**Technical info:** numeric field, DB field: mp.waehrdru

> **The fields Calculate in and Print in**
> The Calculate in and Print in fields are only accessible if the foreign currency module is licensed and a currency was assigned to the customer that deviates from the company's own currency.

## Printout tab
**Master Data > Market Partner > Printout tab**

*Fig. B-18: Market Partner - Printout tab*

All information that relates to the printing options for the market partner is stored on this tab. The right side displays the address information.

### Descriptions of fields

#### Print gross price
Selection whether the gross price should be printed:
- Yes
- No
**Technical info:** toggle field, DB field: mp.preisdrkz

#### Print MP-factor
Selection whether the market partner factor should be printed:
- Yes
- No
**Technical info:** toggle field, DB field: mp.rabdrkz

#### Print process. steps
With this field, you control whether the processing prices should be generated already in the document entry in the processing texts to be printed:
- Yes
- No
- P
Configurable possibility for generating the processings only in the texts if they are present (processing price > 0)
**Technical info:** toggle field, DB field: mp.explbearbkz

### Sub-total
Selection whether a commission-dependent subtotal should be printed:
- Yes
- No
**Technical info:** toggle field, DB field: mp.sumkomis

### OC incl. muntins
Selection whether the muntin structure should be printed with the order confirmation:
- Yes
- No
**Technical info:** <F9>, DB field: mp.sprossenab

### Gross/Net flag
Selection for gross or net flag:
- **G:** Gross flag
- **N:** Net flag
**Technical info:** <F9>, DB field: mp.brutnetkz

### Cust.-indiv. items
Selection for customer-specific item flags if there is an appropriate reference in the customer master data:
- **Item:** For customers who bear this flag, the customer item field is switched on in the order processing in order to enter the desired customer item designation. These details appear on all customer papers and labels.
- **Type:** This is the possibility for typical entry, as is frequently required for schedules of services for public bids. With this procedure, each product is assigned a specified typical designation in the course of the order entry. The printout of such an order confirmation shows in the item section only the respective type designation, while the precise product description appears in the footer of the document.
- **None**
**Technical info:** toggle field, DB field: mp.kndposkz

### Label
Selection for label text. The codes can be assigned via the Label Texts menu (Master Data > Keys > Market Partner).
**Technical info:** <F9>, DB field: mp.etikett

### Label text
If the market partner is a Project, you can enter another text for labels here.
**Technical info:** <F9>, DB field: mp.etitxt1

### Project abbr.
Since there is frequently little space available on labels, a two-letter project abbreviation can be printed on the label.
**Technical info:** alphanumeric field, DB field: mp.etitxt2

### Price presentat.
Selection for the price display on the papers according to the market partner's preference:
- No price
- QU price
- Unit price
- QU + unit price
**Technical info:** <F9>, DB field: mp.prsdarst

### Text formulas
Selection of the text formula.
**Technical info:** <F9>, DB field: mp.prsdarst

### Max. email size
Maximum size of the e-mail with attachment in MBytes. When sending e-mail, by default the attachment is compressed in the zip format. With a system configuration, you can set whether the entire attachment is compressed or only if the attachment exceeds the e-mail size entered here in the field.
**Technical info:** <F9>, DB field: mp.mailsize

## Limits tab
**Master Data > Market Partner > Limits tab**

*Fig. B-19: Market Partner - Limits tab*

All information that relates to the market partner's limits is stored on this tab. The right side displays the address information.

### Descriptions of fields

#### Check limit via
Selection of the limit check:
- **FinAc Debtor:** The limit check is done during order entry for the appropriate customer (FinAc debtor).
- **MP project:** The limit check is done during order entry if this project is assigned to the order and the system is configured appropriately.
**Technical info:** <F9>, DB field: mp.objlimitpruef

#### Cred. limit
Amount in own currency up to which the company grants the customer credit. With appropriate configuration, the order value including the open items and the open orders is checked against the company limit stored here.
**Technical info:** numeric field, DB field: mp.firmlimit

#### Insured up to
The expiration date of the credit limit can be stored in this field.
**Technical info:** numeric field, DB field: mp.firmlimverfall

### Assu. lim.
Amount in own currency up to which the company grants the customer credit. With appropriate configuration, the order value including the open items and the open orders is checked against the assu company limit stored here.
**Technical info:** numeric field, DB field: mp.akvlimit

### Insured up to
The expiration date of the insurance can be stored in this field.
**Technical info:** numeric field, DB field: mp.limverfall

### Limit check order
With this field, you control what happens with orders whose order value including the open items and the open orders exceeds the limit stored in the fields Cred. Limit and Assu. Lim. If the employee has appropriate rights, the order can be entered and it will then land in a release pool (configurable). Orders that are in the release pool can only be released by authorized people. If the employee does not have these rights, he cannot enter the order:
- **Companies:** The value in the Cred. Limit field is used.
- **Assu. Lim.:** The value in the Assu. Lim. field is used.
- **Assu. + Cred. Limit:** The values in the Cred. Limit and Assu. Lim. fields are used.
- **None:** There is no limit check.
**Technical info:** <F9>, DB field: mp.limpruefkz

### Input stop
With this field, you control whether or not a document for this market partner may be entered when the limit is reached.
- **Only quotation:** When the limit is reached, no more quotations can be entered. Only orders can be entered for this market partner.
- **Only order:** When the limit is reached, no more orders can be entered. Quotations can still be entered for this market partner.
- **Order+Quotation:** When the limit is reached, neither quotations nor orders may be entered.
- **No:** No entry stop was entered for this market partner.
**Technical info:** toggle field, DB field: mp.erfasstop

### Delivery stop
With this field you control whether or not a delivery note for this market partner may be printed if the limit is reached.
- **Yes:** There is no more delivery when the limit has been reached.
- **No:** With the reaching of the limit, orders can still be entered.
**Technical info:** toggle field, DB field: mp.lieferstop

### Invoice stop
With this field you control whether or not an invoice for this market partner may be printed if the limit is reached.
- **Yes:** With the reaching of the limit, no more invoices can be issued.
- **No:** With the reaching of the limit, invoices can still be issued.
**Technical info:** toggle field, DB field: mp.fakturastop

### VAT
Selection of the VAT code. The tax codes are stored on the Tax Types menu (Master Data > Keys > System > Taxes).
**Technical info:** <F9>, DB field: mp.mwst

### Int. VAT
Internal VAT. The field is only active if the market partner is a supplier.
**Technical info:** <F9>, DB field: mp.mwstint

## Assessment tab
**Master Data > Market Partner > Assessment tab**

*Fig. B-20: Market Partner - Assessment tab*

On this tab, you can assess the reliability, delivery time, quality, etc. The right side displays the address information.

### Descriptions of fields

#### Cat.
Assessment of the class. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qklass

#### Reliability
Assessment of the reliability. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qzuverl

#### Delivery time
Assessment of the delivery time. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qzeit

#### Prices
Assessment of the prices. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qpreis

### Quality
Assessment of the quality. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qqual

### Service
Assessment of the service. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qservice

### Consultation
Assessment of the consultation. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qberat

### Courtesy
Assessment of the courtesty. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qkulanz

### Fin.standing
Assessment of the financial standing. The evaluation codes are stored on the General menu (Master Data > Keys > Market Partner > Quality Scale).
**Technical info:** <F9>, DB field: mp.qbonitaet

## Production tab
**Master Data > Market Partner > Production tab**

*Fig. B-21: Market Partner - Production tab*

The fields on this dialog served the transfer to PMS. With the introduction of A+W Production, the production transfer has changed. For additional information, please contact a service employee of A+W Software GmbH.

### Descriptions of fields

#### Determine prod. sequence
Selection of whether a production sequence should be specified.
- **Yes:** Production sequence should be specified
- **No:** No production sequence is specified.
**Technical info:** toggle field, DB field: mp.prodfolge

#### Rack Load
This criterion determines the sort sequence on a rack, depending, e.g. on item, AIR, HM (hard dimension), etc.
**Technical info:** toggle field, DB field: mp.gbelad

#### Rack weight (max)
The maximum rack weight can be entered.
**Technical info:** <F9>, DB field: mp.gmaxgew

## Modification tab
**Master Data > Market Partner > Modification tab**

*Fig. B-22: Market Partner - Modification tab*

This tab shows when and by whom the market partner was created, when and by whom changes were made, and when the market partner was replicated. The right side displays the address information.

In the replication area, you see at which sites the market partner was replicated.

### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Private tab
**Master Data > Market Partner > Private tab**

*Fig. B-23: Market partner - private tab*

For individual evaluations or additional customer information, there are two alphanumeric fields available. On request, these can be given individual labels and configured in the system. For customer-specific adjustments, contact your A+W Software GmbH contact person.

### Additional information
⇨ "Market partner - note texts" on page B-106
⇨ "Article - notes" on page B-385

## Contact person
**Master Data > Market Partner > <F4> Contact Data > Contact Person**

*Fig. B-24: Main contact*

On this dialog, you can store various contact people for a market partner. Here, you can add more data records with <F6>.
With several stored contact people, use <F5> to determine a main contact.

### Descriptions of fields

#### Name
Last name of the contact.
**Technical info:** alphanumeric field, DB field: anspr.apname

#### 1stName
First name of the contact.
**Technical info:** alphanumeric field, DB field: anspr.apvname

#### Title
Selection of the title for the contact. The appropriate keys can be assigned via the Titles (Master Data > Keys > Market Partner) menu.
**Technical info:** <F9>, DB field: anspr.anrede

#### Departm.
Contact's department.
**Technical info:** alphanumeric field, DB field: anspr.abteilung

#### Position
Contact's position.
**Technical info:** alphanumeric field, DB field: anspr.position

#### Birthday
Contact's birthday.
**Technical info:** numeric field, DB field: anspr.gebdat

### Phone
Contact's telephone number, e.g. +4964042051-0.
**Technical info:** numeric field, DB field: anspr.telefon

### Fax
Contact's fax number, e.g. +4964042051-877.
**Technical info:** numeric field, DB field: anspr.telefax

### Mobile
Contact's mobile phone number, e.g. +491777500000.
**Technical info:** numeric field, DB field: anspr.telex

### E-mail
Contact's e-mail address.
**Technical info:** numeric field, DB field: anspr.email

### Comment
Text comment fields.
**Technical info:** alphanumeric field, DB field: adr.text1-3

## Addresses
**Master Data > Market Partner > <F4> Contact Data > Addresses**

*Fig. B-25: Addresses*

You can assign the market partner additional addresses on this dialog. The invoice address is the main address and cannot be changed. You can add more data records with <F6>. If the delivery address is different from the main address, the corresponding address has to be determined as default address with <F5>.

> **Deleting and reactivating a market partner address**
> On this dialog, you can delete an address even if it is used in other modules. The first step is simply to close down the address. The second step is to delete or reactivate the address. The [Delete] button changes to [Reactivate]. In both cases, there is a security query, asking whether the action should actually be completed.

### Descriptions of fields

#### Name
Last name or company name.
**Technical info:** alphanumeric field, DB field: adr.adrname

#### 1stName
First name.
**Technical info:** alphanumeric field, DB field: adrvname

#### Title
Title, e.g. Mr., Mrs., company. The codes are stored in the Titles (Master Data > Keys > Market Partner) menu.
**Technical info:** <F9>, DB field: anspr.anrede

#### Attn.
For the attention of (last name, first name).
**Technical info:** alphanumeric field, DB field: adr.zhd

#### Addition
Enables entry of additional address information for output on customer papers.
**Technical info:** alphanumeric field, DB field: adr.branche

#### Street
Street name.
**Technical info:** alphanumeric field, DB field: adr.str

#### PCd, POB
Postal code and post box.
**Technical info:** numeric field/alphanumeric field, DB field: adr.pfplz/postfach

#### POB City
Postal box and city.
**Technical info:** numeric field/alphanumeric field, DB field: adr.pfort

#### PCd.City
Postal code and city.
**Technical info:** numeric field/alphanumeric field, DB field: adr.plz/ort

#### Dispatch region
Selection of the dispatch region. The appropriate codes can be assigned via the Dispatch Regions (Master Data > Keys > System > Dispatch) menu.
**Technical info:** <F9>, DB field: adr.vsregion

#### Country
Selection of the country code. The appropriate codes can be assigned via the Countries (Master Data > Keys > Market Partner) menu.
**Technical info:** <F9>, DB field: adr.kfzcode

#### Distance
Distance to the delivery address in km.
**Technical info:** numeric field, DB field: adr.kilometer

> **Site-specific details about distance and travel time**
> Details about Distance and Travel Time should be entered per site (client) when using internal client separation. The entry dialog starts automatically in such a configuration.
> ⇨ "Site-specific address details" on page B-143

### Travel time
Duration of the travel time to the delivery address in days.
**Technical info:** numeric field, DB field: adr.fahrtzeit

> **Handling time, arrival time and unloading point**
> The fields Handling Time, Arrival Time and Unloading Point are only released with appropriate configuration.

### Handling Time
Is the time between the completion of the product and the day of delivery. Such a time can be necessary if the customer makes particular specifications for the picking of its goods. It is entered as a deadline and thus considered by the date and capacity planning. The time can be entered in days or hours (configurable). The handling time can be stored per delivery address with appropriate configuration.
**Technical info:** numeric field, DB field: adr.handlingszeit

### Arrival time
Arrival time in HH:MM for delivery of the goods.
**Technical info:** numeric field, DB field: adr.ankunftszeit

### Unloading point
Place where the goods will be unloaded on delivery.
**Technical info:** numeric field, DB field: adr.anlieferstelle

### Fax pho.
Fax number and telephone number of the address.
**Technical info:** numeric field/alphanumeric field, DB field: adr.fax/telefon

### E-mail
E-mail address.
**Technical info:** alphanumeric field, DB field: adr.email

### Std. route
Selection field. If the delivery address cannot be reached via the standard route stored in the customer master data, it is possible to assign the address to a separate route.
**Technical info:** <F9>, DB field: adr.routenr

### Remark
Any information.
**Technical info:** alphanumeric field, DB field: adr.text1

> **Address logic**
> At the time of order entry, the stored default delivery address with the associated route number is taken over in the rules for the customer in question. If a default delivery address with separate route number has been stored for the customer, the route number entered in the customer master data is overridden. There are various deviations in this function; these are usually configuration-dependent. If you have questions or need additional information, contact the responsible A+W Software GmbH employee.

> **New addresses in the order and in the A+W iQuote document**
> New customer addresses can be taken over into the master data. In the order entry, use the <F3> key to do this:
> ⇨ Sales, "New delivery address" on page D-119
> In an A+W iQuote document, the new address is taken over into the customer master data by default. If this is not what you want, please contact an A+W employee to change the configuration.

## Site-specific address details

*Fig. B-26: Site-specific address details*

On this dialog, you can store site-specific address data per site. This dialog appears automatically if you are using the internal client separation and you enter the Distance field on the Addresses dialog.
⇨ "Addresses" on page B-139

### Descriptions of fields

#### Site
Selection of the site number.
**Technical info:** <F9>, DB field: mdzu.hnr

#### Name
The site name is displayed automatically in plain text when you leave the Site field.

#### Distance
Distance to the delivery address in km for the current site.
**Technical info:** numeric field, DB field: adr.kilometer

#### Travel time
Duration of the travel time to the delivery address in days or hours for the current site.
**Technical info:** numeric field, DB field: adr.fahrtzeit

## Bank accounts
**Master Data > Market Partner > <F4> Contact Data > Bank Accounts**

*Fig. B-27: Bank accounts*

The market partner-specific bank details are stored on this dialog. Here, you can add more data records with <F6>. If there are several bank accounts, the main bank account has to be determined with <F5>.

### Descriptions of fields

#### Bank name
Name of the bank.
**Technical info:** alphanumeric field, DB field: bankv.bname

#### Branch
Branch of the bank.
**Technical info:** alphanumeric field, DB field: bankv.sitz

#### Country
Selection field. The country code.
**Technical info:** <F9>, DB field: bankv.kfzcode

#### Bk.cd
Bank code of the bank.
**Technical info:** numeric field, DB field: bankv.blz

#### Acc. no.
Account number at the bank.
**Technical info:** numeric field, DB field: bankv.blz

#### BIC
Business Identifier Code.
**Technical info:** alphanumeric field, DB field: bankv.bic

#### IBAN
International bank account number.
**Technical info:** alphanumeric field, DB field: bankv.iban

## E-Mail addresses
**Master Data > Market Partner > <F4> Contact Data > E-mail Addresses**

*Fig. B-28: E-mail addresses*

On this dialog, you have the possibility to store various e-mail addresses. The data stored is maintained in the associated database table xemail. It contains the details for the e-mail dispatch of forms. The MP type, market partner, form type, employee, and the department and the e-mail addresses can be specified here. If an employee is entered, no department can be entered. If a department is entered, no employee can be entered. It is possible to create values for a market partner and an employee (or a department), for a market partern, a form type, and an employee (or department) or just for a market partner. The e-mail address to which the form associated with the document is sent is determined precisely in this sequence when dispatching the forms.

The data stored here always relates to the document for which a form should be dispatched; that is, the employee number stored here has to match the person entering the document so that the appropriate e-mail address can be determined.

### Descriptions of fields

#### Form
Select the desired form (quotation, invoice, etc.).
**Technical info:** <F9>, DB field: xemail.formart

#### Employ.
Select the desired employee number. If the e-mail should not go to an employee but rather to a department, then leave this field blank and select the appropriate department in the Department field.
**Technical info:** <F9>, DB field: xemail.manr

### Departm.
Select the department to which the e-mail should go. If you have entered an employee number in the Employ. field, you cannot make any entry in this field.
**Technical info:** <F9>, DB field: xemail.abtnr

### E-mail
Enter the appropriate e-mail address here.
**Technical info:** alphanumeric field, DB field: xemail.email

### C
If the e-mail address is one that has been closed for this form type:
- **Y:** The mail address is closed for this form type.
- **N:** The mail address is active for this form type.
**Technical info:** toggle field, DB field: xemail.still

### Additional information
⇨ "E-Mail addresses - detail" on page B-147

## E-Mail addresses - detail
**Master Data > Market Partner > <F4> Contact Data > E-mail Addresses > F2**

*Fig. B-29: E-mail addresses*

This dialog displays additional information about the selected e-mail addresses.

### Descriptions of fields

#### Partn. type
The field is pre-populated with the partner type from which you opened the context menu. You can change the type.
**Technical info:** toggle field

#### MktPt.
The field is pre-populated with the market partner from whom you opened the context menu. You can change the market partner.
**Technical info:** <F9>, DB field: xemail.mpnr

#### Form
The field is pre-populated with the form that you selected on the previous dialog. You can change the form.
**Technical info:** <F9>, DB field: xemail.formart

#### Employee
The field is pre-populated with the employee that you selected on the previous dialog. You can change the employee.
**Technical info:** <F9>, DB field: xemail.manr

#### Departm.
The field is pre-populated with the department that you selected on the previous dialog. You can change the department.
**Technical info:** <F9>, DB field: xemail.abtnr

#### E-mail
The field is pre-populated with the e-mail address that you selected on the previous dialog. You can change the address.
**Technical info:** alphanumeric field, DB field: xemail.email

#### E-mail from
Different sender address when using this e-mail address.
**Technical info:** alphanumeric field, DB field: xemail.emailabs

### CC
Additional CC address for use of this e-mail address.
**Technical info:** alphanumeric field, DB field: xemail.cc

### BCC
Additional BCC address for use of this e-mail address.
**Technical info:** alphanumeric field, DB field: xemail.bcc

### Disp.type
Dispatch type of the file attachment:
- **0 (default):** One PDF file per e-mail
- **1:** Use several file attachments per e-mail
- **2:** Combine all file attachments into one PDF.
**Technical info:** alphanumeric field, DB field: xemail.bcc

### Password
You can assign a password here.
**Technical info:** alphanumeric field, DB field: xemail.passwort

### Suspended
The field is pre-populated with the flag that you set on the previous dialog. You can change the flag.
**Technical info:** toggle field, DB field: xemail.still

## Discounts
**Master Data > Market Partner > <F4> Discounts**

*Fig. B-30: Discounts*

You assign the selected market partner discounts here. Key areas of the dialog are described in detail here:
⇨ "Discounts" on page B-227

The values for the respective discount method can be agreed upon individually per market partner and changed.

## Discount - details
**Master Data > Market Partner > <F4> Discounts > Details**

*Fig. B-31: Discounts, details*

This dialog presents a detailed view of the discounts. The dialog is described in detail here:
⇨ "Discounts - details" on page B-230

## Exchange/additional rules
**Master Data > Market Partner > <F4> Exchange/Additional Rules**

*Fig. B-32: Exchange/Additional Rules*

The Exchange/Additional Rules menu element allows the storage of customer-specific rules according to which the BOM can be added and parts exchanged for individual articles or article types.

The dialog is described in detail here:
⇨ "Exchange/additional rules" on page B-304
"Exchange/additional rules - details" on page B-308
⇨ "Exchange/additional rules - test mode" on page B-310

## Rack types
**Master Data > Market Partner > <F4> Rack Types**

*Fig. B-33: Rack types*

On this dialog, you specify on which racks the goods should preferably be delivered to a customer.
With hse of priority-controlled packing optimization, a priority can also be specified, for which rack type is the most desirable and which is the least favored. The priority number can be selected between 1 and 100 and then specifies the sequence of the racks. Larger values cause a preferring of this rack type before others with lower priority values.
The information stored here uses the automatic rack planning to load the order as well as possible onto the racks preferred by the customer, heeding lite sizes and limits of the rack types For automatic rack planning, either the rack type or the main group can be stored here.

Use <F2> to reach the rack details dialog.
⇨ "Rack types - details" on page B-153

### Descriptions of fields

#### Type
Selection of the rack type. The rack types are stored in the Rack Types menu element (Logistics > Rack Management > Rack Master Data). After selecting the rack type, the associated designation appears in the second field.
**Technical info:** <F9>, DB field: kugest.gtypnr

#### Main group
Selection of the main group. The main groups are stored in the Main Groups menu element (Logistics > Rack Management > Rack Master Data). After selecting the main group, the associated designation appears in the last field. With use of the priority-controlled configuration, entry of the main group is not possible.
**Technical info:** <F9>, DB field: kugest.gtypnr

#### Priority
Rack priority from the customer's perspective. The field is only visible for customer-specific configuration.
**Technical info:** numeric field, DB field: kugest.prioritat

## Rack types - details
**Master Data > Market Partner > <F4> Rack Types > F2**

*Fig. B-34: Rack types, F2*

On this dialog, you can store a customer-specific packing text and define whether it should be printed on the packing order.
Return to the main dialog with <F2>.
⇨ "Rack types" on page B-152

### Descriptions of fields

#### Text
Customer-specific packing text.
**Technical info:** alphanumeric field, DB field: kugest.kuspectxt/kuspectxt1

#### Purchase Flg
Should the text be printed on the PO:
- Yes
- No.
**Technical info:** toggle field, DB field: kugest.bestelldru/bestelldru1

## Configured market partner fields
**Master Data > Market Partner > <F4> Configured MP-fields**

*Fig. B-35: Configured market partner fields*

Each field on this dialog is configured and evaluated customer-specifically. The fields can be defined under the menu element MP-Field Configuration (Master Data > Field Configuration).
⇨ "MP field configuration" on page B-495

The evaluation of the fields can only be designed individually. For additional information, please contact a service employee of A+W Software GmbH.
The data in the screenshot above serves only as an example.

## Sales representative allocation
**Master Data > Market Partner > <F4> Employee Allocation > Representative Allocation**

*Fig. B-36: Employee allocation*

On this dialog it is possible to assign a customer several representatives (employees).
Selection is made with <F9>. Only those employees are available for selection to whom a representative function is assigned in the employee master data.
Use <F5> to specify a representative as main representative (= sales representative).

### Descriptions of fields

#### Empl.no.
Selection of the employee number. The name is displayed in the Sales Repr. field.
**Technical info:** <F9>, DB field: mitarbzu.manr

## User allocation
**Master Data > Market Partner > <F4> User Allocation**

*Fig. B-37: User allocation*

On this dialog it is possible to assign a customer several users (employees). Selection is made with <F9>.

### Descriptions of fields

#### Empl.no.
Selection of the employee number. The name is then displayed in the Operator field.
**Technical info:** <F9>, DB field: mperfasszu.manr

#### Ord. Confirm.
Use this field to control how the employee should receive copies of the OC to the customer. The following values are possible:
- **no:** The employee receives no copy of the OC.
- **via Email:** The employee receives the copy via e-mail.
- **via Fax:** The employee receives the copy via fax.
**Technical info:** toggle field, DB field: mperfasszu.abflag

## Group allocation
**Master Data > Market Partner > <F4> Group Allocation**

*Fig. B-38: Group allocation*

On this dialog, a customer can be allocated to various groups with <F9>. Maintenance of the group codes is done on the Groups menu (Master Data > Market Partner).

The various market partner groups can be assigned various texts in the course of text processing (Master Data > Text Management > Group Texts) that can be output on the market partner's papers. This way, the market partner group Window Manufacturers can be informed about the introduction of a new insulated glass product.

### Descriptions of fields

#### Group
Selection of the group code. The name is then displayed in the Description field.
**Technical info:** <F9>, DB field: grpzu.grpnr

#### Categ.
Group classification. Via the defined Class, you can make statistical evaluations.
**Technical info:** numeric field, DB field: grpzu.klasskz

## Project allocation
**Master Data > Market Partner > <F4> Project Allocation**

*Fig. B-39: Project allocation*

On this dialog, one or several projects (e.g. large construction sites) can be assigned to a customer. The projects are displayed with <F9> and entered with their project number.

Use <F3> to open the dialog for customer-specific Project Texts in which you assign the project texts and define on which papers the text is printed.
Use <F5> to define the default project.

### Descriptions of fields

#### Proj.
Selection of the project number. The name of the project is then displayed in the Project Name field.
**Technical info:** <F9>, DB field: okkond.objnr

### Additional information
⇨ "Project texts" on page B-159

## Project texts
**Master Data > Market Partner > <F4> Project Allocation <F3>**

*Fig. B-40: Project texts*

On this dialog, you assign a project text and determine on which papers the text will be printed.

### Descriptions of fields

#### File
Selection of the text file in which the texts are saved. If you enter a new file name, the Master Texts dialog opens, on which you can enter the new text.
**Technical info:** <F9>, DB field: objtxtzu.datei

#### No
Use this field to control the sequence in which the project texts are printed.
**Technical info:** <F5>, DB field: objtxtzu.lfdnr

#### Printing pos.
Selection of the printing position:
- Header text
- Footer text
**Technical info:** toggle field, DB field: objtxtzu.ludrupos

> **Forms**
> Use <F5> to specify on which form types (order confirmation, invoice, etc.) the files are printed in the sequence specified here.

### Additional information
⇨ "Master texts" on page B-165

## Color allocation
**Master Data > Market Partner > <F4> Color Allocation**

*Fig. B-41: Color allocation*

This dialog is only available for Market partner type=Supplier. The data stored here is relevant for the BMECat master data import. This is an application for importing suppliers' article master data. During the import of a new supplier master data file, it is checked using the corresponding table lieffarbzu whether or not the colors of an item to be imported are already created in AWE as AWE colors. If it is detected that a supplier color is not yet created as AWE color, it is created during the import.

The dialog then delivers the overview of all created supplier colors to the user.

It can also happen that a color is needed for an order for a supplier that is not yet created because after the last supplier master data import from the supplier, new colors were made available. In this case, the new supplier color can be created manually via the dialog in order to enter the PO.

### Descriptions of fields

#### No
The colors are stored on the Colors menu element (Master Data > Keys > Products > Variants > Colors).
**Technical info:** <F9>, DB field: lieffarbzu.farbnr

#### AWE color
AWE color designation. After the color number selection, the appropriate designation is displayed in this field.
**Technical info:** <F9>, DB field: lieffarbzu.farbnr

#### No
Supplier's color number.
**Technical info:** <F9>, DB field: lieffarbzu.lifarbnr

#### Supplier's color
Supplier's color designation
**Technical info:** <F9>, DB field: lieffarbzu.lifarbbez

## Bonus allocation
**Master Data > Market Partner > <F4> Bonus Allocation**

*Fig. B-42: Bonus allocation*

You can assign the market partner a bonus on this dialog.

### Descriptions of fields

#### Rank
Specification for the priority. Use this field to control the allocation in the order entry to the individual order items. The lowest rank number with the most matching points in the product group will be used here.
**Technical info:** numeric field, DB field: bonuszu.rang

#### PGRP Cd
Use this field to allocate the bonus to a particular product group or product group range.
**Technical info:** <F9>, DB field: bonuszu.wagrp

#### Remark
You can store a remark here, e.g. why a bonus was awarded.
**Technical info:** alphanumeric field, DB field: bonuszu.txt

#### Bonus
Selection of the desired bonus. The appropriate codes can be assigned via the Bonus (Codes > Market Partner > Bonus) menu.
**Technical info:** <F9>, DB field: bonuszu.bonusnr

## Product allocation
**Master Data > Market Partner > <F4> Product Allocation**

*Fig. B-43: Product allocation*

You can assign the market partner several articles with specific details on this dialog. Display the articles with <F9> and enter their article numbers.

### Description of the fields on the Overview tab

#### Article
Selection of the article number.
**Technical info:** <F9>, DB field: artkuzu.artnr

#### Description
Article description.

#### Art. type
Article type of the selected article.

#### Ext. article
Market partner's article number. With this number, the order item can be entered directly.
**Technical info:** alphanumeric field, DB field: artkuzu.kuartnr

#### External article name
Market partner's article name.
**Technical info:** alphanumeric field, DB field: artkuzu.kuartbez

#### Price
Customer article price. Depending on the price type, it is then calculated in the order.
**Technical info:** numeric field, DB field: artkuzu.preis

#### Type
Price type:
- **CU/piece:** currency unit per piece.
- **CU/QU:** currency unit per quantity unit.
**Technical info:** toggle field, DB field: artkuzu.ptyp

### Description of the fields on the Details tab

#### Preferred suppl
Enter the market partner's favorite supplier for this article in this field.
**Technical info:** <F9>, DB field: artkuzu.liwunsch

#### Additional name
Enter the additional name this partner uses for the article in these fields. There are three fields for this purpose. Enter the field with <Enter>.
This name will override the article name in document management (for this customer).
**Technical info:** alphanumeric field, DB field: artkuzu.zusatz1, artkuzu.zusatz2, artkuzu.zusatz3

#### EAN code
Enter the EAN code this market partner uses for the article in this field. This will be printed on all customer-bound documents. The EAN code can be used to convert external articles into A+W Enterprise articles at automatic order import.
**Technical info:** numeric field, DB field: artkuzu.eancode

#### Spacer text no.
Enter the spacer text number the partner uses for an IG article in this field. The text formula is entered on the Text management > Text creation > Text formula menu.
This formula is analyzed when text is created at order entry, and will be printed on the spacer.
**Technical info:** numeric field, DB field: artkuzu.rahmtxtnr

#### Size 1-20
You can enter article sizes used by the market partner in these fields. These will override the values from the parameters defined for this article during article dimensioning.

> **There will be no feasibility check!**
> Your entries here have to make sense.

**Technical info:** numeric fields, DB fields: artkuzu.gv1 – artkuzu.gv20

## Market partner texts
**Master Data > Market Partner > <F4> > Text/Print > MP Texts**

*Fig. B-44: Market partner texts*

On this dialog, you assign market partner texts for printing on the forms.
Use <F3> to open a dialog on which you can store the master texts.

> **Forms**
> Use <F5> to specify on which form types (order confirmation, invoice, etc.) this file is printed in the sequence specified here.

### Descriptions of fields

#### File
Selection or input of the text file in which the texts are saved.
**Technical info:** <F9>, DB field: kltxtzu.dateiname

#### No
Use this field to control the sequence in which the market partner texts are printed.
**Technical info:** <F5>, DB field: kltxtzu.Ifdnr

#### Printing pos.
Selection of the printing position:
- **Header:** The file is printed in the header.
- **Footer:** The file is printed in the footer.
**Technical info:** toggle field, DB field: kltxtzu.ludrupos

### Additional information
⇨ "Master texts" on page B-165

## Master texts
**Master Data > Market Partner > <F4> > Text/Print > MP Texts > <F3>**

*Fig. B-45: Master Texts*

On this dialog, new text blocks are entered and managed in several languages for printout of the forms. With this it is possible, for example, to store Christmas greetings, general customer notes or text for advertising campaigns in order to print them out on the customer-bound papers.

### Descriptions of fields

#### File
Name of the text file in which the texts are saved.
**Technical info:** alphanumeric field, DB field: xtxtnr.datei

#### Language
Selection of the language. Only the languages are available for selection that are stored in the system master data (Master Data > Keys > System > Languages)
**Technical info:** <F9>, DB field: xtxtnr.sprkz

#### Text
Entry of the appropriate text. Multi-line inputs are possible. A maximum of 160 characters on a line can be entered. The individual lines are distinguished with the sequence number.
**Technical info:** alphanumeric field, DB field: stammtxt.stammtxt, stammtxt.seqnr

### Additional information
⇨ "Market partner texts" on page B-164

## Market partner - article texts
**Master Data > Market Partner > <F4> > Text/Print > MP Article Text**

*Fig. B-46: Article texts*

This dialog is used to store market partner-specific article texts in different languages. Depending on the customer language code, these texts can be output on the forms.

### Descriptions of fields

#### Article
Selection of the appropriate article number. The article description appears in the field here.
**Technical info:** <F9>, DB field: artxtzu.artnr

#### File
Name of the text file in which the texts are saved. Use <F3> to switch to the Master Data dialog where you can store new texts.
**Technical info:** alphanumeric field, DB field: artxtzu.datei

## Forms
**Master Data > Market Partner > <F4> > Text/Print > Forms**

*Fig. B-47: Forms*

On this dialog, it is possible to store a customer-specific report for the existing form type.

### Descriptions of fields

#### Form
Select the desired form type (quotation, invoice, etc.). The description is then displayed in the Description field.
**Technical info:** <F9>, DB field: kundruckanz.formart

#### Copies
Determines the customer-specific default output quantity of the form.
**Technical info:** numeric field, DB field: kundruckanz.anzahl

#### Comm
With this field, you control whether commission texts should be output.
- [x] Commission texts are printed.
- [ ] Commission texts are not printed.
**Technical info:** toggle field, DB field: kundruckanz.kommdrkz

#### Report name (w.o. extension)
Different, customer-specific report name.
**Technical info:** alphanumeric field, DB field: kundruckanz.repname

## Document types
**Master Data > Market Partner > <F4> > Text/Print > Document Types**

*Fig. B-48: Document types*

On this dialog, you can store various document types and the type of output. The dialog is described in detail here:
⇨ "Document types" on page B-245

## Search document
**Master Data > Market Partner > <F4> > Search Document**

*Fig. B-49: Search document*

Use of the document search was already discussed in the chapters Sale and Purchasing; please consult those sections for details!

## Market partner - info
**Master Data > Market Partner > <F4> > MP Info**

*Fig. B-50: Market partner info*

Various statistical information about the market partner is kept under this element:
- Amounts of open items for a FinAc connection
- Amounts of unpaid invoices (open items)
- Amounts of orders in progress (not yet invoiced)
- Date, number, site, and amount for the last order, the last quotation, and the last invoice
- Total sales in the current year.

### Descriptions of fields

#### Cust.
Selection of the customer number. The customer name is displayed in plain text after the number is selected.
**Technical info:** <F9>, DB field: kuplus.kunr

> **Market partner info**
> The fields on this dialog are for information purposes only and cannot be changed. The amounts are taken from the database table kuplus. The remaining fields are determined from daily business and displayed.

## Replication data
**Master Data > Market Partner > <F4> > Replication Data**

*Fig. B-51: Replication data*

Depending on the configuration, on this dialog you can specify a limit distribution for the individual branch offices.

### Descriptions of fields

#### tot. limit
Display of the company limit. The value comes from the Company Limit field (Master Data > Market Partner > Limits tab).
**Technical info:** display field

#### tot. assu.lim.
Display of the assu. limit. The value comes from the AKV Limit field (Master Data > Market Partner > Limits tab).
**Technical info:** display field

#### Site
Selection of the site for which the limit data applies.
**Technical info:** <F9>, DB field: limits.hausnr

#### Limit
Company limit for the appropriate site. If you leave the field, in the next field you will see the percentage that this value represents in relation to the total limit.
**Technical info:** <F9>, DB field: limits.limit

#### Assu. lim.
Assu. company limit for the appropriate sites. If you leave the field, in the next field you will see the percentage that this value represents in relation to the total assu. limit.
**Technical info:** <F9>, DB field: limits.akvlimit

#### Route
Selection of the route. In the next field, you will see the route name. The Routes and their Names are stored under Master Data > Keys > System > Dispatch > Route > Routes.
**Technical info:** <F9>, DB field: limits.routenr

### Def.site
Default site for the clients. Use <F5> to select the current site as default site for all entries.
**Technical info:** <F9>, DB field: limits.defhausnr

> **Insured up to**
> Neither the total limit nor the total assu. limit can be exceeded. If they are exceeded, there will be a message to that effect.

> **Lower dialog area**
> In the lower dialog area, you will see the total values both for the amounts as well as for the percentages.

## Configuration
**Master Data > Market Partner > <F4> > EDI Configuration**

*Fig. B-52: EDI configuration*

On this dialog, you configure the control of the EDI.
For additional information, please contact a service employee of A+W Software GmbH.

### Descriptions of fields

#### Partn. type
Selection of the partner type.
**Technical info:** <F9>, DB field: mpdfuectrl.kuliflag

#### Partners
Selection of the market partner number. The customer name is displayed in plain text after the number is selected.
**Technical info:** <F9>, DB field: mpdfuectrl.mpnr

#### Type of EDI
Selection of the EDI type. In the next field, you will see the description. Type of EDI decides about the type and manner of data transmission and should be selected very carefully. You can make the selection in the dialog header. In this case, new configuration entries can also only be made for this Type of EDI.
**Technical info:** <F9>, DB field: mpdfuectrl.dfuetyp

#### Control mode
Control mode of the EDI. In the next field, you will see the description.
**Technical info:** <F9>, DB field: mpdfuectrl.id

#### Val.
Control value.
- [x] The EDI type is active.
- [ ] The EDI type is not active.
**Technical info:** <F9>, DB field: mpdfuectrl.value

## Site specific details
**Master Data > Market Partner > <F4> > Site Specific Details**

*Fig. B-53: Site specific details*

The site-specific details are used for the multi-site system. Here you can assign individual representatives and condition debtors to different sites.

### Description of the fields

#### Site
Selection of the site number.
**Technical info:** <F9>, DB field: mdzu.hnr

#### Name
The site name is displayed automatically in plain text when you leave the Site field.

#### Sales repres.
Selection of the relevant sales representative. The respective commission rates for the representative entered here can be booked and they are ready for invoicing.
**Technical info:** <F9>, DB field: mpmdzu.lager

#### Name
Name of the representative responsible for the sales is displayed automatically in plant text when you leave the Sales Repres. field.

#### Debtor conditions
Selection of the customer number whose conditions should apply for the documents entered.
**Technical info:** <F9>, DB field: mpmdzu.konddebnr

#### Name
The customer name is displayed automatically in plant text when you leave the Debtor conditions field.
**Technical info:** <F9>, DB field: mp.name

#### VAT
Selection of a VAT. If the sites are in different VAT areas, the differing VAT for a market partner can be specified here.
**Technical info:** <F9>, DB field: mpmdzu.mwst

#### VAT (%)
After selecting the VAT, the name is displayed here in plain text.
**Technical info:** <F9>, display field

# Employee
**Master Data > Employee**

All identifying details (such as employee number, name, code, etc.) for the employee, system services, and authorization groups are specified in the employee master data.

In addition, all EDI rights and restrictions that affect the employee or an authorization group are stored here. This makes sure that employees can access only certain areas, and are given the appropriate rights in A+W Enterprise.

This chapter provides information on the following subjects:
- "Employee/authorization groups" on page B-176
- "Employees - rights" on page B-181

## Employee/authorization groups
**Master Data > Employee**

*Fig. B-54: Employee*

All details about employees, employee groups, and system services are stored on this dialog.

### Description of the fields in the Employee Data section

#### Empl. no.
Selection of the employee number. If this is a new employee, enter the desired number.
**Technical info:** <F9>, DB field: mitarb.manr

#### Type
This field specifies the type of master data record. The following values are possible:
- **Employee:** Each employee number can only be assigned once. With <F6> you have the opportunity to let the system assign the next free number.
- **System service:** An employee record with employee number -1 should be created as system service. The existence of this record is necessary since all A+W Enterprise background processes (e.g. background order processing, etc.) report with employee number -1.
- **Authorization group:** An authorization group is created with program access rights for a particular personnel area. Employees in this task area are then assigned the group number in the Authorization Group field. This eliminates the assignment of the individual group-specific module access authorizations for each individual employee.
**Technical info:** toggle field, DB field: mitarb.matyp

#### Name
Employee's last name. Use <F5> to open the Remark Texts dialog on which you can store the information about the employee. Use <F3> to open the dialog for the overview of the employee rights.
**Technical info:** alphabetic field, DB field: mitarb.maname

> **Employee and department notes**
> Employee and department notes with priority high and location everywhere can be displayed directly when starting the A+W Enterprise main menu or when starting the Dispatch module. This way, important employee-related information can be presented at the start. Your system must be configured appropriately.

#### 1stName
Employee's first name.
**Technical info:** alphabetic field, DB field: mitarb.mavname

#### Sex
Toggle field. Employee's sex.
- female
- male
**Technical info:** toggle field, DB field: mitarb.sex

#### Title
Selection of the title. The appropriate codes can be assigned via the Titles (Master Data > Keys > Market Partner) menu.
**Technical info:** <F9>, DB field: mitarb.anrede

#### Birth dt.
Employee's date of birth
**Technical info:** numeric field, DB field: mitarb.gebdat

#### Initials
Employee's initials.
**Technical info:** alphanumeric field, DB field: mitarb.zeichen

### Description of the fields in the Last Modification section

#### Name
This field displays the employee who made the last modification to the master data record.

#### Date
This field displays the date on which the master data record was last modified.

### Description of the fields in the Login Information section

#### Login
A+W Enterprise Login name, which together with the password permits the user to start the program. When using the A+W Enterprise Web application and A+W iQuote, the name entered here is also used for login.
**Technical info:** alphanumeric field, DB field: mitarb.loginname

### Password
Password, which together with the A+W Enterprise login name entitles the employee to start the program. The password can only be entered or changed by the administrator. For the use of the A+W Enterprise standard application, the password is assigned via the Unix or Linux administrator. The password from this field entitles the employee to log into the A+W Enterprise Web application or A+W iQuote.

### Description of the fields in the Restrictions section

#### Shell
Shell authorization. If the operating system level should also be accessible, please check this box.
**Technical info:** toggle field, DB field: mitarb.shjn

#### Department restriction
If this checkbox is active, various evaluations (e.g. list of uninvoiced orders, production release, etc.) are restricted to the documents of the department to which the employee is assigned.
**Technical info:** toggle field, DB field: mitarb.abtview

#### Client limitation
If this checkbox is active, various evaluations (e.g. list of uninvoiced orders, production release, etc.) are restricted to the documents of the client.
**Technical info:** toggle field, DB field: mitarb.hausview

### Description of the fields in the Employee/Contact Data section

#### DirectNo.
Internal telephone extension.
**Technical info:** numeric field, DB field: mitarb.durchw

#### Fax
Fax number.
**Technical info:** numeric field, DB field: mitarb.faxnr

#### E-mail
Employee's e-mail address.
**Technical info:** alphanumeric field, DB field: mitarb.email

#### Client
Plant or branch office number (main client). Use <Shift> + <F5> to open the dialog for the site assignment. There, you can assign the employee to additional sites.
**Technical info:** alphanumeric field, DB field: mitarb.hnr

#### Job title
Selection of the employee's job title.
**Technical info:** <F9>, DB field: mitarb.pos

#### Function
Selection whether the employee is active as managing director or sales representative. This way, e.g. only people who are identified as sales representatives can be assigned as such to a customer in the customer master data.
**Technical info:** <F9>, DB field: mitarb.funktion

#### Mail subs.
Selection of the employee number for the forwarding of an e-mail.
**Technical info:** <F9>, DB field: mitarb.vertretung

### Activate
With this checkbox, you activate the e-mail forwarding.
**Technical info:** toggle field, DB field: mitarb.vertr_aktiv

### Departm.
Number of the department. For statistical program access reasons, each employee should be assigned to a department. The department is then displayed in the next field. The appropriate departments are assigned via the menu by the same name.
**Technical info:** <F9>, DB field: mitarb.abtnr

### Customer
Here you can assign a customer to the employee.
**Technical info:** <F9>, DB field: mitarb.manrkunr

### External employee
Activate the checkbox if this is an external employee (with restricted rights).
**Technical info:** toggle field, DB field: mitarb.externflag

### SQL authorization group
Selection of the authorization group.
**Technical info:** <F9>, DB field: mitarb.logingrp

### Description of the fields in the RightGroups section

#### Group
Selection of the group number. The description is displayed in the next field. This eliminates the assignment of the individual group-specific module access authorizations for each individual employee.
**Technical info:** <F9>, DB field: bengrpzu.grp

#### Site
Selection of the assigned site number.
**Technical info:** <F9>, DB field: bengrpzu.hausnr

### Description of the fields in the Rights section

#### EDP Mod.
Selection of the EDP module in which the employee can exercise his or her EDP rights. * stands for all program modules. The module description is displayed in plain text in the next field. Use <F9> to search for a particular module. For the overview of all modules and their significance, please contact a A+W Software GmbH employee.
**Technical info:** <F9>, DB field: login.modul

#### Terminal
Selection of the terminal or terminal group for which the employee has rights for the module in question. * stands for all terminals.
**Technical info:** <F9>, DB field: login.ort

#### Rights
Selection of the employee rights:
- **-**: No rights.
- **r**: Read right
- **w**: Write right
**Technical info:** toggle field, DB field: login.rwx

### Site
Selection of the assigned site number in which this restriction applies (for multi-site systems). The site-specific restrictions can only be made for local rights. For additional information, consult the responsible A+W Software GmbH employee.
**Technical info:** <F9>, DB field: login.hausnr

## Employees - rights
**Master Data > Employee > Rights (Overview) <F3>**

*Fig. B-55: Employee, rights*

On this dialog, you specify the employee number and site number for which you would like to see the rights.

### Descriptions of fields

#### Employee
Entry of the employee number.
**Technical info:** numeric field

#### Site
Entry of the site number.
**Technical info:** numeric field

If you leave the dialog with [OK], the desired information is displayed on the next dialog:

*Fig. B-56: Employee, rights*

### Descriptions of fields

#### Module
Display of the module number. A * stands for all modules.
**Technical info:** display field

### Right
Display of the right:
- **-**: No rights.
- **r**: Read right
- **w**: Write right
**Technical info:** display field

### User/Group
Here you can see whether this is a user right or a group right:
- **U:** User right
- **G:** Group right
**Technical info:** display field

### Print
With this button, you can print out the overview of employee rights.

## Departments
**Master Data > Departments > Descriptions**
**Master Data > Departments > Individual Descriptions**
**Master Data > Departments > All Descriptions**

*Fig. B-57: Departments*

All of the identifying details (such as name, abbreviation, etc.) for the departments at the company are specified on this dialog.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Departments.

Use <F5> to open the Remark Texts dialog on which you can store the information about the department.

> **Employee and department notes**
> Employee and department notes with priority high and location everywhere can be displayed directly when starting the A+W Enterprise main menu or when starting the Dispatch module. This way, important employee-related information can be presented at the start. Your system must be configured appropriately.

### Descriptions of fields

#### Departm.
Selection of the department.
**Technical info:** <F9>, DB field: abteilung.abtnr

#### Abbreviation
Displays the abbreviation for the name.
**Technical info:** alphanumeric field, DB field: abteilung.abtid

#### Description
Department description. The description can be overwritten.
**Technical info:** alphanumeric field, DB field: abteilung.bez

#### Cost center
Selection of the cost center. The entry can be used for statistical purposes. The appropriate codes can be assigned via the Cost Center (Master Data > Cost Center) menu.
**Technical info:** <F9>, DB field: abteilung.kostenst

#### Message for
Selection of the message recipient. The system message recipient of the department is the person or group of people who receive messages from other employees of this department.
**Technical info:** <F9>, DB field: abteilung.manr

#### Form group
An entry in the form group that uses this department is taken into consideration when printing forms. Generally one form group per department is stored.
**Technical info:** numeric field, DB field: abteilung.formgrp

#### Fax
If there is an individual fax connection, this number can be stored here.
**Technical info:** numeric field, DB field: abteilung.faxnr

#### Last change
This field displays the employee who made the last change to the data and the corresponding date.

#### Langu.
Language ID.
**Technical info:** <F9>, DB field: xsprbez.sprkz

## Market Partner Keys
**Master Data > Keys > Market Partner**

In this area, characteristics for describing the market partner (customer, supplier, etc.) are created. They are then available for the entry of the market partner. The individual characteristics are explained below.

You have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a a/b | Titles | ⇨ "Titles-descriptions" on page B-187 |
| b | Bonus | ⇨ "Bonus" on page B-188 |
| c a | Groups | ⇨ "Groups" on page B-190 |
| c b/c | Group designations | ⇨ "Group descriptions" on page B-191 |
| d a/b | Industries | ⇨ "Industry descriptions" on page B-192 |
| e | Label Texts | ⇨ "Label texts" on page B-193 |
| f a | Calendars | ⇨ "Calendar" on page B-194 |
| f b | Special Calendar | ⇨ "Special calendar" on page B-196 |
| f c | Customer Calendar | ⇨ "Customer calendar" on page B-198 |
| f d | Client Calendar | ⇨ "Client calendar" on page B-200 |
| g | FinAc Clients | ⇨ "FinAc clients" on page B-202 |
| h a | Countries | ⇨ "Countries" on page B-203 |
| h b/c | Country names | ⇨ "Countries" on page B-203 |
| i a/b | Economic Areas | ⇨ "Economic area descriptions" on page B-205 |
| j a/b | Region/Federal states | ⇨ "Areas/Counties" on page B-206 |
| k a | Quality Scale | ⇨ "General quality scale" on page B-207 |
| k b | Qual. scale dates | ⇨ "Quality scale dates" on page B-209 |
| k c | Qual. scale prices | ⇨ "Quality scale prices" on page B-211 |
| k d | Qual. scale quantities | ⇨ "Quality scale quantities" on page B-213 |
| k a | Qual. scale special | ⇨ "Quality scale special" on page B-215 |
| i a | Reason for Complaint | ⇨ "Reasons for complaint" on page B-217 |
| i b | Places for Complaint | ⇨ "Places of complaint" on page B-219 |
| I c | Types of Complaint | ⇨ "Types of complaint" on page B-221 |
| m a | Discount Methods | ⇨ "Discount methods" on page B-223 |
| m a | Discounts | ⇨ "Discounts" on page B-227, "Discounts - details" on page B-230 |
| n | Site Specific Details | ⇨ "Site specific master data" on page B-235 |

> **Multi-language support**
> All language-dependent key data is saved in the table `xsprbez`. For the dialog in question, e.g. Market Partner > Titles, a view is built at runtime that contains the data for the titles. This view can also be accessed from the database level. That's why we have provided the information about the view on the dialogs that are affected by this. In some cases, there is also language-independent data. It is kept via xx*-View.

### Titles-descriptions
**Master Data > Keys > Market Partner > Titles > Individual Descriptions**
**Master Data > Keys > Market Partner > Titles > All Descriptions**

*Fig. B-58: Titles*

Both of these dialogs include the title forms that can occur when entering market partners, in the relevant languages.

#### Descriptions of fields

**Number/No**
Key number. To create a new title, enter the next free number.
**Technical info:** <F9>, DB field: xsprbez.id
**View:** xanrede.anrkz

**Lng**
Language ID.
**Technical info:** <F9>, DB field: xsprbez.sprkz

**Description**
Description of the title, e.g. Company.
**Technical info:** alphanumeric field, DB field: xsprbez.bez1
**View:** xanrede.anrkz

### Bonus
**Master Data > Keys > Market Partner > Bonus > Bonus**
**Master Data > Keys > Market Partner > Bonus > Individual Descriptions**
**Master Data > Keys > Market Partner > Bonus > All Descriptions**

*Fig. B-59: Bonus*

On this dialog, you enter the rules for the bonus. The assignment of a bonus can be done in the market partner master data or during order entry.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Bonus.

#### Descriptions of fields

**Bonus/No**
Selection of a process. By entering a new number, a new process is created.
**Technical info:** <F9>, DB field: xbonus.bonusnr

**Description**
Textual explanation of the process.
**Technical info:** alphanumeric field, DB field: xbonus.bonbez

**Tpe**
Selection of the criteria according to which the bonus should be granted.
First field:
- **CU:** The bonus is granted according to the order volume in the currency unit.
- **QU:** The bonus is granted according to the quantity purchased in square meters.
**Technical info:** <F9>, DB field: xbonus.bonart

Second field:
- **QU/sqm:** Here you control whetehr the bonus is calculated using the currency unit per square meter.
- **Max %:** Here you control whether the bonus is a maximum percentage value.
**Technical info:** <F9>, DB field: xbonus.bontyp
In the next field, you enter the corresponding calculation value.
**Technical info:** numeric field, DB field: xbonus.satz

**Accounting period**
Here, the maximum amount of the granted bonus is kept as information, e.g. 3 means every 3 months.
**Technical info:** numeric field, DB field: xbonus.zeitraum

**in Month**
Here you specify when exactly the check should be done. Enter a y in the desired month. In the fields that are marked with an n, there is no calculation.
**Technical info:** toggle field, DB field: xbonus.zp1-12

**Bonus**
After the general area comes the bonus scale. The Bonus column indicates the assignment to the bonus key. There are several lines available for the scaling, in which it is described starting with which sales or which purchase quantity % rate is granted.

**Lng**
Language ID.
**Technical info:** <F9>, DB field: xsprbez.sprkz

### Groups
**Master Data > Keys > Market Partner > Groups > Groups**

*Fig. B-60: Groups*

This dialog displays the market partner group in the client language. The groups can be divided into classes for informational purposes. However, the class has no effect.
Deleting individual groups is only possible on this dialog.
**Technical info:** table xxgrp

#### Additional information
⇨ "Group descriptions" on page B-191

### Group descriptions
**Master Data > Keys > Market Partner > Groups > Individual Descriptions**
**Master Data > Keys > Market Partner > Groups > All Descriptions**

*Fig. B-61: Groups*

Both of these dialogs include the market partner groups that can occur when entering market partners, in the relevant languages.

#### Descriptions of fields

**Group**
Key number. To create a new group, enter the next free number.
**Technical info:** <F9>, DB field: xsprbez.id
**View:** xgrp.grpnr

**Lng**
Language ID.
**Technical info:** <F9>, DB field: xsprbez.sprkz

**Description**
Description of the group, e.g. IG production.
**Technical info:** alphanumeric field, DB field: xsprbez.bez1
**View:** xgrp.atxt

### Industry descriptions
**Master Data > Keys > Market Partner > Industries > Individual Descriptions**
**Master Data > Keys > Market Partner > Industries > All Descriptions**

*Fig. B-62: Industries*

This dialog contains the industries that can occur when entering market partners, in the relevant languages. All special conditions can be maintained using these industries.

#### Descriptions of fields

**Number/No**
Key number. To create a new industry, enter the next free number.
**Technical info:** <F9>, DB field: xsprbez.id
**View:** xbranche.branchenr

**Lng**
Language ID.
**Technical info:** <F9>, DB field: xsprbez.sprkz

**Description**
Description of the industry, e.g. IG manufacturer.
**Technical info:** alphanumeric field, DB field: xsprbez.bez1
**View:** xbranche.branche

### Label texts
**Master Data > Keys > Market Partner > Label Texts**

*Fig. B-63: Label texts*

On this dialog, you store customer-specific label texts.
The entry in the Product Name field appears as customer-specific additional information on the sheet labels. The long text is referenced with the freely-selectable abbreviation.

#### Descriptions of fields

**Number**
To create a new label text number, select the next free number.
**Technical info:** numeric field, DB field: xetikett.txtnr

**Product name**
In this field, you assign the customer or project.
**Technical info:** alphanumeric field, DB field: xetikett.etitxt1

**Abbrev.**
The long text is referenced with the freely-selectable abbreviation.
**Technical info:** numeric field, DB field: xetikett.etitxt2

**Text**
This text appears as customer-specific additional information on the sheet labels.
**Technical info:** alphanumeric field, DB field: xetikett.etitxt3

### Calendar
**Master Data > Keys > Market Partner > Calendar**
**System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Calendar**

*Fig. B-64: Calendar (Daily view)*

You maintain your operating calendar on this dialog.
If you are working with a multi-site system, this is the main client's calendar. You can maintain different site calendars under
⇨ "Client calendar" on page B-200.

There are two different views available (<F2>):
- Daily view
- Monthly view

#### Descriptions of fields

**Date**
Each individual date is displayed here.

**Day**
Each individual day is displayed here.

**CW**
The calendar week is displayed here.

**H**
Selection of whether this is a business day.
**Technical info:** toggle field, DB field: alkal.htag

**PD**
Selection of whether this is a production day.
**Technical info:** toggle field, DB field: alkal.ptag

**T-CL**
Here you can see whether this day is a site-specific business day. The entry here overrides the entry in the Dt field. The site-specific business days are maintained in System > Keys > Market partner > Calendar > Site Calendar and cannot be changed here.

**P CL**
Here you can see whether this day is a site-specific production day. The entry here overrides the entry in the P field. The site-specific business days are maintained in System > Keys > Market partner > Calendar > Site Calendar and cannot be changed here.

**Remark**
You can store an appropriate remark in this field.
**Technical info:** alphanumeric field, DB field: alkal.bem

> **Working with A+W Production**
> If you are working with A+W Production, the system can be configured so that this calendar is also evaluated in production. This configuration is done in A+W Production.

### Special calendar
**Master Data > Keys > Market Partner > Calendar > Special Calendar > Special Calendar**
**Master Data > Keys > Market Partner > Calendar > Special Calendar > Individual Descriptions**
**Master Data > Keys > Market Partner > Calendar > Special Calendar > All Descriptions**
**System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Special Calendar**
**System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Special Calendar > Individual Descriptions**
**System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Special Calendar > All Descriptions**

*Fig. B-65: Special calendar*

On this calendar, you can store dates for events, for example.

#### Descriptions of fields

**Calendar**
Selection of the calendar number.
**Technical info:** <F9>, DB field: almpkal.kalnr

**Date**
You specify the date here.
**Technical info:** numeric field, DB field: almpkal.datum

**Day**
If you leave the Date field, the day is displayed automatically.

**CW**
If you leave the Date field, the calendar week is displayed automatically.

**CTD**
Here you can see whether or not this is a business day.

**H**
In this field, you can define days that are normally not workdays (e.g. Sundays) as business days.
**Technical info:** toggle field, DB field: almpkal.htag

**Remark**
You can store an appropriate remark in this field.
**Technical info:** alphanumeric field, DB field: almpkal.bem

**Calendar**
Key number. To create a new calendar, enter the next free number.
**Technical info:** numeric field, DB field: xsprbez.id
**View:** xkalender.kalnr

**Lng**
Language ID.
**Technical info:** <F9>, DB field: xsprbez.sprkz

**Description**
Description of the calendar, e.g. supplier.
**Technical info:** alphanumeric field, DB field: xsprbez.bez1
**View:** xkalender.atxt

### Customer calendar
**Master Data > Keys > Market Partner > Calendar > Customer Calendar**
**System Menu (<Ctrl> + <F4>) > Information Services > Calendar > Customer Calendar**

*Fig. B-66: Customer calendar*

For market partners of the type Customer and Other, you can store your own data in the customer calendar. That is, market partner-specific business and production days and holidays can be stored.

#### Descriptions of fields

**Partn. type**
Selection of the partner type.
**Technical info:** <F9>, DB field: almpkal.kuliflag

**Partners**
Selection of the market partner number.
**Technical info:** <F9>, DB field: almpkal.mpnr

**Date**
You specify the date here.
**Technical info:** numeric field, DB field: almpkal.datum

**Day**
If you leave the Date field, the day is displayed automatically.

**CW**
If you leave the Date field, the calendar week is displayed automatically.

**CTD**
Here you can see whether or not this is a business day.

**H**
In this field, you can define days that are normally not workdays (e.g. Sundays) as business days.
**Technical info:** toggle field, DB field: almpkal.htag

**Remark**
You can store an appropriate remark in this field.
**Technical info:** alphanumeric field, DB field: almpkal.bem

### Client calendar
**Master Data > Keys > Market Partner > Calendar > Client Calendar**
**System Menu (<Ctrl> + <F4>) > Information Services >Calendar > Client Calendar**

*Fig. B-67: Client Calendar*

After you have selected the client number, the calendar opens.
This calendar function is used for the multi-site system. Here you can store your own data for each internal site in the operating calendar. This way, you can store client-specific business and production day and holiday data.

There are two different views available:
- Daily view
