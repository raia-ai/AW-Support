---
description: "EN-CONFIG-AW_Business-11"
---


At document entry, tax calculation has to be triggered when fields are changed. This requires menu customizing. Save the field contents in the order structure and open tax calculation and display of fields.

*Fig. 212: Search formula in document entry*

Tax rates can be entered in program Master data/Finances/Tax matrix. Input limits have to be filled via menu customizing.

Customer master data now offers the checkboxes Tax code for the individual taxes. These can be used for control purposes in the tax formulas. By default, they have no function. The code 'end user' has been adopted from customer master data and can be changed as required in the document.

Taxes can be named by means of the system text modules 151-155

---
## Tax calculation formulas for Brazil

Tax calculation formulas are assigned using Brazilian tax for example. Brazilian tax calculation knows five taxes.

**ICMS** - Depending on the shipping area (route), the tax is calculated by means of a code, ICMS contribute'.

Customers with this flag are distinguished by end customers and resellers.

The definition is made in program Tax matrix

This table shows the tax rates and dependences:

*Tab. 49: Brasil. Tax rates and dependences:*

| Regions | For companies which contribute with ICMS taxes (If destined to subsequent commercialization or industrialization) | For companies which contribute with ICMS taxes (End Customers) | For companies which DOES NOT contribute with ICMS taxes |
| :--- | :--- | :--- | :--- |
| **SP** | 18% | 18% | |
| **Zona Franca/Manaus** | 0% | 0% | 0% |
| **Southeast & South** | 12% | 12% | 18% |
| **Northeast, North, Center-West & Espirito Santo State** | 7% | 7% | 18% |

**PIS** - The tax is 1.65% and is added to the ICMS tax.

**CONFIX** - The tax is 7.60% and is added to the ICMS tax.

**IPI** - The tax depends on the product and is calculated by item. It is added to all former taxes. Exception: the customer is an end customer and subject to ICMS tax in which case, the IPI tax is calculation basis for ICMS tax, and is calculated first.

**ISS** - Service tax depending on the customer's area

### Setting up formula calculation for Brazil

The customizing dialog Master data/company/customizing, tab Programs, serves to define the formulas for tax calculation.

**Formula allocation point:**
*   50 - Allocate formula 350
*   51 - Allocate formula 351
*   52 - Allocate formula 352

The following formulas have to be allocated for menu customizing:
*   Formula 353 - Document header - Click Event - combo box Route and Add button, and delete the shipping address
*   Formula 354 - Document header - Click Event - combo box State
*   Formula 355 - Document header - Click Event - end customer
*   Formula 360 - Tax matrix - create window

The demo database includes all formulas

### Form printing

For printing of forms, the same tax variables are available for tax 3-5 and for tax 1-2.
To fulfil (for Brazilian tax calculation) the requirement that the tax must be included in the price per price unit, the tax amount for the item (for tax 1-5) can be loaded from the item variable (POS_ITEM_MWST1-5). The form has to be customized to get the value of price/price unit. The total item tax has to be adapted to the item's price unit using the function `float udf_AdjustValueOnItemPricePerUnit(Value, item object)`.

### Import and Export of Payment Information

In Brazil, the payment traffic is normaly handled via the banks. The customizing formulas are used in order to transfer payments to the banks and also read in the report about payments made. These formulas must be adjusted individually for each bank for their file format. After that, the formulas for the import and export of the bank in question are assigned in the bank administration.

*Fig. 213: Import and export of payment information*

Furthermore, it is necessary to set the external keys of the currency identifiers to the international currency identifiers.

*Fig. 214: Adjusting currency identifiers*

The tax number must be entered in the company master data.

*Fig. 215: Tax number in the company master data*

