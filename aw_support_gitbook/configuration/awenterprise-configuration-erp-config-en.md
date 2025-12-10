---
description: "EN-CONFIG-AW_Enterprise_2"
---


---
## 3.1.13. Additional element for the item article/product type

You can also insert a simple additional element on the 1st level of the BOM. This rule is called only once for the item article if it has not been replaced by an exchange rule (see 1.).

## 3.1.14. Supply type alcib - 13.04.10373

*(Juni 2021)*

For product exchange via exchange/addition rules, with manual entry of the customer's desired supplier it is always taken over if for the product the supply type = "PO" is permitted (one of the possible supply types). For EDI orders, by contrast, the desired supplier is taken over if PO is created as the preferred supply type. With a setting, you can adjust the logic for EDI orders to the manual entry and here too have the desired supplier taken over if one of the supply types for the product is "PO."

Environment variable `INTAUF_DFUE_WUNSCHLIEFERANT`

## 3.1.15. Transfer article description

*June 2025 - alcib 13.04.20475*

You can enter an article description when defining a exchange/addition rule. The article description can be entered in the MODE menu (right side of menu). It will be included in the BOM when the E/A rules are analyzed.

**Please note:** If the internal transfer between clients with different article names takes place (e.g. other language) and the obtaining of the local article names for the client is active (NEUKAUF_NEUE_TEXTE), then the local names are obtained from the master data for all BOM elements. Thus, the name is not taken over from the E/A rule.

## 3.1.16. External EDI

see also "EN-CONFIG-A+W Enterprise EDI"

# 4. Article search

Within A+W Enterprise, you can search on various dialogs for article numbers (article selo). How the dialog for article search looks and how it behaves can be configured.

