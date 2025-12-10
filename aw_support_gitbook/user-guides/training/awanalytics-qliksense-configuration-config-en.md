---
title: "A+W Configuration: A+W Analytics powered by QLIK Sense"
category: "training"
product: "AWAnalytics"
doc_type: "Configuration"
language: "EN"
tags: ["AWAnalytics", "QlikSense", "Configuration", "Config"]
version: "1.0"
last_updated: "2025-12-10"
description: "title: "EN-CONFIG-AW_Analytics" source: "EN-CONFIG-AW_Analytics.pdf" tags: ["A+W Analytics", "Qlik Sense", "Configuration", "Implementation", "Data Loading", "Software for Glass", "ERP", "PPS", "Data Architecture", "Customizing"] version: "1.0" last_updated: "2025-10-03" short_description: "This document is an internal configuration guide for A+W Analytics, a business intelligence solution powered by Qlik Sense. It details the steps for implementation, customization, data loading architecture, a"
source_file: "AWAnalytics-QlikSense-Configuration-Config-EN.md"
---


title: "EN-CONFIG-AW_Analytics"
source: "EN-CONFIG-AW_Analytics.pdf"
tags: ["A+W Analytics", "Qlik Sense", "Configuration", "Implementation", "Data Loading", "Software for Glass", "ERP", "PPS", "Data Architecture", "Customizing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is an internal configuration guide for A+W Analytics, a business intelligence solution powered by Qlik Sense. It details the steps for implementation, customization, data loading architecture, and usage of various analytical applications (APPs) designed for the glass industry."
long_description: "This is a comprehensive internal guide for configuring and implementing A+W Analytics, which leverages the Qlik Sense platform to provide powerful data analysis for the glass manufacturing industry. The document serves as a technical manual for A+W project teams and customers' IT departments. It begins with a detailed implementation checklist, covering server setup, port configuration, licensing, and user management. It then explains how to configure the core `CU_CONFIG.XLSX` file, which manages client lists, database connections, languages, and specific A+W parameters. The guide outlines the multi-layered data loading architecture, which includes extract, union, and compaction layers, explaining how data is collected from A+W databases (like A+W Business, Production, and Cantor), processed into QVD files, and prepared for visualization. It also covers customizing the solution, such as extending the data model and using Qlik Sense extensions. Finally, the document provides an overview of the various standard analytical applications (APPs) available, including those for turnover, customer receivables, stock forecasting, delivery reliability, and production statistics, explaining their purpose and requirements."
---

# A+W Configuration: A+W Analytics powered by QLIK Sense

**- INTERNAL -**

*A+W - Software for Glass*

---

## Change history

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2018-04-06 | DLA | Original version | 1.0 |
| 2019-05-21 | DLA | AWP O4P Performance APP | 1.1 |

---

## Content

1.  **Implementation**
    1.1. Checklist of implementation
    1.2. Configure CU_CONFIG.XLSX
        1.2.1. CLIENT_LIST
        1.2.2. DATABASE_LIST
        1.2.3. LANGUAGE
        1.2.4. QLIK_PARAMETER
        1.2.5. A+W Analytics parameter
        1.2.6. CUSTOMER_GEO_LIST (optional)
2.  **Customizing**
    2.1. QLIK Sense® Extensions
        2.1.1. InputVariable
        2.1.2. Automated Task Failure Email Alerts
        2.1.3. Simple KPI Box
    2.2. Extend data model by customizing
3.  **Data loading architecture**
    3.1. Extract layer
        3.1.1. Data collection
        3.1.2. Data union
        3.1.3. AW_TABLES_*.XLSX
    3.2. Compaction layer
        3.2.1. Multilingualism
    3.3. Presentation layer
        3.3.1. Tools
        3.3.2. Title bar
4.  **APPs**
    4.1. Common APPs
        4.1.1. AW Load Data Clarity
        4.1.2. AW Load Data Cantor
        4.1.3. AW Documentation
    4.2. A+W Business APPS
        4.2.1. Turnover APPS
        4.2.2. Customer receivables, credit limit, budget
        4.2.3. Stock forecast
        4.2.4. Delivery reliability
    4.3. A+W Production APPs
        4.3.1. AWP breakage statistics
        4.3.2. AWP waste statistics
        4.3.3. AWP production statistics
        4.3.4. AWP work in process
        4.3.5. AWP production workload
        4.3.6. AWP charge overview
        4.3.7. AWP O4P Performance

---

## 1. Implementation

For the implementation of A+W Analytics a SETUP does not exist. The steps need to be done manually on an installed QLIK Sense® Server.

### 1.1. Checklist of implementation

1.  **QLIK Sense®**
    - Install and configure QLIK Sense® Server if customer has bought an OEM version from A+W. If not, server has to be prepared by customer.
    - The installation must be on a dedicated INTEL (not AMD, this will be slow) server. It can be a virtual machine. The system requirements are on QLIK homepage: [http://www.qlik.com/us/products/qlik-sense/system-requirements](http://www.qlik.com/us/products/qlik-sense/system-requirements)
    - A Windows QLIK user for the QLIK Services is necessary. This user can be used for the QLIK root administrator.
    - **During the installation the QLIK repository database super user Password is set. This password must be remembered! Without this, no updates are possible.**

2.  **Ports**
    - It is necessary to release several ports in firewall to make QLIK Sense working. A port overview can be found on QLIK homepage, here a link for QLIK Sense 3.2: [http://help.qlik.com/en-US/sense/3.2/Subsystems/PlanningQlikSenseDeployments/Content/Server/Server-Deployment-Ports.htm](http://help.qlik.com/en-US/sense/3.2/Subsystems/PlanningQlikSenseDeployments/Content/Server/Server-Deployment-Ports.htm)

3.  **Configure license**
    - Start the QMC and configure the license you got from QLIK, license key with control number. If the server is not connected to the internet, you can get the license information over the following link. Enter license key and copy the license set into your QLIK Sense server: [http://lef1.qliktech.com/manuallef](http://lef1.qliktech.com/manuallef)

4.  **Assign token for QLIK root administrator**
    - Assign one token to you QLIK windows user and configure this user as QLIK root administrator.

5.  **User, streams and security**
    - Check with the customer which Windows users shall assign to QLIK Sense, which QLIK Sense streams they need and which users have which rights in QLIK environment.
    - You can assign Windows user a token if the user is in the QLIK user list. The user appears in the QLIK user list if they try to login, or you must create a task to synchronize QLIK Sense with your active directory to get all users in the QLIK user list.
    - The following streams are recommended, if customer has no other ideas:
      - Load data, A+W Business, A+W Production, A+W Cantor

6.  **Install A+W Analytics and ODBC Driver diskset**
    - Use the A+W SetupLauncher to install A+W Analytics diskset and the needed ODBC Driver disksets on the central QLIK Sense® Server.
    - The SetupLauncher asks for a destination folder. In this folder a subfolder `QLIKDATA` is generated. This subfolder has to be integrated in customer's data backup concept.
    - In `QLIKDATA` folder the following subfolder exist:
        - **Subfolder APPS**: Backup of the APPs from A+W Analytics package. The APPs are stored in a sub directory of their language.
        - **Subfolder EXCEL**: A+W Analytics excel files for configuration: `CU_CONFIG.XLSX`, `AW_TABLES_*.XLSX`, `AW_TEXT.XLSX`
        - **Subfolder SCRIPTS**: A+W Analytics script files for QLIK Sense®: `AW_*.QVS`
        - **Subfolder extensions**: Backup of all necessary QLIK Sense® extensions, below the one which are necessary for A+W Analytics. It is necessary to import the extensions into QLIK Sense®.
        - **Subfolder QVD**: The different QVD files are stored in subfolders under this folder. The folders are generated automatically during the first run of data loading architecture.
            - `1_Collection` - QVD files for data collection
            - `2_Union` - QVD files for data union
            - `3_Compaction\<language>` - QVD files for data compaction in the different languages
        - **Subfolder PNG**: `AW_*.PNG` files which must be imported into QLIK Sense® default content library

7.  **Data sources**
    - For A+W Analytics different data sources must be configured to give QLIK Sense® access to the data.
    - **3.1 ODBC data sources**: Create ODBC data sources to the different database server resp. databases. For INFORMIX and SQLServer you need one data source for each database server, for SQLBase one data source for each database (lock level `Release lock` for SQLBase, read only doesn't work).
    - **3.2 QLIK - ODBC data source**: In QLIK Sense create a data source for each ODBC data source. The name of this data sources must be configured in `CU_Config.xlsx`.
    - **3.3 QLIK - folder data source**: Create a folder data source in QLIK Sense® to the `QLIKDATA` folder from installation. The name of the data source must be `QLIKDATA`, if not some A+W Analytics functions don't work.

8.  **Configure CU_Config.xlsx**
    - Configure environment, client and databases for all integrated sites in the excel list.
    - **4.1 CLIENT_LIST**: Every site of the customer needs to configure one client for each ERP- and PPS-system combination.
    - **4.2 DATABASE_LIST**: Every A+W database which shall be integrated into A+W Analytics must be configured.
    - **4.3 LANGUAGE**: Set the supported languages which shall be used for the customer.
    - **4.4 QLIK_PARAMETER**: Set the list of parameters to the customer values.
    - **4.5 Optional setting**: Configure optional settings if needed like `CUSTOMER_GEO_LIST` or `USER_ACCESS`.

9.  **Import and configure objects in QLIK Sense®**
    - Objects from A+W Analytics package must be imported into QLIK Sense®.
    - **5.1 PNG files**: Import `QLIKDATA\PNG\*.PNG` into QLIK Sense® default content library.
    - **5.2 Extensions**: Import extensions from `QLIKDATA\Extensions` into QLIK Sense®.
    - **5.3 AW Load Data APP**: Import `QLIKDATA\APPS\AW Load Data <Version>.QVF`, test the APP and generate a reload task. The APP must be executed without errors and QVD files should be generated. If APP works, create a QLIK Sense® reload task to execute the APP every day. We recommend the night outside the maintenance tasks of databases and file systems. Publish this APP in the Stream "Load Data".
    - **5.4 Visualization APPS**: Import the necessary visualization APPs `QLIKDATA\APPS\<language>\*.QVF`, test the APPs and if they run without troubles, publish the APPs in the streams and generate a reload task based of successful execution of AW Load Data APP.
    - **5.5 AW Documentation APP**: Import and publish `QLIKDATA\APPS\AW Documentation <Version>.QVF`. Create a reload task once a day. This APP shows the actual configuration and the description of the compacted QVD files in the configured languages. Publish this APP in the stream for everyone.

10. **Backup**
    - Customers IT has to include the QLIK Sense® Server into their backup concept. Our `QLIKDATA` directory and the QLIK Sense® Data directory, `C:\ProgramData\QLIK\` if not configured otherwise, must be included in the backup concept.

### 1.2. Configure CU_CONFIG.XLSX

The excel file `EXCEL\CU_CONFIG.XLSX` contains the main configuration of the customers system and some data sheets with additional data to include in the analysis. This file has to be configured at the beginning of a project.

#### 1.2.1. CLIENT_LIST

The table sheet `CLIENT_LIST` contains a list of all clients of the customer. It is assumed that for each client a maximum of one A+W database per A+W product exists. In the compaction layer the content of this table sheet will be stored in QVD file `[AW Client List.QVD]`.

-   **AWCLIENT** - [KEY] The number of the client. This field is added to each QVD file `[%awclient]` to distinguish data from different databases. The number should be the real client number of the customer. This is important for visualization because some of our products doesn't know a client number (e.g. A+W Production).
-   **CLIENT_NAME** – Name of the Client, it is used in A+W Visualization APPs
-   **CLIENT_CITY** – [Optional] Client city
-   **CLIENT_COUNTRY** - [Optional] Client country
-   **LATITUDE** - [Optional] width of geographic coordinate system
-   **LONGITUDE** - [Optional] height of geographic coordinate system

**Example Table `CLIENT_LIST`:**

| AWCLIENT | CLIENT\_NAME | CLIENT\_CITY | CLIENT\_COUNTRY | LATITUDE | LONGITUDE |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | A+W Pohlheim | Pohlheim | Deutschland | 50,525 | 8,733333 |
| 2 | A+W Lyon | Lyon | Frankreich | 45,758889 | 4,841389 |
| 3 | A+W Chicago | Chicago | USA | 41,881944 | -87,627778 |
| 4 | A+W Halmstadt | Halmstadt | Germany | 56,666667 | 12,85 |
| 5 | A+W Toronto | Toronto | Kanada | 43,66135 | -79,383087 |
| 50 | A+W Frankfurt | Frankfurt | Deutschland | 50,110556 | 8,682222 |
| 51 | A+W London | London | England | 51,50939 | -0,11832 |
| 100 | A+W London | London | England | 51,50939 | -0,11832 |

#### 1.2.2. DATABASE_LIST

Every A+W database you want include, must be listed in the table sheet `DATABASE_LIST`.

-   **AWCLIENT** - [KEY] number of client defined in table sheet `CLIENT_LIST`
-   **DBSYSTEM** - [KEY] ID of database system:
    -   `AWB` - A+W Business
    -   `AWC` - A+W Cantor
    -   `AWCC` - A+W Cantor CIM
    -   `AWP` - A+W Production
    -   `AWE` - A+W Enterprise
-   **DBTYPE** - [KEY] database type, `MAIN` or `ARCHIVE` database. Some systems have no archive database
-   **DBNAME** - database name
-   **COLLECTION_DATA** - 1 = use database to unload raw data from database; 0 = don't use database (e.g. old archive where raw data QVD still exist)
-   **UNION_DATA** - 1 = linked raw data QVD files; 0 = don't link raw data QVD files
-   **DBOWNER** - DB owner of the database; maybe, this is necessary for SQLServer databases. If set, all tables which shall be unloaded need to have this DBOWNDER
-   **QLIK_DATASOURCE** - name of data source for this database configured in QLIK Sense®
-   **DBSYSTEMTYPE** – database system type: `INFORMIX`, `SQLSERVER`, `SQLBASE`
-   **DBVERSION** - [optional] Version of DB, if filled the value is compared with the value of TBVERSION and COLVERSION in the `AW_TABLES_*.XLSX`

**Example Table `DATABASE_LIST`:**

| AWCLIENT | DBSYSTEM | DBTYPE | DBNAME | COLLECTION DATA | UNION DATA | DBOWNER | QLIK DATASOURCE | DBSYSTEMTYPE | DBVERSION | DESCRIPTION |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | AWP | MAIN | alcimdb | 1 | 1 | alcimdb | AWP01_INF | INFORMIX | 6 | QM-AWEAWP6 |
| 2 | AWP | MAIN | alcimdb | 1 | 1 | dbo | AWP02_SQL | SQLSERVER | 6 | QM-AWBAWP60 |
| 2 | AWP | ARCHIVE | alcimqry2016 | 1 | 1 | dbo | AWP02_SQL | SQLSERVER | 6 | QM-AWBAWP60 |

#### 1.2.3. LANGUAGE

The table sheet `LANGUAGE` contains a list of possible languages and a flag whether the language is active or not. If a language is active, the compaction function generates compaction files for this language provided that the language is released in A+W Analytics.

**Example Table `LANGUAGE`:**

| LANGUAGE | ACTIVE |
| :--- | :--- |
| de-DE | 0 |
| en-US | 1 |

#### 1.2.4. QLIK_PARAMETER

The table sheet `QLIK_PARAMETER` contains a list of parameters which can used in QLIK Sense® APPs as variables. In the list we have special A+W parameters which have the prefix "AWParam_" and a list of the QLIK Sense® standard parameters. Our A+W visualization APPs will load this parameters, so e.g. if you transfer APPs from Europe to USA you have to change only the QLIK Sense® parameter `MoneyFormat` in the list and the APP work with $ instead of €.

With A+W Analytics function `AW_LOAD_QLIK_PARAMETER` in `AW_TOOLS.QVS` you can automatically load this parameter in an APP.

> If you need your own customized parameter in an A+W Analytics project, you can increase the list. Begin the name for your parameter with "CU_" or the shortcut of the customer site.

#### 1.2.5. A+W Analytics parameter

The following list of A+W Analytics parameters exist and will be used in some APPs.
-   **AWParam_Measuerment**: A+W Analytics parameter for used measurement. Allowed values are "mm" or "inch".
-   **AWParam_MeasuermentArea**: A+W Analytics parameter for used area measurement. Allowed values are "qm" or "sqft".
-   **AWParam_AreaFormat**: A+W Analytics parameter for format area values, e.g. "#.##0,0 m²" or "#,##0 sqft".
-   **AWParam_AWBOfferStatusMaxValid**: A+W Analytics parameter that describes the status of an offer in A+W Business when the offer is no longer valid.
-   **AWParam_LengthFormat**: A+W Analytics parameter for format length values, e.g. "#.##0,0 mm" or "#,##0.00"".
-   **AWParam_WasteMinResidualPlateLength**: A+W Analytics parameter for waste statistics. Minimum length in mm a residual plate can be reused. Smaller residual plates can't be reused and are put into waste.
-   **AWParam_iQuoteIdentificationText**: A+W Analytics parameter for identifying A+W iQuote documents in A+W Business.
-   **AWParam_AWBClassifierForBudgetCustomer**: A+W Analytics parameter for identifying A+W Business classifier that is used to define the budget for the customer.
-   **AWParam_StockDaysForcast**: A+W Analytics parameter, number of days of stock forecast.

#### 1.2.6. CUSTOMER_GEO_LIST (optional)

With the configuration of the table sheet `USER_ACCESS` you have the possibility to simple limit the access of users on the data amount of an APP. E.g. a sales person is only allowed to analyze his data.

-   **DBSYSTEM** - [KEY] ID of database system (e.g. AWB, AWP, AWC) in upper case
-   **ACCESS** – `ADMIN` or `USER`, one `ADMIN` is needed so you do not lock yourself out
-   **USERID** - [KEY] domain and user name in lower case, login name of user in QLIK sense
-   **ACCESS_ID** - field `ACCESS_ID` must exist in the data model in the APP. The data is filtered to the value defined here.

**Example Table `USER_ACCESS`:**

| DBSYSTEM | ACCESS | USERID | ACCESS_ID |
| :--- | :--- | :--- | :--- |
| AWB | ADMIN | domain\user1 | |
| AWB | USER | domain\user2 | 4711 |
| AWB | USER | domain\user3 | 4712 |

In our standard AWB TurnOver APPs we have add the `USER_ACCESS` function. It works if minimum one record exists in the `USER_ACCESS` table for database system AWB. The `ACCESS_ID` is the number of the sales representative. If you need a more complex rule system, you have to implement it outside the standard.

**Example of TurnOver APP**

During data load generate `ACCESS_ID` as new field:
`[Sales Representative Number] AS [ACCESSS_ID]`

At the end of the data load, load the user ACCESS rule table:
```qvs
SECTION ACCESS;
LOAD
    [ACCESS],
    [USERID],
    [ACCESSS_ID]
FROM [lib://QLIKDATA/QVD/3_COMPACTION/en-US/AW User Access List.qvd] (qvd)
WHERE DBSYSTEM = 'AWB';
```

---

## 2. Customizing

After installation of A+W Analytics with our standard visualization APPs the project isn't finished. Each customer has individual requests on what he needs to analyses. Or customer itself want to improve the existing visualizations.

Like our crystal reports, our A+W project team can make offers if adjustments are need. Use the documentation APP "AW Documentation” to get information which data exist in our A+W Analytics QVD files.

**Create a new customized visualization**
Create a complete new APP or make a copy of an existing A+W Analytics visualization. Load the needed A+W Analytics QVD files into the new APP `[QLIKData\QVD\3_Compaction\<Language>\]`.

**Change an existing A+W Analytics visualization**
Before changing an existing A+W Analytics visualization, we recommend to make a copy of the APP and give the copy name the customer shortcut as prefix: e.g. “AWP Waste Statistics” → “XXX Waste Statistics"

**Information is missing in a visualization**
Check the visualization. Not all loaded information in an APP is visualized, but if they exist they can be used. In a published APP you can use for personal pages values from predefined dimensions and measurements, so if the information is loaded it could be that you have to define a dimension or measurement for this.

If the information is not loaded in the visualization, check our "AW Documentation" APP. The information you need does not exist in one of our QVD files? This could happen because if our data model crows we don't automatically improve our visualization APPs. If the information exist, include it in the data load editor of the visualization.

**Information is missing in the A+W Analytics QVD files**
If an information is missing we can improve A+W Analytics with the new information. This will be done by development (email request to market.solutions@a-w.com).

The goal should be to include new information direct in A+W Analytics, so we can give support for this, we have the information for further projects and it will be easier for project team to implement it into visualizations.

We can not only include "standard" information, it is also possible for us to include information which are especially only for one of our customer or information the customer want to add but aren't exist direct in our database (e.g. the possibility to add GEO coordinate for customer ID using `CU_CONFIG.XLS`).

> **Important fact is that such improvements should be offered to our customer and will be realized by development.**

The customer can add information himself, if he do this he has to create his own structure, it is not allowed to manipulate the `AW_*` files of A+W Analytics. He has to create customer's own data loading APPs, excel files, QVD files and/or QLIK script files. How he does that is then the responsibility of the customer, we can advise if necessary.

Take care, if the customer has bought the QLIK Sense Server OEM license from A+W, it is only allowed to include data from A+W databases.

### 2.1. QLIK Sense® Extensions

A+W Analytics could contain some QLIK Sense® extensions which are used in standard APPs or tested in APPs during A+W Analytics projects. Extension can be found in [http://branch.qlik.com](http://branch.qlik.com).

The following chapters describe extensions which were used. The used version of an extension is found in the A+W Analytics disc set.

#### 2.1.1. InputVariable

This extension allows the user to set the value of a QLIK Sense variable. So it is possible to change the behavior of the APP dynamically.
[http://branch.qlik.com/#!/project/56728f52d1e497241ae698a9](http://branch.qlik.com/#!/project/56728f52d1e497241ae698a9)

#### 2.1.2. Automated Task Failure Email Alerts

This extension must be installed on a QLIK Server. Read installation manual of this extension.
User that execute the scheduled windows task needs rights to connect to the QMC. He doesn't need a token.
[http://branch.qlik.com/#!/project/56fd8bd3353d08684f6726bc](http://branch.qlik.com/#!/project/56fd8bd3353d08684f6726bc)

#### 2.1.3. Simple KPI Box

This extension provides a KPI box with more possibilities as the standard KPI Box. Beside the extension you find a demo APP which shows the possibilities of this extension.
[http://branch.qlik.com/#!/project/5677d80b7f70718900987bff](http://branch.qlik.com/#!/project/5677d80b7f70718900987bff)

### 2.2. Extend data model by customizing

If a customer need information which are not in our data model, contact MarketSolution (market.solutions@a-w.com) to extend our data model. So you need no customizing. Also not all information from our QVD files are include in our standard visualization APPs.

The main work of implementation is to create visualization APPs based on our standard APPs. Increase the data model with the data editor in this APPs, if the information exist in our QVD files.

If you need information which will not be add in our A+W Analytics package, you can create a customizing to generate a CU-QVD file which can be load into customer's visualization APPs.

Here an example which generates a CU-QVD file with data from all A+W Production databases from table `AWBAR_HISTORIE` for breakage. The QVD file will be stored in the sub directory `.\QLIKDATA\QVD\CU\`

```qvs
LET vDS_QLIKDATA = 'QLIKDATA';

[DATABASE_LIST]:
LOAD
    [AWCLIENT], [DBTYPE], [DBNAME], [DBOWNER], [QLIK_DATASOURCE], [DBSYSTEMTYPE]
FROM [lib://$(vDS_QLIKDATA)/EXCEL/CU_CONFIG.xlsx] (ooxml, embedded labels, table is DATABASE_LIST)
WHERE [COLLECTION_DATA] = 1 AND UPPER(Trim([DBSYSTEM])) = 'AWP';

FOR vDBCounter=0 TO NoOfRows('DATABASE_LIST') -1
    // Load parameter of database record
    LET vAWClient = TRIM(Peek('AWCLIENT', $(vDBCounter), 'DATABASE_LIST'));
    LET vDBName = TRIM(Peek('DBNAME', $(vDBCounter), 'DATABASE_LIST'));
    LET vQLIKDataSource = TRIM(Peek('QLIK_DATASOURCE', $(vDBCounter), 'DATABASE_LIST'));
    LET vDBOwner = TRIM(Peek('DBOWNER', $(vDBCounter), 'DATABASE_LIST'));
    LET vDBSystemType = TRIM(Peek('DBSYSTEMTYPE', $(vDBCounter), 'DATABASE_LIST'));
    
    TRACE Client=$(vAWClient) Databases=$(vDBName) DBOWNER=$(vDBOwner) DBSYSTEMTYPE=$(vDBSystemType);
    
    LIB CONNECT TO [$(vQLIKDataSource)];
    
    LET vSelectFrom = '$(vDBName).$(vDBOwner).';
    IF ('$(vDBSystemType)' = 'INFORMIX') THEN
        LET vSelectFrom = '$(vDBName):';
    END IF
    IF ('$(vDBSystemType)' = 'SQLSERVER') THEN
        LET vSelectFrom = '$(vDBName).$(vDBOwner).';
    END IF

    [AWP_CU_AWBAR_HISTORIE]:
    LOAD
        $(vAWClient) AS [%awclient],
        etikettnr AS [%Label Number],
        station AS [Breakage Station];
    SQL SELECT etikettnr, station
    FROM $(vSelectFrom)awbar_historie
    WHERE esnr = 19 and zustandnr > 0;
    
    DISCONNECT;
NEXT vDBCounter

// Store table into QVD file
If NoOfRows('AWP_CU_AWBAR_HISTORIE') > 0 Then
    LET vRowCounter = NoOfRows('AWP_CU_AWBAR_HISTORIE');
    
    STORE [AWP_CU_AWBAR_HISTORIE] INTO [lib://$(vDS_QLIKDATA)\QVD\CU\CU Production Breakage Station.qvd];
    
    TRACE $(vRowCounter) rows of table stored in .\CU\CU Production Breakage Station.qvd;
End If

// drop table if exist
If LEN(TRIM(NoOfRows('AWP_CU_AWBAR_HISTORIE'))) > 0 Then
    DROP TABLE [AWP_CU_AWBAR_HISTORIE];
End If

IF LEN(TRIM(NoOfRows('DATABASE_LIST'))) > 0 THEN
    DROP TABLE [DATABASE_LIST];
END IF
```

---

## 3. Data loading architecture

> This chapter is to understand how A+W Analytics works. It is not necessary (and not allowed!) to change scripts and excel files which are part of the A+W Analytics package (the files start with AW_*).

In A+W Analytics we are pursuing a multi-level approach to unload reappraise data for analysis purposes from A+W databases with QLIK Sense. The goal is at the end to have easily understandable data packages on which the final analysis APPs access.

**A+W Analytics Data Loading Architecture Diagram**
- **Source Layer**: Contains A+W Databases (one per system/client) and A+W Analytics Configuration files.
- **Extract Layer**:
    - **Data collection**: Uses `AW_DATA_COLLECTION.QVS` to store one QVD file for each table and database (e.g., `AWB_KU_KUNDEN_1.QVD`).
    - **Data union**: Uses `AW_DATA_UNION.QVS` to concatenate collected QVD files into one QVD file per table (e.g., `AWB_KU_KUNDEN.QVD`).
- **Compaction Layer**:
    - **Data compaction**: Uses `AW_DATA_COMPACTION.QVS` to compact data into QVD files that are easy to use for Analysis APPs (e.g., `Customer.QVD`). This layer also enriches data, for example by adding GEO points from `EXCEL\AW_DATA.XLSX`.
- **Presentation Layer**:
    - **Visualization**: Consists of QLIK Sense APPs that access the compacted Data Model.

### Layers Explained

1.  **Source Layer**
    The source layer contains the A+W Analytics source excel sheets and all A+W databases which will be included in A+W Analytics. If customer has bought QLIK Sense® QEM Version from A+W, it is only allowed to use A+W data, no other ones.

2.  **Extract Layer**
    a. **Data collection**
    The data required for analysis are copied per database and table 1:1 and stored in one QVD file per table and database. At this point the reading connection to our databases is made over ODBC, in the further course we only work on QVD files. In this step, the field names are renamed to understandable English names.

    b. **Data union**
    Collected data of a table from different databases will be concatenate into one QVD file. So you have one QVD file for each table of each database.

3.  **Compaction Layer**
    Based on the concatenated data, create packages of compacted data and store them into QVD files for visualization APPs. Loading architecture can create QVD files for each supported language. The files are stored in a language sub directory.

4.  **Presentation Layer**
    In the last step we have couple of APPs for visualization with data models based on the compacted data QVD files. The APPs must fit to the compaction QVD files, so we have a version for each supported language of each APP.
    The extract and compaction Layer is summarized in the APP `AW Load Data`. You can split the functions of this APP in different APPs e.g. if you want parallelize the different processes to increase the work.

### 3.1. Extract layer

To extract data from A+W databases A+W Analytics use QLIK® scripts. The script function uses our `QLIKDATA/EXCEL/AW_TABLES_*.XLSX` to know which tables and columns should be extracted. It is not allowed to change this excel sheets. The configuration of the databases is read from `QLIKDATA/EXCEL/CU_CONFIG.XLSX`. The configured database connection must exist and work.

#### 3.1.1. Data collection

A+W Analytics contains the QLIK® script `AW_DATA_COLLECTION.QVS`. All configured tables are read from database and stored in QVD files in `QLIKDATA/QVD/1_COLLECTION/`. One QVD file per table and database. During export the column names will be renamed into the alias names if set in configuration.

The following columns will be added automatically during export into QVD files:
-   **[%AWCLIENT]** – Client ID from configuration of this record
-   **[AWDATALOADTIME]** – Timestamp of unload of this record
-   **[AWARCHIVEDB]** – This column exists in tables which are not of table type MAIN. Value is the name of the archive database; Value 0 = record is from a MAIN database.

The actual existing functions will perform each time a complete unload.
-   **AW_DATA_COLLECTION_AWB** - for A+W Business, use `AW_TABLES_AWB.XLSX`
-   **AW_DATA_COLLECTION_AWP** - for A+W Production, use `AW_TABLES_AWP.XLSX`
-   **AW_DATA_COLLECTION_AWE** - for A+W Enterprise, use `AW_TABLES_AWE.XLSX`
-   **AW_DATA_COLLECTION_AWC** - for A+W Cantor, use `AW_TABLES_AWC.XLSX`
-   **AW_DATA_COLLECTION_AWCC** - for A+W Cantor CIM, use `AW_TABLES_AWC.XLSX`

#### 3.1.2. Data union

A+W Analytics contains the QLIK® script `AW_DATA_UNION.QVS`. This function read all QVD files from `QLIKDATA/QVD/1_COLLECTION/`. All files of the same database table will be concatenate into one QVD file per table and stored in `QLIKDATA/QVD/2_UNION/`.

The actual existing functions will perform each time a complete unload.
- **AW_DATA_UNION_AWB** - for A+W Business, use `AW_TABLES_AWB.XLSX`
- **AW_DATA_UNION_AWP** - for A+W Production, use `AW_TABLES_AWP.XLSX`
- **AW_DATA_UNION_AWE** - for A+W Enterprise, use `AW_TABLES_AWE.XLSX`
- **AW_DATA_UNION_AWC** - for A+W Cantor, use `AW_TABLES_AWC.XLSX`
- **AW_DATA_UNION_AWCC** - for A+W Cantor CIM, use `AW_TABLES_AWC.XLSX`

#### 3.1.3. AW_TABLES_*.XLSX

The excel configuration file `QLIKDATA/EXCEL/AW_TABLES_*.XLSX` contains the information about the tables and columns which A+W Analytics automatic unload. The files are part of the A+W Analytics package and **it is not allowed to manipulate the files.**

**TABLE_LIST**
The table sheet `TABLE_LIST` contains a list of tables for each database system which are to be unloaded.
-   **DBSYSTEM** - [KEY] ID of database system. Prefix of QVD file name. (AWB, AWP, AWC, AWCC, AWE)
-   **TBNAME** – [KEY] name of table
-   **TBLOADTYPE** - `MAIN` = load data only from databases with DBTYPE= MAIN of the DBYSYSTEM; `ALL` = unload from all databases of the DBSYSTEM
-   **TBVERSION** - [Optional] If filled and higher value as DBVERSION, this table will be ignored

**COLUMN_LIST**
The table sheet `COLUMN_LIST` contains a list of column names for each table in every database system.
-   **DBSYSTEM** - [KEY] ID of database system. Prefix of QVD file name. (AWB, AWP, AWC, AWCC, AWE)
-   **TBNAME** – [KEY] name of table, linked to TABLE_LIST
-   **COLNAME** - [KEY] name of column in database
-   **COLALIAS** - [KEY] name of column in QVD file, if not set COLNAME is used
-   **COLVERSION** – [Optional] if filled and higher as DBVERSION the column will not collect from database, column will be added into table with value '0'
-   **COLFORMAT** - [Optional] if set with value TEXT the column will be fix convert into a text format with the TEXT() function.

### 3.2. Compaction layer

A+W Analytics contains QLIK® scripts which compact and consolidate data for the visualization APPs. The result is stored in QVD files for the configured language; e.g. `QLIKDATA/QVD/3_COMPACTION/en-US/`.

-   **AW_DATA_COMPACTION_AW.QVS**: This script generates common compacted QVD files, the names starts with AW (e.g. `AW Client List.QVD`, `AW Text.QVD`). Run this functions before the other compactions functions, because other functions needs some of this QVD files. To execute all existing functions, call sub `AW_DATA_COMPACTION_AW`.
-   In the script common functions are stored which are used by the other compaction scripts, e.g. the function to translate and store the compaction result into QVD file: **AW_DATA_COMPACTION_TRANSLATE_STORE_QVD**
-   **AW_DATA_COMPACTION_AWP.qvs**: This script generates compacted QVD files based on A+W Production data, the names start with Production (e.g. `Production Batch.QVD`). To execute all existing functions, call sub `AW_DATA_COMPACTION_AWP`.
-   **AW_DATA_COMPACTION_AWB.qvs**: This script generates compacted QVD files based on A+W Business data, the names start with Business (e.g. `Business Documents.QVD`). To execute all existing functions, call sub `AW_DATA_COMPACTION_AWB`.
-   **AW_DATA_COMPACTION_AWC.qvs**: This script generates compacted QVD files based on A+W Cantor data, the names start with Cantor (e.g. `Cantor Order.QVD`). To execute all existing functions, call sub `AW_DATA_COMPACTION_AWC` for AW Cantor and `AW_DATA_COMPACTION_AWCC` for AW Cantor CIM.

#### 3.2.1. Multilingualism

The translation of the file and column names is controlled by the `AW_TABLES_*.XLSX` files. There we have one table for the file names `COMP_FILES`, and one table for the column names `COMP_FIELDS`. Also for both tables one table for the documentation: `COMP_FILES_INFO` and `COMP_FIELDS_INFO`.

During compaction the result gets an internal table ID. This table ID must exist in `COMP_FILES`. For each existing language it is possible to generate a QVD file.

The columns also have an ID. If this ID exist in `COMP_FIELDS` in the selected language, the column will be stored with the translated name. If no translation exists, the column is stored with his ID.

If a compaction function has generate a compacted table, it calls the function `AW_DATA_COMPACTION_TRANSLATE_STORE_QVD` (found in QLIK script `AW_DATA_COMPACTION_AW.QVS`). This function manages the translation and stores the QVD files. This function also can translate the content of fields in the right language from `AW_TEXT.XLSX`. If you have a numeric field, e.g. the part type, you can tell the function to translate this field if a translation group for this exist, part type is group number 2 in `AW_TEXT.XLSX`. The function converts the numeric field into a DUAL field with the translated text.

### 3.3. Presentation layer

A+W Analytics contains a bundle of standard analysis QLIK APPs. The APPs are stored in `QLIKDATA\APPS\<language>` folder and must be imported in QLIK Sense if customer need them.

If an APP exists in different languages, it uses the compaction QVD files of the language it is created in.

The APPs need a QLIK folder connection to `QLIKDATA`. In the folder it reads the QVD files and load the QLIK script `AW_TOOLS.QVS` to use helpful functions.

Each APP has a set of QLIK and A+W parameters. The parameters are not stored in APP, they are loaded from configuration `QLIKDATA\EXCEL\CU_CONFIG.XLSX` tab `QLIK_PARAMETER`. So it is possible to configure our standard APPs without changing the APP.

> **If a customer want change something in a standard visualization APP, make a copy of the APP and give the APP name a new prefix with a customer shortcut, so we can identify the APPs easily.**

#### 3.3.1. Tools

In the QLIK script `QLIKDATA\SCRIPTS\AW_TOOLS.QVS` we have a collection of common function which can be used in the apps.

**AW_CALENDAR**

This function generates a calendar for a date field for each AWClient in a fact table. The calendar contains fields for year, month, week, quarter, fiscal year, etc.

The date field has to be a date value. Remove the hour part if it is a timestamp. If not you get performance troubles.
`Date(Floor([DateField])) AS [DateField]`

**Parameters:**

1.  **vAWFactTable** - Name of the fact table. In this table a field `[%awclient]` must exist
2.  **vDateField** – Name of the date field which must exist in the fact table, if you want join the calendar into the table
3.  **vOnlyExistingDates** - (optional)
    -   `0` = (default) it generates calendar from minimum date to maximum date of date field
    -   `1` = generates calendar only for existing dates
4.  **vCalenderName** – (optional) if no calendar name (default) is set, the calendar is joined into the fact table. If a calendar name is set, a separate table with this name will be generated. Depending on the data model, the generation of synthetic keys can take a while and maybe generate performance troubles
5.  **vFiscalYearStartMonth** – (optional) if not set it uses the global parameter `FirstMonthOfYear`. If this parameter isn't set it uses 4 (april).
6.  **vQVD_DS_COMPACTIONFOR_CALENDAR** – (optional) QLIK data source for QVD files, if not set use `QLIKDATA`
7.  **vLanguage** - (optional) the description of the date field values (year, month,...) is set in the specified language. If not set or no translation exists, values are in English.

*Example Usage:*
```qvs
$(Must_Include=[lib://QLIKDATA/SCRIPTS/AW_TOOLS.qvs]);
CALL AW_CALENDAR('[MyFactTable]', '[MyDate]');
```

**AW_LOAD_QLIK_PARAMETER**

This function loads the common and AWParam parameters from `QLIKDATA\EXCEL\CU_CONFIG.XLSX` tab `QLIK_PARAMETER`, so you can configure all environment parameters, like `MoneyFormat` or `FirstMonthOfYear`, without changing the APPs.

*Example Usage:*
```qvs
$(Must_Include=[lib://QLIKDATA/SCRIPTS/AW_TOOLS.qvs]);
CALL AW_LOAD_QLIK_PARAMETER('QLIKDATA/EXCEL/CU_CONFIG.XLSX');
```

**AW_TEXT_TO_VARIABLE**

Loads text values from the `AW Text.qvd` file into variables in the APP to localize the APP.

*Example Usage:*
```qvs
$(Must_Include=[lib://QLIKDATA/SCRIPTS/AW_TOOLS.qvs]);
CALL AW_TEXT_TO_VARIABLE('QLIKDATA/QVD/3_COMPACTION', '100', 'en-US');
```

#### 3.3.2. Title bar

The title bar of A+W Analytics APPs in the base package must look the same.
- First color code: **#0041c4** (A+W Blue)
- Second color code: **#000000** (black)
- A+W Logo is on the right side.

---

## 4. APPs

This chapter lists existing APPs in the A+W Analytics Package with a short description. Each APP has a version number in the name (and as comment in the data editor), so it is easy to see if the customer uses the actual version or not.

For all APPs a QLIK folder data source with the name `QLIKDATA` is recommended.

### 4.1. Common APPs

#### 4.1.1. AW Load Data Clarity

The APP has no visualization part and need the QLIK ODBC data sources to the A+W databases. In the data editor it is possible to control the different A+W Clarity products.

#### 4.1.2. AW Load Data Cantor

This APP is similar to the APP for Clarity.

#### 4.1.3. AW Documentation

This APP visualizes the actual configuration and the documentation of the compacted QVD files and their fields.

### 4.2. A+W Business APPs

#### 4.2.1. Turnover APPs

Turnover analysis by customer and sales representative. Visualizes turnover, cost and margin values.

-   **Turnover analysis on order level.** No products, but freight cost which are on order level.
    -   `EN_AWB TurnOver.qvf`
    -   `DE_AWB Umsatz.qvf`
    -   `ES_AWB Volumen de ventas.qvf`
-   **Turnover of final products.** Analysis on line item level.
    -   `EN_AWB TurnOver - Final Products.qvf`
    -   `DE_AWB Umsatz - Endprodukte.qvf`
    -   `ES_AWB Volumen de ventas - Producto Final.qvf`
-   **Turnover of all products.** Analysis on BOM level.
    -   `EN_AWB TurnOver - All Products.qvf`
    -   `DE_AWB Umsatz - Alle Produkte.qvf`
    -   `ES_AWB Volumen de ventas - Todos los productos.qvf`

#### 4.2.2. Customer receivables, credit limit, budget

Requirements to use the full power of this new APP are:
-   Receivables in A+W Business from Financial accounting system.
-   Customer budget defined in A+W Business with a classifier. Configure in A+W Analytics parameter `AWParam_AWBClassifierForBudgetCustomer`.

-   Files:
    -   `EN_AWB Receivables.qvf`
    -   `DE_AWB Forderungen.qvf`

#### 4.2.3. Stock forecast

Calculates how the stock will be in the next x days. X days can be configured in the global A+W Analytics parameter `AWParam_StockDaysForcast`. If parameter is not set, default value 20 days is used.

-   Files:
    -   `EN_AWB Stock Forecast.qvf`
    -   `DE_AWB Lager Prognose.qvf`

#### 4.2.4. Delivery reliability

Compares the planned and actual delivery date from A+W Business and shows the numbers of documents in relation to the net amount of documents of delayed documents. Documents could be orders or purchase orders. So that the planned delivery date is not overwritten during order changes, the rules for entry in the ERP system must be observed.

-   Files:
    -   `DE_AWB Liefertreue.qvf`
    -   `EN_AWB Delivery Reliability.qvf`

### 4.3. A+W Production APPs

#### 4.3.1. AWP breakage statistics

Statistics of all breakages booked with barcoding system. The consumed costs are displayed if the values are configured right in ERP and PPS system and stored right in A+W Production which is possible since A+W Clarity Version 6.

-   Files:
    -   `DE_AWP Bruchstatistik.qvf`
    -   `EN_AWP Breakage Statistics.qvf`

#### 4.3.2. AWP waste statistics

Waste statistics based on `XOPT_STATISTIK_JUMBO` in A+W Production.

-   Files:
    -   `DE_AWP Verschnittstatistik.qvf`
    -   `EN_AWP Waste Statistics.qvf`

#### 4.3.3. AWP production statistics

All processing steps from A+W Processing catalog and booked by barcoding system will be analyzed.

-   Files:
    -   `DE_AWP Produktionsstatistik.qvf`
    -   `EN_AWP Production Statistics.qvf`

#### 4.3.4. AWP work in process

It shows the actual WIP value of your production. You can analyze the values on different registration points, articles or racks. The data for the WIP values are available since A+W Production version 6.

-   Files:
    -   `DE_AWP Work in Process.qvf`
    -   `EN_AWP Work in Process.qvf`

#### 4.3.5. AWP production workload

Actual production workload based on batch date. Designed for IG production, but other products are also possible.

-   Files:
    -   `DE_AWP Produktion Arbeitslast.qvf`
    -   `EN_AWP Production Workload.qvf`

#### 4.3.6. AWP charge overview

All booked charges in A+W Production barcoding system, which are entered with A+W Production Terminal charge field. You can analyze an order and see which charges has the order or you analyze a charge and see which orders are affected to this charge.

-   Files:
    -   `DE_AWP Chargenübersicht.qvf`
    -   `EN_AWP Charge Overview.qvf`

#### 4.3.7. AWP O4P Performance

This APP analyses the CSV files with the performance data which are create during O4P order import process of A+W Production.

The files `O4P_item.csv` and `O4P_ORDER.CSV` can be found in A+W Production system in folder `C:\ProgramData\A+W\Techsoft\Performance\` and must be transferred on QLIK Sense environment into `[QLIKDATA/Performance]`.

You can use CSV files from different systems. Add the system name in the filename as prefix.

-   File:
    -   `EN_AWP_O4P_Performance.qvf`

