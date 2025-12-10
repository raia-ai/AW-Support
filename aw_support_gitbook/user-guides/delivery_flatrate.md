---
title: "Delivery flatrate"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["Delivery_flatrate"]
version: "1.0"
last_updated: "2025-12-10"
description: "Delivery flat rate  1.      First, you have to define the product as a service (product type and product class):     2.      Define the price for the delivery flat rate: 3.   The product has also to be defined in the Company data Basic data / Company / Surcharge:     3.   In Partner Management, the checkbox "Delivery Flat rate" has to be enabled  Partner /      Customer / Customer / 2. Order:     4.   It is possible to realise exceptions per routes  Basic data / Shipping / Routes  the"
source_file: "Delivery_flatrate.pdf"
---


# Delivery flatrate

Delivery flat rate

1.      First, you have to define the product as a service (product type and product class):




2.      Define the price for the delivery flat rate:
3.   The product has also to be defined in the Company data Basic data / Company / Surcharge:




3.   In Partner Management, the checkbox "Delivery Flat rate" has to be enabled  Partner /
     Customer / Customer / 2. Order:




4.   It is possible to realise exceptions per routes  Basic data / Shipping / Routes  the
     definition here has a major priority in comparison to the checkbox "Delivery Flat rate". This
     means, that if the checkbox "Delivery Flat rate" is enabled in the partner management but the
     checkbox "No Delivery Forfeit" is also enabled in Basic data / Shipping / Routes  the
     customer does not pay Delivery Forfeit for this route !
5.     Now you can create your order with different items. When printing your invoice, delivery flat
       rate will automatically be added to the invoice one time at the end of the last order. Please
       note: When printing the invoice, the number control must be sorted by customers!


The whole procedure works like this:

A)     Create your orders

B)     Print your invoice:




C)     Your delivery flat rate (here: product number 6501) appears automatically under your last item
       in your order entry:




Advice: Even if the invoices are printed in more than one print batch the delivery flat rate is only
calculated once per customer\delivery date/tour.
Further pre-conditions:

       Tour and delivery date must be identical.
       Delivery note has to be printed (Delivery note no. >0)
       When creating/printing the invoice no open orders (not delivered) are allowed for this delivery
        date. Otherwise the delivery Flatrate won’t be calculated.
       The defined delivery date on the day of the invoice printout is the essential one (in case of
        date changes).
       The deviating delivery address is considered, but it needs to be a defined delivery address
        (Subsidiary), a manually entered “construction site address” will not be considered.



Delivery flat rate in case of a shortfall of a total orders value per delivery date:

This is a combination of delivery flat rate and limit type „net value (delivery date)“.
The delivery flat rate is always calculated with the invoice printout. With the combination of delivery flat
rate and the graduation of ist price by the limit type „net value (delivery date)“ the delivery flat rate will
only be delivered if the total orders value of a whole date falls under a defined limit.

Price definition for such a delivery flat rate:
Delivery date or shipment date?
There is a setting in Company master data on the price calc tab, 6. Here it is possible to adjust if the
delivery fee should calculate using the delivery date or the shipment date:

