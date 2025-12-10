---
title: "EN FUNC A+W Business Excel Import"
category: "functional_descriptions"
product: "A+W Business Excel Import"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Business Excel Import"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W – Business Excel Import of Items                                    english 1. Content 1.   Content                                                             3 2.   Notes on this Document                                              4      2.1. Trademarks                                                     4      2.2. Copyrights                                                     4      2.3. Disclaimer of liability                                        4 3"
source_file: "EN-FUNC-A+W Business Excel Import.pdf"
---


# EN FUNC A+W Business Excel Import

      Functional Description


A+W – Business
Excel Import of Items




                               english
1. Content
1.   Content                                                             3
2.   Notes on this Document                                              4
     2.1. Trademarks                                                     4
     2.2. Copyrights                                                     4
     2.3. Disclaimer of liability                                        4
3.   Performance Description                                             5
     3.1. Data                                                           5
     3.2. Description                                                    5
     3.3. Prerequisites                                                  7
     3.4. List of functions                                              7
     3.5. Restrictions                                                   7
     3.6. Notes                                                          7
4.   Contact Address                                                     8




A+W Software GmbH               EN-FUNC-A+W Business Excel Import.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are for
information purposes only and are subject to changes without prior notice. The text and
illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W
Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to
wilful or grossly negligent action.


2.1. Trademarks
All hardware and software names mentioned in this documentation may also be registered
trademarks or other industrial property rights held by third parties. Copyrights of third parties
must be complied with.


2.2. Copyrights
© 2021, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in
an archiving system, or transferred in any other form only in accordance with our license
agreement. The documentation may not be transmitted electronically, by recording or in any
other form without the prior written permission of A+W Software GmbH.


2.3. Disclaimer of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This also includes possibly
necessary long-term costs and expenses for amending and extending subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH              EN-FUNC-A+W Business Excel Import.docx                               4
3. Performance Description
3.1. Data
 Product                    A+W Business
 Article number             210018, 230018
 Module                     Excel Line Item Import
 Brief description          Import of line items from the MS Excel clipboard
 Available                  Starting with A+W Business 5.5/6.0


3.2. Description
There is an import of items based on an already existing item with the addition of particular
properties via the clipboard. The data to be added has to be included in a specified format on the
clipboard.
The import is divided into two steps. First, the transfer of the clipboard to a screen table. Here, no
data is taken over into the document. Changes to the data can be made now, before the actual
import. Only in the second step is the marked data from the screen table transferred into the
document and saved there.
To start the functionality, an existing item is marked in item entry and the "Import from
clipboard" function is selected via context menu. Then the following dialog starts.




Here, you can use the key combination <CTRL> - <V> or the "+" key to copy the data from the
clipboard to the table.


A+W Software GmbH               EN-FUNC-A+W Business Excel Import.docx                               5
The clipboard has to include the data to be imported in the following format:




Here, the line with the column header can be omitted. The individual columns are separated with
a tab (TAB) and can also be omitted if instead the original value from the template should be
retained.
A particularity applies for the takeover of the article number. Here, it is possible to use the article
referencing from the program Master Data > B2B > Customer/Supplier > Products. If no
references are created there or if the reference there cannot be found, the import uses the article
number from the clipboard directly. This way, complex product structures can be defined, which
can be selected via a brief reference in the article field.
The values for the width and height are interpreted depending on the measurement system of the
document. That is, if the document is set to metric, the import expects a metric number format. If
the measurement system is set to imperial, either a decimal inch value or the specification of an
inch break is expected. As separator for the inch break, the following characters are permissible:*
"\ /
If the specified dimension precision cannot be mapped because the actual dimension precision is
less than in the clipboard, an error is displayed and no import is performed.
On the right side of the dialog, you can assign the data from the clipboard to the properties of the
item. This assignment can also be saved for later use. Already-saved assignments can be selected
with the combo box.
By pressing the OK button, you start the import of the marked lines. Here, a new item is created
in the document for each marked line. Each item is practically a copy of the template item in


A+W Software GmbH               EN-FUNC-A+W Business Excel Import.docx                                6
which the properties that exist in the clipboard were replaced. If the clipboard includes an article
number, then manual changes (e.g. price specifications or exchange glass) are deleted from the
template item. During the import, a progress bar is displayed. In the end, the item entry is
displayed with the new items in the table. The marking remains on the previously selected item.
Prices for all new items were calculated and if necessary, these were also reserved in the
warehouse. Entirely as if they had been entered manually.




3.3. Prerequisites
    •   A+W Business (core module)


3.4. List of functions
    •   Transfer of the data from the clipboard to a screen table
    •   Editing and selection of the data to be imported on the Import dialog
    •   Generation of the new items in the current document including price calculation with the
        previously selected item as template


3.5. Restrictions
    •   No items can be created in an empty document. A saved item always has to be selected; it
        serves as a template
    •   The maximum number of items per document is 800
    •   Items can only be inserted at the end


3.6. Notes




A+W Software GmbH              EN-FUNC-A+W Business Excel Import.docx                                  7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH           EN-FUNC-A+W Business Excel Import.docx   8