Examples for custommizing are located in the installation path of the formulas (normally `C:\Program Files\A+W\ALFAK 2011\Formula\`) with the name `brasiliantax_paymentbankexportXXX.txt` or `brasiliantax_paymentbankimportXXX.txt`.

For the actual import or export of the payment, you access the import/export of payments via Documents > Order.

There, the payments to be exported are selected, the appropriate bank is selected, the file name specified and the export started with a click on OK. During the import, the bank and the file name must also be specified and the import is started with a click on OK.

*Fig. 216:Import/export of payments*

## 10.23. Cash discount date calculation

Calculation of the cash discount date requires flexibility on the application's part. This is because the conditions are subject to negotiation. It is therefore possible to implement this via customizing. Standard calculation will still be run, i.e. even partial aspects can be changed. Customising runs in the context of the document category.

In the customizing dialog, the formula for item **40-cash discount date** has to be entered. The following variables can be set via customizing:

| Variable | Description |
| :--- | :--- |
| `m_nCashDiscountRate1...3` | -> Cash discount1-3 |
| `m_nCashDiscountDays1...3` | -> Cash discount days 1-3 |
| `m_dCashDiscountDate1...3` | -> Cash discount date 1-3 |

Standard implementation uses the function `ABC_ValutaDate` to calculate the cash discount date.
`Set m_dCashDiscountDate1 = ABC_ValutaDate( m_dDATUM_RECHNUNG, m_dDATUM_RECHNUNG, 0, 1, m_nCashDiscountDays1, 0, 0, 0)`

`dDate = ABC_ValutaDate (dInputDate, dDeliveryDate, nInvoiceDay, nFlag, nCashDays, nCashDay1, nCashDay2, nCashDay3)`

**Cash discount date calculation**

**Parameter:**

| Parameter | Description |
| :--- | :--- |
| `dInputDate` | Date/Time: Starting date (invoice date) |
| `dDeliveryDate` | Date/Time: Shipping date (if nFlag=11) |
| `nInvoiceDay` | Number: Invoicing date (Standard 0) |
| `nFlag` | Number: Cash discount calculation type (Standard 1) |
| `nCashDays` | Number: Number of cash discount days |
| `nCashDay1...3` | Number: Payment date 1 to 3 (Standard 0) |

**Returns:**

New cash discount date

## 10.24. Data container for customizing data

The data container for customizing data can be used to manage data required for customizing, flexibly by means of the database. The names of the tabs and tables on screen can be defined by the project manager by means of formulas.

*Fig. 217: Formula dialog - Data container - creating formulas*

So that the administrator maintains control over the individual functionalities, the management of the dialog can be configured via the ALFAK rights system.

These scripts must be executed. - 20081006a.sql/20081007a.sql/20081007m.sql

### Customizing data recording

A dialog has been created with the help of which new or changed customizing data can be saved in an appropriate database. You call the dialog from the master data\company\data container. It has five tabs. Each tab represents another aspect of customizing. On each tab, there is a screen tablewhere the storing of the data takes place. On Insert, all columns can be edited. The user has the possibility to make new entries with the help of the Control element combo box.

The names of the tabs can be specified by the planner (see below: 8.23.2.2). If something is already set up, it can be found under Screen customizing on the Customizing dialog.

### Adjusting the data container dialog with formulas

**Sample formulas**

### Example 1: Formula data container for customizing data:

**Tab descriptions**

```
!***************************************************************************,
!** Set labels for all tabs **,
|*************************************************************************,
picTabs.SetLabel(0, 'Erlöskontenermitlung', FALSE);
picTabs.SetLabel(1, 'Wetter', FALSE);
picTabs.SetLabel(2, 'Land', FALSE);
picTabs.SetLabel(3, 'Kunden', FALSE);
picTabs.SetLabel(4, 'MyTest', FALSE);
```

**Table headers**
The table headers can be defined in the same formula.

```
!***************************************************************************,
! ** Set row header for all tables **,
|*************************************************************************;
SalTblSetColumnTitle(tblCustomizingData1.cbBorder1, 'Produkt');
SalTblSetColumnTitle(tblCustomizingData1.cbBorder2, 'Doktyp');
SalTblSetColumnTitle(tblCustomizingData1.cbBorder3, 'AV-Bereich');
SalTblSetColumnTitle(tblCustomizingData1.cbWert, 'Erlöskonten');

SalTblSetColumnTitle(tblCustomizingData2.cbBorder1, 'Vormittag');
SalTblSetColumnTitle(tblCustomizingData2.cbBorder2, 'Tag');
SalTblSetColumnTitle(tblCustomizingData2.cbBorder3, 'Nacht');
SalTblSetColumnTitle(tblCustomizingData2.cbWert, 'Datum/Temperatur');

SalTblSetColumnTitle(tblCustomizingData3.cbBorder1, 'Rusland');
SalTblSetColumnTitle(tblCustomizingData3.cbBorder2, 'USA');
SalTblSetColumnTitle(tblCustomizingData3.cbBorder3, 'Östereich');
SalTblSetColumnTitle(tblCustomizingData3.cbWert, 'Wert');
```

**Table fields**
The table fields (monitor) shall be edited.
Additionally, you can enter fix values from combo boxes, that have been defined with the help of the formula.

```
!***************************************************************************,
!** Set value for columns Table 1 **,
|*************************************************************************,
tblCustomizingData1.cbBorder1.AddValueString('1004-Float 4 mm', '1004');
tblCustomizingData1.cbBorder1.AddValueString('1006-Float 6 mm', '1006');
tblCustomizingData1.cbBorder1.AddValueString('1008-Float 8 mm', '1008');
tblCustomizingData1.cbBorder1.AddValueString('ESG Klar 4 mm', '4004');

tblCustomizingData1.cbBorder2.AddValueString('Auftrag', '2');
tblCustomizingData1.cbBorder2.AddValueString('Gutschrift', '1');

tblCustomizingData1.cbBorder3.AddValueString('ESG-Fertigung', 'ESG-Fertigung');
tblCustomizingData1.cbBorder3.AddValueString('<k.A.>', '<k.A.>');
tblCustomizingData1.cbBorder3.AddValueString('Isolierglasfertigung', 'Isolierglasfertigung');
tblCustomizingData1.cbBorder3.AddValueString('Vitropur', 'Vitropur');
```

### Customizing access to the data container

The function determines a value with particular limits, which was saved to the database by the Data container dialog. So that a query to the database can be performed without problems, the following parameters should be entered when the function is called.

`udf_ReadData(nMode, nTyp, sBorder1, sBorder2, sBorder3, sValue)`

**Parameter:**

| Parameter | Type | Description |
| :--- | :--- | :--- |
| `nMode` | Number | Predefeined mode. **1** - In the query, the limits in the WHERE clause are established with "=". A particular value is searched for. **0** - For the mode, the limits in the WHERE clause are established with ">=". That is, if no data record with the specified limits is found, the next such one is determined for which the limits are larger. For examples, see below. |
| `nTyp` | Number | Tab on the Data container dialog |
| `sBorder1` | String | Limit 1 |
| `sBorder2` | String | Limit 2 |
| `sBorder3` | String | Limit 3 |
| `sValue` | Receive String | The value that is determined. |

**Returns:** TRUE = no error

### Example 2: Formula - call of the function udf_ReadData(...)

In the example, a formula is defined in customizing that calls the function `udf_ReadData(...)` mentioned above. The result is then available in the variable `m_sWdv[0]` and is communicated to the user in the form of a `MessageBox`. The formula is executed from the price formulas in the context of the document class through the call of the function `udf_ExecFormula(999)`.

```
|***************************************************************************,
!** Use Function udf_ReadData for data container customizing data **.
!*************************************************************************;
!** Used Variables **;
! m_nUdv[1] -> Product number ;
! m_nUdv[2] -> Document type ;
! m_sUdv[0] -> The value of the read data ;
! m_sUdv[1] -> number area ;
|*************************************************************************,
Set m_nUdv[1] = m_Pos[m_nCurltemIdx].m_nPROD_ID;
Set m_nUdv[2] = m_nDocType;
Set m_sUdv[1] = m_sOR_AVBEREICH;
! ** The function udf_ReadData delivers one certain value from table KA_CUSTOMIZINGDATA by insert **;
! ** mode, type and 3 borders **.
! ** Parameters: **;
|** Number: nMode The mode for the query. These are two values permit: **;
|** 1 - determines the value with exactly eingegebeneb borders **;
|** 0 - If it exists no value with the given borders, it is used in **;
|** WHERE Klaus instead of BORDER1= :sBORDER1, BORDER1 >= :sBORDER1 **;

|** Number: nTyp Tab number in dialog Datencontainer **;
|** String: sBorder1 border 1 **.
|** String: sBorder2 border 2 **.
|** String: sBorder3 border 3 **;
|** Receive String: sWert The value of the entered data. If it was found no record the string delivers **;

udf_ReadData(0,1, SalNumberToStrX( m_nUdv[1], 0), SalNumberToStrX(m_nUdv[2], 0), m_sUdv[1],m_sUdv[0]);

SalMessageBox ( m_sUdv[0], 'WERT', MB_Ok );
```

### Apply formulas

Using the Selection menu, the formulas are assigned to the dialog. The Selection menu can be called up with a right-click on the window header.

*Fig. 218: Data container selection menu*

You can also reach the Customizing dialog using the Selection menu.

In order to incorporate the tabs and table header formula, select the menu element: Event handling "Create window" and search for the created formula that adjusts the tab and the table header.

*Fig. 219: Data container - creating a window*

For the sake of simplicity, insert the formulas from the examples above into a complete one. And implement this as described.

So that the effect is visible, you must restart the dialog.

If after the fact you would like to fill the table columns, use the "Create new data record" menu element and search for the formula that should be incorporated.

In order to examine all formulas set up for the dialog, use the "Customizing" menu element on the Customizing dialog. The first tab "Screens" displays the formulas set up.

## 10.25. Sending the declaration of performance

In order to make the sending of the declaration of performance more flexible, a customizing element has been introduced. In the customizing management (Master data > Company > Customizing), the element 500 - Sending of declarations of performance is used for this. The formula is called up before sending each declaration of performance once. In the formula that is assigned to this element, you have access to the complete e-mail and the associated customer number. The following variables are available:

| Variable | Type | Description |
| :--- | :--- | :--- |
| `nCustomerID` | Number | Number of the customer |
| `fktMail.m_sSMTPServer` | String | Address of the SMTP server |
| `fktMail.m_sSMTPUser` | String | User for the log in to the SMTP server |
| `fktMail.m_sSMTPPassword` | String | Password for the log in to the SMTP server |
| `fktMail.m_sFrom` | String | Address of the sender |
| `fktMail.m_sTo` | String | Address of the recipient |
| `fktMail.m_sCC` | String | Address of the copy recipient |
| `fktMail.m_sBCC` | String | Address of the bcc recipient |
| `fktMail.m_sSubject` | String | Re |
| `fktMail.m_sData` | String | Content of the mail in text format |
| `fktMail.m_sDataHtml` | String | Content of the mail in HTML format |
| `fktMail.m_saAttachment[*]` | String Array | Array with the attachments of the mail. Contains the declarations of performance. |
| `fktMail.m_nAttachementCount` | Number | Number of entries contained in the array of the attachments. |

The customer number in the variable `cCustomerID` should not be changed. If necessary, it serves only to communicate additional information about the customer within customizing via SQL query. In the following example, the content of the classifier "LE receiver" is read out of the customer's classifier via SQL query and used as alternate mail address for sending the declaration of performance.

```
! Open the database connection;
If DbMakeTempConnect (g_sqlUdv[0] );
    ! Read ID of the classifier (LE-Receiver);
    If SqlPrepareAndExecute ( g_sqlUdv[0], 'SELECT ID FROM SYSADM.KA_KLASSI_DEF WHERE K_BEZ = \'LE-Receiver\' INTO :g_nUdv[0]' );
        If SqlFetchNext ( g_sqlUdv[0], g_nUdv[1] );
            ! Read content of the classifier;
            If SqlPrepareAndExecute (g_sqlUdv[0], 'SELECT K_WERT FROM SYSADM.KU_KLASSI_WERTE WHERE ID = :nCustomerID AND K_ID = :g_nUdv[0] INTO :g_sUdv[0]');
                If SqlFetchNext (g_sqlUdv[0], g_nUdv[1] );
                    Set fktMail.m_sTo = g_sUdv[0];
                EndIf;
            Endlf;
        EndIf;
    EndIf;
    ! Close database connection;
    DbDisconnect (g_sqlUdv[0]);
Endlf;
```

## 10.26. Form printing via the reporting service

Two functions can be used to transfer documents to the reporting service. The function `udf_PrintDocument(...)` transfers the individual documents and the function `udf_PrintNumberManager(...)` transfers a complete number manager to the reporting service. Therefore, it is possible, e.g. to send order confirmations via mail automatically using a workflow task. The documents can be selected depending on their status, for example, and added to a number manager. In chapter 10.29 Beispiele such a formula is presented as workflow formula for the exchange service.

`bReturn = udf_PrintDocument ( nID, nDocType, nForm, nOutputType, sOutputDevice, sArchiveYear, nNumberRangeMode, nClientID, sOrderArea, dDate, nLabelMode, nNumberOfCopies, bCollectivePrintout)`

Prints out the specified document with the help of the reporting service.

**Parameter:**

| Parameter | Type | Description |
| :--- | :--- | :--- |
| `nID` | Number | The number of the document |
| `nDocType` | Number | The type of the document (nMODE_AUFTRAG, nMODE_BESTELLUNG, nMODE_ANGEBOT, nMODE_GUTSCHRIFT, nMODE_BESTELLANFRAGE) |
| `nForm` | Number | The number of the form with which printing should be done can be seen from the table in the form management |
| `nOutputType` | Number | 0=output on printer (sOutputDevice), 1=output via mail, 2=output to file (file name and path must be specified in the form) |
| `sOutputDevice` | String | Exact name of the printer on which output should occur. For possible names, see the reporting services from the infrastructure services. |
| `sArchiveYear` | String | The year of the archive or empty for main database |
| `nNumberRangeMode` | Number | Mode for access to the number ranges for invoice and delivery note number (0=uses the values from nClientID for site and sOrderArea for AV-area, 1=site and AV area from document;sOrderArea and nClientID are empty,2=client from document and AV area from sOrderArea;nClientID remains empty) |
| `nClientID` | Number | The specified site number for the number ranges. Only important if nNumberRangeMode = 0. |
| `sOrderArea` | String | The specified AV area for the number ranges. Only important if nNumberRangeMode = 0 or 2 |
| `dDate` | Date/time | Print date for invoice date. If empty, the current date is used. |
| `nLabelMode` | Number | Mode for the label printing (0=per unit, 1=per item, 2=setting from document) |
| `nNumberOfCopies` | Number | Number of copies at least 1 |
| `bCollectivePrintout` | Boolean | TRUE = collective print, FALSE = no collective print |

`bReturn = udf_PrintNumberManager (sNumberManager, sUser, nDocType, nForm, nOutputType, sOutputDevice, sArchiveYear, nNumberRangeMode, nClientID, sOrderArea, dDate, nLabelMode, nNumberOfCopies, bCollectivePrintout)`

Prints out the specified number manager with the help of the reporting service.

**Parameter:**

| Parameter | Type | Description |
| :--- | :--- | :--- |
| `sNumberManager` | String | The number manager to be printed |
| `sUser` | String | User of the number manager |
| `nDocType` | Number | The type of the document (nMODE_AUFTRAG, nMODE_BESTELLUNG, nMODE_ANGEBOT, nMODE_GUTSCHRIFT, nMODE_BESTELLANFRAGE) |
| `nForm` | Number | The number of the form with which printing should be done can be seen from the table in the form management |
| `nOutputType` | Number | 0=output on printer (sOutputDevice), 1=output via mail, 2=output to file (file name and path must be specified in the form) |
| `sOutputDevice` | String | Exact name of the printer on which output should occur. For possible names, see the reporting services from the infrastructure services. |
| `sArchiveYear` | String | The year of the archive or empty for main database |
| `nNumberRangeMode` | Number | Mode for access to the number ranges for invoice and delivery note number (0=uses the values from nClientID for site and sOrderArea for AV-area, 1=site and AV area from document;sOrderArea and nClientID are empty, 2=client from document and AV area from sOrderArea;nClientID remains empty) |
| `nClientID` | Number | The specified site number for the number ranges. Only important if nNumberRangeMode = 0. |
| `sOrderArea` | String | The specified AV area for the number ranges. Only important if nNumberRangeMode = 0 or 2 |
| `dDate` | Date/time | Print date for invoice date. If empty, the current date is used. |
| `nLabelMode` | Number | Mode for the label printing (0=per unit, 1=per item, 2=setting from document) |
| `nNumberOfCopies` | Number | Number of copies at least 1 |
| `bCollectivePrintout` | Boolean | TRUE = collective print, FALSE = no collective print |

## 10.27. OrderXML transfer via the import service

Two functions can be used to transfer documents to the import service and/or delete them. The function `"udf_CleanUpOrderXmlTable(...)"` deletes all old OrderXMLs and the function `"udf_TransferOrderXmlToProduction(...)"` transfers all OrderXMLs that are finished to the import service through the exchange service. In chapter 10.29 Beispiele such a formula is presented as workflow formula.

`bReturn = udf_TransferOrderXmlToProduction (bResetErrors, sMessages)`

Prints out the specified document with the help of the exchange service.

**Parameter:**

| Parameter | Type | Description |
| :--- | :--- | :--- |
| `bResetErrors` | Boolean | TRUE = flawed OrderXMLs should be transferred again, FALSE = flawed OrderXML will not be transferred again |
| `sMessages` | Receive string | Info or error messages as character string that can be traced or sent via e-mail |

`bReturn = udf_CleanUpOrderXmlTable ()`

Removes all OrderXMLs from the BW_ORDERXML table that are older than the number of storage days (default value = 7 days).

## 10.28. Breakage transfer from the Logistic Service

The function `"udf_RetreiveBreakages(...)"` transfers all breaks that were not yet transferred from the Logistic Service. In chapter 10.29 Beispiele such a formula is presented as workflow formula.

`bReturn = udf_ RetreiveBreakages ( sMessages)`

Generates the complaints for breakages from the Logistic Service.

**Parameter:**

| Parameter | Description |
| :--- | :--- |
| `sMessages` | Receive string: info or error messages as character string that can be traced or sent via e-mail |

## 10.29. Examples

### User-defined variables and the Customizer

In this example, the user-defined variable "depth" – previously added to the Customizer - is analysed and saved in the item. When the item is saved in the database at item entry, the system also saves the user-defined variables in the database. This is a menu formula which can linked with the event "change record" at item entry for instance.

```
! Determine the actual item index;
w_fktDoc.Search (g_nUdv[0], frmDocumentItems.tblPos.cnPOS_NR );

! Load the depth from Customizer;
g_hUdv[0].tblCustomizer.GetValue ('Tiefe', g_sUdv[0] );
! Save the depth in the item structure;
w_fktDoc.m_Pos[g_nUdv[0]].udf_SetVariable ('Tiefe', g_sUdv[0]);

! Write the depth in the BOM;
w_fktDoc.m_Pos[g_nUdv[0]].udf_GetIdxByOccurrence (40002, 1, g_nUdv[1] );
If g_nUdv[1] != -1;
    Set w_fktDoc.m_Pos[g_nUdv[0]].m_PosStukl[g_nUdv[1]].m_nSTL_BREITE = SalStrToNumber (g_sUdv[0]);
EndIf;

! Delete row flags from Customizer;
SalTblSetFlagsAnyRows (g_hUdv[0], ROW_Edited, FALSE, 0, 0 );
```

### New formula variable

In this example, the user-defined variable "depth" is sent to printing of forms.
`w_fktDoc.m_Pos[w_nRepPosZaehler].udf_GetVariable ( 'Tiefe', g_sUdv[0] );`
`SalReportSetStringVar (hWndReport, 'TIEFE', g_sUdv[0]);`

### Spacer Text

The formula tag is replaced by the IG structure and spacer color.

```
!************************************************************;
!** Get the DGU Structure to the Variable sResult for bendertexts **;
!************************************************************;
!** Used Variables;
!** m_nUdv[0] => Sorting index;
!** m_nUdv[1] => B.O.M. index for access;
!** m_sUdv[0] => Buffer string;
!************************************************************;
! Sorting B.O.M by BOM_ID;
m_Pos[m_nCurltemIdx].CreateSort ();
! Index for B.Ο.Μ.;
Set m_nUdv[0] = 1;
! Loop on all B.O.M items;
WHILE m_Pos[m_nCurltemIdx].GetSort(m_nUdv[0], m_nUdv[1]);
    ! Init buffer;
    SET m_sUdv[0] = '';
    ! Is parent of main item;
    IF m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_nBOM_NODE = 0;
        ! For glass only the short description;
        IF ProduktartIsGlas( m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_nSTL_PRODART );
            Set m_sUdv[0] = m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_sSTL_KURZ_BEZ;
        ENDIF;
        ! For gas only the short description;
        IF m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_nSTL_PRODART = PRDART_FUELL;
            Set m_sUdv[0] = m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_sSTL_KURZ_BEZ;
        ENDIF;
        ! For Spacer add the color;
        IF m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_nSTL_PRODART = PRDART_ABST;
            Set m_sUdv[0] = m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].m_sSTL_KURZ_BEZ;
            IF m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].GetFarbBez( ) != ' ';
                Set m_sUdv[0] = m_sUdv[0] || ' ' || m_Pos[m_nCurltemIdx].m_PosStukl[m_nUdv[1]].GetFarbBez();
            ENDIF;
        ENDIF;
    ENDIF;
    ! Add the text to the result variable;
    IF SalStrLength(m_sUdv[0]);
        ! Add slash if has length;
        IF SalStrLength(sResult);
            SET sResult = sResult || '/';
        ENDIF;
        SET sResult = sResult || m_sUdv[0];
    ENDIF;
    Set m_nUdv[0] = m_nUdv[0] + 1;