**ARSELO_SEARCH_UPPER (client reference: no)**
The environment variable activates the search within the article search regardless of the capitalization. So that the non-case-sensitive search can be activated, the current environment (LIBS/mfo/arseloneu*, mfo) must be installed (#405083)

**ARTSEARCH_WITH_LONGNAME (client reference: no)**
The variables switch on the possibility within the article search of searching for the long article name (artbezfremd.langbez).
PF [AW-117222] / QR 22/11

**ARSELO_ALT (client reference: no)**
This environment variable deactivates the sensitive article search.

**TYPAUSTAUSCH_OHNE_TEST (client reference: no)**
If in the BOM, you search for an exchange article via selo, then the selection is restricted immediately to the appropriate article types by pre-populating the start value for article type. By default, there is also a check whether the exchange article is replaced with an article of the same type, which can cause serious consequences in production. However, you can also switch this check off. If the check is switched off, then the pre-population of the article type on the search dialog is removed for all BOM elements (except glass), so that all articles are immediately available for selection.
[AW-139425]/ QR 2304

# 5. Shipping area / routes

**#196831 - MODUL_REGIONALROUTEN**

Dialog Post codes in Master data > Keys > System > Post codes now offers another column, Shipping area. For every post code, you can enter a shipping area as defined in Master data > Keys > System > Dispatch > Shipping areas. The post code header dialog has been completed by another selection criterion in order to search for the shipping areas.

The shipping area can be used to link a post code and a route.

In the addresses in partner data, in Master data > Partners > <F4> > Contact data > Addresses, this link between post code, shipping area and route is analyzed; the site number will be analyzed as well. The following details also refer to the entry of new shipping addresses in the following dialogs:
- Document entry (Sales/purchasing) > <F4> > Addresses > Select shipping address > <F6>
- Shipping control > Order level > <F4> > Shipping address > Select shipping address > <F6>

A new function will suggest a suitable route for the defined post code. This function can be enabled by means of the button [Search route] or shortcut <Ctrl> + <E>. A route will be suggested automatically after the post code is changed if the switch `ADR_AUTO_ROUTE_SUGGESTION` is active but only if there is no route number for this address yet.

The post code is used in table `XPLZORT` to determine the defined shipping area. If several places are found for a post code, the selected place will be taken into account when determining the shipping area. Based on this and a site number (see below), table `ROUTE` will select the route number with the lowest entry (= highest priority) in field Priority. When a route has been found, the program will ask whether this route shall be adopted for the address.

If the Priority field shows no clear entry for a shipping area, the program will be unable to find a matching route. If no route number can be found, the program will issue a message to this effect. This can be due to several reasons, e.g. if no shipping area has been defined for the post code, etc.

If internal client separation is active in partner data, the site number will be loaded from the switch `CALLCENTER`.

If internal client separation is inactive, the site number for the search in route data is loaded from the ENV variable `$HAUS`. If no route can be found, another search is made, using site number 0.

Document entry and shipping control will use the site number of the corresponding order for the search. If internal client separation is inactive, another search is made based on site number 0 if no route could be found based on the order's site number.

If the switch `MODUL_REGIONALROUTEN` is set to ON, the fields for alternative routes, routes 2-4, cannot be accessed. If before an activation of the environment variable there are already alternative routes in the market partner master data, it absolutely has to be deleted manually with activation. Thanks to the activation of the environment variable, the alternative routes for the market partner are not removed automatically from the system.

When an order is entered in the call centre, the route will not be optimized based on the date requested by the customer because the route can be allocated only after the site has been assigned. The date requested by the customer will be taken into account unless the calculated delivery date lies in the past. If this is the case, the delivery date will be moved to the next possible route day because the calculated delivery date must not lie in the past. This applies also to the correction of orders in which data are changed later on, which can lead to a new date. Even then, delivery dates must not lie in the past, the delivery date will be moved to the next possible route day. To calculate the date, the program first uses the route defined for the customer's standard address. If this route does not match the current site, it will be moved to the current site (call centre) by means of the area and priority. If there is no individual route for this address (standard address or manually selected address), the post code, area, and priority will be used in the described way, to find a route. By allocating the area to the post code, the shipping address is determined; the route for the region with the highest priority will be chosen. If this search is unsuccessful, the route will be adopted from partner data. The program checks whether the route is allocated to the call center and if it has to be changed acc. to the "Area+route" principle.

### Area-route optimization

When the producing site has been determined or entered, the search for the route can be optimized further. Once the shipping area is known (based on the route assigned to the address or the post code) and the customer's favorite date is clear, the program checks whether the arrival date at the customer's matches the requested date. If not, all other routes defined for this area in master data, will be checked acc. to their priority until a route is found which offers better results and an optimal arrival date. When this route is found, the user will be asked whether it shall be adopted. The new route will be adopted only if the user answers Yes.

### Calculation and optimization in the background

If no site is assigned right at order entry, the route will be allocated together with the site in the background. The system can be customized in this case so that the route with the highest priority will be used always. In this case, it has to be accepted that the delivery date may be later than the requested date, or the system can be configured so that the date requested by the customer always has top priority, and the system will try to find the optimum route in the background.

### Order link/PO transfer

When orders are created after an internal transfer, the route defined by the sending site can be adopted. This is done by setting the switch `INTAUF_ROUTEALT` or `INTAUF_ROUTEALT_DIREKTAUSLIEFERUNG` and `INTAUF_ROUTEALT_HAUSART`. The direct or collection route can also be defined for the receiving site in general (switch `INTAUF_DIREKTROUTE` and `INTAUF_ABHOLROUTE` or by defining the corresponding routes at the receiving site) to automate the setting of the new route at the receiving site.

If the route shall not be adopted from the sending site, it will be determined at the receiving site as described in item "Calculation and optimization in background". You can define per site (irrespective of the setting described in "Calculation and optimization in background") whether the date requested by the customer or the route priority shall be the decisive factor for route selection.

Transferred orders that shall be shipped directly from production site to customer (the order has been defined as a drop shipment by the sending site, or a direct shipping route has been entered) will be defined as direct shipments; the program first loads the internal route from the receiving site's master data (or it is determined by the switch `INTAUF_DIREKTROUTE`). If the post code of the shipping address is known however, the area is determined by means of the new allocation, and the route for this area is added. For calculating the date, the above-described optimization will be started.

### Recording of the search process

By enabling the switch `ROUTEN_PROTOKOLL`, the route search as well as the optimization will be recorded in the site's log directory in `route<XXXX>`.

# 6. Market partner master data

## 6.1. Canceled market partners

*[AW-163884] Nov 10, 2023 alcib - 13.04.16512*

By default, market partners are canceled in the end if nothing new should be entered. However, for a canceled market partner, existing documents can be processed until finished. Therefore, no change of the master data is required.

If, however, you are working with the external market partner interface, new market partners are only canceled because not all data is complete. In order to be able to correct all data for such market partners, the system can be configured so that even for canceled market partners, whose data can be accessed via the menu, it can be changed. This configuration can be done employee-specifically.

If you want to change the data for a discontinued market partner, the configurable notice "Discontinued market partner" appears. This notice can be switched off.

The number of the notice is 19563.

**MP_STORNO_CHANGE (client reference: no)**
For discontinued market partners, the data on the subdialogs cannot be changed. If this variable is active, this is possible. The variable can be activated employee-specifically.

## 6.2. Addresses

**Removal:** The removal can be used for the calculation/determination of Discounts/surcharges. They can be entered directly for the market partner or in the addresses. Removal entered directly for the market partner applies for the invoice address and is also saved in the invoice address record.
See also "EN-CONFIG-A+W Enterprise Interne Mandantentrennung"

**Route:** If you are working with „Via Plant", a route must be entered in each address
See also "EN-CONFIG-A+W Enterprise Interne Mandantentrennung"

### 6.2.1. Dutch address logic

With the new Dutch address logic in A+W Enterprise, the address maintenance is made easier for the person entering the information and it should help stop additional problems with imprecise address information.

**1. Prerequisite**

To switch on the Dutch address logic, the environment variable `ADR_LOGIC_NL` must be set to ON. If this has not happened, the old address logic will still be used in A+W Enterprise.

To use the address logic, the database table `xplzortnl` must be filled because the data fields City and Postal code refer to this database table.

**2. Application**

**2.1. ZIP code**
If now you enter a Postal code in the associated data field and precisely one record in the database is found, it is expanded directly. The data fields City, Street, Automobile and Country are filled.

If after the entry of a Postal code more than one record is found in the database, a selo is opened. This selo displays all existing records that it found for the postal code entered, sorted by Postal code, City and Street.

Furthermore, the opening of the selos with F9 works and if no value was entered in the Postal code data field, then the selo delivers the complete quantity of data.

**2.2. Town**
If you enter a value in the City field and there is precisely one record in the database, then the data fields City, Street, Automobile and Country are filled automatically.

If the entry causes several data records to be found in the database, then a selo is called up that displays the hit quantity for the city entered. Similarly, on this selo you can limit the hit quantity according to the Street in ascending order. The selo is sorted by Postal code, City and Street.

With F9 the selo is opened manually and if you have not entered a value in the City data field, the complete hit quantity is output.

### 6.2.2. Cancellation of addresses

*QR23/03 [AW-112001]*

In the market partner master data, you can close down the addresses that cannot be deleted because they are still used in active documents, in dispatch or in ordering. If it is determined that the addresses cannot be deleted, there is a question about whether these should then be closed down. If you answer YES, then the close ID is set for the address and it can no longer be selected in the document entry. Furthermore, you may neither delete nor close down the invoice address and the main address.

In the dialog footer, there is a new switch "Delete" (for active addresses)/"reactivate" (for closed down addresses). This switch is disabled for the main and invoice addresses.

Closing down the addresses is only possible in the market partner master data. In the document entry, the only possibility is to obtain active addresses for selection or to enter a new address. Only the new address can be deleted immediately after entry.

If a new order/quotation is entered as reference to an old document with the closed-down address, the user is informed that this delivery address has been closed down and that a check is required.

If an order contains a closed-down delivery address, then this will also be taken over in a PO and an order resulting from it (internal EDI). In this case, there is no notice that the address has been cancelled.

Within the market partner replication, canceled addressed are replicated. Here too, there is no notice that there are cancelled addresses.

## 6.3. Routes

If the switch `MODUL_REGIONALROUTEN` is set to ON, the fields for alternative routes, routes 2-4, cannot be accessed. If before an activation of the environment variable there are already alternative routes in the market partner master data, it absolutely has to be deleted manually with activation. Thanks to the activation of the environment variable, the alternative routes for the market partner are not removed automatically from the system.

s.a. chapter „Shipping area / routes“ and „Addresses“

## 6.4. Department

The customer's department is not taken over into the order. (see also `ABTNR_ENTRY`)

*QR 23/01*

The department can be used for the calculation/determination of Discounts/surcharges.
It is possible to group the discounts according to a new criterion "special". This criterion can be adjusted customer-specifically.

The 1st variant is the market partner's department
`SPEZ_RABATTGRUPPE = 'MPABTNR'`

## 6.5. E-mail

Within the market partner master data, you can store various e-mail addresses. Which is used in the end for printing forms is multi-stage. There is an explanation in the separate documentation "EN-CONFIG-A+W Enterprise Print Service"

Whether forms can be sent to the market partner printed or via e-mail can be controlled via system configurations. There is an explanation in the separate documentation "EN-CONFIG-A+W Enterprise Print Service" in the "Form printing or e-mail" section.

## 6.6. Type of EDI

In the "Type of EDI" "PU 1:1" or "PU 1:n" can be set for internal market partners. This setting does not define whether an order-related PO only belongs to one order or to several. This setting controls the population of the kauf.org* fields in the PO or of the internal order at the production site. For more details, see "EN-CONFIG-A+W Enterprise EDI".

## 6.7. Fixed private fields

`mpcomfld.fldnr = -3001` (LS print from dispatch) can contain 1 or 0. Is queried via the Ifdnr and not via the name.
=> Delivery note printing in dispatch depending on a configured field in market partner master.

## 6.8. Environment variables

**MP_STORNO_CHANGE (client reference: no)**
For discontinued market partners, the data on the subdialogs cannot be changed. If this variable is active, this is possible. The variable can be activated employee-specifically.

# 7. Document types

Reference here is not to `kauf.vorgang`, that is, inquiry, PO, etc., but to `kauf_kaufart`; that is, complaint, free of charge, etc.

| Kaufart | Sales | Purchasing | Dependent functions |
| :--- | :--- | :--- | :--- |
| 1 | errno 32406<br>Internal order | errno 32424<br>Internal P.Ο. | |
| 2 | | errno 32425<br>Free P.O. | |
| 3 | | | |
| 4 | | | |
| 5 | | errno 38332<br>Replacement PO | |

# 8. Sealing Depth

## 8.1. Motivation and goals of this development

`\\JUPITER\DOKU_DocuWare\ALCIB-PMS\!General\Release Documents\2011\ReleaseNotes\DE-ALCIB-2011-ERN-IN-Variable-Versiegelungstiefe.docx`

AWDesk case: #115597

## 8.2. Key terms

**(Figure 4: Chart for the terms)**

