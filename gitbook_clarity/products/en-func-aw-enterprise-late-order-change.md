---
description: "EN FUNC A+W Enterprise Late Order Change"
---



# EN FUNC A+W Enterprise Late Order Change

     Functional Description


A+W Late Order Change




                              english
1. Content
1.   Content                                                                3
2.   Notes on this Document                                                 4
     2.1. Trademarks                                                        4
     2.2. Copyrights                                                        4
     2.3. Disclaimer of liability                                           4
3.   Performance Description                                                5
     3.1. Data                                                              5
     3.2. Description                                                       5
     3.3. Requirements                                                      5
     3.4. List of functions                                                 6
          3.4.1. Purely commercial changes                                  6
          3.4.2. Changes that are forwarded to production as information    6
          3.4.3. Production-relevant change that require new scheduling     6
     3.5. Restrictions                                                      7
     3.6. Notes                                                             7
4.   Contact Address                                                        8




A+W Software GmbH           EN-FUNC-A+W Enterprise Late Order Change.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only be
used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The text and illustrations were
compiled with the utmost care. However it is not possible to exclude errors completely. A+W
Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to
wilful or grossly negligent action.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in an
archiving system, or transferred in any other form only in accordance with our license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


2.3. Disclaimer of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH          EN-FUNC-A+W Enterprise Late Order Change.docx                           4
3. Performance Description
3.1. Data
 Product               A+W Enterprise
 Module number 200020
 Module                Late Order Change
 Brief                 With this module, non-technical data can also be transferred
 description           to A+W Production even after production has already
                       started.
 Available             Starting with A+W Enterprise v6


3.2. Description
With this module, non-technical data can also be transferred to A+W Production even after
production has already started.
Select commercial data such as delivery data, address, and routes can be updated during ongoing
production in A+W Production. This improves the organization of the production and delivery
processes.


3.3. Requirements
For the activation of this function, the following modules must be in versions that are compatible
with one another.
    •   A+W Enterprise 5
    •   A+W Enterprise 5 OrderXML Service
    •   A+W Production 5
Both the PPS and the ERP system must be Version 5 with the Service Pack 5.
Minimum requirement for ORDERXML_VERSION is "5.2."
This module is a for-fee module that must be activated in the system. The A+W Enterprise system
configuration may only be done after the update of A+W Production 5.5!
The use of the module may depend on other system settings. These will be discussed later in the
document.




A+W Software GmbH          EN-FUNC-A+W Enterprise Late Order Change.docx                             5
3.4. List of functions
Three types of order changes in A+W Enterprise will be classified:
    • Purely commercial changes
    • Changes that are forwarded as information to production
    • Production-relevant changes


3.4.1. Purely commercial changes
Such as prices, terms, user data, invoice and print options, payment options, etc.: these changes
always remain local and are not forwarded, there is no query.
If another transfer is nevertheless desired, it can be made with the Renewed transfer to
production menu element. For this transfer, no change in the order is required.


3.4.2. Changes that are forwarded to production as information
Such as packaging type, declaration of performance, file attachments, delivery address, customer
address, delivery date (for locked orders): These changes can be taken over by all items and
forwarded, even if they are already locked by ordering or production.
 Thus, there is no new scheduling.


3.4.3. Production-relevant change that require new scheduling
Such as change to product, quantity, dimensions, delivery date, route, etc.: These changes are
only possible for items that are not locked and are only forwarded for such. If there is only one
comprehensive production-relevant change in the order, then the locked items have the identifier
"no change" and are read over during takeover into production. Items with the procurement type
"none" can also not get an identifier for the production-relevant changes. All newly-entered items
in correction mode naturally count immediately as production-relevant, except those with the
procurement type "none."
Exception: All items that are run on "error during scheduling" are set to "production-relevant"
correction with each correction of the order.
The changes that set the status "info to production" or "production-relevant" are logged. This
logging is not active by default, however, and it has to be activated. The reason for the transfer to
production as well as the decision of the person whether the changes should be transferred to
production is also logged. This logging runs by default.
The changes are noted item by item. If there is an order-spanning change (such as change of the
customer data), then the change type is taken over into all items if these still do not have their
own or a lower change status. The already-locked items will not assume the status "production-
relevant." For these items, production-relevant changes remain local. The change status in the
items is retained until the changes are acknowledged by production (kauf.uebertragen = 1).
The evaluation of the changes in the process takes place with each correction. As long as the
order was not forwarded to production and was not reported "processed" by production, the
change status on all items remains "production-relevant."
Depending on the type of change, items can have different status and change flags in the order.


A+W Software GmbH          EN-FUNC-A+W Enterprise Late Order Change.docx                             6
3.5. Restrictions
The transfer of order changes to production depends on other system settings such as "Lock logic
by item" and permissible status update with existing purchase orders or receipt of goods


3.6. Notes
This functionality is a Value+ function.




A+W Software GmbH           EN-FUNC-A+W Enterprise Late Order Change.docx                      7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH       EN-FUNC-A+W Enterprise Late Order Change.docx   8