WEND;
```

### Processing text

The formula tag is replaced by the item size.

```
!************************************************;
!** Sets the item width and height in the processing text **;
!************************************************;
Set sResult = SalNumberToStrX( m_Pos[m_nCurltemIdx].m_nPP_BREITE, 0 ) || 'x' || SalNumberToStrX( m_Pos[m_nCurltemIdx].m_nPP_HOEHE, 0 );
```

### Load program via buttons

Every dialog has two buttons (pbTB_DUMMY1 and pbTB_DUMMY2) in its toolbar. These have to be visualized in the event „show dialog" by means of a formula. After that, you can add a formula to the button at the Cklick event. This allows to load an external program for example.

**Show window**
```
! ** Change location, visibility and Text of the dummy button **;
|******************************************************;
SalSetWindowLoc (pbTB_DUMMY1, 5, 0.1);
SalSetWindowText (pbTB_DUMMY1, 'Test' );
SalShow Window (pbTB_DUMMY1 );
```
**Click on the button:**
```
|******************************;
! ** Call the Notepad **;
!******************************;
! SalLoadApp ('Notepad.exe', '');
! SalLoadAppAndWait ( 'Notepad.exe', Window_Normal, g_nUdv[0] );
SalLoadAppAndProcessMsgs( 'Notepad.exe', Window_Normal, g_nUdv[0] );
```

### Energy surcharge by fixed size, stocksize, and box

The energy surcharge shall be graduated. Special discounts 4+5 are used for the energy surcharge on stocksizes and boxes. Glass products can only be assigned the common energy surcharge. Allocation is done at pricing. The formula has to be allocated via general program formula allocation (see 3.5).

```
!
! ** Using auto. Discount for Stock sizes an boxes (Discount 4+5) **;
!** Used Variables;
! ** m_nUdv[0] = Discount surcharge flags of product ZUSCHLAG_xxx;
! ** m_nUdv[1] = Fetch variable;
! ** m_sqlUdv[0] = Handle to main database;

