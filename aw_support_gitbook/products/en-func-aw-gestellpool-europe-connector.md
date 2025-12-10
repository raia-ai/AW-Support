---
title: "EN FUNC A+W Gestellpool Europe Connector"
category: "functional_descriptions"
product: "A+W Gestellpool Europe Connector"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Gestellpool Europe Connector"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   Gestellpool Europe Connector                                    english 1. Contents 1.         Contents                                                            3 2.         Notes on this document                                              4   2.1.     Trademarks                                                          4   2.2.     Copyrights                                                          4   2.3.     Exclusion of liability"
source_file: "EN-FUNC-A+W Gestellpool Europe Connector.pdf"
---


# EN FUNC A+W Gestellpool Europe Connector

     Functional Description


Gestellpool Europe Connector




                               english
1. Contents
1.         Contents                                                            3
2.         Notes on this document                                              4
  2.1.     Trademarks                                                          4
  2.2.     Copyrights                                                          4
  2.3.     Exclusion of liability                                              4
3.         Performance Description                                             5
  3.1.     Data                                                                5
  3.2.     Description                                                         5
  3.3.     Prerequisites                                                       5
  3.4.     List of functions                                                   5
     3.4.1. Interface description                                              7
     3.4.2. GPE rack header                                                    8
 3.5.      Restrictions                                                        8
 3.6.      Notes                                                               8
4.         Contact Address                                                     9




A+W Software GmbH              EN-FUNC-A+W Gestellpool Europe Connector.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly
negligent action.


2.1. Trademarks
All hardware and software names mentioned in this documentation can also be registered
trademarks or other property rights of third parties. Third-party copyrights must therefore be
observed.


2.2. Copyrights
© 2022, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may be copied, completely or in part, saved in an archiving
system, or transferred in any other form only in accordance with our license agreement. The
documentation may not be transmitted electronically, by recording or in any other form without
the prior written permission of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions that have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions that
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH          EN-FUNC-A+W Gestellpool Europe Connector.docx                              4
3. Performance Description
3.1. Data
 Product               Gestellpool Europe Connector
 Article no.           262030
 Module                A+W Logistics Optimizer - Gestellpool Europe Connector
 Brief                 Interface for the import of information (CSV file) for racks
 description           that are ready for pick-up
 Available             QR2210


3.2. Description
The Gestellpool Europe Connector is an interface between Gestellpool Europe and the A+W
Logistics Optimizer. With this interface, racks from the Gestellpool Europe ready for pick-up can
be imported via CSV file into the A+W Logistics Optimizer.


3.3. Prerequisites
Prerequisite is the use of Gestellpool Europe and one of the modules
    -   A+W Smart Delivery
    -   A+W Smart Delivery Maps
    -   A+W Logistics Optimizer


3.4. List of functions
From the A+W Logistics Optimizer, click the Pack… button




A+W Software GmbH         EN-FUNC-A+W Gestellpool Europe Connector.docx                             5
.. to reach the Import GPE button. This button is only available if the license for the Gestellpool
Europe Connector is in use.




After execution of the import, the A+W Logistics Optimizer writes the pick-up address into a
geolocation (address, latitude and longitude), which is assigned to a real map.
If a geolocation is not found or if more than one is found, the packing action is marked as
geolocation error so that it can be geolocalized by the user.
After the import, these packing actions can be planned into a route --> Route planner > Packing
tab.




A+W Software GmbH          EN-FUNC-A+W Gestellpool Europe Connector.docx                              6
3.4.1. Interface description
GPE – CSV file example
Group;plant;number;reference;product;status;description;last comment;last movement;last
movement by; GPE customer number;customer name;customer number;delivery
address;reporting date;supplier group;supplier plant;delivery date;in hand;outgoing goods
route;outgoing goods route stop;contact on-site;pick-up location;pick-up route;pick-up route
stop;barcode number;packaging ID
002;160;203000047;10279848;A-rack medium;ready for pick-up;A-rack medium;beds
I;20.03.2022 10:41:17;marvin_gortmann;K38750;Duinkerke Glasservice BV;1515050;Steenoven 6
, 3911 TR, Rhenen;03.03.2022 10:38:00;002;150;20.03.2022 10:41:17;45;19;5;;Steenoven 6 , 3911
TR, Rhenen;;;002160203000047;2
002;160;203000242;218864;A-rack medium;ready for pick-up;A-rack medium;;25.03.2022
14:01:27;KY-621;K30121;Tietjen Holz-Kunststoff-;800313;Huchtinger Straáe 18, 28197,
Bremen;08.03.2022 10:13:00;002;160;25.03.2022 14:01:27;14;706;;;Huchtinger Straáe 18, 28197,
Bremen;;;002160203000242;2
002;160;203000352;2215520;A-rack medium;ready for pick-up;A-rack medium;;24.03.2022
00:00:00;NO_USER;K14713;Fenster 2000;2215520;Georg-Leppien-Str. 21, 21337,
Lüneburg;25.08.2019 00:00:00;002;160;24.03.2019 00:00:00;63;;;;Georg-Leppien-Str. 21, 21337,
Lüneburg;;;002160203000352;2




A+W Software GmbH        EN-FUNC-A+W Gestellpool Europe Connector.docx                      7
3.4.2. GPE rack header




3.5. Restrictions
A CSV file is used for the transport of the information. No Web service!
The Gestellpool Europe Connector does not provide any information about the packaging type
such as width, height, depth, etc., so that after the first import of a new packaging type, the
Gestellpool Europe interface automatically initializes the packaging type, but this must absolutely
be checked by the user since otherwise the freight optimization does not have the corresponding
dimensions in order to optimize the cargo space of the truck.


3.6. Notes


A+W Software GmbH          EN-FUNC-A+W Gestellpool Europe Connector.docx                          8
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH       EN-FUNC-A+W Gestellpool Europe Connector.docx   9