IF m_sFormulaContext = 'AFTER_SELECT_PRICE';
    ! Connect to main database;
    IF DbMakeTempConnect(g_sqlUdv[0] );
        ! Search main product in basic data and get the surcharge flag;
        IF SqlPrepareAndExecute( g_sqlUdv[0], 'SELECT PRZ_ZUSCHLAG_BIT FROM SYSADM.BA_PRODUKTE WHERE BA_PRODUKT=:m_Pos[m_nCurltemIdx].m_nPROD_ID INTO :g_nUdv[0]');
            IF SqlFetchNext(g_sqlUdv[0], g_nUdv[1] );
                ! Main product has energy surcharge;
                IF g_nUdv[0] & ZUSCHLAG_ENERGIE;
                    TRACE ('Price formula (310): Basic data product has energy surcharge', EVENT_INFORMATION, TRACE_PRICECALC );
                    ! Item is not a stock size and not a box, so change to surcharge ZUSCHLAG_ENERGIE, disable the others;
                    IF NOT m_Pos[m_nCurltemIdx].m_bLagermass AND m_Pos[m_nCurltemIdx].m_nPROD_PRODART != PRDART_KISTE;
                        TRACE ('Price formula (310): Item has energy surcharge', EVENT_INFORMATION, TRACE_PRICECALC );
                        SET m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT = m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT | ZUSCHLAG_ENERGIE;
                        SET m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT = m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT & ( 0xFFFFFFFF - ZUSCHLAG_SONDERRABATT4 - ZUSCHLAG_SONDERRABATT5);
                    ENDIF;
                    ! Item is a stock size, so change to surcharge ZUSCHLAG_SONDERRABATT4, disable the others;
                    IF m_Pos[m_nCurItemIdx].m_bLagermass AND m_Pos[m_nCurltemIdx].m_nPROD_PRODART != PRDART_KISTE;
                        TRACE ('Price formula (310): Item has energy surcharge for stock sizes', EVENT_INFORMATION, TRACE_PRICECALC );
                        SET m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT = m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT | ZUSCHLAG_SONDERRABATT4;
                        SET m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT = m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT & ( 0xFFFFFFFF - ZUSCHLAG_ENERGIE - ZUSCHLAG_SONDERRABATT5);
                    ENDIF;
                    ! Item is a box, so change to surcharge ZUSCHLAG_SONDERRABATT5, disable the others;
                    ! Attention: Box is a stocksize as well, so it must be the last question;
                    IF m_Pos[m_nCurltemIdx].m_nPROD_PRODART = PRDART_KISTE;
                        TRACE ('Price formula (310): Item has energy surcharge for boxes', EVENT_INFORMATION, TRACE_PRICECALC );
                        SET m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT = m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT | ZUSCHLAG_SONDERRABATT5;
                        SET m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT = m_Pos[m_nCurltemIdx].m_nPROD_ZUSCHLAG_BIT & ( OxFFFFFFFF - ZUSCHLAG_ENERGIE - ZUSCHLAG_SONDERRABATT4);
                    ENDIF;
                ENDIF;
            ENDIF;
        ENDIF;
        SqlDisconnect(g_sqlUdv[0]);
    ENDIF;
ENDIF;
```

### Direct shipment of P.O. to a certain supplier

POs are always transferred to suppliers as drop shipments. You do not have to set the code Direct shipment in the order.

```
!*****************************************************************;
!** Direct delivery for DORMA **;
!*****************************************************************;
!** Used Variables;
! fktAuftr = Order document;
! fktBest = P.O. document;
!*****************************************************************;
! CAUTION: Please change the Supplier no to your value for Dorma **;
!*****************************************************************;
! Supplier no for Dorma;
IF fktBest.m_nAH_IDENT = 7003;
    ! Set flag for direct delivery in P.O.;
    Set fktBest.m_nAH_LIEFER_KZ = 1;
    ! transfer main adress from order to purchase order;
    Set fktBest.m_sAL_KOPF = fktAuftr.m_sAH_KOPF;
    Set fktBest.m_sAL_NAME1 = fktAuftr.m_sAH_NAME1;
    Set fktBest.m_sAL_NAME2 = fktAuftr.m_sAH_NAME2;
    Set fktBest.m_sAL_NAME3 = fktAuftr.m_sAH_NAME3;
    Set fktBest.m_sAL_STRASSE = fktAuftr.m_sAH_STRASSE;
    Set fktBest.m_sAL_PLZ = fktAuftr.m_sAH_PLZ;
    Set fktBest.m_sAL_ORT = fktAuftr.m_sAH_ORT;
    Set fktBest.m_sAL_LAND = fktAuftr.m_sAH_LAND;
    Set fktBest.m_sAL_PROVINZ = fktAuftr.m_sAH_PROVINZ;
    Set fktBest.m_sAL_TELEFON = fktAuftr.m_sAH_TELEFON;
    Set fktBest.m_sAL_FAX = fktAuftr.m_sAH_FAX;
    Set fktBest.m_sAL_ANREDE = fktAuftr.m_sAH_ANREDE;
    Set fktBest.m_sAL_PARTNER = fktAuftr.m_sAH_PARTNER;
    !;
    ! Order delivery adress has priority;
    IF SalStrLength( fktAuftr.m_sAL_NAME1 || fktAuftr.m_sAL_NAME2 || fktAuftr.m_sAL_NAME3 || fktAuftr.m_sAL_STRASSE || fktAuftr.m_sAL_ORT );
        ! Lieferanschrift uebernehmen;
        Set fktBest.m_nAL_IDENT = fktBest.m_nAH_IDENT;
        Set fktBest.m_sAL_KOPF = fktAuftr.m_sAL_KOPF;
        Set fktBest.m_sAL_NAME1 = fktAuftr.m_sAL_NAME1;
        Set fktBest.m_sAL_NAME2 = fktAuftr.m_sAL_NAME2;
        Set fktBest.m_sAL_NAME3 = fktAuftr.m_sAL_NAME3;
        Set fktBest.m_sAL_STRASSE = fktAuftr.m_sAL_STRASSE;
        Set fktBest.m_sAL_PLZ = fktAuftr.m_sAL_PLZ;
        Set fktBest.m_sAL_ORT = fktAuftr.m_sAL_ORT;
        Set fktBest.m_sAL_LAND = fktAuftr.m_sAL_LAND;
        Set fktBest.m_sAL_PROVINZ = fktAuftr.m_sAL_PROVINZ;
        Set fktBest.m_sAL_TELEFON = fktAuftr.m_sAL_TELEFON;
        Set fktBest.m_sAL_FAX = fktAuftr.m_sAL_FAX;
        Set fktBest.m_sAL_ANREDE = fktAuftr.m_sAL_ANREDE;
        Set fktBest.m_sAL_PARTNER = fktAuftr.m_sAL_PARTNER;
    ENDIF;
ENDIF;
```

### BOM printing

BOM printing is controlled by the array `w_nRepBOM_ID[*]`. It includes the BOM IDs which are printed in the corresponding position. The BOM ID allows to access the BOM element using the function `udf_SearchBOMbyID()`.

```
!*****************************************************************;
!** Adding the cost price/PU on BOM items to the form printing **;
!** Create new variables UDV_BOM_COST_PUxx (xx = 0 to maxBOM items) **;
!** Assign this formula to the detail event of the form **;
!*****************************************************************;
!** Used Variables;
!** g_nUdv[0] => Fetch variable;
!** g_nUdv[1] => Index of BOM item;
!*****************************************************************;
! Loop for maximum of 20 printed BOM items;
Set g_nUdv[0] = 0;
WHILE g_nUdv[0] < 20;
    ! by default BOM isn't printed;
    SalReportSetNumberVar ( hWndReport, 'UDV_BOM_COST_PU'||SalNumberToStrX( g_nUdv[0], 0 ), NUMBER_Null );
    ! BOM is printed;
    IF w_nRepBOM_ID[g_nUdv[0]] != NUMBER_Null;
        IF w_fktDoc.m_Pos[w_nRepPosZaehler].udf_SearchBOMbyID ( w_nRepBOM_ID[g_nUdv[0]], g_nUdv[1] );
            ! Adding cost price per price unit to the form;
            SalReportSetNumberVar ( hWndReport, 'UDV_BOM_COST_PU'||SalNumberToStrX( g_nUdv[0], 0 ), w_fktDoc.m_Pos[w_nRepPosZaehler].m_PosStukl[g_nUdv[1]].m_nEK_PREIS_ME );
        ENDIF;
    ENDIF;
    SET g_nUdv[0] = g_nUdv[0] + 1;
```

### Amending the proceeds account record for transfer to financial accounting

A customer requires a different format for the proceeds account record. The standard is five-digit customer numbers while the customer uses eight-digit numbers.

One needs to enter a formula describing the proceeds account record in the new format; this formula has to be allocated to item 302 – FinAcc transfer (proceeds account record) in Customising.

```
!******************************************************************;
! Interface desciption for the sales account record of the standard DATEV interface **;
! with increased field lengths for invoice number and customer account **.
!******************************************************************;
!
! Field Start Length Description;
! 1 01 1 Leading "-" if orders are exported, otherwise the record starts with field 2;
! 2 02 10 Gross amount;
! 3 12 7 Sales account;
! 4 19 7 Invoice number;
! 5 26 6 not needed;
! 6 32 2 Day of the invoice date;
! 7 34 2 Month of the invoice date;
! 8 36 8 Customer account;
! Used functions;

! Adjust_NrToStr (value, fieldLength, digits);
! Converts the number in value into a string with the desired number of digits.;
! The string is filled with leading Zeros until the desired field length is reached;

! Adjust_NrToStrB (value, fieldLength, digits);
! Converts the number in value into a string with the desired number of digits.;
! The string is filled with leading blanks until the desired field length is reached;

! Adjust_String (value, fieldLength);Adjust_String (value, fieldLength);
! Adds trailing blanks until the string in value gets the desired field length;

!******************************************************************;
! Initialize the result value;
SET sResult = '';
! If orders are exported the record requires a leading '-';
If w_nDocType = nMODE_AUFTRAG;
    SET sResult = '-';
EndIf;
! Adding gross amount to the record;
SET sResult = sResult || Adjust_NrToStr(w_nGrossAmount * 100, 10, 0);
! Adding the sales account to the record;
SET sResult = sResult || Adjust_NrToStrB( SalStrToNumber(w_sSalesAccount), 7, 0 );
! Adding the invoice number to the record;
SET sResult = sResult || Adjust_NrToStrB(w_nInvoiceNo, 7, 0 );
! Adding an field with 000000 to the record;
SET sResult = sResult || Adjust_String( '000000', 6 );
! Adding day of the invoice date to the record;
SET sResult = sResult || Adjust_NrToStr( SalDateDay (w_dInvoiceDate), 2, 0 );
! Adding month of the invoice date to the record;
SET sResult = sResult || Adjust_NrToStr( SalDateMonth (w_dInvoiceDate), 2, 0 );
! Adding the customer account number to the record;
SET sResult = sResult || Adjust_NrToStr(w_nCustomerAccount, 8, 0);
```

The formula creates text consisting of the required fields in the desired format, and allocates it to the variable sResult.

sResult is analysed by transfer to financial accounting, and is then transferred to the financial accounting file.

### Transfer to financial accounting - transfer of customer master data

This formula creates a record from the necessary fields of customer master data (customer number, street, post code, name, ...). The fields of this record have no fixed length and are separated by semicolons.
**Formula - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\Financ DATEV CustomerExport.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - print job after scheduling in Capacity Planning

This formula selects all orders of status 38 (schedule in time management) and adds in the user's calendar a task for printing, faxing, and emailing. The orders are moved to a number manager, and the date list is updated.
**Formula - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\Workflow AddPrintTask.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - check orders for purchased elements

This formula checks all orders of a certain status for purchased elements. If purchased elements are involved, the order will get a certain status; if there are no purchased elements, the order will get a different status.
**Formula see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow CheckForPurchaseParts.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - Release for production

This formula selects all order of the same status with an order confirmation print date of over two hours, and raises the status to 'release for production'.
**Formula - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow StatusUpdate ToReleaseForProduction.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - Production release in ALCIM

This formula selects all orders of the status, release for production', raises the status to,transfer to AWPool' and releases the orders for production by calling the PPS Webservice. The production status in BW_LOCK_KAPA is raised to ‘release for production'.
**Formula - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow ReleaseForProduction.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - Production transfer to Capacity Planning

This formula selects all orders within a status area and transfers them as an OrderXML document to ALCIM Capacity Planning. The type of the OrderXML documents is, planning'. Explicit release for production must be made separately. The production status in BW_LOCK_KAPA is raised to 'transfer'.
**Formula see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow TransferToCapacityPlanning.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - Production transfer and release for production

This formula selects all orders within a status area and transfers them as an OrderXML document to ALCIM. The type of the OrderXML documents is,order' so that the order is released for production at once. The production status in BW_LOCK_KAPA is raised to 'release for production'.
**Formula - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow TransferToProduction.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - updating the BW_LOCK_KAPA status for an order

This formula sets the order status in table BW_LOCK_KAPA. This status reflects the order's current state in ALCIM.

Valid entries are:

| Nummer (number) | Constant | Description |
| :--- | :--- | :--- |
| 0 | KAPA_NEW_ENTRY | New document or amended document |
| 1 | KAPA_TRANSFERRED | Transfer to ALCIM complete |
| 2 | KAPA_IMPORTED | Document imported into ALCIM without error |
| 5 | KAPA_IMPORT_ERROR | Document imported into ALCIM with error |
| 10 | KAPA_READY_FOR_RELEASE | Document can be released for production |
| 11 | KAPA_RELEASE_SEND | Release to ALCIM complete |
| 12 | KAPA_RELEASE_FOR_PRODUCTION | Document has been released for production |

**Formula see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow UpdateKapaLock.txt`
Or in the local ALFAK installation directory 'formula'.

### Workflow - reducing the order status after a scheduling error in ALCIM Capacity Planning

This formula reduces the order status if an error has occurred during scheduling in ALCIM Capcity Planning so that the order status was reduced to the user status of status point 39 „Scheduling error".
**Formula - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Workflow StatusUpdateAfterPlanningError.txt`
Or in the local ALFAK installation directory ‘formula'.

### Interfaces - goFX - transfer of order data of EDI documents to XML file

This formula exports all entries in table FS_TRANSFER as an XML file to the goFX interface of glas online. The entries in FS_TRANSFER are made by triggers monitoring the status and delivery date changes, and the deletion of EDI orders.
**Formula see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\ Interface goFX FileOutput.txt`
**Trigger - see** `\\jupiter\ALFAK Install\Versions\4.4.xxx\Formula\Interface goFX Trigger SqlBase.sql`
Or in the local ALFAK installation directory 'formula'.

To use this function, install the triggers and enter the formula as a work-flow task in the AIS, then adapt the status mapping of the ALFAK status to the goFX status customised in formula `Interface_goFX_FileOutput.txt`.

**Example for status mapping:**

```
! Set the status of the order in the output file;
IF g_nUdv[2] < 400;
    Set g_sUdv[6] = 'imported';
ENDIF;

IF g_nUdv[2] >= 400 AND g_nUdv[2] < 540;
    Set g_sUdv[6] = 'processing';
ENDIF;

IF g_nUdv[2] >= 540 AND g_nUdv[2] < 590;
    Set g_sUdv[6] = 'packed';
ENDIF;

IF g_nUdv[2] >= 590;
    Set g_sUdv[6] = 'delivered';
ENDIF;

IF g_nUdv[2] = 852;
    Set g_sUdv[6] = 'revoked';
ENDIF;
```
In this example, all EDI orders with a status below 400 will be set to goFX status, imported', all EDI orders of status 400 to 539 to,processing', all EDI orders of status 540 to 589 to,packed', and all EDI orders of status 590 and above to,delivered'. ALFAK status 852 is mapped to goFx status,revoked'.

### Credit limit snapshots

The credit limit snapshot allows to analyse the development of certain financial data for a customer within a defined period.

The system will analyze the credit limit 1, credit limit 2, receivables, liability, balance 1, balance 2, and the 4 orders on hand.

The orders on hand are
1.  Undelivered orders
2.  Orders shipped but not yet invoiced
3.  invoiced orders which have not been transferred to financial accounting
4.  Totals of 1-3

Credit limit snapshots can be viewed and printed in dialog Master data - Customer – Credit limit analysis and directly at customer management, tab Balance.

Snapshots are created by a daily workflow task run by the ALFAK Interface Service, which analyses the financial data.

For details on workflow tasks in AIS, see chapter Workflow in this document.

**Installation:**
First, define a formula in formula management for creating the financial snapshots (Master data > Company > Formulas). An example formula can be found in the formula directory of the ALFAK installation „Workflow_TransferCreditLimit.txt".

*Fig. 220: Finance snapshot formula*

This formula is allocated to a workflow task in customizing management (Master data > Company > Customizing > tab Workflow Tasks)

*Fig. 221: Finance snapshot Workflow*

on tab Automatic process execution, data for the ALFAK Interface Service are added.

*Fig. 222: Finance snapshot activation*

If the VB script is loaded several times a day, the snapshots of the corresponding day will be deleted before a new one is created.

### Printout of documents via the reporting service via workflow task

The following example selects all documents of the main database whose status is in a specified range and inserts them into a new number manager. This number manager is then transferred to the reporting service with the function `udf_PrintNumberManager()` and sent there via mail.

The example is also found in the file `workflow_print_documents.txt` in the folder of the Exchange Service formulas (e.g. C:\Program Files (x86)\A+W\Business 6\Formula\ExchangeService).

The formula contains a section for assigning the variables that must be adjusted depending on application case. In the end, the formula is attached and activated as workflow formula.

```
! This formula is selecting all orders that are in between the defined stauts, put them into
! a new number manager and send that number manager to the reporting service for print an order
! confirmation;

! Used variables;
! g_nUdv [0] : Fetch result;
! g_nUdv [1] : Document no.;
! g_nUdv [2] : Number of documents to be printed;
! g_nUdv [3] : Document type (nMODE AUFTRAG, MODE BESTELLUNG, MODE GUTSCHRIFT,..);
! g_nUdv [4] : Form ID (see form management in basic data);
! g_nUdv [5] : Lower bound of the status for selectiong the documents;
! g_nUdv [6] : Upper bound of the status for selectiong the documents;
! g_bUdv [0] : Boolean for result of every function call;
! g_sqlUdv (0) : Sql Handle to the main database;
! g_sUdv [0] : Name of the number manager;
! g_sUdv [1) : Name of the user for the number manager;

! =============================================================================;
! Initialization section. Variables can be changed;
! =============================================================================;
! Name of the number manager;
Set g_sUdv [0] = 'Rep' || SalFmtFormatDateTime ( SalDateCurrent ( ), 'yyyyMMddhhhhmmss' );

! Username used for number manager and printing;
Set g_sUdv [1] = 'Administrator';

! Document type of the documents;
Set g_nUdv [3] = nMODE_AUFTRAG;

! Form ID, see form management to find the proper value. This has to be changed for every
! database;
Set g_nUdv [4] = 10049;

! Select documents with a status between the both following values g_nUdv [5] and g_nUdv [6];
Set g_nUdv [5] = 8;
Set g_nUdv [6] = 8;
! =============================================================================;
! End of Initialization section;
! =============================================================================;

! Database connection;
Set g_bUdv [0] = DbMakeTempConnect ( g_sqlUdv [0]);

! Selection of orders that should be printed by status ordered by entry date;
If g_bUdv[0];
    Set g_bUdv [0] = SqlPrepareAndExecute ( g_sqlUdv[0], DbParse ( 'SELECT ID FROM SYSADM.BW_AUFTR_KOPF WHERE STATUS BETWEEN : g_nUdv [5] AND : g_nUdv [6] INTO : g_nUdv [1] ORDER BY DATUM_ERF' ) );
EndIf;

! And put them into a new number manager;
Set g_nUdv [2] = 0;
If g_bUdv[0];
    While g_bUdv [0] AND SqlFetchNext ( g_sqlUdv [0], g_nUdv[0]);
        Set g_bUdv [0] = udf_AddDocumentToNumberManager ( g_sUdv[0], g_sUdv [1], g_nUdv [1], MODE_AUFTRAG );
        Set g_nUdv [2] = g_nUdv [2] + 1;
    Wend;
EndIf;

! Now send the numbermanager to the reporting service for printout the order confirmation;
! Parameters are:;
! - name of number manager;
! - name of user for that number manager;
! - document type;
! - ID of the form that should be used (see form management dialog);
! - output type (0=printer, 1=mail);
! - output device (name of printer or empty if using mail);
! - archive year (empty if main DB);
! - number range mode (0=preset of client and order area, 1=order area and client from document, 2=client from document and preset of order area);
! - client ID;
! - order area;
! - date (if empty, current date is used);
! - label mode (0=per unit, 1=per line item, 2=per order, 3=use setting from document);
! - number of copies;
! - collective printout flag (TRUE=yes, FALSE=no);

If g_bUdv [0] AND g_nUdv [2] > 0;
    Set g_bUdv [0] = udf_PrintNumberManager ( g_sUdv [0], g_sUdv [1], g_nUdv [3], g_nUdv [4], 1, '', '', 1, 1, '', DATETIME _Null, 0, 1, FALSE);
EndIf;

! Send a short message to the workflow monitor;
If g_bUdv [0] AND g_nUdv [2] > 0;
    COMMessageBox ( 0, 'Numbermanager ' || g_sUdv [0] || ' successfully transferred for printout.', 'Exchange service', MB_Ok | MB_IconInformation, IDOK );
EndIf;

If g_bUdv [0] = FALSE;
    COMMessageBoxError ( 0, 'Error transferring numbermanager ' || g_sUdv [0] || ' for printout. See trace for more info.', MB_Ok, IDOK );
EndIf;

! Disconnect database handle;
If g_sqlUdv[0];
    DbDisconnect ( g_sqlUdv [0] );
EndIf;
```

### Transfer of OrderXMLs via the import service via workflow task (fileless)

The following example deletes all OrderXMLs that are older than the number of storage days. After that, all OrderXMLs that were not flawed were sent to production by the import service. The function `udf_TransferOrderXmlToProduction()` specifies with the `g_sUdv[0]` parameter a string with information messages that are then traced. The string can also be sent to an e-mail sending udf function.

The example is also found in the file `workflow_transferorderxmltoproduction.txt` in the folder of the formulas (e.g. C:\Program Files (x86)\A+W\Business 6\Formula\).

For start-up, the formula must be attached as workflow formula and activated.

```
! *************************************************************************;
! ** Transfer all ready OrderXMLs to production. **;
! ** Delete the OrderXMLs that are older than the retention time beforehand. **;
! *************************************************************************;
! Used Variables;
! g_sUdv [0] = Transfer messages;
! Used functions;
! udf_CleanUpOrderXmlTable();
! Cleans up the BW ORDERXML Table by removing OrderXMLs that are older than the retention time;
! udf_TransferOrderXmlToProduction (Boolean, Receive String);
! Transfers all Ready OrderXMLs to Production;
! Parameters: udf_TransferOrderXmlToProduction ( Retry failed OrderXMLs, Transfer messages );
! Example: udf_TransferOrderXmlToProduction ( FALSE, g_sUdv [0]);
! If the tranfer to production (without retrying failed OrderXMLS ) was successful variable
! g_sUdv [0] holds the Info messages, otherwhise variable g_sUdv (0) holds the Error messages;
! *************************************************************************;
! Clean up OrderXMLS;
udf_CleanUpOrderXmlTable();

! Transfer OrderXMLs to Production (AWP);
IF udf_TransferOrderXmlToProduction (FALSE, g_sUdv [0]);
    TRACE ('Tranfer to Production Informations: ' || g_sUdv [0], EVENT_INFORMATION, TRACE_CUSTOMIZING);
ENDIF;
```

### Transfer of the breaks from the Logistic Service via workflow task

The following example collects all breakage reports from the Commercial Logistic Service that have not yet been sent to A+W Business 6. After that, all breakage reports that were not incorrect are created as complaints. The function `udf_RetreiveBreakages()` specifies with the `g_lsUdv[0]` parameter a string with information messages that are then traced. The string can also be sent to an e-mail sending udf function.

The example is also found in the file `workflow_check_logistics_breakages.txt` in the folder of the formulas (e.g. C:\Program Files (x86)\A+W\Business 6\Formula\).

For start-up, the formula must be attached as workflow formula and activated.

```
! *****************************************************************;
! ** Retrieve all breakages from Logistic Service ********************;
! *****************************************************************;
! Used Variables;
! g_bUdv [0] = Return value from udf_RetreiveBreakages;
! g_sUdv [3] = Message for result mail;
! g_lsUdv [0] = Receive parameter for all messages that the export creates;
! *****************************************************************;
! Start of the transfer process;
! *****************************************************************;
Set g_lsUdv [0] = '';
Set g_bUdv [0] = udf_RetreiveBreakages (g_lsUdv[0]);
If g_bUdv[0];
    Set g_sUdv [3] = 'Retrieved all breakages from Logistic Service';
EndIf;
If NOT g_bUdv[0];
    Set g_sUdv [3] = 'Breakage retrieve from Logistic Service failed';
EndIf;

! Put the result into a TRACE file if configured.;
TRACE (g_sUdv [3], EVENT_INFORMATION, TRACE_CUSTOMIZING );
TRACE (g_lsUdv [0], EVENT_INFORMATION, TRACE_CUSTOMIZING );
! Send the result of the transfer process via mail;
! udf_SendMail ( '<MAILSERVER>', '<AUTH_USER>', '<AUTH_PASS>','<FROM>', '<TO>', '<CC>', g_sUdv [3], g_lsUdv[0], "" );
```

## 10.30. User-defined column in number manager

### Simple allocation

In the screen table of the number manager, there is a column "csCustomeText" in which you can fill any data via customizing. It is a column of the type "string" and behaves accordingly for the sorting with a double-click on the column header. To assign this column to data, it is necessary to create a customizing formula with an appropriate assignment and to assign this formula to the "Load data record" element via the context menu of the table.

```
Set g_sUdv[0] = 'Hello world';
Set tbl_NV.csCustomText = g_sUdv[0];
```
Thus, the text "Hello world" appears in the "csCustomText" column of the number manager.

### Assignment of data from database

If, however, the desired data has to be procured via SQL statement from the database, this method alone does not perform well enough. It is possible to extend the actual statement that uses the number manager for filling with individual columns. Thus it is not necessary with each loading of a data record to make a connection to the database. There are two string variables for this: `"tbl_NV.w_sSubSelect"` and `"tbl_NV.w_sSubInto."` These should be populated via customizing formula when generating the number manager with the SELECT columns and the Into variables. The number manager uses these columns to select as soon as they are filled. It must be noted that the columns used, insofar as they come from the document header, should be named with the alias "B."

Here is an example for the reading of the net amount:

```
Set tbl_NV.w_sSubSelect = ', B.FI_BETR_NETTO';
Set tbl_NV.w_sSubInto = ', :g_sUdv[0]';
SalTblSetColumnTitle ( tbl_NV.csCustomText, 'Netto Betrag' );
```

This formula has to be assigned to the Customizing - Event "Set window" of the number manager.

After that, only the formula from 10.30.1 has to be assigned the table even "data record loaded." And as even, you thus have the net amount of the order in the "csCustomText" column of the number manager.

### Assignment of data from database with Sub-SELECT

Another possibility is to select data from another table and link it to the data from the current document. Thus, for example, it is possible to select data that is not included in the document from the customer master data after the fact.
In the following two formulas, the credit limit is selected from the customer master data after the fact with 2 places after the decimal point:

```
Set tbl_NV.w_sSubSelect = ', cast ((SELECT KREDIT_LIMIT1 FROM SYSADM.KU_KUNDEN WHERE ID = B.AH_IDENT) as decimal (30,2))';
Set tbl_NV.w_sSubInto = ', :g_sUdv[0]';
SalTblSetColumnTitle ( tbl_NV.csCustomText, 'Kreditlimit' );
```

The formula for the table event "data record loaded" can thus remain unchanged:

```
Set tbl_NV.csCustomText = g_sUdv[0];
```

## 10.31. Creating a product description from BOM

With the customizing expansion point 30, it is possible to attach a formula that creates the product designation according to your own rules.

Here, the function `udf_ProdDescByBOMNode( nBOM_ID, sDelimiter, bShortDescription)` creates the product description from the BOM; it can be determined whether the description should be taken from the short descriptions and how the separator should be set.
The formula `"..\Formula\description_IG+LamiDesc2byShortDescription.txt"` creates a sample implementation; here the BOM is composed in the product description 2 and the separator is a "/". The short description is used and not the BOM description. The formula runs in the context of the item class; access to the header structures is not possible.

## 10.32. ITOE rules

The iTOE rule editor allows you to store a formula as condition. The condition is TRUE if this formula sets the variable bReturn = TRUE.

Access to the order is gained via `fktDoc`, so the customer number can be queried via `fktDoc.m_nAH_IDENT`.

The current item can be accessed via `fktPos`.

The processings are not yet created; that's why no access to them is possible.

In order to access the processing found from iTOE/DXF, the object `fktSNBearb` must be used that belongs to the class `cfktSNProcessing`.

### cfktSNProcessing

**Description:** Class with all properties of a processing from SN

**Instance Variables**
*   `Number: m_nAWID` ! The AW-ID of the processing
*   `Number: m_nSN_BEA_PARAM[30]` ! The SN processing parameters
*   `String: m_sCornerVector` ! The corner vector
*   `String: m_sEdgeVector` ! The edge vector
*   `String: m_sLayerNumber` ! The layer
*   `Number: m_nLevel` ! The level
*   `Number: m_nMeasureType` ! The measurement type
*   `Number: m_nInnerReferenceCorner` ! The reference corner for interior cut-outs
*   `Number: m_nRotationReferenceEdge` ! The angle of rotation
*   `Number: m_nEdgeQuality` ! Edge quality from AWB !!!
*   `String: m_sMacroName` ! Macro name
*   `Number: m_nProcessingMode` !

**Function: udf_GetParamText**
*   Description: Get all parameter from CAD.
*   Returns String: Returns Parameter String

The A+W processing type dialog defines the AWID and which parameters are transferred. These are in the array `m_nSN_BEA_PARAM`.

To output the parameters during the formula development, you can use the function: `fktSNBearb.udf_GetParamText()`

It returns all parameter values as string.

Sample formulas are found in Formula/iTOE

# 11. Workflow

## 11.1. Introduction

The workflow is used for the mainly automatic processing of orders, from input up to production release in ALCIM. All following steps (receipt of goods, printing of shipping notes, transfer to financial accounting, ...) will still be performed by hand, by the user.
The work-flow application tool is the ALFAK Interface Service (AIS) which can run the individual tasks either periodically (e.g. production transfer) or at a fixed time (e.g. transfer to statistics).

You have to assign to the tasks the property cyclic or fixed time in Customizing management, tab Automatic process execution. Process execution with the property cyclic or fixed time.

*   In customzing management, periodical work-flow tasks (e.g. report tasks) are now entered and displayed acc. to the 00:00 pattern, but with execution type "00-cyclic".
*   Example: the cyclic execution time of 00:30 defines that the work-flow task is run every 30 minutes
*   Example: the cyclic execution time of 02:00 defines that the work-flow task is run every 2 hours

The tasks to be performed by AIS can be defined individually in the workflow management of ALFAK Customizing, depending on the company's processes.

After all, every workflow task consists of several customizing formulas which gives the engineer a maximum of freedom when defining the workflows.

The following examples refer to the a initial installation at SOTRAVER, France.

The following graphs shall illustrate the order processing procedure.

## 11.2. Schematic display

*(This section contains a flowchart illustrating the workflow procedure up to the release of production.)*

*Fig. 223: Workflow - Procedure up to the release of production*
*(This section contains a flowchart illustrating the workflow procedure after release for production.)*

*Fig. 224: Workflow - Procedure after release for production*

First you need to analyse which tasks can be automatically performed via workflow. For every task, a workflow task has to be defined which again is based on a customising formula. The customizing reference in this document describes how formulas should be defined and programmed.

## 11.3. Transfer to ALCIM Capacity Planning

Newly entered orders are transferred by means of the first task Workflow Task Transfer To Capacity Planning to ALCIM Capacity Planning. These orders are planned, but not scheduled as jobs; no rough or detailed planning is made. After transfer, orders will get the user status of status point 980 Transfer to Capacity Planning.

## 11.4. Report status from ALCIM Capacity Planning

As a planning result, ALCIM Capacity Planning sets the status of the planned orders to the user status of status point 38 Scheduled in TM or, in case of an error, to 39 Error during automatic scheduling.

## 11.5. Printout after ALCIM Capacity Planning

After successful scheduling in ALCIM Capacity Planning, order can be printed, emailed, and/or faxed. The task Workflow Task After Scheduling adds a print job to the user's diary. Additionally, the order can be assigned to a certain number manager.

If the user double-clicks on a printjob while in module Documents, the print module will be directly started on the number manager defined in the formula.

## 11.6. Status reduction due to an error in ALCIM Capacity Planning

Scheduling errors may necessitate a reduction of the order status so that the following processes can be performed without manual status changes (e.g. order is set to status 39 after a scheduling error while the lock status for order confirmation printing is 21).

The task Workflow Task Update Status After Planning Error resets the status of the orders where a scheduling error occurred to the status required by the user.

→ Orders will get the user status of the required status point

## 11.7. Check for ordered elements

When the order confirmation has been printed, the Task Workflow Task Transfer To Capacity Planning checks all orders with status Print OC for ordered elements and assigns a new status.

The new status can be configured freely.
→ Orders with ordered elements e.g. get the user status of status point 1029 Order includes ordered elements.
→ Orders without ordered elements e.g. get the user status of status point 35 Release for production.

## 11.8. Release for production in ALFAK

So far, orders have been scheduled but not released for production yet. If the customer does raise an objection within two hours after printing the order confirmation, it can be assumed that production can be started. The condition for this release is not fixed but can be amended by means of the formula on which the task is based.

The task Workflow Task Update Status to Release for Production sets the status of the orders of status Print OC which have been printed more than two hours ago, to the user status of status point 35 Release for production.

→ Orders will get the user status of status point 35

## 11.9. Release for production in ALCIM

When the order has got the status 'Released for production', it can be released for production in ALCIM. The task Workflow Task Release for Production in ALCIM sets the status of the orders of status Release for production to the user status of status point 40 Transfer to AWPool. The reason is that a standard release for production contains an implicit release for production, and the order meets this status after the usual transfer. Moreover, the PPS web service is contacted; ALCIM is informed that the order can be produced.

→ Orders will get the user status of status point 40

## 11.10. Management

**Formulas**

All necessary formulas (9000–9006) are managed by module Formulas in ALFAK master data.

*Fig. 225: Administration - Formula example*

All formulas and settings for the workflow are saved in the databases DEMO44 and ALF on the database server SPEEDY.

Additionally, all formulaas are part of an ALFAK installation (as text files) in sub-directory Formula or are available in `\\Jupiter\ALFAK Install\Versions\4.4.xxx\Formula`.

## 11.11. Workflow Tasks

Formulas are allocated to tasks. A task is a process step that can be periodically run by AIS.

*Fig. 226: Workflow tasks - Example*

**Automatic setting of tasks**

All tasks get settings regarding their sequence and cycle time. The sequence defines the sequence in which AIS performs these tasks. The cycle time defines the interval – in minutes – in which the task will be performed.

*Fig. 227: Workflow Tasks - Automatic setting*

## 11.12. Report from ALCIM Capacity Planning

ALCIM Capacity Planning returns the following information to ALFAK:
1.  Time costs
2.  Production date on item and BOM level

Based on the production date, ALFAK checks if all stock articles required for this order are available and, if not, whether they can be ordered and delivered on time.

A shortage on stock results in a task for the user (→ postponement of shipping date).

The production dates determined by ALCIM Capacity Planning are adopted in the order for items and BOM.

The actions to be performed during the ALCIM Capacity Planning report can be individually defined in CommonBase.

*Fig. 228: User-defined CommonBase settings*

## 11.13. Change of order after release for production

An order can be changed even after it has been released for production, by means of menu „Functions → Change locked item“. If in order entry the delivery data is moved to the past, the system attempts to cancel it in the production system.

The PPS web service is contacted; the system tries to cancel the order to be produced (orders can be cancelled in ALCIM until the job has been created).

If cancellation has been successful, the order can be changed.

If the order could not be cancelled, the user will be asked whether he still wants to change the order.

Changing the locked item will set the order status to the user status of status point 810 Transfer to AWPool cancelled.

The changed order now goes through the cycle again, starting from the transfer to ALCIM Capacity Planning.

*Fig. 229: Change the blocked position*

*(This section contains a flowchart clarifying the order status during production transfer and cancellation.)*

## 11.14. Automatic transfer to production

In connection with the workflow, automatic transfer to production via AIS is unnecessary because this is done by a workflow task.

## 11.15. Notifying the Service Monitor

With every formula - these are the core of every Workflow task – a notification can be sent to the Service Monitor to visualise to the user the actions of the workflow and possibly occurring errors. The function `udf_EventToServiceMonitor` can be used for this in the formulas.

## 11.16. EDI orders

For EDI orders, order confirmations do not have to be printed. This is why EDI orders can be exempted from selection for the print job.

## 11.17. Notification at order entry

As soon as new tasks - created by a report from ALCIM Capacity Planning - are added to the user's task list, the message 'You have got new messages' will appear in the status bar at order entry/print program.

*Fig. 230: Order entry, tab Totals*
