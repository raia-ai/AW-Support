---
title: "EN A+W EDI Import"
category: "configuration"
product: "A+W EDI Import"
doc_type: "Unknown"
language: "EN"
tags: ["A+W EDI Import"]
version: "1.0"
last_updated: "2025-12-10"
description: "Interface Description     Import/export interface of orders and purchase orders                                        english                                  - -INTERNAL-         Date         Edited by      Remarks                                                           Version                      Andreas Noll   Original version                                                  2.0.000                                     New fields K1/13, K1/14, P1/19, P1/20, P1/21, P2/14, P2/15,"
source_file: "EN-A+W EDI Import.pdf"
---


# EN A+W EDI Import

     Interface Description




Import/export interface of orders
and purchase orders




                                   english




                             - -INTERNAL-
        Date         Edited by      Remarks                                                           Version
                     Andreas Noll   Original version                                                  2.0.000
                                    New fields K1/13, K1/14, P1/19, P1/20, P1/21, P2/14, P2/15,
                     Andreas Noll                                                               2.2.001
                                    P2/16
                     Andreas Noll   New field C1/25                                                   2.2.002
                     Andreas Noll   New fields K1/15, S1/16                                           2.2.003
                     Andreas Noll   #END# added to the end of a file                                  2.2.004
                     Andreas Noll   New record type T2 (header/footer texts)                          2.2.005
                     Andreas Noll   New field T1/5                                                    2.2.006
                     Andreas Noll   New field S1/17                                                   2.2.007
                     Andreas Noll   New field P1/22 and S1/18                                         2.2.009
                     Andreas Noll   Fields FH/4 and FH/5 now have four digits                         2.2.010
                     Andreas Noll   New field C1/26                                                   2.2.011
                     Andreas Noll   New field S1/19                                                   2.2.012
                     Andreas Noll   New field P1/23                                                   2.2.014
                     Andreas Noll   New fields K1/16, K2/14, K3/12, K3/13, P2/17, S1/20, S1/21        2.2.015
                     Andreas Noll   New fields B1/21-30, P1/24, P1/22                                 2.2.016
                     Andreas Noll   New record type P3                                                2.2.017
                     Andreas Noll   New record types DL/PL (document links)                           2.2.018
                     Andreas Noll   Field M1/12 has been extended from 1 digit to 6 digits            2.2.019
                                    Muntin calculation identifier (field C1/3) was expanded to
                     Andreas Noll   include equal bar length and glass edge reference (4,5 and
                                    6)
                     Silvia Höpp    Addition: ALCIB-specific notes
                     Andreas Noll   Bit vectors diagonal bars (field C1/27 )                          2.2.020
        2010-11-15   Silvia Höpp    Addition: ALCIB-specific notes
        2011-08-04   Andreas Noll   New field S1/23                                                   2.2.021
        2011-08-26   Andreas Noll   New fields P1/25, S1/24-26                                        2.2.022
                                    Transfer of P2/15 - Complaint key
        2013-10-11   Ina Seifert                                                                      2.2.023
                                    Transfer of object K1 in AWE
        2014-02-26   Ina Seifert    Transfer of DI / PL record into AWE                               2.2.023
                                    K1/17, K1/18, B1/31, edge quality for drilling (only export) in
        2014-03-24   Andreas Noll   B1, level for edges only inside and outside (see note in B1 -     2.2.023
                                    Edges)
        2014-02-20   André Münch    New field S1/27                                                   2.2.024
                                    AWE: Extended parameter list in B1 record for special
                                    surface processings
        2015-09-25   Ina Seifert                                                                      2.2.023
                                    AWE: Extended transfer of processings according to A+W
                                    processing catalog (section 4: processings / overview)
                                    Dimensional precision and inch transfer in AWE
        2016-01-13   Ina Seifert    (field FH/6)                                                      2.2.025
                                    Dimension type of muntins (field C1/31)
        2016-05-02   Ina Seifert    New data record PT (only AWE)                                     2.2.025
        2016-05-02   A. Noll        New fields P1/26 and S1/28                                        2.2.026


A+W Software GmbH                         EN-A+W EDI Import.docx                                                2 / 162
        Date         Edited by      Remarks                                                      Version
                                    New record types K5 and K6 (only AWB and only import)
        2016-06-29   A. Noll                                                                     2.2.027
                                    New field K1/20
        2016-07-25   A. Noll        New fields K1/21 and K1/22                                   2.2.028
        2016-10-13   A. Münch       New macro types documented (A+W Business 5.5 + 6)
        2017-03-03   A. Weil        New field in C1/32 and new data record PA( only AWE)         2.2.029
                                    New fields (only AWB) FH/7 (Customizing) and P1/27 (only
        2017-04-03   A. Münch                                                                    2.2.029
                                    export)
                     S.             New data record A1 (down payments)
        2017-05-04                                                                               2.2.029
                     Weil           New fields P2/2 and P2/3 Reason or place for complain
        2017-05-05   A.Münch        New fields K5/13 and K5/14 (only export)                     2.2.029
                                    Extended information for A+W Enterprise
        2017-06-12   A.Weil                                                                      2.2.029
                                    regardingA1,P2/18, P2/19,K5/9, P1/20
                                    Dimensioning type of corner cut-out/cut-off in processing
        2017-06-12   A.Münch                                                                     2.2.030
                                    parameter 12
        2017-07-27   A. Weil        New record types KP and PP                                   2.2.031
        2017-10-20   I.Seifert      Automatic mapping S1 product type and S1 product group       2.2.031
                                    Extensions SGG OMS II New fields P2/20, P2/21, S1/29,
        2018-03-06   D. Langsdorf                                                                2.2.032
                                    S1/30, K5/15, P3/8, S1/31
        2018-04-25   D. Langsdorf   Extensions SGG OMS II New fields K5/16,P3/9                  2.2.032
        2018-08-21   A. Weil        Expansion of Unicode possibilities for AWE, new field FH/8   2.2.033
        2019-07-18   A. Noll        Barcodes (P3/10, P3/11, S1/32, S1/33)                        2.2.034
        2019-10-17   I.Seifert      M1 record without shape number for templates
        2019-12-03   I.Seifert      AWE Export
                                    Barcodes (P3/10, P3/11, S1/32, S1/33) are only read and
        2019-01-16   D. Langsdorf                                                                2.2.034
                                    written starting with Version 2.2.034.
        2020-05-11   I.Seifert      P.O. export A+W Enterprise (section 5)                       2.2.032
        2020-05-20   A.Weil         Complaint order (only AWE)                                   2.2.033
        2020-06-23   S.Höpp         A+W EDI Export (AWDesk #422752)                              2.2.032
        2020-09-08   A. Noll        New field M1/13 (rotation in shape record)                   2.2.035
        2020-09-17   S.Höpp         A+W EDI Export (AWDesk #422752)
        2020-10-08   A. Noll        Change mode for quotations (#457852) (K1/3)                  2.2.035
        2020-10-16   A. Weil        Mirror stamp around center point (#456954) (B1/13)
        2020-11-06   A. Weil        Inclusion of A+W processing type 1650 for A+W Enterprise
                                    A+W processing type filled corner 1661 and capillary tube
        2021-01-25   A. Weil
                                    1662 (#456924)
        2021-03-12   A. Noll        Grouping for totals in form printing (P2/22) [AW-69502]




A+W Software GmbH                         EN-A+W EDI Import.docx                                           3 / 162
Content


       1            General explanations..................................................................... 9
                    1.1      Assign record types (alphabetical) ........................................................... 10

       2            Field description ............................................................................ 12
                    2.1      File header record FH .............................................................................. 12
                    2.2      General header record K1 ........................................................................ 13
                    2.3      Address header record K2 ....................................................................... 15
                    2.4      Shipping address header record K3 ......................................................... 16
                    2.5      Invoice address header record K4 ........................................................... 17
                    2.6      Header record extensions 1 K5 ................................................................ 18
                    2.7      Header record extensions 2 K6 ................................................................ 19
                    2.8      Document link header record DL.............................................................. 19
                    2.9      Header record - down payments A1......................................................... 19
                    2.10     Header record private KP ......................................................................... 20
                    2.11     Item record P1.......................................................................................... 22
                    2.12     Item record P2.......................................................................................... 24
                    2.13     Item record P3.......................................................................................... 26
                    2.14     Item record P9.......................................................................................... 27
                    2.15     Item record document link PL................................................................... 27
                    2.16     Item private PP......................................................................................... 27
                    2.17     Private table PT (item-related) (only AWE) .............................................. 28
                    2.18     Item record PA (only AWE) ...................................................................... 28
                    2.19     BOM record S1 ........................................................................................ 30
                             2.19.1     Details on the BOM structure............................................................................ 32
                    2.20 Shape record M1...................................................................................... 34
                    2.21 Processing record B1 ............................................................................... 37
                             2.21.1     Edge processings ............................................................................................. 39
                             2.21.2     Drillings ............................................................................................................. 41
                             2.21.3     Surface processings ......................................................................................... 44
                             2.21.4     Corner processings ........................................................................................... 46
                             2.21.5     Complex geometric processings ...................................................................... 47
                             2.21.6     IGU processings ............................................................................................... 48
                             2.21.7     Miscellaneous ................................................................................................... 48
                    2.22     Processing record B2 ............................................................................... 51
                    2.23     Bar code record BC.................................................................................. 53
                    2.24     Muntin record C1...................................................................................... 54
                    2.25     Asymmetrical muntin record CA ............................................................... 56
                             2.25.1     Example for muntin codes ................................................................................ 57
                    2.26 Text record T1 .......................................................................................... 58
                    2.27 Header/footer text record T2 .................................................................... 58

A+W Software GmbH                                         EN-A+W EDI Import.docx                                                                             4 / 162
                    2.28 Template record V1 (only AWE, cf. Vg.160653)....................................... 59

       3            Import-specific field notes ............................................................ 60
                    3.1      File header record FH .............................................................................. 60
                    3.2      General header record K1 ........................................................................ 61
                    3.3      Address header record K2 ....................................................................... 63
                    3.4      Shipping address header record K3 ......................................................... 64
                    3.5      Invoice address header record K4 ........................................................... 65
                    3.6      Header record extensions 1 K5 ................................................................ 65
                    3.7      Header record down payments A1 ........................................................... 66
                    3.8      Document link header record DL.............................................................. 67
                    3.9      Header record private KP ......................................................................... 67
                    3.10     Item record P1.......................................................................................... 69
                    3.11     Item record P2.......................................................................................... 71
                    3.12     Item record P3.......................................................................................... 73
                    3.13     Item private PP......................................................................................... 73
                    3.14     Item record document link PL................................................................... 74
                    3.15     Private table PT (item-related) (only AWE) .............................................. 74
                    3.16     Item-related parameter PA (only AWE) .................................................... 74
                    3.17     BOM record S1 ........................................................................................ 76
                    3.18     Shape record M1...................................................................................... 78
                    3.19     Processing record B1 ............................................................................... 79
                    3.20     Processing record B2 ............................................................................... 81
                    3.21     Bar code record BC.................................................................................. 82
                    3.22     Muntin record C1...................................................................................... 83
                    3.23     Asymmetrical muntin record CA ............................................................... 85
                    3.24     Text record T1 .......................................................................................... 86
                    3.25     Header/footer text record T2 .................................................................... 86
                    3.26     Template record V1 (only ALCIB, see op. 160653) .................................. 87

       4            A+W Enterprise import-specific function description................. 88
                    4.1   General Information ................................................................................. 88
                    4.2   File header record .................................................................................... 88
                    Order header (K1)............................................................................................... 90
                             4.2.1      Document type .................................................................................................. 90
                             4.2.2      Mode ................................................................................................................. 90
                             4.2.3      Delivery code .................................................................................................... 90
                             4.2.4      User-defined field .............................................................................................. 91
                             4.2.5      Packaging type (AWE 6) ................................................................................... 92
                             4.2.6      Delivery type (AWE 6) ...................................................................................... 92
                             4.2.7      External P.O. text .............................................................................................. 93
                             4.2.8      Height above nn ................................................................................................ 93


A+W Software GmbH                                         EN-A+W EDI Import.docx                                                                            5 / 162
                             4.2.9      Priority ............................................................................................................... 94
                             4.2.10     Object................................................................................................................ 94
                             4.2.11     E/A debtor ......................................................................................................... 95
                             4.2.12     Initial ID ............................................................................................................. 95
                    4.3      Addresses (K2 , K3, K4) ........................................................................... 95
                             4.3.1      First name / Attn ............................................................................................... 95
                             4.3.2      Invoice address ................................................................................................. 95
                             4.3.3      Delivery Address ............................................................................................... 96
                    4.4      Header record extension 1 K5.................................................................. 96
                    4.5      Header record-down payments A1........................................................... 96
                    4.6      Header record document link DL.............................................................. 96
                    4.7      Item (P1) .................................................................................................. 97
                             4.7.1      Item split (AWE 6) ............................................................................................. 97
                             4.7.2      Product sets (AWE 5.4) .................................................................................... 97
                             4.7.3      Dimensional precision (AWE 6) ........................................................................ 99
                             4.7.4      Article names .................................................................................................... 100
                             4.7.5      Color ................................................................................................................. 100
                             4.7.6      Dimensional variants ........................................................................................ 101
                             4.7.7      Customer item .................................................................................................. 102
                             4.7.8      Special logic ...................................................................................................... 102
                             4.7.9      Free of charge flag ; Complaint ........................................................................ 102
                    4.8      Item extension (P2) .................................................................................. 103
                             4.8.1      Document reference and item reference .......................................................... 103
                             4.8.2      Complaint type .................................................................................................. 103
                             4.8.3      Place of complaint and reason of complaint ..................................................... 104
                             4.8.4      Complaint order (#455928) ............................................................................... 104
                    4.9  Item references (P3) (AWE 6) .................................................................. 104
                    4.10 Item-related parameter (PA)..................................................................... 104
                    4.11 Private tables (item-related) (PT) ............................................................. 105
                             4.11.1     Supported tables and parameters .................................................................... 105
                    4.12 Item document link PL .............................................................................. 106
                    4.13 Item text record (T1)................................................................................. 106
                    4.14 Bill of materials (BOM) (S1)...................................................................... 107
                             4.14.1     Supported product types and groups ............................................................... 107
                             4.14.2     Color ................................................................................................................. 108
                             4.14.3     Frame / AIR....................................................................................................... 109
                             4.14.4     Additional processing / miscellaneous articles ................................................. 110
                             4.14.5     Price relevance ................................................................................................. 111
                             4.14.6     Print flag ............................................................................................................ 111
                             4.14.7     Gas ................................................................................................................... 112
                             4.14.8     Glass replacement ............................................................................................ 113
                             4.14.9     Muntins in triple IG (op. 118656) ...................................................................... 116
                             4.14.10    Steps (op. 220022) ........................................................................................... 117
                    4.15 Processings (B1) ...................................................................................... 119
                             4.15.1     Overview (starting with AWE version 6 and interface 2.2.023) ........................ 119
                             4.15.2     Drillings ............................................................................................................. 122
                             4.15.3     Surface processings ......................................................................................... 125
                             4.15.4     Corner processings ........................................................................................... 129


A+W Software GmbH                                         EN-A+W EDI Import.docx                                                                             6 / 162
                             4.15.5     Complex geometric processings ...................................................................... 129
                             4.15.6     Other processings ............................................................................................. 131
                             4.15.7     Dimensional precision (AWE 6) ........................................................................ 132
                    4.16 Barcode (BC) ........................................................................................... 132
                    4.17 Muntins (C1)............................................................................................. 133
                             4.17.1     Muntin symmetry / Calculation type .................................................................. 133
                             4.17.2     Muntin parameters ............................................................................................ 133
                             4.17.3     Dimensional precision (AWE 6) ........................................................................ 134
                    4.18 Muntins (CA) ............................................................................................ 134
                    4.19 SN template (V1)...................................................................................... 134
                    4.20 Environment variables .............................................................................. 135

       5            A+W Enterprise export-specific field notes
                    ........................................................................................................ 13
                    8
                    5.1      Supplier configuration .............................................................................. 138
                    5.2      File header record FH .............................................................................. 138
                    5.3      General header record K1 ........................................................................ 140
                    5.4      General header K2 ................................................................................... 142
                    5.5      General header K3 ................................................................................... 143
                    5.6      Document link DL ..................................................................................... 144
                    5.7      Text record T2 .......................................................................................... 144
                    5.8      Item record P1.......................................................................................... 144
                    5.9      Item record P2.......................................................................................... 146
                    5.10     Item record P3.......................................................................................... 147
                    5.11     Document link PL ..................................................................................... 147
                    5.12     Bar code record BC.................................................................................. 147
                    5.13     BOM record S1 ........................................................................................ 148
                             5.13.1     Product Types ................................................................................................... 148
                    5.14     Shape record M1 (shape)......................................................................... 151
                    5.15     Shape record M1 (step)............................................................................ 151
                    5.16     Muntin record C1...................................................................................... 152
                    5.17     Muntin record CA ..................................................................................... 153
                    5.18     Item text record (T1)................................................................................. 154
                    5.19     Item record P9 (not implemented yet) ...................................................... 155

       6            A+W Enterprise-specific function description
                    ........................................................................................................ 15
                    6
                    6.1      K1 mode ................................................................................................... 156
                    6.2      Export of processings (B1 record) ............................................................ 156
                             6.2.1      B1 record for A+W standard processings ......................................................... 156


A+W Software GmbH                                        EN-A+W EDI Import.docx                                                                       7 / 162
                    6.2.2   (No!) B1 record for A+W Enterprise processings (without A+W-processing type)   162




A+W Software GmbH                      EN-A+W EDI Import.docx                                       8 / 162
1    General explanations

Third-party orders that should be taken over into A+W software must be prepared according to the description. The
file must be made available in ASCII format. Please note Sections 3 and 4 in particular when you use the interface in
connection with A+W software.

Field type

        A       =       Alpha-numerical (left-aligned, pad with blanks)

        I       =       Numerical without decimals (right-aligned with leading zeros)

        F       =       Numerical with decimals (right-aligned with leading zeros, decimal separator is omitted. e.g.
                F6,1 = 000300 = 30.0)

        D       =       Date in the format YYYYMMDD

Field type

        M       =       this field must always be filled

        K       =          This field can be omitted
                (if a field should be omitted, it must be filled up with blank spaces. This applies to
                numerical and alpha-numerical fields.)



The definition of the mandatory and optional fields may deviate in the case of a transfer into the ERP system A+W
Enterprise. The definitions that are listed here apply to the ERP system A+W Business.

The record length of the file is 512 characters plus CARRIAGE RETURN LINE FEED. For transfer into the ERP
system A+W Enterprise, it is allowed to send the shorter record length.

The file end is marked by an end record to be able to easily recognize completely transferred files. The end record
consists of the text END, with a rhombus at the start and end ( -> #END# ).

When transferring all structures and dimensions, take into account that the lites are always viewed "from the
outside"!

Please note sections 3 and 4 for transfers to the ERP system A+W Enterprise.

For the takeover into the ERP system, it must be noted that the filter used (i000filter) is not Unicode capable.
(older than 2.2.033)

With the expansion 2.2.033, a possibility was created to handle the takeover into the ERP system via
Unicode and particular file codings. For more see 2.1 Dateikopfsatz FH

Definition

Documents       Are orders, quotations, purchase orders, or credit notes




A+W Software GmbH                                EN-A+W EDI Import.docx                                         9 / 162
1.1   Assign record types (alphabetical)
Record        Meaning                        Comment                              AWE - Export
type

A1            Header record - down
              payments

B1            Processing parameters                                               √

B2            Processing parameters          Special AWE

BC            Barcode                        Special AWE                          √

C1            Muntin record                                                       √

CA            Asymmetric muntins                                                  √

DL            Documents link header                                               √

FH            File Header                                                         √

K1            Header 1 - general                                                  √

K2            Header 2 - address                                                  √

K3            Header 3 – delivery address                                         √

K4            Header 4 - invoice address

K5            Header record extensions 1

K6            Header record extensions 2

KP            Header private                 (#373062) Special AWE

M1            Shape                                                               √

QU            Shape record 3E                Special AWE

ML            Shape record Lisec             Special AWE

P1            Item                                                                √

P2            Item                                                                √

P3            Item                                                                √

P9                                           Special AWE only export per report
                                             #399213

PL            Document link item                                                  √

PP            Item private                   (#373062) Special AWE

PT            Private Table (item-related)   Special AWE

PA            Item                           Item-related parameter AWE

S1            Bill of materials (BOM)                                             √

T1            Text record (item)                                                  √

T2            Text record (document)                                              √



A+W Software GmbH                            EN-A+W EDI Import.docx                              10 / 162
V1            Template   Special AWE



#             Comment




A+W Software GmbH        EN-A+W EDI Import.docx   11 / 162
2 Field description
2.1      File header record FH
This record type exists once in every file; it helps the receiving system to control and check the transfer.

See also 3.1 AWE File header record




                                                                                                         Contents
                                                                                    Position


                                                                                               Length
         No     Name




                                                                             Type
                                                                      Kind
         .


         1      Record type                                          M       A      1          2        FH
         2      Version number                                       M       A      3          8        02.2.034
         3      Total characters                                     M       N      11         12       3)
         4      Sending company number                               K       N      23         4
         5      Receiving company number                             K       N      27         4
         6      Dimension precision                                  K       N      31         3        1=metric;
                                                                                                        32,64,…=imperial
         7      User-defined field                                   K       A      34         100      1)
         8      Coding                                               K       A      134        10       2) starting with
                                                                                                        02.2.033
         9      Filler                                               M       A      144        369
          Table: File header record


      1) Field can be filled and loaded by AWB via customizing (variable m_sHEADER_USER_FIELD)

      2) Starting with interface version 02.2.033: Field can be filled with the file coding. If the field is empty, the old
         processing will be used.
         Only AWE accepted entries: ISO8859-1, ISO8859-2, ISO8859-15, UTF-8, 819, 1250, 1252, 57372

      3) Total number of bytes in the file.




A+W Software GmbH                                   EN-A+W EDI Import.docx                                                 12 / 162
2.2    General header record K1
This record type exists once in every document; if it is repeated, a new document is created.

See also section 3 AWE „Header record general“




                                                                                                      Contents
                                                                                 Position


                                                                                            Length
        No.    Name




                                                                          Type
                                                                   Kind
        1      Record type                                        M       A      1          2        K1
        2      Document type                                      M       N      3          1        1) 1-5,6,9

        3      Mode                                               M       N      4          1        2) 1-3 (4)

        4      Customer no.                                       M       N      5          8
        5      Dispatch date                                      K       D      13         8
        6      P.O. date                                          K       D      21         8
        7      Purchase text 1                                    K       A      29         40
        8      Purchase text 2                                    K       A      69         40
        9      Predefined document number                         K       N      109        8
        10     Bill of landing number                             K       N      117        8
        11     Client number                                      K       N      125        3
        12     Height above nn (in meters)                        K       N      128        4        7)

        13     Status                                             K       N      132        4        3)

        14     KZ locked                                          K       N      136        1        0=No, 1=Yes

        15     Delivery code                                      K       N      137        1        4)

        16     User-defined field                                 K       A      138        100      5)

        17     Priority                                           K       N      238        1        6)

        18     Object                                             K       N      239        8        10)

        19     Architect                                          K       N      247        8        8)

        20     Delivery date                                      K       D      255        8        Only AWB and only import

        21     Production preparation                             K       A      263        40       9)

        22     Business type                                      K       A      303        80       9)

        23     Filler                                             K       A      383        130
        Table: General header record

1) Here the document type of the exported document is specified, that is, from the point of view of the sending system.
   1=quotation (AWB only import), 5=purchase order, 9 -Product Type (only AWE)
   An exported purchase order receives the value 5 here. An exported quotation receives the value 1. A file with the
   document type 5 (purchase order) is always imported by A+W Business as an order. A file with the value 1 (quotation)
   is always imported by A+W Business as a quotation, no export of quotations. A+W Business only supports 1 and 5
   here. Starting with version 2.2.32 A+W Business supports the new document type 6, this is a purchase order, which is
   imported as purchase order and not as order. This data record can not be exported.

2) 1=New, 2=Change, 3=Cancel (AWE + AWB support only mode 1, starting with 2.2.32 AWB supports also mode 2+3
   for document type 6, starting with 2.2035 and AWB version 13.04.1145 mode 2 is also supported during import but
   only for quotations

A+W Software GmbH                               EN-A+W EDI Import.docx                                                          13 / 162
    4 – Reserved for new development in AWE [AW-162329]

3) Status

    0000 = Ok

4) 0=no direct delivery, 1 =direct delivery by supplier, 2 = pick-up by customer ( AWE: see section 4 "Delivery code" ; not
   supported by AWB )

5) Allows to transfer customized data. However, this requires customized programming in the ERP systems. (AWE: see
   section 4 "User-defined field")

6) 0 = Normal; 1 = Rush, 9 = Call (AWE: see section 4 "Priority")

7) AWE: see section 4 "Height above nn"

8) Customer number for item referencing (must be activated in A+W Business in the company master data)

    AWE: E/A debtor

9) OP area and business type are only imported by A+W Business and not exported. Both fields must exist in
   the master data if they are filled. The OP area overrides the setting of the import dialog. The document
   number is determined from the number range of the transmitted OP area.
   It is possible to transfer the corresponding number instead of description of OP area and business type. Enter a
   hashtag in front of the number. (e.g. #2 or #15 )

10) Only export




A+W Software GmbH                                 EN-A+W EDI Import.docx                                            14 / 162
2.3    Address header record K2
Writing this record type is not mandatory; it must be preceded by a K1 record.

See also AWE „Address“




                                                                                                    Contents
                                                                                Position


                                                                                           Length
        No.     Name




                                                                         Type
                                                                  Kind
        1       Record type                                      M       A      1          2        K2
        2       Customer address - name 1                        K       A      3          40
        3       Customer address - name 2                        K       A      43         40
        4       Customer address - name 3                        K       A      83         40
        5       Customer address - street                        K       A      123        40
        6       Customer address - city                          K       A      163        40
        7       Customer address - zip code                      K       A      203        11
        8       Customer address - post box                      K       A      214        40
        9       Customer address - post box - zip code           K       A      254        11
        10      Customer address - country code                  K       A      265        6
        11      Customer address - province/state                K       A      271        40
        12      Customer address - fax                           K       A      311        40
        13      Customer address - phone                         K       A      351        40
        14      Customer address - employee                      K       A      391        40
        15      Filler                                           K       A      431        82
       Table: General header record




A+W Software GmbH                              EN-A+W EDI Import.docx                                          15 / 162
2.4    Shipping address header record K3

Writing this record type is not mandatory; it must be preceded by a K1 record.

See also AWE „Address“




                                                                                                    Contents
                                                                                Position


                                                                                           Length
       No
              Name




                                                                         Type
                                                                  Kind
       .


       1      Record type                                       M        A      1          2        K3
       2      Shipping address - no.                            K        N      3          8
       3      Shipping address - name 1                         K        A      11         40
       4      Shipping address - name 2                         K        A      51         40
       5      Shipping address - name 3                         K        A      91         40
       6      Shipping address - street                         K        A      131        40
       7      Shipping address - city                           K        A      171        40
       8      Shipping address - zip code                       K        A      211        11
       9      Shipping address - province/state                 K        A      222        40
       10     Shipping address - country code                   K        A      262        6
       11     Delivery request                                  K        A      268        40
       12     Shipping address - phone                          K        A      308        40
       13     Shipping address - employee                       K        A      348        40
       14     Filler                                            K        A      388        125
       Table: Shipping address header record




A+W Software GmbH                               EN-A+W EDI Import.docx                                         16 / 162
2.5    Invoice address header record K4

Writing this record type is not mandatory; it must be preceded by a K1 record.

See also AWE „Address“




                                                                                                      Contents
                                                                                  Position


                                                                                             Length
        No
               Name




                                                                           Type
                                                                    Kind
        .


        1      Record type                                         M       A      1          2        K4
        2      Invoice address - no.                               M       N      3          8
        3      Invoice address - name 1                            K       A      11         40
        4      Invoice address - name 2                            K       A      51         40
        5      Invoice address - name 3                            K       A      91         40
        6      Invoice address - street                            K       A      131        40
        7      Invoice address - city                              K       A      171        40
        8      Invoice address - zip code                          K       A      211        11
        9      Invoice address - post box                          K       A      222        40
        10     Invoice address - post box - zip code               K       A      262        11
        11     Invoice address - country code                      K       A      273        6
        12     Invoice address - province/state                    K       A      279        40
        13     Invoice date                                        K       D      319        8
        14     Invoice number                                      K       N      327        8
        15     Filler                                              K       A      335        178
       Table: Invoice address header record




A+W Software GmbH                                 EN-A+W EDI Import.docx                                         17 / 162
2.6      Header record extensions 1 K5
Writing this record type is not mandatory; it must be preceded by a K1 record. It is imported by AWB starting with
interface version V2.2.027 but not exported. Depending on customer code an export is possible from version
v2.02.029 on.

For AWE see also: Header record extensions 1 K5




                                                                                                        Contents
                                                                                  Position


                                                                                              Length
          No
                 Name




                                                                           Type
                                                                    Kind
          .


          1      Record type                                       M       A      1          2         K5
          2      Tax key                                           K       A      3          40        1)

          3      Percentage of tax                                 K       N      43         6,4       1)

          4      Production start date                             K       D      49         8
          5      LG start date                                     K       D      57         8
          6      Production end date                               K       D      65         8
          7      Route                                             K       A      73         40
          8      Delivery terms                                    K       A      113        40
          9      Document Type                                     K       A      153        40        2)

          10     Packing                                           K       A      193        40
          11     Consultant                                        K       A      233        40
          12     Sales Repr.                                       K       A      273        40
          13     Original P.O. number                              K       N      313        8         3)

          14     Route number                                      K       A      321        20        3)

          15     eCommerce number (SGG)                            K       A      341        40        4)

          16     Delivery note number (SGG)                        K       A      381        40        4)

          17     Filler                                            K       A      421        92
         Table: Header record extensions 1


      1) If the sales tax key is not present with the specified designation, it is created anew. In the newly created tax
         record, the percentage from field 3 (percentage of tax) is taken over. If the tax record is present, the
         percentage is updated with the value from field 3.

      2) If the document type begins with "@" (ASCII Code 40hex), the target system assumes that the data is the
         foreign key for the document type. The character string can also start with a "#". Then, the sequence number
         is checked.

      3) Only export

      4) Only AWB import




A+W Software GmbH                                 EN-A+W EDI Import.docx                                            18 / 162
2.7    Header record extensions 2 K6
Writing this record type is not mandatory; it must be preceded by a K1 record. It is imported by AWB starting with
interface version V2.2.027 but not exported.




                                                                                                              Contents
                                                                                  Position


                                                                                                 Length
        No
               Name




                                                                           Type
                                                                    Kind
        .


        1      Record type                                         M       A      1              2            K6
        2      Mailing address                                     K       A      3              254
        3      Filler                                              K       A      257            256
       Table: Header record extensions 2



2.8    Document link header record DL

Writing this record type is not mandatory; it must be written between a K1 and a P1 record. It is also possible that
several document links follow each other.

See also0




                                                                                                              Contents
                                                                                  Position


                                                                                                 Length
        No
               Name
                                                                           Type
                                                                    Kind




        .


        1      Record type                                         M       A      1              2            DL
        2      Description of document link                        K       A      3              80
        3      Relative link to linked document                    M       A      83             254
        4      Filler                                              K       A      337            176
       Table: Header record document link




2.9    Header record - down payments A1

Writing this record type is not mandatory; it must be written between a K1 and a P1 record. It is imported by AWB but
not exported.

See also AWE: Header record down payments A1
                                                                                                                Contents
                                                                                      Position


                                                                                                     Length




       No
             Name
                                                                           Type
                                                                    Kind




       .


       1     Record type                                           M       A      1              2            A1
       2     Payment date                                          K       D      3              8            YYYYMMDD
       3     Payment mode                                          M       A      11             10           1)



A+W Software GmbH                                 EN-A+W EDI Import.docx                                                   19 / 162
                                                                                                              Contents
                                                                                    Position


                                                                                                   Length
       No
             Name




                                                                         Type
                                                                  Kind
       .


       4     Payment number                                      K       N      21             3
       5     Payment procedure                                   K       A      24             10
       6     Payment direction                                   K       N      34             2            1=Payment credit
                                                                                                            note
                                                                                                            -1=Payment
                                                                                                            cancelled
       7     Currency                                            K       A      36             3
       8     Amount                                              K       A      39             12
       9     Payment reference – Order                           K       A      51             30
       10    Exchange rate Currency                              K       A      81             12           Example :
                                                                                                            000000000100 if
                                                                                                            currency = EUR and
                                                                                                            the document is
                                                                                                            entered in EUR
       11    Filler                                              K       A      93             420
       Table: Header record-down payments


    1) The field may contain the external key of payment method. If no data record is found for external key, it is
       assumed that the correct AWB payment method is contained.


2.10 Header record private KP
This record type does not absolutely have to be written, it must be preceded by a K1 record.
If necessary, the record can be extended, as long as they are A+W standard fields, that are already used in EDI
order header-related tables.

The new record type is only evaluated in A+W Enterprise or ALCIB. A+W Business or ALFAK does not write this
record type and ignores this record type during import.
See also AWE „Kopfsatz Privat KP“
                                                                                                            Contents
                                                                                Position


                                                                                               Length




        No
              Name
                                                                         Type
                                                                  Kind




        .


        1     Record type                                        M       A      1              2            KP
        2     Private_long1                                      K       N      3              8
        3     Private_long2                                      K       N      11             8
        4     Private_char1                                      K       A      19             15
        5     Private_char2                                      K       A      34             15
        6     Filler                                             K       A      49             464
       Table: Header record private KP




A+W Software GmbH                               EN-A+W EDI Import.docx                                                           20 / 162
A+W Software GmbH   EN-A+W EDI Import.docx   21 / 162
2.11 Item record P1

This record type exists once in every item; if it is repeated, a new item is created; it must be preceded by a K1
record.

See also AWE „Item record P1“




                                                                                             Contents
                                                                       Position

                                                                                   Length
        No
              Name




                                                                Type
                                                         Kind
        .


        1     Record type                              M        A      1          2         P1
        2     Product no.                              M        A      3          64        4)

        3     Description1                             K        A      67         40
        4     Description 2                            K        A      107        40
        5     Description 3                            K        A      147        40
        6     Color                                    K        A      187        40        1)

        7     Short Name                               K        A      227        20
        8     Width                                    M        F      247        6,1       - If shape, then K
                                                                                            - For dimensional precision, see FH
                                                                                            record/field 6

        9     Height                                   M        F      253        6,1       - If shape, then K
                                                                                            - For dimensional precision, see FH
                                                                                            record/field 6

        10    Quantity                                 M        F      259        10,2
        11    Item price                               K        F      269        10,2      5)

        12    Sense of pattern                         K        N      279        2         0=none, 1=horiz., 2=vertical, 3=irrelevant

        13    Pattern side                             K        N      281        2         0=none, 1=inside, 2=outside
                                                                                            3)

        14    Reference                                K        A      283        80
        15    Customer item                            K        A      363        40
        16    Total installation thickness             K        F      403        5,1       For dimensional precision, see FH
                                                                                            record/field 6

        17    Edge prot.                               K        N      408        2         0=No, 1=Yes

        18    Tight size                               K        F      410        5,1       For dimensional precision, see FH
                                                                                            record/field 6

        19    KZ locked                                K        N      415        1         0=No, 1=Yes

        20    Free                                     K        N      416        1         0=No, 1=Yes

        21    Single cutback                           K        F      417        5,1
        22    Coated side                              K        N      422        2         0=none, 1=inside, 2=outside
                                                                                            3)

        23    Dimensional variant                      K        A      424        40        2)

        24    Procurement type                         K        N      464        3
        25    Price relevance identifier               K        N      467        1         0=not price-relevant, 1=price-relevant
                                                                                            Export only with change (starting with
                                                                                            2.2.022), Import +Export only if price
                                                                                            change allowed

        26    Price type                               K        N      468        1         5)



A+W Software GmbH                               EN-A+W EDI Import.docx                                                                   22 / 162
                                                                                               Contents
                                                                          Position

                                                                                     Length
        No
               Name




                                                                   Type
                                                            Kind
        .


        27     Item number                                 K       N      469        3        6)

        28     Filler                                      K       A      472        41
        Table: General item record

1) If the color begins with "@" (ASCII Code 40hex), the target system assumes that the date is the foreign key for
   the color. The foreign key may be a maximum of 40 characters long! (in versions before 13.04.0924, the foreign
   key is limited to 6 characters)

2) This field is supported only by A+W Enterprise; A+W Business neither reads nor writes it.

3) The coating side is transferred in a separate field (P1/22) starting with the interface version 2.2.009. In previous
versions, the coated side was transferred in the field for the pattern side (P1/13).

4) Only A+W Enterprise: If the product number begins with an "@" (ASCII code 40hex), it is assumed that the item
being transferred is a product set. (see section 4 "Product Type"). The product set name may not contain the
following characters:
' ' (0x20)      space (SPC)
'\t'    (0x09) horizontal tab (TAB)
'\n'    (0x0a) newline (LF)
'\v'    (0x0b) vertical tab (VT)
'\f'    (0x0c) feed (FF)
'\r'    (0x0d) carriage return (CR)
5) The price type (field 26) controls how the field 11/item price should be interpreted. Starting with interface version
2.2.026, the values 0=item piece price (as previously), 1=price per qm/sqft, 2= price per Lfm/lin. inch and 3=price per
piece are permissible.

6) Only AWB export




A+W Software GmbH                                  EN-A+W EDI Import.docx                                                 23 / 162
2.12 Item record P2

Writing this record type is not mandatory; it must be preceded by a P1 record.

See alsoItem record P2




                                                                                                    Contents
                                                                               Position


                                                                                          Length
        No
               Name




                                                                        Type
                                                                 Kind
        .


        1      Record type                                      M       A      1          2        P2
        2      Logo no.                                         K       N      3          3
        3      Logo position                                    K       N      6          2
        4      Rack type                                        K       N      8          3
        5      Lites per rack                                   K       N      11         6
        6      Document reference                               K       N      17         8
        7      Item reference                                   K       N      25         4
        8      Item group of order                              K       N      29         4
        9      Item text 1                                      K       A      33         40
        10     Item text 2                                      K       A      73         40
        11     Item text 3                                      K       A      113        40
        12     Item text 4                                      K       A      153        40
        13     Item text 5                                      K       A      193        40
        14     Edge decoating                                   K       N      233        1        0=No, 1=Yes

        15     Foreign key for complaints                       K       A      234        6
        16     Restriction check for alternative products       K       N      240        1        0=No, 1=Yes

        17     User-defined field                               K       A      241        100      1)

        18     Reason for complaint                             K       A      341        40       2) Only import

        19     Complaint place                                  K       A      381        40       3) Only import

        20     Supplier of item                                 K       N      421        8        4)

        21     Confirmed delivery date                          K       D      429        8        4)

        22     Group for subtotals                              K       N      437        4        5)

        23     Filler                                           K       A      441        72
        Table: Item record supplement


        1) Allows to transfer customized data. However, this requires customized programming in the ERP systems.

        2) If the complaint reason begins with "@" (ASCII Code 40hex), the target system assumes that the date is
           the foreign key for the complaint reason. The character string can also start with a "#". Then, the
           sequence number is checked.

        3) If the complaint place begins with "@" (ASCII Code 40hex), the target system assumes that the date is
           the foreign key for the complaint place. The character string can also start with a "#". Then, the
           sequence number is checked.



A+W Software GmbH                              EN-A+W EDI Import.docx                                               24 / 162
      Examples for 2) and 3):

                    -   Alphanumeric @BRUCH_GRUND@ or @PRODUKTION_ORT@

                    -   Numeric: #123456#

       4) Only AWB

       5) Only AWB, equal values mean that the items together belong to a group. These are summarized in the
          form printing and the price per group is indicated separately. If empty or 0, then no group. Groups are
          marked in color in the item entry.




A+W Software GmbH                             EN-A+W EDI Import.docx                                        25 / 162
2.13 Item record P3

Writing this record type is not mandatory; it must be written after a P1 record. The processing of this record type is
done with interface version 2.2.or higher. This both for import and export.

See also AWE „Item record P3“




                                                                                                             Contents
                                                                                        Position


                                                                                                   Length
        No
              Name




                                                                                 Type
                                                                          Kind
        .


        1     Record type                                                 M      A      1          2        P3
        2     Reference for previous P.O. number                          K      A      3          40       1)

        3     Reference for previous item number                          K      A      43         40       1)

        4     Reference for shipping order number                         K      A      83         40
        5     Reference for the shipping item number                      K      A      123        40
        6     Reference for end customer's P.O. number                    K      A      163        40
        7     Reference for end customer's item number                    M      A      203        40
        8     Link ext. P.O./Order GUID (SGG OMS/Xavannah)                K      A      243        40       2)

        9     Link delivery note GUID (SGG OMS)                           K      A      283        40       3)

        10    Start barcode                                               K      A      323        20       4)

        11    Barcode type                                                K      N      343        2        4)

        12    Filler                                                      K      A      345        168
       Table: Item record supplement


    1) Special solution depending on customer code:

        If the document to be imported is a complaint, which can be determined via the document type (field 9) from
        the header record K5, the fields No. 2 and 3 are checked here, whether a reference number (and reference
        item) is entered there. If there are several P3 item records with different references to a header record K1,
        the same number of complaints must be generated since the restriction in AWB is as follows: you can only
        assign one complaint to an original order (assignment of the original via database column
        AH_HAUPT_AUFTR in the complaint).

    2) only AWB import. For transfers from Xavannah to AWB/AWE the GUID of the configuration is transferred in
       the first 36 digits. The remaining 4 digits transfer the item reference.

    3) Only AWB import

    4) The start barcode is adopted from the reference order. The barcode is reported back by Production. Serves
       within several A+W Business installations to transfer the barcodes for the labels between the subsidiaries.
       Starting with version 2.2.034




A+W Software GmbH                                EN-A+W EDI Import.docx                                                 26 / 162
2.14 Item record P9

Writing this record type is not mandatory; it must be written after a P1 record. This record type is not currently read
in. It is only exported customer-specifically from A+W Enterprise.




                                                                                                                      Contents
                                                                                             Position


                                                                                                            Length
        No
               Name




                                                                                      Type
                                                                           Kind
        .


        1      Record type                                                 M      A          1            2          P9
        2      Additional text                                             K      A          3            140        1)

        12     Filler                                                      K      A          144          370
        Table: Item record supplement


    1) Individual additional text to be filled (only export)


2.15 Item record document link PL
Writing this record type is not mandatory; it must be written after a P1 record. It is also possible that several
document links follow each other.


See also3.14
                                                                                                          Contents
                                                                                  Position


                                                                                                 Length




         No
               Name
                                                                           Type
                                                                    Kind




         .


         1     Record type                                         M       A      1          2            PL
         2     Description of document link                        K       A      3          80
         3     Relative link to linked document                    M       A      83         254
         4     Filler                                              K       A      337        176
         Table: Item record document link



2.16 Item private PP
This record type is not compulsory. If it is written, it must be located behind the belonging item record (P1,P2 or P3).

If necessary, the record can be extended, as long as they are A+W standard fields, that are already used in EDI
item-related tables.

The new record type is only evaluated in A+W Enterprise or ALCIB. A+W Business or ALFAK ignore this this record
type.

See also „Position Privat PP“




A+W Software GmbH                                 EN-A+W EDI Import.docx                                                         27 / 162
                                                                                                                         Contents
                                                                                        Position


                                                                                                           Length
          No
                 Name




                                                                                 Type
                                                                      Kind
          .


          1      Record type                                        M        A          1              2            PP
          2      Private_long1                                      K        N          3              8
          3      Private_long2                                      K        N          11             8
          4      Private_char1                                      K        A          19             15
          5      Filler                                             K        A          34             479
         Table: Item record private PP



2.17 Private table PT (item-related) (only AWE)

This record type is not compulsory. It must be preceded by a P1 record. The record type permits to transfer variable
tables and their content for an item. This record type is supported only by AWE. AWB ignores this record type.

See also AWE „Private table“




                                                                                                                     Contents
                                                                                            Position


                                                                                                       Length
                 No.      Name
                                                                             Type
                                                                   Kind




                 1        Record type                             M          A          1              2            PT
                 2        Table name                              M          A          3              30           1)

                 3        Parameter string                        M          A          33             480          2) Separator | (pipe)
                     Table: Template record


    1)    The table name in which the data of the following parameter string should be stored.
    2)    Separator | (Pipe, ASCII 124).




2.18 Item record PA (only AWE)

This record type does not absolutely have to be written. It allows the transfer of item-related parameter that can be
switched by a flag (record type). This record type is supported only by AWE. AWB ignores this record type.
Transfer of item-related parameter for A+W Enterprise.

See also AWE Item-related parameters
                                                                                                                     Contents
                                                                                            Position


                                                                                                       Length




                 No.      Name
                                                                             Type
                                                                   Kind




                 1        Record type                             M          A          1              2            PA

A+W Software GmbH                                  EN-A+W EDI Import.docx                                                                   28 / 162
                                                                                                  Contents
                                                                            Position


                                                                                        Length
              No.   Name




                                                                     Type
                                                            Kind
              2     Record type                            M       N        3          2         1)

              3     Parameter 1                            K       F        5          6,2
              4     Parameter 2                            K       F        11         6,2
              5     Parameter 3                            K       F        17         6,2
              6     Parameter 4                            K       F        23         6,2
              7     Parameter 5                            K       F        29         6,2
              8     Parameter 6                            K       F        35         6,2
              9     Parameter 7                            K       F        41         6,2
              10    Parameter 8                            K       F        47         6,2
              11    Filler                                 M       A        53         460


   1) Which parameter type will be transferred




A+W Software GmbH                           EN-A+W EDI Import.docx                                           29 / 162
2.19 BOM record S1

Writing this record type is not mandatory; it must be preceded by a P1 record.

See also AWE „BOM record“




                                                                                                      Contents
                                                                               Position


                                                                                           Length
      No
            Name




                                                                        Type
                                                                Kind
      .


      1     Record type                                       M        A       12         2         S1
      2     Number (number)                                   M        N       3          4
      3     Parent number (0=main product)                    K        N       7          4
      4     Level                                             M        N       11         4
      5     Position within level                             M        N       15         4
      6     Product no.                                       M        A       19         64
      7     Name                                              K        A       83         40
      8     Color                                             K        A       123        40        1)

      9     Short Name                                        K        A       163        20
      10    Width                                             M        F       183        6,1       For dimensional precision, see
                                                                                                    FH record/field 6

      11    Height                                            M        F       189        6,1       For dimensional precision, see
                                                                                                    FH record/field 6

      12    Quantity                                          M        F       195        10,2
      13    Unit price (do not multiply with main quantity)   K        F       205        10,2      7)

      14    Sense of pattern                                  K        N       215        2         0=none, 1=horiz., 2=vertical,
                                                                                                    3=irrelevant

      15    Pattern side                                      K        N       217        2         0=none, 1=inside, 2=outside
                                                                                                    5)

      16    Product type                                      K        N       219        3         6)

      17    Product group                                     K        N       222        3         6)

      18    Coated side                                       K        N       225        2         0=none, 1=inside, 2=outside
                                                                                                    5)

      19    Thickness                                         K        N       227        4,1       2)
                                                                                                    For dimensional precision, see
                                                                                                    FH record/field 6

      20    Vector for production BOM                         K        N       231        20,0      3)

      21    User-defined field                                K        A       251        100       4)

      22    Procurement type                                  K        N       351        3
      23    BOM number from main article                      K        N       354        3
      24    Price printing code                               K        N       357        1         0=will not be printed, 1=will be
                                                                                                    printed

      25    Modification code                                 K        N       358        1         0=not changed,
                                                                                                    1=added or changed




A+W Software GmbH                              EN-A+W EDI Import.docx                                                                  30 / 162
                                                                                                         Contents
                                                                                   Position


                                                                                              Length
      No
             Name




                                                                            Type
                                                                    Kind
      .


      26     Price relevance identifier                           K        N       359        1        0=not price-relevant, 1=price-
                                                                                                       relevant
                                                                                                       Export only with change
                                                                                                       (starting with 2.2.022), Import
                                                                                                       +Export only if price change
                                                                                                       allowed

      27     Vector for production BOM 2                          K        N       360        10       3)

      28     Price type                                           K        N       370        1        7)

      29     Supplier of part                                      K       N       371        8        8)

      30     Confirmed delivery date                               K       D       379        8        8)

      31     Link ext. P.O./Order GUID (OMS)                       K       A       387        40       9)

      32     Start barcode                                         K       A       427        20       11)

      33     Barcode type                                          K       N       447        2        12)

      34     Filler                                                K       A       449        64
        Table: BOM record, general

1) If the color begins with "@" (ASCII Code 40hex), the target system assumes that the date is the foreign key for
   the color. The foreign key may be a maximum of 40 characters long! (in Versionen before 13.04.0924, the
   foreign key is limited to 6 characters)

2) Is only exported by ALFAK. ALFAK ignores this field when importing.

3) In this vector, every bit shows whether the BOM element requires the corresponding processing for a production
   BOM breakdown. Is only supported for transfers between ALFAK systems.

4) Allows to transfer customized data. However, this requires customized programming in the ERP systems.

5) The coating side is transferred in a separate field (S1/18) starting with the interface version 2.2.009. In previous
   versions, the coated side was transferred in the field for the pattern side (S1/15).

6) The fields Product Type and Product Group must be filled in for the A+W Enterprise import (MANDATORY fields).

    From A+W Enterprise version 6 release 19.10.2017 on, these fields are not mandatory fields any longer. A automatic
    mapping was provided.

7) The price type (field 28) controls how the field 13/item price should be interpreted. Starting with interface version
   2.2.026, the values 0=item piece price (as previously), 1=price per qm/sqft, 2= price per Lfm/lin. inch and 3=price
   per piece are permissible.

8) Only AWB

9) Only AWB import, starting with Version 2.2.034

10) empty

11) The start barcode is adopted from the reference order. The barcode is reported back by Production. Serves
    within several A+W Business installations to transfer the barcodes for the labels between the subsidiaries.
    Starting with version 2.2.034

12) 0=none, 1=high quantity, 9=high volume. Starting with version 2.2.034



A+W Software GmbH                                  EN-A+W EDI Import.docx                                                                31 / 162
2.19.1 Details on the BOM structure

The structure of the BOM is described through fields 2 through 5 of the S1 record. This allows you to clearly define
where each BOM element shall be attached. Field 2 (number) is unique within a BOM structure and serves for
unique identification purposes. The field is consecutively numbered, starting with 1. Field 3 (parent number) always
refers to field 2 (number) to clearly define to which BOM element the current element is going to be attached. If the
value 0 is entered here, the BOM element is attached to the main item. This is always the case for all BOM elements
at the top BOM level. Field 4 (level) defines the level where the current element is located. Here, value 1 is always
the top level. Field 5 (item) specifies the item for the respective BOM element. Numbering always starts at 1 and per
BOM node. See also the schema further below.




Illustration: BOM structure, using IG with LAMI as an example



However, it is also possible to only transfer the BOM elements that have been replaced in comparison to the original
product. This could result in gaps of the appearance of field 2 (number) in the file. If this is the case, the BOM
element is replaced based on fields 4 (level) and 5 (position) in the current item.

The muntin set must absolutely be written in A+W Business according to the gas that depends on the spacer (AIR).
The gas position is always in front of the muntin. This does not apply if the muntin depends on the insulated glass.




A+W Software GmbH                                         EN-A+W EDI Import.docx                               32 / 162
See below for some examples regarding the BOM structure and how fields 2 through 5 in the S1 records should be
filled:


Example 1)

On an insulated glass lite (150124) with standard structure 2 x float 4 mm, the airspace is replaced by the airspace
with article number 12012 in deviation of the product master data of the IG. The BOM structure now looks as follows:

…
P1150124………………………………………………………………………
S1000200000001000212012………………………………
…

If only the airspace is exchanged, the AIR is shown in the S1 record. Only fields 4 and 5 are relevant for the
exchange. For example, if it is a triple IG and only the 2nd AIR should be changed, then only field 5 (position) is
changed from value 2 to 4.


Example 2)

The complete structure of the triple insulating glass is transferred:

…
P1350000……………………………………………………………………………………………………………
S100010000000100011004…………………………………………………………………………
S1000200000001000212012………………………………………………………………………
S100030000000100031004…………………………………………………………………………
S1000400000001000412012………………………………………………………………………
S100050000000100051004………………………………………………………………………
…




A+W Software GmbH                                EN-A+W EDI Import.docx                                           33 / 162
2.20 Shape record M1

Writing this record type is not mandatory if a shape BOM record exists. It follows directly after its S1 record.
For A+W Enterprise, no shape S1 record is required.

For A+W Business, the shape set must always be sent after the lite layout and before the processings (see example
below). The exception are processings on the individual lites.

See also Shape record in section 3




                                                                                                        Contents
                                                                                  Position


                                                                                              Length
         No
               Name




                                                                           Type
                                                                    Kind
         .


         1     Record type                                         M       A      1          2         M1
         2     Shape number/ 999=steps                             M       N      3          8
         3     SN name                                             K       A      11         40
         4     Parameter 1                                         K       N      51         6,1       2)

         5     Parameter 2                                         K       N      57         6,1       2)

         6     Parameter 3                                         K       N      63         6,1       2)

         7     Parameter 4                                         K       N      69         6,1       2)

         8     Parameter 5                                         K       N      75         6,1       2)

         9     Parameter 6                                         K       N      81         6,1       2)

         10    Parameter 7                                         K       N      87         6,1       2)

         11    Parameter 8                                         K       N      93         6,1       2)

         12    Reference lite for steps                            K       N      99         6         1)

         13    Rotation                                            K       N      105        3         3)

         14    Filler                                              K       A      108        405
         Table: Shape record

    1) Bit vector for the lites the step refers to (seen from the outside). The parameters then define the allowance or
       reductions for the edges. Positive values mean a reduction, negative values are allowances. As from
       interface version 2.2.019, this field has six digits while it used to have just one digit in former versions.

         This table shall help to understand the bit vector:
         Step at                 Bit value
             1. Lite             1
             2. Lite             2
             3. Lite             4
             4. Lite             8
             5. Lite             16
                 etc.

         If there are several stepped lites, the bit values are simply added up. For example, if the first and fourth lite
         are to be stepped, value 9 has to be transferred in field 12 ( = 1 + 8 ).

    2) The dimensional precision depends on the definition in the FH record field 6.
    3) Shape turning in degrees clockwise (0, 90, 180, 270)



A+W Software GmbH                                 EN-A+W EDI Import.docx                                             34 / 162
A+W Software GmbH   EN-A+W EDI Import.docx   35 / 162
Example:

S1     1st lite
S1     AIR
S1     2nd lite
S1     shape (only required for A+W Business)
M1     Shape parameter
S1     Muntin




A+W Software GmbH                               EN-A+W EDI Import.docx   36 / 162
2.21 Processing record B1

Writing this record type is not mandatory if a processing BOM record exists. It follows directly after its S1 record. All
dimensions that are transferred depending on the processing type depend on the dimensional precision that is
specified in the FH record field 6.
See also AWE „Processings – overview“




                                                                                                      Contents
                                                                                 Position


                                                                                             Length
        No
              Name




                                                                          Type
                                                                   Kind
        .


        1     Record type                                         M       A      1          2         B1
        2     Parameter 1                                         K       N      3          6,1
        3     Parameter 2                                         K       N      9          6,1
        4     Parameter 3                                         K       N      15         6,1
        5     Parameter 4                                         K       N      21         6,1
        6     Parameter 5                                         K       N      27         6,1
        7     Parameter 6                                         K       N      33         6,1
        8     Parameter 7                                         K       N      39         6,1
        9     Parameter 8                                         K       N      45         6,1
        10    Parameter 9                                         K       N      51         6,1
        11    Parameter 10                                        K       N      57         6,1
        12    Parameter 11                                        K       N      63         6,1
        13    Parameter 12                                        K       N      69         6,1
        14    Parameter 13                                        K       N      75         6,1
        15    Parameter 14                                        K       N      81         6,1
        16    Parameter 15                                        K       N      87         6,1
        17    Parameter 16                                        K       N      93         6,1
        18    Parameter 17                                        K       N      99         6,1
        19    Parameter 18                                        K       N      105        6,1
        20    Parameter 19                                        K       N      111        6,1
        21    Parameter 20                                        K       N      117        6,1
        22    Parameter 21                                        K       N      123        6,1
        23    Parameter 22                                        K       N      129        6,1
        24    Parameter 23                                        K       N      135        6,1
        25    Parameter 24                                        K       N      141        6,1
        26    Parameter 25                                        K       N      147        6,1
        27    Parameter 26                                        K       N      153        6,1
        28    Parameter 27                                        K       N      159        6,1
        29    Parameter 28                                        K       N      165        6,1
        30    Parameter 29                                        K       N      171        6,1


A+W Software GmbH                                EN-A+W EDI Import.docx                                             37 / 162
                                                                                       Contents
                                                                  Position


                                                                              Length
       No
             Name




                                                           Type
                                                    Kind
       .


       31    Parameter 30                         K        N      177        6,1
       32    SN macro name                        K        A      183        254
       33    Filler                               K        A      437        76
       Table: Processing record




A+W Software GmbH                 EN-A+W EDI Import.docx                                          38 / 162
2.21.1 Edge processings
The numbers in brackets next to the processing specify the default A+W processing type according to processing
catalog


2.21.1.1        Seaming (1000)
2.21.1.2        Grinding (1005)
2.21.1.3        Polishing (1010)
Parameter                       Meaning
1..8                            Edge 1 - 8
9..17                           (free)
18                              exact calculation
19                              x width
20                              x height


2.21.1.4        Mitering (1015)

Parameter                       Meaning
1..8                            Edge 1 - 8
9                               Mitre angle
10                              Level (outside=1,inside=-1)
11..17                          (free)
18                              exact calculation
19                              x width
20                              x height


2.21.1.5        Faceting (1020)

Parameter                       Meaning
1..8                            Edge 1 - 8
9                               Depth
10                              Grinding angle
11                              Level (outside=1,inside=-1)
12..17                          (free)
18                              exact calculation
19                              x width
20                              x height

Note: In deviation to the processing catalog, the level is only defined for the inside or for the outside. Other values
are not allowed here and will be rejected. For such a case, two processings must be transferred, one for interior and
one for exterior.


2.21.1.6        Edge decoatings (1025)

Parameter                       Meaning
1..8                            Edge 1 - 8
9..10                           (free)
11                              Stripping width

Note: the level of the edge decoating is transferred by the data record S1 field 18 "Coating side".




A+W Software GmbH                                 EN-A+W EDI Import.docx                                         39 / 162
2.21.1.7       Bonding (mitering)

Parameter                   Meaning
1..8                        Edge 1 - 8
9                           Mitre angle
10                          Level (outside=1,inside=-1)
11-17                       (free)
18                          exact calculation
19                          width
20                          Height


2.21.1.8       Bonding (facet)

Parameter                   Meaning
1..8                        Edge 1 - 8
9                           Depth
10                          Grinding angle
11                          Level (outside=1,inside=-1)
12-17                       (free)
18                          exact calculation
19                          width
20                          Height


2.21.1.9       Edge prot.

Parameter                   Meaning
1..8                        Edge 1 - 8




A+W Software GmbH                          EN-A+W EDI Import.docx   40 / 162
2.21.2 Drillings
The numbers in brackets next to the processing specify the default A+W processing type according to processing
catalog)


2.21.2.1        Drillings (1100)

Parameter                       Meaning
1                               Item x drilling position 1
2                               Item y drilling position 1
3                               Diameter of drilling 1
4                               Item x drilling position 2
5                               Item y drilling position 2
6                               Diameter of drilling 2
7                               Item x drilling position 3
8                               Item y drilling position 3
9                               Diameter of drilling 3
10                              Item x drilling position 4
11                              Item y drilling position 4
12                              Diameter of drilling 4
13                              Dimensioning type (1, 2, 3)
14                              Reference corner drilling 1 X
15                              Reference drilling 1 Y (only for dimensioning types 2+3)
16                              Reference drilling 2 X
17                              Reference drilling 2 Y (only dimensioning type 2+3)
18                              Reference drilling 3 X
19                              Reference drilling 3 Y (only dimensioning type 2+3)
20                              Reference drilling 4 X
21                              Reference drilling 4 Y (only dimensioning type 2+3)
22                              Relief cut (0, 1)
23                              Edge quality (only export)

Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

Reference corners:
The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.

Note: The diameter is valid for all drilled holes but will be saved per drilling.
A+W Business: The edge quality is only exported since it is defined in the article master.
A+W Enterprise: See section 4 „Drilling“




A+W Software GmbH                               EN-A+W EDI Import.docx                                          41 / 162
2.21.2.2        Counter-sunk holes (1110)

Parameter                       Meaning
      1                                 Position x
 2                              Position y
3                               Diameter (inside)
4                               Hole depth (top)
5                               Hole depth (bottom)
6                               Angle (top)
7                               Angle (bottom)
8                               Sinking type (both sides=102, outside=103,inside=104)
9                               Diameter (top)
10                              Diameter (bottom)
11                              Input type (diameter=0, hole depth=1)
12                              Dimensioning type          (1, 2, 3)
13                              Reference drilling 1 X
14                              Reference drilling 1 Y (only dimensioning type 2+3)
15                              Relief cut (0, 1)
16                               (FREE)
17                              Position drilling 2 X
18                              Position drilling 2 Y
 19                             Reference drilling 2 X
20                              Reference drilling 2 Y (only for dimensioning types 2+3)
21                              Position drilling 3 X
22                              Position drilling 3 Y
 23                             Reference drilling 3 X
24                              Reference drilling 3 Y (only for dimensioning types 2+3)
25                              Position drilling 4 X
26                              Position drilling 4 Y
 27                             Reference drilling 4 X
28                              Reference drilling 4 Y (only for dimensioning types 2+3)
29                              Edge quality (only export)

Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

Reference corners:
The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.

A+W Business: The edge quality is only exported since it is defined in the article master.
A+W Enterprise: See section 4 „Countersunk hole“




A+W Software GmbH                               EN-A+W EDI Import.docx                                          42 / 162
2.21.2.3        Stepped drilling (1120)

Parameter                       Meaning
1                               Position drilling 1 X
2                               Position drilling 1 Y
 3                              Reference drilling 1 X
4-13                            Diameter 1-10 (one diameter per lite in the BOM)
14                              Dimensioning type          (1, 2, 3)
15                              Reference drilling 1 Y (only for dimensioning types 2+3)
22                              Relief cut
17                              Position drilling 2 X
18                              Position drilling 2 Y
 19                             Reference drilling 2 X
20                              Reference drilling 2 Y (only for dimensioning types 2+3)
21                              Position drilling 3 X
22                              Position drilling 3 Y
 23                             Reference drilling 3 X
24                              Reference drilling 3 Y (only for dimensioning types 2+3)
25                              Position drilling 4 X
26                              Position drilling 4 Y
 27                             Reference drilling 4 X
28                              Reference drilling 4 Y (only for dimensioning types 2+3)
29                              Edge quality (only export)

Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

Reference corners:
The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.

A+W Business: The edge quality is only exported since it is defined in the article master.
A+W Enterprise: See section 4 „Stepped drilling“




A+W Software GmbH                               EN-A+W EDI Import.docx                                          43 / 162
2.21.3 Surface processings

The numbers in brackets next to the processing specify the default A+W processing type according to processing
catalog


2.21.3.1        Coating (1200)
2.21.3.2        Matting (1205)
2.21.3.3        Area enameling (1220)
2.21.3.4        Screen printing (1225)

Parameter                       Meaning
1                               Dimensioning type           (1, 2, 3)
2..8                            (free)
9                               width
10                              height
      11                                Position x
 12                             Position y
13                              Reference X
14                              Shift number
15                              Saturation
16                              Reference Y
30                              Entry type (1 = Multi, 2 = Single)

Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.



2.21.3.5        Enameling / UV protection (1650)

Parameter                       Meaning
1..8                            Edge 1 - 8
9                               Depth
10                              Edge distance

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list and the restriction that
per B1 record, only ONE edge may be defined as processed (parameters 1-8) (see section 4)


2.21.3.6        Bending

Parameter                       Meaning
1..8                            (free)
9                               width
10                              height



2.21.3.7        Fluted bevel (1230)

Parameter                       Meaning


A+W Software GmbH                               EN-A+W EDI Import.docx                                          44 / 162
1..8                            Edge 1 - 8
9                               Distance to the edge
10                              Distance to the corner
11..18                          Length on edges 1-8
19                              width
20                              bevel number
21                              Reference corner

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list and the restriction that
per B1 record, only ONE edge may be defined as processed (parameters 1-8) (see section 4)


2.21.3.8        Decoatings (1203)

Parameter                       Meaning
1                               Dimension type (1, 2, 3)
2                               Angle of rotation
3                               Reference edge of the angle of rotation
4                               Reference corner of the decoating
5…8                             (free)
9                               width
10                              height
11                              Position X
12                              Position Y
13                              Reference X
14…15                           (free)
16                              Reference Y (only for dimensioning types 2+3)
17…29                           (free)
30                              Entry type (1 = Multi, 2 = Single)

Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge


Reference corners:
The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.


2.21.3.9        Alarm net (1245)

Parameter                       Meaning
1..8                            Corner 1 – 8



2.21.3.10       Stamp (1250)
2.21.3.11       Logos (1255)

Parameter                       Meaning
1                               Distance A
2                               Distance B
3                               Reference X
4                               Logo number
5                               Reference Y
6                               Type (1-4)
7                               Dimensioning type          (1, 2, 3)


A+W Software GmbH                               EN-A+W EDI Import.docx                                          45 / 162
8                               width
9                               height
10                              Reference of the logo
11                              Reference edge for angle
12                              angle
18                              Mirror stamp around center point (only supported by AWE)


Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge


Caution:
Reference corners:
The reference corners are NOT zero-based. That is, for corner 1, a 1 is written, for corner 2 a 2, etc.The numbering
begins in the lower left corner and is incremented counter-clockwise.

With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Logo").




2.21.4 Corner processings
The numbers in brackets next to the processing specify the default A+W processing type according to processing
catalog


2.21.4.1        Corner cutouts (1300)

Parameter                       Meaning
1..8                            Corner 1 – 8
9                               Distance A
10                              Distance B
11                              (free)
12                              Dimension type (1=acc. to catalog, 2=for rectangular lites A horizontal B vertical)
Starting with version 2.02.030 export and import, if not set, the company parameters are valid
13-18                           (free)
19                              Cutout edge A (vert./parallel)
20                              Cutout edge B (vert./parallel)
21                              Radius outer corner
22                              Radius inner corner

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Corner
cut-out")



2.21.4.2        Corner cutouts (1305)
2.21.4.3        Diagonal corners
Parameter                       Meaning
1..8                            Corner 1 – 8
9                               Distance A ( width )
10                              Distance B ( height )
12                              Dimension type (1=acc. to catalog, 2=for rectangular lites A horizontal B vertical)
Starting with version 2.02.030 export and import, if not set, the company parameters are valid




A+W Software GmbH                               EN-A+W EDI Import.docx                                          46 / 162
Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Corner
cut-off")




2.21.4.4       Rounded corners (1310)

Parameter                      Meaning
1..8                           Corner 1 – 7
9..10                          (free)
11                             Radius

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4
"Rounded corner")


2.21.5 Complex geometric processings
2.21.5.1       Edge cutouts (1400)

Parameter                      Meaning
1..8                           Edge 1 - 8
9                              Length ( width )
10                             Depth ( height )
11..18                         free
19                             Distance to the corner
20                             Reference corner
21                             Radius outer corner
22                             Radius inner corner
30                             Entry type (1 = Multi, 2 = Single)


Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Edge
cut-out")



2.21.5.2       Arc-shaped edge cutouts

Parameter                      Meaning
1..8                           Edge 1 – 8 (only for type 1)
9                              Radius
10                             Chord length (only for type 1)
11                             Distance to the corner (only type 1)
12                             Position x (only type 0)
13                             Position y (only type 0)
15                             Type (x/y = 0, Chord/Radius = 1)
19                             Reference corner
21                             Radius outer corner
30                             Entry type (1 = Multi, 2 = Single)

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Arc-
shaped edge cut-out")




A+W Software GmbH                              EN-A+W EDI Import.docx                                        47 / 162
2.21.5.3       Speaker holes (1405)

2.21.5.4       Interior cutouts (1415)

Parameter                      Meaning
      1                                Position x
 2                             Position y
3..8                           (free)
9                              width
10                             height
11                             Reference corner
12                             Reference edge
13                             Inner radius
14                             Dimensioning type           (1, 2, 3)
15                             Angle of rotation
16                             Edge (alignment)
17                             Object reference point
30                             Entry type (1 = Multi, 2 = Single)

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Speak-
thru")


2.21.5.5       Handles

Parameter                      Meaning
1..8                           Edge 1 - 8
9                              Length ( width )
10                             Depth ( height )
11..18                         Length on edges 1-8
19                             Reference corner
20                             Distance to the corner
21                             Distance to the edge
22                             Dimensioning type           (1, 2, 3)
23                             Angle of rotation
24                             Edge (alignment)
25                             Object reference point
30                             Entry type (1 = Multi, 2 = Single)


2.21.6 IGU processings

2.21.6.1       Edge prot.

Parameter                      Meaning
1..8                           Edge 1 - 8
9..17                          (free)
18                             exact calculation
19                             x width
20                             x height


2.21.7 Miscellaneous

2.21.7.1       Macro (edge) (1900)


A+W Software GmbH                              EN-A+W EDI Import.docx                                       48 / 162
Parameter                      Meaning
1..8                           Edge 1 - 8
9..10                          (free)
11                             Distance
12                             Alignment (0 = right, 1 = left)
30                             Entry type (1 = Multi, 2 = Single)

Caution: With respect to the storage in A+W Enterprise, there is an expanded parameter list (see section 4 "Macro")



2.21.7.2       Macro (corner)

Parameter                      Meaning
1..8                           Edge 1 - 8
9..11                          (free)
12                             Alignment (0 = right, 1 = left)
30                             Entry type (1 = Multi, 2 = Single)


2.21.7.3       Macro (surface) (1910)

Parameter                      Meaning
      1                                Position x
 2                             Position y
3..10                          (free)
11                             Reference corner
12                             Reference edge
13                             (free)
14                             Dimensioning type           (1, 2, 3)
15                             Angle of rotation
16                             Edge (alignment)
30                             Entry type (1 = Multi, 2 = Single)


2.21.7.4       Parameterizable macro (edge) (1920)

Parameter                      Meaning
1..8                           Edge 1 - 8
9..10                          (free)
11                             Distance
12                             Alignment (0 = right, 1 = left)
13                             Number of parameter
14                             Bit vector for parameter 15-22 (1 = SIze (conversion for Inch), 0 = not-size e.g.
angle)
15-22                          Parameter 1-8
30                             Entry type (1 = Multi, 2 = Single)


2.21.7.5       Parameterizable macro (surface) (1930)

Parameter                      Meaning
      1                                Position x
 2                             Position y
3..10                          (free)
11                             Reference corner
12                             Reference edge
13                             (free)
14                             Dimensioning type           (1, 2, 3)


A+W Software GmbH                              EN-A+W EDI Import.docx                                              49 / 162
15                               Angle of rotation
16                               Edge (alignment)
17                               Number of parameter
18                               Bit vector for parameter 19-26 (1 = Size (conversion for inch, 0 = not-size e.g. angle)
19-26                            Parameter 1-8
30                               Entry type (1 = Multi, 2 = Single)


2.21.7.6        6.3 Profile miters
2.21.7.7        6.4 Regrinding
Parameter                        Meaning
1..8                             Edge 1 - 8
9                                Mitre angle


2.21.7.8        Edge silk screening (1970)

Parameter                        Meaning
1..8                             Edge 1 - 8
9..10                            (free)
11                               width
14                               Screen number
15                               Saturation
2.21.7.9        Filled corner (1661) (only AWE status as of: February 15, 2021)
Parameter                        Meaning
1                                Corner

2.21.7.10       Capillary tube (1662) (only AWE status as of: 25.01.21)
Parameter                        Meaning
1                                Corner
2                                Distance to the corner
3..10                            Edge 1 - 8
11                               Angle of rotation
12                               Reference edge
13                               Type no. (different articles)


Notes
1. Processing level:
Levels of processing that are not listed (e.g. edge stripping) are saved in field FER_BESCHICH_SEITE of the BOM.

2. Processing quantity:
A quantity that is not listed (e.g. drilling) is saved in the field STL_MENGE of the BOM.




A+W Software GmbH                                EN-A+W EDI Import.docx                                          50 / 162
2.22 Processing record B2
Writing this record type is not mandatory if a processing BOM record exists. It follows directly after its S1 record. This
record is written alternatively to the B1 record. This record type is only supported by ALCIB. ALFAK ignores this
record type.
See also 3.20




                                                                                                      Contents
                                                                                 Position


                                                                                            Length
        No
              Name




                                                                          Type
                                                                   Kind
        .


        1     Record type                                         M       A      1          2        B2
        2     internal order number                               K       N      3          8        Niu         *)
        3     internal item number                                K       N      11         5        Niu         *)
        4     Customer number                                     K       N      16         8        Niu         *)
        5     Item that is exchanged or for which there is        K       N      24         8        Niu         *)
              an additional item
        6     Item type that is exchanged and for which           K       N      32         5
              there is an additional item
        7     Exchange/supplement article                         K       N      37         8
        8     Exchange/supplement indicator                       M       N      45         5        0-none
                                                                                                     1-Exchange
                                                                                                     2-Supplement
                                                                                                     3-Delete
        9     new assembly position                               K       N      50         5
        10    Parent article (product)                            K       N      55         8
        11    Customer-specific article number                    K       A      63         20       Niu         *)
        12    Project #                                           K       N      83         8        Niu         *)
        13    Quantity1 (widths)                                  K       N      91         5
        14    Quantity2 (heights)                                 K       N      96         5
        15    Original assembly position where the                K       N      101        5
              exchange or supplement takes place
        16    Sense of pattern                                    K       N      106        5        0-none
                                                                                                     1-vertical
                                                                                                     2-horizontal
                                                                                                     3-diagonal
        17    Print code                                          K       N      111        5        0-No
                                                                                                     1-Yes
                                                                                                     2-Yes, only Sales
                                                                                                     3-Yes, only
                                                                                                     Production
        18    Price calculation code                              K       N      116        5        0-No
                                                                                                     1-Yes
        19    Color number                                        K       N      121        5



A+W Software GmbH                                EN-A+W EDI Import.docx                                                  51 / 162
                                                                                                    Contents
                                                                               Position


                                                                                          Length
        No
              Name




                                                                        Type
                                                                 Kind
        .


        20    Size parameter 1                                 K        N      126        8
        21    Size parameter 2                                 K        N      134        8
        22    Size parameter 3                                 K        N      142        8
        23    Positioning 1                                    K        N      150        8
        24    Positioning 2                                    K        N      158        8
        25    Positioning 3                                    K        N      166        8
        26    Edge vector                                      K        A      174        10       Starting at the
                                                                                                   bottom edge in
                                                                                                   clockwise direction
                                                                                                   0 – Edge is not
                                                                                                   processed
                                                                                                   1 – Edge is
                                                                                                   processed
        27    Market partner type                              K        N      184        5        Niu    *)
                                                                                                   0-Customer
                                                                                                   1-Supplier
        28    Priority                                         K        N      189        8
        29    Article text that should be used as a            K        A      196        30
              replacement


*) Niu = Not in use




A+W Software GmbH                              EN-A+W EDI Import.docx                                                    52 / 162
2.23 Bar code record BC
This record type is not compulsory. This record type is currently only analyzed by A+W Enterprise.

See also3.21




                                                                                                   Contents
                                                                               Position


                                                                                          Length
        No
               Name




                                                                        Type
                                                                 Kind
        .


        1      Record type                                      M       A      1          2        BC
        2      Barcode                                          K       A      3          500
        3      Filler                                           K       A      503        10




A+W Software GmbH                              EN-A+W EDI Import.docx                                         53 / 162
2.24 Muntin record C1
Writing this record type is not mandatory if a muntin BOM record exists. It follows directly after its S1 record. All
dimensions depend on the dimensional precision that is specified in the FH record field 6.
The muntin set must absolutely be written in A+W Business according to the gas that depends on the spacer. The
gas position is always in front of the muntin. This does not apply if the muntin depends on the insulated glass.
See also3.22




                                                                                                        Contents
                                                                                  Position


                                                                                              Length
        No
               Name




                                                                           Type
                                                                    Kind
        .


        1      Record type                                         M       A      1          2         C1
        2      Type                                                M       N      3          3         1)

        3      Calculation type                                    M       N      6          3         3)

        4      Direction                                           M       N      9          3         0=horizontal
                                                                                                       1=vertical
        5      Parameter 1                                         K       N      12         6,1
        6      Parameter 2                                         K       N      18         6,1
        7      Parameter 3                                         K       N      24         6,1
        8      Parameter 4                                         K       N      30         6,1
        9      Parameter 5                                         K       N      36         6,1
        10     Parameter 6                                         K       N      42         6,1
        11     Parameter 7                                         K       N      48         6,1
        12     Parameter 8                                         K       N      54         6,1
        13     Parameter 9                                         K       N      60         6,1
        14     Parameter 10                                        K       N      66         6,1
        15     Parameter 11                                        K       N      72         6,1
        16     Parameter 12                                        K       N      78         6,1
        17     Parameter 13                                        K       N      84         6,1
        18     Parameter 14                                        K       N      90         6,1
        19     Parameter 15                                        K       N      96         6,1
        20     Parameter 16                                        K       N      102        6,1
        21     Parameter 17                                        K       N      108        6,1
        22     Parameter 18                                        K       N      114        6,1
        23     Parameter 19                                        K       N      120        6,1
        24     Parameter 20                                        K       N      126        6,1
        25     Number of muntins                                   M       N      132        10,2      2)

        26     Muntin pads code                                    K       N      142        2         8)

        27     Bit vector diagonal bars                            K       N      144        10        4) new from 2.2.020

        28     AWDesign file name                                  K       A      154        40        5) new from 2.2.020

        29     Color code of muntin in AWDesign file               K       A      194        40        6) new from 2.2.020

        30     Muntin color name in AWDesign file                  K       A      234        40        7) new from 2.2.020



A+W Software GmbH                                 EN-A+W EDI Import.docx                                                     54 / 162
                                                                                                         Contents
                                                                                   Position


                                                                                               Length
        No
               Name




                                                                            Type
                                                                     Kind
        .


        31     Dimension type of the drilling dimension            K        N      274        1         9) new starting with
                                                                                                        2.2.025
                                                                                                        0 = to the origin,
                                                                                                        1 = chain dimension

        32     Simulated Divided Lite Bar Size                     K        F      275        5,2       10)

        33     Filler                                              K        A      280        233
        Table: Muntin record



1) Muntin bar pattern type must be coordinated with the technical software since they can be adjusted variably.

2) A maximum of 12 muntins are allowed per level of the muntin grid.

3) Muntin calculation type:
   0 = drilling point sym., 1 = field sym., 2 = drilling point asym., 3 = field asym., 4 = same bar length, 5 = drilling
   point sym. glass edge, 6 = drilling point asym. glass edge

    The calculation type must be the same for both muntin bars (horizontal/vertical).

4) Bit vector for transferring diagonal muntins in the grid. The following values apply here:
   0 = no diagonal muntin, 1 = diagonal muntin top left, 2 = diagonal muntin top right, 4 = diagonal muntin bottom
   left, 8 = diagonal muntin bottom right.
   Here any values can be linked in binary fashion. E.g. to transfer a diagonal muntin bottom left and bottom right,
   12 is required.

5) If this field is filled, the remaining muntin parameters will be ignored. The file must be located in the same
   directory as the EDI file. Each muntin item is transferred only once in case of a sample Georgian bar. Not once
   per bar. This guarantees that the prices are weighted correctly.

6) If a grid pattern is transferred by AWDesign file, the muntin's color code must be entered exactly as it appears in
   the AWDesign file.

7) If a grid pattern is transferred by AWDesign file, the muntin's color name must be entered exactly as it appears in
   the AWDesign file.

8) Code for muntin pads (0 = no muntin pads, 1 = with muntin pads)

9) Identifier for the interpretation of the drilling dimension (0=absolute dimension for each drilling point starting from
   the origin, 1=relative dimensioning starting from the immediately preceding drilling). Here, A+W Business only
   uses the dimensioning type 1. The value is only written by A+W Business during export. During import this value
   is ignored.


A+W Business: The dimensions in all parameter fields are to be understood as additional dimension for the
preceding drilling point and not as absolute dimension from the origin!

A+W Enterprise: The dimensions in all parameter fields must be transferred as absolute dimension from the origin!

10) See also section 4 - Item-related parameters (AWE)




A+W Software GmbH                                 EN-A+W EDI Import.docx                                                       55 / 162
2.25 Asymmetrical muntin record CA

Writing this record type is not mandatory if a muntin BOM record exists.
See also section 3 AWE „Asymmetrical muntin record CA“




                                                                                                    Contents
                                                                               Position


                                                                                          Length
        No
              Name




                                                                        Type
                                                                 Kind
        .


        1     Record type                                       M       A      1          2        CA
        2     Direction                                         K       N      3          3        0=horizontal
                                                                                                   1=vertical
        3     1. Muntin code                                    K       N      6          20
        4     2. Muntin code                                    K       N      26         20
        5     3. Muntin code                                    K       N      46         20
        6     4. Muntin code                                    K       N      66         20
        7     5. Muntin code                                    K       N      86         20
        8     6. Muntin code                                    K       N      106        20
        9     7. Muntin code                                    K       N      126        20
        10    8. Muntin code                                    K       N      146        20
        11    9. Muntin code                                    K       N      166        20
        12    10. Muntin code                                   K       N      186        20
        13    11. Muntin code                                   K       N      206        20
        14    12. Muntin code                                   K       N      226        20
        15    13. Muntin code                                   K       N      246        20
        16    14. Muntin code                                   K       N      266        20
        17    15. Muntin code                                   K       N      286        20
        18    16. Muntin code                                   K       N      306        20
        19    17. Muntin code                                   K       N      326        20
        20    18. Muntin code                                   K       N      346        20
        21    19. Muntin code                                   K       N      366        20
        22    20. Muntin code                                   K       N      386        20
        23    Filler                                            K       A      406        107
        Table: Asymmetrical muntin record


Reference point is always the left bottom corner




A+W Software GmbH                              EN-A+W EDI Import.docx                                             56 / 162
2.25.1 Example for muntin codes




Muntin code for the first vertical bar        1110 0000 0000 0000 0000

Muntin code for the second vertical bar       1111 0000 0000 0000 0000

Muntin code for the third vertical bar        1111 0000 0000 0000 0000

Muntin code for the first horizontal bar 1111 0000 0000 0000 0000

Muntin code for the second horizontal bar     1111 0000 0000 0000 0000

Muntin code for the third horizontal bar 1110 0000 0000 0000 0000




A+W Software GmbH                            EN-A+W EDI Import.docx      57 / 162
2.26 Text record T1

Writing this record type is not mandatory; it enables the definition of describing texts for products and items.

See also AWE „Text record T1“




                                                                                                      Contents
                                                                                 Position


                                                                                            Length
         No
                Name




                                                                          Type
                                                                   Kind
         .


         1      Record type                                       M       A      1          2        T1
         2      Text identifier                                   M       A      3          1
         3      Type ( 1=before item, 2=after item, 3=product)    M       N      4          1        1-3
         4      Text                                              M       A      5          480
         5      Text number                                       K       N      485        6
         6      Filler                                            M       A      491        22
         Table: Text record



2.27 Header/footer text record T2

Writing this record type is not mandatory; it enables the definition of header or footer texts for an order.

See also3.25
                                                                                                      Contents
                                                                                 Position


                                                                                            Length




         No
                Name
                                                                          Type
                                                                   Kind




         .


         1      Record type                                       M       A      1          2        T2
         2      Type                                              M       N      3          1        1=header;2=footer 1)
         3      Text identifier                                   M       A      4          1
         4      Text                                              M       A      5          480
         5      Filler                                            M       A      485        28
          Table: Text record 2

    1)    Currently Alfak only processes header texts! Incoming footer texts are interpreted as header texts.




A+W Software GmbH                                EN-A+W EDI Import.docx                                                     58 / 162
2.28 Template record V1 (only AWE, cf. Vg.160653)

This record type is not compulsory. It must be preceded by a P1 record. The record type permits to transfer template
parameters for an item when using SN. This record type is supported only by ALCIB. ALFAK ignores this record
type.

See also AWE „Template“




                                                                                                      Contents
                                                                                 Position


                                                                                            Length
              No.      Name




                                                                          Type
                                                                 Kind
              1        Record type                              M       A        1          2        V1
              2        Parameter string                         M       A        3          510      1)
                  Table: Template record


1) Parameter string the format of which can be defined by an ALCIB environment variable. Previously, control is
   implemented through the variable MODUL_SN_TEMPLATE. With an activated variable, the parameter string is
   interpreted by numeric values of the format 7.1. The parameters transferred (maximum 73) are saved in the table
   kpostemplate.




A+W Software GmbH                                EN-A+W EDI Import.docx                                              59 / 162
3 Import-specific field notes
Abbreviations:

IV = Interface version (from which on this field is supported)

AV = ALCIB version (from which on this field is supported)

NIU = Not In Use

NR =Not Read (not read by i000filter yet)


3.1       File header record FH
See also: AWB File header record and for AWE specific details section 4 File header record




      No.     Name                                    ALCIB note                             IV        PS


      1       Record type                                                                    2.2.000
      2       Version number                          nn.mm.zzz                              2.2.000
      3       Total characters                        Niu                                    2.2.000
      4       Sending company number                  Niu                                    2.2.010   3.1
      5       Receiving company number                *1                                     2.2.010   3.1
      6       Inch fraction                           Imperial system                        2.2.025   6,0
      7       User-defined field                      NIU                                    2.2.029
      8       Coding                                  *2                                     2.2.033   6.0
      7       Filler


          Table: File header record


*1: Glasmarkt speciality: If GLASMARKT=2 and CHECK_GLAMA_LINR = 2, the company name = the market
partner number in the $INDIR.

Starting with interface version 02.2.033:

*2: If the field is empty, the old processing will be used.

Accepted entries: ISO8859-1, ISO8859-2, ISO8859-15, UTF-8, 819(like ISO-1), 1250(like ISO-2), 1252(like ISO-
15), 57372(like UTF-8)




A+W Software GmbH                                 EN-A+W EDI Import.docx                                     60 / 162
3.2       General header record K1
See also 2.2 AWB "Header record general"




      No.    Name                             ALCIB note                                     IV        PS


      1      Record type                                                                     2.2.000

      2      Document type                    1=quotation, 2=order, 3=credit, 4=quotation,   2.2.015
                                              5=order, 9 – Product Type

      3      Mode                             NIU                                            2.2.000
                                              4 – Reserved for new development in AWE
                                              [AW-162329]

      4      Customer no.                     Customer number                                2.2.000
      5      Delivery date                    Requested customer delivery date (if empty,    2.2.000
                                              then today); format: yyyymmdd
      6      P.O. date                        NIU                                            2.2.000

      7      Purchase text 1                  External number or purchasing info             2.2.000
                                              See section 4 "External P.O. text"
      8      Purchase text 2                  Dispatch Info                                  2.2.000
                                              See section 4 "External P.O. text"
      9      Predefined document number       NIU                                            2.2.000
      10     Bill of landing number           NIU                                            2.2.000
      11     Site number                      NIU                                            2.2.000
      12     Height above nn (in meters)      See section 4 "Height above nn"                2.2.000
      13     Status                           NIU                                            2.2.001   3.1
      14     KZ locked                        NIU                                            2.2.001   3.1
      15     Delivery code                    0=no direct delivery                           2.2.003   3.1
                                              1 =direct delivery by supplier
                                              2 = pick-up by customer (not supported by
                                              Alfak 2000)
                                              See section 4 "Delivery code"
      16     User-defined field               1) Allows to transfer customized data.         2.2.015   2008
                                              However, this requires programming                       (4.2)
                                              amendments in the ERP system.
                                              (Environmental variable
                                              DFUE_PRIVATE_K1)
                                              See section 4 "User-defined field"
      17     Priority                         Transferring priority (kauf.schnell)           2.2.023   2009
                                              See section 4 "Priority"                                 (4.4)
      18     Object                           Transferring an object (kauf.objnr)            2.2.023   2009
                                              See section 4 "Object"                                   (4.4)




A+W Software GmbH                          EN-A+W EDI Import.docx                                              61 / 162
     No.   Name                        ALCIB note                  IV        PS


     19    Architect                   Takeover of an A/Z debtor   2.2.023   2011
                                       See section 4 "AZ debtor"
     20    Delivery date               NIU                         2.2.027
     21    Production preparation      NIU                         2.2.028
     22    Business type               NIU                         2.2.028
     23    Filler                      NIU




A+W Software GmbH                   EN-A+W EDI Import.docx                          62 / 162
3.3       Address header record K2
See also 2.3 AWB "Address " and AWE section 4 "Addresses"




      No.      Name                                   ALCIB note                                  IV        PS


      1        Record type                                                                        2.2.000
      2        Customer address - name 1              Name                                        2.2.000
      3        Customer address - name 2              Attn / First name
                                                      To be controlled via environment variable
                                                      DFUE_NAME2_VORNAME                          2.2.000
                                                      See section 4 "Addresses"
      4        Customer address - name 3              NIU                                         2.2.000
      5        Customer address - street              Street                                      2.2.000
      6        Customer address - city                Town                                        2.2.000
      7        Customer address - zip code            PCd                                         2.2.000
      8        Customer address - post box            NIU                                         2.2.000
      9        Customer address - post box - zip      NIU
                                                                                                  2.2.000
               code
      10       Customer address - country code        Country code                                2.2.000
      11       Customer address - province/state      Country name                                2.2.000
      12       Customer address - fax                 Fax no.                                     2.2.000
      13       Customer address - phone               Phone no.                                   2.2.000
      14       Customer address - employee            NIU                                         2.2.015   NR
      15       Filler
          Table: General header record




A+W Software GmbH                                  EN-A+W EDI Import.docx                                        63 / 162
3.4       Shipping address header record K3

See also AWB "Delivery Address" and AWE section 4 " insert segmentsDelivery Address"




      No.      Name                                   ALCIB note                                  IV        PS


      1        Record type                                                                        2.2.000
      2        Shipping address - no.                 NIU                                         2.2.000
      3        Shipping address - name 1              Name                                        2.2.000
      4        Shipping address - name 2              Attn / First name
                                                      To be controlled via environment variable
                                                      DFUE_NAME2_VORNAME                          2.2.000
                                                      See section 4 "Addresses"
      5        Shipping address - name 3              Addition                                    2.2.000   5.1
      6        Shipping address - street              Street                                      2.2.000
      7        Shipping address - city                Town                                        2.2.000
      8        Shipping address - zip code            PCd                                         2.2.000
      9        Shipping address - province/state      Country name                                2.2.000
      10       Shipping address - country code        Country code                                2.2.000
      11       Delivery request                       Special configuration
                                                      Controlled by environment variables         2.2.000
                                                      DFUE_EDI_LIEFERWUNSCH
      12       Shipping address - phone               niu                                         2.2.015   NR
      13       Shipping address - employee            niu                                         2.2.015   NR
      14       Filler
          Table: Shipping address header record




A+W Software GmbH                                  EN-A+W EDI Import.docx                                         64 / 162
3.5       Invoice address header record K4

See also2.5




      No.      Name                                  ALCIB note                                  IV         PS


      1        Record type                                                                       2.2.000
      2        Invoice address - no.                 NIU                                         2.2.000
      3        Invoice address - name 1              Name                                        2.2.000
      4        Invoice address - name 2              Attn / First name
                                                     To be controlled via environment variable
                                                     DFUE_NAME2_VORNAME                          2.2.000
                                                     See section 4 "Addresses"
      5        Invoice address - name 3              NIU                                         2.2.000
      6        Invoice address - street              Street                                      2.2.000
      7        Invoice address - city                Town                                        2.2.000
      8        Invoice address - zip code            PCd                                         2.2.000
      9        Invoice address - post box            NIU                                         2.2.000
      10       Invoice address - post box - zip      NIU
                                                                                                 2.2.000
               code
      11       Invoice address - country code        Country code                                2.2.000
      12       Invoice address - province/state      Country name                                2.2.000
      13       Invoice date                          NIU                                         2.2.000
      14       Invoice number                        NIU                                         2.2.000
      15       Filler
          Table: Invoice address header record




3.6       Header record extensions 1 K5


      No.      Name                                  ALCIB note                                  IV         PS


      1        Record type                                                                       2.2.0.29
      2        Tax                                   NIU                                         2.2.0.29
      3        Tax amount                            NIU                                         2.2.0.29



A+W Software GmbH                                 EN-A+W EDI Import.docx                                         65 / 162
      No.   Name                       ALCIB note                                 IV         PS


      4     Production start date      NIU                                        2.2.0.29
      5     LG start date              NIU                                        2.2.0.29
      6     Production end date        NIU                                        2.2.0.29
      7     Route                      NIU                                        2.2.0.29
      8     Delivery terms             NIU                                        2.2.0.29
      9     Document Type              See alsoHeader record extension 1          2.2.0.29
      10    Packing                    NIU                                        2.2.0.29
      11    Consultant                 NIU                                        2.2.0.29
      12    Sales Representative       NIU                                        2.2.0.29
      13    Original P.O. number       NIU                                        2.2.0.29
      14    Route number               NIU                                        2.2.0.29
      15    Filler




3.7       Header record down payments A1


      No.   Name                       ALCIB note                                 IV         PS


      1     Record type                                                           2.2.0.29   6.0
      2     Payment date               YYYYMMDD                                   2.2.0.29   6.0
      3     Payment mode               NIU                                        2.2.0.29   6.0
      4     Payment number                                                        2.2.0.29   6.0
      5     Payment procedure          See alsoHeader record - down payments A1   2.2.0.29   6.0




A+W Software GmbH                   EN-A+W EDI Import.docx                                         66 / 162
      No.      Name                                  ALCIB note                                 IV         PS


      6        Payment direction                     1=Payment credit note                                 6.0
                                                                                                2.2.0.29
                                                     -1=Payment cancelled
      7        Currency                              See alsoHeader record - down payments A1   2.2.0.29   6.0
      8        Amount                                                                           2.2.0.29   6.0
      9        Payment reference – Order                                                        2.2.0.29   6.0
      10       Exchange rate Currency                Example : 000000000100 if currency =                  6.0
                                                                                                2.2.0.29
                                                     EUR and the document is entered in EUR
      11       Filler                                                                           2.2.0.29   6.0
          Table: Header record down payments




3.8       Document link header record DL

See also2.8




      No.      Name                                  ALCIB note                                 IV         PS


      1        Record type                                                                      2.2.018    2011
      2        Description of document link          NIU                                        2.2.018    2011
      3        Relative link to linked document      See section 4 "Document link"              2.2.018    2011
      4        Filler
          Table: Header record document link



3.9       Header record private KP

See also 2.10 Kopfsatz Privat KP




      No.      Name                                  ALCIB note                                 IV         PS


      1        Record type                                                                      2.2.031
      2        Private_long1                         kauf._private_long1                        2.2.031
      3        Private_long2                         kauf._private_long2                        2.2.031
      4        Private_char1                         kauf._private_char1                        2.2.031


A+W Software GmbH                                 EN-A+W EDI Import.docx                                          67 / 162
     No.      Name                               ALCIB note                          IV        PS


     5        Private_char2                      kauf._private_char2                 2.2.031
     6        Filler                                                                 2.2.031
         Table: Header record document link


See also Fehler! Verweisquelle konnte nicht gefunden werden. Fehler! Verweisquelle konnte nicht gefunden
werden..




A+W Software GmbH                             EN-A+W EDI Import.docx                                68 / 162
3.10 Item record P1
See also AWB "Item record" and AWE section 4 " insert segmentsItem record"




     No.     Name                                   ALCIB note                                 IV        PS


     1       Record type                                                                       2.2.000
     2       Product no.                            3) Product sets                            2.2.000
     3       Description1                           Only 30 characters                         2.2.000
     4       Bezeichnung2 (designation2)            Only 30 characters                         2.2.000
     5       Bezeichnung3 (designation3)            Only 30 characters                         2.2.000
     6       Color                                  1)                                         2.2.000
     7       Short Name                             NIU                                        2.2.000
     8       Width (mm)                             Dimensional precision                      2.2.000
     9       Height (mm)                            Dimensional precision                      2.2.000
     10       Quantity                                                                         2.2.000
     11      Item price                             Item net price/piece                       2.2.000
     12      Sense of pattern                                                                  2.2.000
     13      Pattern side                                                                      2.2.000
     14      Reference                                                                         2.2.000
     15      Customer item                                                                     2.2.000
     16      Total installation thickness (mm)      NIU                                        2.2.000
     17      Edge protection                                                                   2.2.000
     18      Deduction for rebate (mm)              NIU                                        2.2.000
     19      KZ locked                              NIU                                        2.2.001   3.1
     20      Free                                   See also Free of charge flag ; Complaint   2.2.001   3.1
     21      Single cutback                                                                    2.2.001   3.1
     22      Coated side                            NIU                                        2.2.009   3.2
     23      Dimensional variant                    2)                                         2.2.014   3.2
     24      Procurement type                       NIU                                        2.2.016   NR
     25      Price relevance identifier             NIU                                        2.2.022
     26      Price type                             NIU                                        2.2.026
     27      Filler
         Table: General item record




A+W Software GmbH                                EN-A+W EDI Import.docx                                        69 / 162
   1) If the color begins with "@" (ASCII Code 40hex), the target system assumes that the date is the foreign key
      for the color.

       In the "Color" field, a color name is sent (e.g. white). The color number for this color name is determined in
       the ALCIB color keys (Master data - Keys - Product keys – Colors).If the first character in field "color“ is "@",
       a number is expected right after that (e.g: @2 or @002). This number is interpreted as the ALCIB color
       number. Field "Color“ can still process external information regarding the color. Structure "@@code@value"
       (e.g @@RAL@9010; @@EAN@880110100003) is intended for this purpuse. To determine an ALCIB color
       number based on these two entries (code and color information), use the stored procedure
       cu_dfue_getfarbe() with the parameters: code, color information, customer number, sequential order number,
       item number, customer article number, client number.


   2) This field is supported only by ALCIB; ALFAK neither reads nor writes it. (see section 4 „Dimensional
      variant“)

       In the dimensional variant field, a constant number is transferred. Currently, this is 1 which means: If 1 is
       transferred in field 23, the import routine tries - by means of the sizes entered in field 8 "width" and 9 "height"
       - to determine the corresponding ALCIB variant number. For this purpose, the stored procedure
       cu_dfue_getbitnr() with the parameters: customer number, sequential order number, item number, customer
       article number, and client number is loaded.

       If the dimensional variant begins with an @ (ASCII CODE 40hex), then a number is expected right
       afterwards (e.g.: @2 or @003). This number is interpreted as the ALCIB variant number.

       Within the "dimensional variant" field, additional third-party information with respect to variants can be
       processed. The structure provided for this is "@@code@value" (e.g @@RAL@9010;
       @@EAN@880110100003). In order to determine an ALCIB variant number from this information (code and
       variant information), the stored procedure cu_dfue_getvar() is called with the parameters Code,
       Varianteninformation, Kundennummer, Sequentielle Auftragsnummer, Positionsnummer,
       Kundenartikelnummer, Mandantennummer.

   3) If the product number begins with an "@" (ASCII code 40hex), it is assumed that the item being transferred is
      a product set. For this, A+W Enterprise must be configured for the entry of product sets. In addition, the
      order scheduling must be configured for the use of product sets. Both functions are modules for which you
      must pay. (See also section 4 "Product Type")




A+W Software GmbH                               EN-A+W EDI Import.docx                                             70 / 162
3.11 Item record P2
See also2.12




     No.      Name                                     ALCIB note                                     IV         PS


     1        Record type                                                                             2.2.000
     2        Logo no.                                 NIU                                            2.2.000
     3        Logo position                            NIU                                            2.2.000
     4        Rack Type                                NIU                                            2.2.000
     5        Lites per rack                           NIU                                            2.2.000
     6        Document reference                       kposzusatz.dokuref                             2.2.000
     7        Item reference                           kposzusatz.posref                              2.2.000
     8        Item group of order                      NIU                                            2.2.000
     9        Item text 1                              NIU                                            2.2.000
     10       Item text 2                              NIU                                            2.2.000
     11       Item text 3                              NIU                                            2.2.000
     12       Item text 4                              NIU                                            2.2.000
     13       Item text 5                              NIU                                            2.2.000
     14       Edge decoating                           NIU                                            2.2.001    3.1
     15       Foreign key for complaints               The first occurrence is transferred to the     2.2.001    4.4
                                                       order header (kauf._reklamart)                            1)

     16       Restriction check for alternative        NIU                                            2.2.001    3.1
              products
     17       Benutzerdefiniertes Feld                 NIU                                            2.2.015    NR
     18       Reason for complaint                     2) See also Item extension (P2) 4)             2.2.029
     19       Complaint place                          3) See also Item extension (P2) 4)             2.2.029
     18       Filler
         Table: Item record supplement


   1) If the first (!) character is @, the program expects a number after that. This number is interpreted as ALCIB-
      internal number for the type of complaint.

          If the first character is not an @, the complaint specification is transferred as a text and through the call of
          the customer-specific SP
          cu_dfue_getcompltype(p_custcompl CHAR(10), p_customer INTEGER, p_aufnr INTEGER, p_site SMALLINT)
          RETURNING SMALLINT;
          Parameter: complaint text sent in the interface
                     Customer number
                     Order number
                     Site number
          Return value: ALCIB-type of complaint
          Translated into the ALCIB complaint type.



A+W Software GmbH                                  EN-A+W EDI Import.docx                                              71 / 162
    2) If the complaint reason begins with "@" (ASCII Code 40hex), the target system assumes that the date is the
       foreign key for the complaint reason. The character string can also start with a "#". Then, the sequence
       number is checked.

    3) If the complaint place begins with "@" (ASCII Code 40hex), the target system assumes that the date is the
       foreign key for the complaint place. The character string can also start with a "#". Then, the sequence
       number is checked.

Examples for 2) and 3):

                    -   Alphanumeric @BRUCH_GRUND@ or @PRODUKTION_ORT@

                    -   Numeric: #123456#

    4) If the reason for complaint and/or complaint location should be set, then you can use a P3/2 reference to the PO
       number directly before to communicate the original order number. This order number is then written to the
       database field kauf.referenz and serves as reference to the original order. (#455928)

        See also: 4.8.4 Reklamationsauftrag




A+W Software GmbH                               EN-A+W EDI Import.docx                                            72 / 162
3.12 Item record P3


See also AWB "Item record P3" and AWE section 4 " insert segmentsItem references"




     No.      Name                                 ALCIB note                       IV        PS


     1        Record type                                                           2.2.000   6.0
     2        Reference for previous P.O.          kposref.exbestnr                 2.2.000   6.0
              number
     3        Reference for previous item          kposref.exbestposnr              2.2.000   6.0
              number
     4        Reference for shipping order         kposref.exauftrnr                2.2.000   6.0
              number
     5        Reference for the shipping item      kposref.exauftrposnr             2.2.000   6.0
              number
     6        Reference for end customer's         kposref.exendbestnr              2.2.000   6.0
              P.O. number
     7        Reference for end customer's         kposref.exendposnr               2.2.000   6.0
              item number
     8        Filler
         Table: Item record supplement



3.13 Item private PP


See also AWE „Position Privat PP“




     No.      Name                                 ALCIB note                       IV        PS


     1        Record type                                                           2.2.031
     2        Private_long1                        kposp.privat_long1               2.2.031
     3        Private_long2                        kposp.privat_long2               2.2.031
     4        Private_char1                        kposp.privat_char                2.2.031
     5        Filler                                                                2.2.031
         Table: Position private PP




A+W Software GmbH                               EN-A+W EDI Import.docx                              73 / 162
3.14 Item record document link PL
See alsoFehler! Verweisquelle konnte nicht gefunden werden.




     No.     Name                                  ALCIB note                   IV        PS


     1       Record type                                                        2.2.018   2011
     2       Description of document link          NIU                          2.2.018   2011
     3       Relative link to linked document      See Section 4                2.2.018   2011
     4       Filler
         Table: Item record document link



3.15 Private table PT (item-related) (only AWE)
See also section 4 "Private tables (PT)"




     No.     Name                                  ALCIB note                   IV        PS


     1       Record type                                                                  6.0
     2       Table names                           Currently supported Tables             6.0
     3       Parameter string
                  Table: Template record




3.16 Item-related parameter PA (only AWE)
See section 4 Position-related parameters




A+W Software GmbH                               EN-A+W EDI Import.docx                           74 / 162
     No.    Name                                   ALCIB note                   IV         PS


     1      Record type                                                         2.2.0.29   6.0
     2      Record type                            Flag for type of parameter   2.2.0.29   6.0
     3      Parameter 1                                                         2.2.0.29
     4      Parameter 2                                                         2.2.0.29
     5      Parameter 3                                                         2.2.0.29
     6      Parameter 4                                                         2.2.0.29
     7      Parameter 5                                                         2.2.0.29
     8      Parameter 6                                                         2.2.0.29
     9      Parameter 7                                                         2.2.0.29
     10     Parameter 8                                                         2.2.0.29
     11     Filler
                Table: Item-related parameter


   1) If record type = 1  Window frame overlap (offset frame)

         Parameter 1-4 are expected

         Offset frame sides parameter 1-4  1=bottom, 2=right, 3=top, 4=left




A+W Software GmbH                               EN-A+W EDI Import.docx                           75 / 162
3.17 BOM record S1
See also AWB „BOM record“




    No.   Name                                 ALCIB note                                             IV         PS


    1     Record type                                                                                 2.02.000
    2     Number (number)                      NIU                                                    2.02.000
    3     Parent number (0=main product)                                                              2.02.000
    4     Level                                                                                       2.02.000
    5     Position within level                                                                       2.02.000
    6     Product no.                                                                                 2.02.000
    7     Name                                                                                        2.02.000
    8     Color                                1)                                                     2.02.000
    9     Short Name                           NIU                                                    2.02.000
    10    Width (mm)                           Dimensional precision                                  2.02.000
    11    Height (mm)                          NIU                                                    2.02.000
    12     Quantity                                                                                   2.02.000
    13    Unit price (do not multiply with     NIU                                                    2.02.000
          main quantity)
    14    Sense of pattern                                                                            2.02.000
    15    Pattern side                         Exchange of a glass                                    2.02.000
    16    Product type                         3)                                                     2.02.000
    17    Product group                        3)                                                     2.02.007   3.1
    18    Coated side                          NIU / only evaluated for processings – not for glass   2.02.009   3.1
    19    Thickness (mm)                       2) Dimensional precision                               2.02.012   3.1
    20    Vector for production BOM            NIU                                                    2.02.015   NR
    21    User-defined field                   NIU                                                    2.02.015   NR
    22    Procurement type                     NIU                                                               NR
    23    BOM number from main article         NIU                                                               NR
    24    Price printing code                  NIU                                                               NR
    25    Modification code                    NIU                                                               NR
    26    Price relevance identifier           If the item should flow into the price                            AWE
                                                                                                      2.02.022
                                               calculation (set A/Z flag in BOM)                                 6
    27    Vector for production BOM 2          NIU                                                    2.02.024
    28    Price type                           NIU                                                    2.02.026
    29    Supplier of part                     NIU                                                    2.02.032
    30    Confirmed delivery date              NIU                                                    2.02.032
    31    Link ext. P.O./Order GUID (OMS)      NIU                                                    2.02.032
    32    Start barcode                        NIU                                                    2.02.034


A+W Software GmbH                            EN-A+W EDI Import.docx                                                    76 / 162
    No.     Name                                   ALCIB note                                    IV           PS


    33      Barcode type                           NIU                                           2.02.034
    34      Filler
         Table: BOM record, general



         1) If the color begins with "@" (ASCII Code 40hex), the target system assumes that the date is the foreign
            key for the color.

             In the "Color" field, a color name is sent (e.g. white). The color number for this color name is determined
             in the ALCIB color keys (Master data - Keys - Product keys – Colors).If the first character in field "color“
             is "@", a number is expected right after that (e.g: @2 or @002). This number is interpreted as the ALCIB
             color number. Field "Color“ can still process external information regarding the color. Structure
             "@@code@value" (e.g @@RAL@9010; @@EAN@880110100003) is intended for this purpose. To
             determine an ALCIB color number based on these two entries (code and color information), use the
             stored procedure cu_dfue_getfarbe() with the parameters: code, color information, customer number,
             sequential order number, item number, customer article number, client number.

         2) Is only exported by ALFAK. ALFAK ignores this field when importing.
            For product type =60 and product code=80 (IGU frame) the thickness is interpreted as SZR

         3) Not all product types and product groups that are possible in ALFAK are supported. Currently, the
            product types 1,2,3 are supported as glass replacement. For product type 40, product group 3 is
            supported as a basic miscellaneous article. In product type 60, product group 80 is supported as a
            spacer replacement or AIR transfer.

             Product type 12 + product group 50 are expected for steps.

             (see section 4 „Supported product types and groups“)




A+W Software GmbH                                EN-A+W EDI Import.docx                                            77 / 162
3.18 Shape record M1
See also2.20

For A+W Enterprise, the parameters have to be filled correctly – also for shape 99. [AW-73649]




     No.     Name                                 ALCIB note                              IV        PS


     1       Record type                                                                  2.2.000
     2       Shape number/ 999=steps              Until shape 115
                                                  Starting with AWE 5: Until shape        2.2.000
                                                                                                    AWE5
                                                  999
     3       SN name                              Shape designation                       2.2.000
     4       Parameter 1 (mm)                                                             2.2.000
     5       Parameter 2 (mm)                                                             2.2.000
     6       Parameter 3 (mm)                                                             2.2.000
     7       Parameter 4 (mm)                                                             2.2.000
     8       Parameter 5 (mm)                                                             2.2.000
     9       Parameter 6 (mm)                                                             2.2.000
     10      Parameter 7 (mm)                                                             2.2.000
     11      Parameter 8 (mm)                                                             2.2.000
     12      Reference lite for steps             Bit vector                              2.2019    4.5
     13      Filler
         Table: Shape record


    See also ALCIB-specific function description, point "Step (M1)" in section 4




A+W Software GmbH                              EN-A+W EDI Import.docx                                      78 / 162
3.19 Processing record B1
See also2.21




     No.   Name                ALCIB note              IV        PS


     1     Record type                                 2.2.000
     2     Parameter 1         Dimensional precision   2.2.000
     3     Parameter 2                                 2.2.000
     4     Parameter 3                                 2.2.000
     5     Parameter 4                                 2.2.000
     6     Parameter 5                                 2.2.000
     7     Parameter 6                                 2.2.000
     8     Parameter 7                                 2.2.000
     9     Parameter 8                                 2.2.000
     10    Parameter 9                                 2.2.000
     11    Parameter 10                                2.2.000
     12    Parameter 11                                2.2.000
     13    Parameter 12                                2.2.000
     14    Parameter 13                                2.2.000   AWE5.4
     15    Parameter 14                                2.2.000   AWE5.4
     16    Parameter 15                                2.2.000   AWE5.4
     17    Parameter 16                                2.2.000   AWE5.4
     18    Parameter 17                                2.2.000   AWE5.4
     19    Parameter 18                                2.2.000   AWE5.4
     20    Parameter 19                                2.2.000   AWE5.4
     21    Parameter 20                                2.2.016   AWE5.4
     22    Parameter 21                                2.2.016   AWE5.4
     23    Parameter 22                                2.2.016   AWE5.4
     24    Parameter 23                                2.2.016   AWE5.4
     25    Parameter 24                                2.2.016   AWE5.4
     26    Parameter 25                                2.2.016   AWE5.4
     27    Parameter 26                                2.2.016   AWE5.4
     28    Parameter 27                                2.2.016   AWE5.4
     29    Parameter 28                                2.2.016   AWE5.4
     30    Parameter 29                                2.2.016   AWE5.4
     31    Parameter 30                                2.2.016   AWE5.4
     32    Filler




A+W Software GmbH           EN-A+W EDI Import.docx                        79 / 162
        Table: Processing record

The processing list is as yet invalid for the import into ALCIB. For a detailed list of all supported processing types,
please see item 4.12




A+W Software GmbH                                EN-A+W EDI Import.docx                                             80 / 162
3.20 Processing record B2
See also2.22




     No.   Name                                     ALCIB note            IV        PS


     1     Record type                                                    2.2.000
     2     internal order number                                          2.2.000
     3     internal item number                                           2.2.000
     4     Customer number                                                2.2.000
     5     Item that is exchanged or for which
                                                                          2.2.000
           there is an additional item
     6     Item type that is exchanged and for
                                                                          2.2.000
           which there is an additional item
     7     Exchange/supplement article                                    2.2.000
     8     Exchange/supplement indicator                                  2.2.000
     9     new assembly position                                          2.2.000
     10    Parent article (product)                                       2.2.000
     11    Customer-specific article number                               2.2.000
     12    Project #                                                      2.2.000
     13    Quantity1 (widths)                                             2.2.000
     14    Quantity2 (heights)                                            2.2.000
     15    Original assembly position where
           the exchange or supplement takes                               2.2.000
           place
     16    Sense of pattern                                               2.2.000
     17    Print code                                                     2.2.000
     18    Price calculation code                                         2.2.000
     19    Color number                                                   2.2.000
     20    Size parameter 1                                               2.2.000
     21    Size parameter 2                                               2.2.000
     22    Size parameter 3                                               2.2.000
     23    Positioning 1                                                  2.2.000
     24    Positioning 2                                                  2.2.000
     25    Positioning 3                                                  2.2.000
     26    Edge vector                                                    2.2.000
     27    Market partner type                                            2.2.000
     28    Priority                                                       2.2.000
     29    Article text that should be used as
                                                    NIU                             NR
           a replacement



A+W Software GmbH                                EN-A+W EDI Import.docx                  81 / 162
3.21 Bar code record BC
See also2.23




     No.   Name              ALCIB note                              IV        PS


     1     Record type                                               2.2.000
     2                       20 characters kposzusatz.barcode.char
                                                                               3.1
                             80 characters kposzusatz.txt
           Barcode                                                   2.2.000
                                                                               AWE
                             As item text (configuration                       6
                             DFUE_BCAST1)
     3     Filler




A+W Software GmbH         EN-A+W EDI Import.docx                                     82 / 162
3.22 Muntin record C1
See also2.24




     No.   Name                               ALCIB note                                  IV        PS


     1     Record type                                                                    2.2.000
     2     Type                               NIU                                         2.2.000
     3     Calculation type                   The transfer of the calculation type must
                                              be configured appropriately in ALCIB
                                              (DFUE_SPROSSSYMKZ), no different            2.2.000
                                              calculation types are permitted within an
                                              item
     4     Direction                                                                      2.2.000
     5     Parameter 1 (mm)                   Dimensional precision                       2.2.000
     6     Parameter 2 (mm)                                                               2.2.000
     7     Parameter 3 (mm)                                                               2.2.000
     8     Parameter 4 (mm)                                                               2.2.000
     9     Parameter 5 (mm)                                                               2.2.000
     10    Parameter 6 (mm)                                                               2.2.000
     11    Parameter 7 (mm)                                                               2.2.000
     12    Parameter 8 (mm)                                                               2.2.000
     13    Parameter 9 (mm)                                                               2.2.000
     14    Parameter 10 (mm)                                                              2.2.000
     15    Parameter 11 (mm)                                                              2.2.000
     16    Parameter 12 (mm)                                                              2.2.000
     17    Parameter 13 (mm)                  NIU                                         2.2.000
     18    Parameter 14 (mm)                  NIU                                         2.2.000
     19    Parameter 15 (mm)                  NIU                                         2.2.000
     20    Parameter 16 (mm)                  NIU                                         2.2.000
     21    Parameter 17 (mm)                  NIU                                         2.2.000
     22    Parameter 18 (mm)                  NIU                                         2.2.000
     23    Parameter 19 (mm)                  NIU                                         2.2.000
     24    Parameter 20 (mm)                  NIU                                         2.2.000
     25    Number of muntins                                                              2.2.002   3.1
     26    Muntin pads code                   NIU                                         2.2.011   NR
     27    Bit vector diagonal bars           NIU                                         2.2.020   NR
     28    AWDesign filename                  NIU                                         2.2.020   NR
     29    Color code of muntin in AWDesign
                                              NIU                                         2.2.020   NR
           file
     30    Muntin color name in AWDesign
                                              NIU                                         2.2.020   NR
           file


A+W Software GmbH                          EN-A+W EDI Import.docx                                         83 / 162
      No.     Name                                  ALCIB note                                  IV        PS


      31      Dimension type of the drilling
                                                                                                2.2.025
              dimension
      32      Simulated Divided Lite Bar Size                                                   2.2.029
      33      Filler
          Table: Muntin record

          A+W Enterprise: The dimensions in all parameter fields must be transferred as absolute dimension from the
origin!




A+W Software GmbH                                EN-A+W EDI Import.docx                                        84 / 162
3.23 Asymmetrical muntin record CA
This record must mandatory be written into AWE.

See also section 2 AWB "Asymmetrical muntin record CA"




     No.     Name                                 ALCIB note          IV   PS


     1       Record type
     2       Direction
     3       1. Muntin code
     4       2. Muntin code
     5       3. Muntin code
     6       4. Muntin code
     7       5. Muntin code
     8       6. Muntin code
     9       7. Muntin code
     10      8. Muntin code
     11      9. Muntin code
     12      10. Muntin code
     13      11. Muntin code
     14      12. Muntin code
     15      13. Muntin code                      NIU
     16      14. Muntin code                      NIU
     17      15. Muntin code                      NIU
     18      16. Muntin code                      NIU
     19      17. Muntin code                      NIU
     20      18. Muntin code                      NIU
     21      19. Muntin code                      NIU
     22      20. Muntin code                      NIU                      3.1
     23      Filler
         Table: Asymmetrical muntin record




A+W Software GmbH                            EN-A+W EDI Import.docx              85 / 162
3.24 Text record T1
See also AWB "text record T1"




     No.      Name                                     ALCIB note            IV        PS


     1        Record type                                                    2.2.000
     2        Text identifier                          NIU                   2.2.000
     3        Type ( 1=before item, 2=after item,      NIU
                                                                             2.2.000
              3=product)
     4        Text                                                           2.2.000   3.1
     5        Text number                              NIU                   2.2.006   NR
     6        Filler
         Table: Text record




3.25 Header/footer text record T2
See also2.27




     No.      Name                                     ALCIB note            IV        PS


     1        Record type                                                    2.2.005   3.1
     2        Type                                                           2.2.005   3.1
     3        Text identifier                          NIU                   2.2.005   3.1
     4        Text                                                           2.2.005   3.1
     5        Filler
          Table: Text record 2




A+W Software GmbH                                   EN-A+W EDI Import.docx                   86 / 162
3.26 Template record V1 (only ALCIB, see op. 160653)
See also0




     No.    Name                           ALCIB note            IV   PS


     1      Record type                                               4.4
     2      Parameter string                                          4.4
               Table: Template record




A+W Software GmbH                       EN-A+W EDI Import.docx              87 / 162
4 A+W Enterprise import-specific function description
For the takeover into the ERP system, it must be noted that the functions used are not Unicode capable.


4.1   General Information
      As of ALCIB -version 3.1, the interface version is read. If it is higher or equal to 02.2.010, the delivered
      interface version is analyzed. Some new functions are only made available as of certain interface versions.
      See the interface description (abbreviation "NIU" in column "ALCIB") for information as to which fields are not
      analyzed.
      In addition to this documentation on the functions of the standard interface, there is a documentation on
      general functions of external entry available (Extern_Leitfaden_externe_Auftragsübertragung.doc). This
      document describes the scope of functions that are potentially available to all external order interfaces.

4.2   File header record
       As of ALCIB version 3.1

       With interface version 02.2.010, the following changes were implemented:

           1. As of now, the interface version in the FH record is analyzed for new developments.

           2. Within the FH record, the fields
              4 - Sending company number and
              5 - Receiving company number
              were each extended by one place.

       The field "Receiving company number" can be used for a specific ALCIB restriction check.

       If the environment variables GLASMARKT=2 and CHECK_GLAMA_LINR=ON have been set, a check is
       run to determine whether the number at the end of the IN-directory $INDIR/<nummer> matches the
       "receiving company number" that is transferred in the interface.

       ATTENTION: The environment variable GLASMARKT is linked with other special logic.

       Imperial system (inch): Starting with AWE Version 6 an interface version 02.2.025, in the FH record an
       inch fraction can be specified. If the value is greater than 1, the measurement parameters:
       P1:width
       P1:height
       S1:thickness
       M1:<all parameter fields>
       B1B1:<all parameter fields, insofar as they are dimensions for A+W processing types>
       C1:<all parameter fields>
       V1:Parameters according to master data definition
       in inches expected (Inch * Fraction).

       e.g. inch fraction = 64; a glass with a width of 100 inches should be transferred. Then in the field
       P1:width, the value "064000" must be transferred. (100 inch * 64 =6400 => and then the format 6.1 =>
       „064000“).

       Starting with AWE Version 6 and the interface version 02.2.033, under the field FH/9 it will be possible to
       enter a coding type for the incoming file. In the i000filter, this coding is read out and it is then set whether
       the processing is run through with multibyte or singlebyte processing. If the field is empty, then the
       singlebyte processing will be used.

       Accepted entries: ISO8859-1, ISO8859-2, ISO8859-15,               UTF-8,   819(like   ISO-1), 1250(like    ISO-
       2), 1252(like ISO-15), 57372(like UTF-8)



A+W Software GmbH                               EN-A+W EDI Import.docx                                             88 / 162
A+W Software GmbH   EN-A+W EDI Import.docx   89 / 162
Order header (K1)
4.2.1 Document type
       From A+W Enterprise 5.4, you are able to import "product sets" using the standard interface. For this
       purpose, the value 9 is transferred in the field "document type". This value is not supported by A+W
       Business. In field "Order text 2", the external key of the product set is transferred.

       Product sets are imported into A+W Enterprise using kauf.vorgang = 14 and kauf.exbez2=product set key. If
       the product set with the transferred key already exists in the system, the existing product set is canceled and
       an email is sent to message distributor no. 71. The new product set is not imported.

       Currently, product sets must not be imported into a CallCenter client.

       In order to fully use the function, environment variable MODUL_PRODSET = 1 must be set.

       The use of a product set within an order is also implemented in the standard filter (#284739 / #352083 ). See
       the documentation for the P1 record in section 4 "Product sets"



       Field value                             Document in A+W Enterprise         Comment

       1                                       Quotation

       2                                       Order

       3                                       Credit note

       4                                       Quotation                          Starting with interface version
                                                                                  2.2.15

       4                                       Order                              Up to interface version 2.2.15

       5                                       Order                              Starting with interface version
                                                                                  2.2.15

       5                                       Quotation                          Up to interface version 2.2.15

       6                                       NIU

       9                                       Product Type



4.2.2 Mode
This mode is currently not evaluated in A+W Enterprise.

Starting with trm_ctrl <todo> a new mode 4 is introduced.



4.2.3 Delivery code
       Within the delivery identifier field, the customer can specify whether he would like to pick up the goods.

       In this field, there are currently the following options:

       0 – normal delivery to the stored delivery address or th address provided in the interface. The type of delivery
       and procurement is undertaken according to the system configuration and master data definition.



A+W Software GmbH                                 EN-A+W EDI Import.docx                                        90 / 162
        1- Direct delivery by a supplier. Here it must be noted that currently there is no conversion of the
           procurement types in the order by the system. If the item ordered has the standard procurement type
           production or stock, then no purchase order with another supplier is triggered. If in addition, the goods
           should be set to the procurement for a special supplier, then this must currently be implemented
           customer-specifically (#341924)

            The route of the order is set to the configured direct delivery route set in the system.

        2- Pick-up by the customer. The route of the order is set to the configured pick-up route set in the system.

September 2023

If there are multiple direct delivery or pickup routes, there must be at least one route each with a priority greater than
0. The smaller the number, the higher the priority.

4.2.4 User-defined field
        As of ALCIB -version 2008, the interface version 2.2.015.

        The analysis of the "user-defined field" is controlled by environment variable DFUE_PRIVATE_K1.

4.2.4.1 Contact person (#121073) (DFUE_PRIVATE_K1 = 1)
        With activated environment variable DFUE_PRIVATE_K1 = 1, the first thing checked is whether the user-
defined field consists of the string 'QT'. If so, this is a Sample quotation.
        If this is not a sample quotation, then the first 8 characters are interpreted as employee number of a contact
partner in the ALCIB customer master data and taken over according to kauf.busr and kauf.busrname.


4.2.4.2 Sample quotations (#180957) (DFUE_PRIVATE_K1 = 1)
        With activated environment variable DFUE_PRIVATE_K1 = 1, the first thing checked is whether the user-
        defined field consists of the string 'QT'. This character sequence (QT = quotation template) marks the
        document as a sample quotation.
        The Document type (field 2 of the K1 record) is not checked for a particular value for sample quotations,
        but it should be "1".

        The sample quotation is subsequently identified in further processing by trm_ctrl as kauf.vorgang=4 and
        kauf.kaufart=13.

4.2.4.3 Assigning private fields (#334558) (DFUE_PRIVATE_K1 = 2)
        With activated environment variable DFUE_PRIVATE_K1 = 2, the content of the field is broken up into
        individual partial strings. A pipe ("|" – ASCII 124) is expected as separator.
       |<Endcustomername>|<Endcustomerdeliverydate>|<Endcustomerroute>|<Endcustomerpackagingtype>|<En
dcustomer delivery type>



        String      Max.         Application                              Additional processing
                    length

        1           30           End customer name

        2           10           End customer delivery date

        3            5           End customer route

        4           40           End customer packaging type              Implementation in AWE - Packing
                                                                          type

        5           40           End customer delivery type               Implementation in AWE - Delivery


A+W Software GmbH                                EN-A+W EDI Import.docx                                             91 / 162
                                                                          type



The end customer name may be up to 30 characters long. If it is occupied, this name is taken over as original name
in the order header (kauf.orgname) and thus overrides the name of the actual customer from the master data or the
sent-along K2-K4 records. At the same time, the original first name is emptied. The remaining address components
are retained.

The end customer delivery date is expected as a 10-place piece of data. If it is sent and the process field
configuration set 7 is present, it is taken over after kaufprvfld.dateval1.

The end customer route may be a maximum of 5 characters long. If it is sent and the process field configuration set 7
is present, it is taken over after kaufprvfld.longval3.

4.2.4.4 Note (DFUE_PRIVATE_K1 = 3)
If the system is configured accordingly (DFUE_PRIVATE_K1 = 3), a text can be included in the private field in
header record K1. This text is included in the order as an information text with the priority “high”. At the same time
the order is not released.

4.2.5 Packaging type (AWE 6)
Currently, the end customer packaging type can only be sent via the private field of the K1 record! Whether and if the
transfer occurs is controlled via the environment variable DFUE_PRIVATE_K1.

The end customer packaging type may be a maximum of 40 characters long. There are the following possibilities

    a)    Text

          a)    If it is a simple text, there is an attempt to assign this text to a packaging type in Master data - Keys -
          System dispatch - Packaging types. Here, first there is a search with the customer language and then with
          the system language. If nothing is found, then the standard packaging type of the customer (not the end
          customer) is used.

    b)    @<number>

          If the first character is a '@' and it is followed directly by a number, this number is used as the key to be
          taken over directly for the packaging type. If this transferred key value cannot be found in the master data,
          the standard packaging type of the customer (not the end customer) is used.

    c)   @@<key>@<packagingtext>

         If the first two characters are '@@' then a stored procedure cu_dfue_getpacking() with the parameters 'Key,'
         'Packaging text,' 'Customer number,' 'Order number,' 'Company' is called.

    For this, the environment variable INTAUF_DFUE_VERPACKART = ON must be activated.

4.2.6 Delivery type (AWE 6)
Currently, the end customer delivery type can only be sent via the private field of the K1 record! Whether and if the
transfer occurs is controlled via the environment variable DFUE_PRIVATE_K1.

The end customer delivery type may be a maximum of 40 characters long. There are the following possibilities

    a)        Text

              If it is a simple text, there is an attempt to assign this text to a delivery type in Master data - Keys -
              System dispatch - Delivery types. Here, first there is a search with the customer language and then with
              the system language. If nothing is found, then the customer's delivery type (not that of the end
              customer) is used.


A+W Software GmbH                                EN-A+W EDI Import.docx                                             92 / 162
   b)        @<number>

             If the first character is a '@' and it is followed directly by a number, this number is used as the key to be
             taken over directly for the delivery type. If this transferred key value cannot be found in the master data,
             the standard delivery type of the customer (not the end customer) is used.

   c)        @@<key>@<deliverytext>

             If the first two characters are '@@' then a stored procedure cu_dfue_getlart () with the parameters
             'Key,'Delivery text,' 'Customer number,' 'Order number,' 'Company' is called.

   For this, the environment variable INTAUF_DFUE_LIEFERART = ON must be activated.



4.2.7 External P.O. text
        The ALCIB fields “customer order no.” or "external information" (kauf.exaufnr), "purchase information"
        (kauf.exbez1) and "shipping information" (kauf.exbez2) are currently filled in different ways. (Only from
        version 2007 (4.1), the shipping information is passed on to the order)
            a) kauf.exaufnr = K1 PO text 1 (characters 1- 20)
                kauf.exbez1 = Filename without ending (80 characters)
                kauf.exbez2 = K1 PO text 2

            b) with set variables DFUE_EXREF_FILE
               kauf.exaufnr = Filename without ending (maximum 20 characters)
               kauf.exbez1 = K1 PO text 1
               kauf.exbez2 = K1 PO text 2

            c) customer-specific (customer: 12)
                kauf.exaufnr = K1 PO text 1
                kauf.exbez1 = K1 PO text 2
                kauf.exbez2 = K1 PO text 2

            d) Configuration DFUE_POTEXT = 1
                kauf.exaufnr = K1 PO text 1 (characters 1-20)
                kauf.exbez1 = K1 PO text 1 (characters 21 – 40) + K1 PO text 2
                kauf.exbez2 = K1 PO text 2


        Caution: The environment variable DFUE_POTEXT overrides DFUE_EXREF_FILE. The environment
        variable DFUE_GLASPROFI overrides DFUE_POTEXT and DFUE_EXREF_FILE

        If the third-party information (kauf.exausnr) over the order header record is not occupied, however a
        "Reference to end customer PO number" is given within a P3 record, then this is forwarded as third-
        party information.

        If the external information (kauf.exaufnr) is not filled, but there is a frame, gas, and/or sealant exchange or
        this is a colored item, then the fixed keyword "FSG-EXCHANGE" (frame, sealant, gas) is entered.



4.2.8 Height above nn
        If the pressure compensation has been configured in the interface configuration (table exbartyp, artyp=6),
        there must be an entry with the prefix from exbartyp in exchange/supplement rules. (kuaz.kuartnr=<dav-
        prefix><n>). A number is expected directly after the prefix. This number defines as of which height a
        pressure compensation valve should be installed.

        If in the table exbartyp the entry with artyp=6 does not have a prefix, this causes errors when reading in the
        interface files.

A+W Software GmbH                                EN-A+W EDI Import.docx                                            93 / 162
       A+W Enterprise 6 - 16.01.2021: if in the table exbartyp, the entry with artyp=6 does not have a prefix, the
       pressure compensation counts as not configured.

       If the height in the K1 record is higher than the number in kuaz.kuartnr, the article that has been defined in
       the exchange/supplement rules is attached to the BOM.

       Imperial system (Inch): there is no conversion of the K1 value. Since the value itself is not stored in any
       AWE database table. The value is compared 1:1 with the master data. Thus it is irrelevant for the processing
       whether the value is transferred in meter or feet.

4.2.9 Priority
(#218899)

       As of ALCIB version 2009 (Release November 2013) and interface version 2.2.023 it is possible to add a
       priority in the K1 set.

       A new field is added in the external interface for the transfer of an urgent or call order. This new field with
       the name "Priority" is integrated into header record K1 and can have the following values:

       0 = Standard; 1 = Urgent, 9 = Call

       If the field is not required, it can be left blank. In this case, the import uses the value 0 for standard.

       If value 1 is transmitted, the generated order is labeled as urgent order (kauf.schnell = 1, kauf.abruf=2)

       If value 9 is transmitted, the generated order is labeled as call order (kauf._kaufart=9, kauf.abruf=1)

       In all other cases, the generated order is a "standard" order. The A+W standard filter makes no
       differentiation between priority <blank> and 0.



4.2.10 Object
      (#258397)

      As at ALCIB version 2009 (Release November 2013) and interface version 2.2.023, it is possible to add a
      project number in the K1 set. For this purpose, a new record with artyp=15 (default project) has to be created.

      Entry of the default project in exbartyp with artyp=15 for project and dfuetyp=19 for standard filter.

      Insert into exbeartyp values (19,15,'',<objnr>).

      If an object is added in the K1 set it has to be verified whether the project exists in the market partner master
      and if it is allocated to the customer of the order. If the project exists and is allocated, the project is transferred
      to the order. Here attention must be paid that when an A/Z debtor is defined in the object, that this A/Z
      debtor takes precedence over the A/Z debtor of the customer. A further result of the project number
      transfer into the interface is that the conditions of the project are already utilized for the price
      calculation during the order entry. (see also section A/Z debtor)

      If the sent project does not exist, is suspended or not allocated to the customer, the defined default project is
      allocated to the order. This is done so it is recognized that this is in fact a project order and can subsequently
      be corrected.

      In this case, mail 71 - note: Check external order entry with the text "The attached project could not be
      entered in case of order <order number> (customer <customer number>). The default project was used" is
      sent to a defined processor. At the same time the order is not released.

      Up to version 2011, mail no. 59 with the text "Order <order number> (customer <customer number>) contains
      a dummy article. The order is not released" Unfortunately, this is technically not possible any other way.

      If a project is attached in the interface which cannot be validated (see paragraph above) and if no valid default
      project is defined, the order is NOT entered. A defined operator receives the message:

A+W Software GmbH                                EN-A+W EDI Import.docx                                               94 / 162
      71 - note: Check external order entry (up to version 2011, No.59)

      An error has occurred at entry of the order >temporary serial order number> / order text <order text from
      interface file>. Please see protocol <protocol name> for further details.


      In addition, the message

      63 - Note: Incorrect master data definition for external order entry

      The project <project number> does not exist!

      is sent.

4.2.11 E/A debtor
      From interface version 02.2.023 on you can add an architect in K1 record. The architect matches the R/A
      debtor in A+W Enterprise.

      If a R/A debtor is transferred via interface, this R/A debtor takes precedence over the R/A debtor of an object
      maybe sent as well as the R/A debtor of customer.

      In case the transferred R/A debtor is not a valid customer in the A+W Enterprise master data, the R/A debtor
      of the customer is used.

      If Set = 7 is set and K 1 record is set with an architect, A+W Enterprise checks, whether this R/A debtor was
      maintained in the way that a calculation of discounts and surcharges was suppressed. (#415551) (KopfSet 7 -
      decval1 != 0 => contains the architect)

4.2.12 Initial ID
      By default, orders that are scheduled via the external order interface are marked with the initial ID "EDI"
      (kauf.eingang = 4).

      If the environment variable DFUE_ONLINE_TYP is set, the ID can be set to "Online" (kauf.eingang = 14).
      Which ID is evaluated during the scheduling must be discussed with Development. Currently it is possible to
      use the R/A debtor (field K1 "Architect") for this. For this, the environment variable
      DFUE_ONLINE_TYP="1<azdebitor>" must be activated. If the <azdebitor> defined in the environment
      variables is identical to the R/A debtor that is contained in the K1 record of the transfer file, the transaction is
      set to Online (kauf.eingang=14).


4.3   Addresses (K2 , K3, K4)
4.3.1 First name / Attn
       If the environment variable DFUE_NAME2_VORNAME is active, then the field "Name 2" of K2, K3 and the
       K4 record is interpreted as first name. If the variable is not active, then the field is interpreted as "Attn".

4.3.2 Invoice address
       For the customer address (kauf.org fields), it applies that the first K record wins. This means, when a K2
       record is sent, its data will be used and K3 and K4 are ignored. If no K2, but a K3 record is sent, then the
       K3 is used and K4 is ignored. If also no K3 is sent, but a K4, then the K4 is used; and if also no K4, i.e.
       only K1, then the data from the ALCIB master data is used.

       If you want to incorporate a "miscellaneous customer," you must send the K2 and the K3 record. The
       invoice address is in K2 and the delivery address in K3. In addition, DFUE_ORGFELDER must be set
       and name and location must be assigned, otherwise the data is overwritten with the master data by intauf




A+W Software GmbH                                EN-A+W EDI Import.docx                                             95 / 162
4.3.3 Delivery Address
       The following applies to the delivery address: If a K3 record exists, then it will be used and K2 and K4
       shall be ignored. If there is no K3 record, then use K2 and ignore K4. If no K3 or K2 exist, then use K4;
       and if none of these exist, then obtain it from the master.

       So that a sent delivery address can be read in correctly, at least one of the following fields must be filled:
       Name, First name, City, Street

       If you want to incorporate a "miscellaneous customer," you must send the K2 and the K3 record. The
       invoice address is in K2 and the delivery address in K3. In addition, DFUE_ORGFELDER must be set
       and name and location must be assigned, otherwise the data is overwritten with the master data by intauf

       Import of address data has also been extended in the standard interface. So far, the field "Name 3“ would
       not be imported for the three address records. As from release AWE5.1, this field will be imported into the
       address supplement and will be taken into account when searching for an existing address.




4.4   Header record extension 1 K5
      So far, only value K5/9 is read with this key. This is the document type, that is saved for A+W Enterprise in
      kauf._kaufart. First, there is a comparison with table alkaufart.

      EXEC SQL select kauftyp into :sSelKaufart
                    from alkaufart where bez = :helpKaufart;

      Both numerical and alpha-numerical value can be received via EDI. Value kaufart will be manipulated in exbin
      for order entry, this is why you must take care when transferring a value.
      This data field is primary for complaint orders, so that for receiving value = 2 (free-of-charge order) and a set
      value P1/20 – the receiving total item price will be zeroed. This happens already in i000filter!!!

4.5   Header record-down payments A1
      Fields payment procedure and currency code are transferred alpha-numerical to EDI. A+W Enterpise adjusts
      the fields as follows.

      Payment procedure (A1/5) depends on table xzahlm and checks, whether the transferred value exists in the
      database. ($select zmnr into $nr from xzahlm where fib matches $fib;)

      Currency code (A1/7) depends on table xwaehr. ($select wnr into $nr from xwaehr where kurzbez
      matches $kubez;)

      Both fields are transferred as numerical value and serve in A+W Enterprise for a simpler processing. If the
      values do not exist in database, value 0 is written at this place.


4.6   Header record document link DL
       From AWE 5.4, document links can be transferred via the external order interface. If the system is not
       configured for document links (environment variable DATEI_REF_PFAD), the order is imported, a
       process note is generated ("The order includes document attachments that cannot be processed") and
       the order is not released. In addition a corresponding note is shown in the interface protocol.
       WARNING: The system is not configered to support attachments to an order.
                    Please contact A+W implementation team.

       The sent document is expected in the same directory that includes the interface file. If the attached
       documents are saved in a sub-cirectory, a relative or absolute path must be specified in front of the file
       name. The path information must not include any server names. "/", as well as "\" are processed.




A+W Software GmbH                               EN-A+W EDI Import.docx                                             96 / 162
        The attached documents are copied to $DATEI_REF_PFAD/<auftrnr>/0. The original files remain in the
        transfer directory.

        (When configuring, please ensure that the trm_ctrl ftp has access to the server that is defined in the
        variables. You may want to use variable DFUE_DATEI_REF_PFAD.)


4.7    Item (P1)
       See also3.10

        For assigning the BOM number of an item, see separate documentation "DE-CONFIG-A+W Enterprise
        EDI"

4.7.1 Item split (AWE 6)
Starting with AWE 6 the system can be configured so that items are split according to specified criteria. The split item
is attached to the items already sent. According to which criteria an already-sent item is split into n items is defined
via environment variable DFUE_ITEM_SPLITT. (#337294)

4.7.2 Product sets (AWE 5.4)
        For this, A+W Enterprise must be configured for the entry of product sets. In addition, the order scheduling
        must be configured for the use of product sets. Both functions are modules for which you must pay.

4.7.2.1 Restriction
        If product sets should be used within the external transaction interface, it is absolutely necessary that each
        product set consist of precisely one item. Currently, no takeover of product sets with several items is
        possible.

        •   The product set name may not contain the following characters:
            ' ' (0x20) space (SPC)
            '\t' (0x09) horizontal tab (TAB)
            '\n' (0x0a) newline (LF)
            '\v' (0x0b) vertical tab (VT)
            '\f' (0x0c) feed (FF)
            '\r' (0x0d) carriage return (CR)

        •   Transfer of item texts is currently not possible.
            Starting with Version AWE 6 trm_ctrl build 13.04.4835 and alcib build 13.04.8649 (October
            2020).
            The external order storage can use this extension to forward item texts of product sets to the
            A+W Enterprise. If you follow a P1 record, which corresponds to a product set, with a T1
            record in the storage file, the text of the T1 record is assigned to the product set.
        •   Transfer of consignment is possible.

        •   Transfer of customer item (kuposnr) is possible.

        •   The takeover of an item price is possible (February 2020)

        •   The takeover of file attachments is possible (January 2021): here, however, you have to make sure that
            the attached document is not copied into a new order-specific directory, but rather remains in the old
            storage location. In the new order, reference is made to the storage location from the product set with a
            reference. This means that if the document is changed, it is changed in the product set and in all orders
            generated via external EDI in which the product set was used.

        •   Transfer of special texts to kspectxt via record type PT is not possible.




A+W Software GmbH                                EN-A+W EDI Import.docx                                           97 / 162
4.7.2.2 References
       Starting with A+W Enterprise 5.4, in the P1 record record, the product number field is evaluated in
       expanded fashion.

       If the product number begins with a "@" (ASCII code 40hex), it is assumed that the item being transferred
       is a product set.

       In the "Product number" field, the product set designation is sent (e.g. SpecialShower). For this product
       set designation, a corresponding product set is determined in the A+W Enterprise master data (Master
       data – Finished products – Product set). Here, first there is a search in the customer sent in the interface.
       If this does not succeed, then there is a search with the A/Z debtors defined in the customer sent. If this is
       also not successful, a search is done with the defined default product set customer (artyp= 17) defined in
       the interface configuration. If this is also not successful, the default item for product sets (artyp= 16)
       defined in the interface configuration is taken over as item in the order item. If the default item was used,
       the order is not released, but rather placed in the release pool. At the same time, a transaction note that
       indicates this circumstance is generated in the resulting order.

       Definition in the table exbartyp

       artyp= 16 – product set item

       artyp= 17- product set customer

       If the product number begins with a "@" (ASCII code 40hex), it is assumed that the item being transferred
       is a product set whose designation is first determined via a customer-individual stored procedure
       cu_dfue_getprodset(<kunde>,<order>,<item>,<sent product code>, <site>). This
       designation returned by the SP is then referenced in the further course as described above.

4.7.2.3 Dimension change
       If the P1 – record is a product set, the fields 8 "width" and/or 9 "height" will not be filled. If the fields are
       empty or contain a 0, then the master data dimensions of the product set are used as item dimensions. If
       one of the two fields is filled with a value != 0, this dimension is used as item dimension.

4.7.2.4 Exchange
       Within the product set, only the exchange of the header item is possible while retaining the processings
       defined in the product set. For this, a S1 record with level = 0 (field 4) and product type = 1,2 or 3 (field
       16) must be transferred.

       Within the storage program, a plausibility check for the exchange can be configured. If nothing is
       configured explicitly, the item type and item thickness are checked. With the environment variable
       DFUE_PRODSET_EXCHANGE_RESTRICT it is possible to define what is checked (additional checks
       can be programmed on request). The first place defines the checking of the item type and the second
       place the checking of the item thickness.

       IMPORTANT: no separators between the digits – blank characters mean 0

       "00" – no check

       "10" – only check item type

       "01" – only check item thickness

       "11" – check item type and item thickness (default)

       The check refers to the item in the product set with respect to the item sent as replacement. If the check
       is OK, the replacement is made. If not, the product set is taken over unchanged, the system e-mail 71 is
       sent, an appropriate transaction note is generated and the order is not released.

       Internal specification of an extension [AW-147503].


A+W Software GmbH                                EN-A+W EDI Import.docx                                             98 / 162
4.7.2.5 Shape
       Within the product set it is possible to change the shape dimensions and the shape number. This is both
       possible for product sets that were already entered as shape as well as for product sets without shape
       reference. For this a Shape record M1 must be sent according to the normal shape record specification.

       Within the storage program, a plausibility check for the shape reference can be configured. The change of
       the shape reference or shape dimension is not possible for insulated glass (item type 200), glass systems
       (item type 400), cast resin with step (item type 140 with 510 in the BOM) and LSG with steps (item type
       170 with 510 in the BOM).

       The check refers to the item in the product set. If the check is OK, the replacement is made. If not, the
       product set is taken over unchanged, the system e-mail 71 is sent, an appropriate transaction note is
       generated and the order is not released.

4.7.3 Dimensional precision (AWE 6)

       Previously, the external standard interface could be configured so that muntin dimensions in 1/10 mm were
       taken over.
       The item dimensions, shape dimensions and processing parameters, by contrast, could only be taken over in
       full mm. Starting with this version (AWE 6), the function for storage has been expanded.
       In order to be able to enter item dimensions in the manual transaction entry/changing in 1/10 mm, the system
       must in principle be configured for 1/10 mm. For this, the environment variable IMP_CTRL_NTEL_MM must
       be set. Within the standard interface, the environment variable DFUE_NTEL_MM is evaluated. If the
       variable DFUE_NTEL_MM is active, then all dimensions are taken over from the standard interface in 1/10
       mm.

       If the variable DFUE_NTEL_MM is not active, it is possible to control the individual dimensions separately.

           1. Shape dimensions.

               Since shape dimensions are also taken over into the item dimensions, it is not possible to take over
               shape dimensions in 1/10 mm if the item dimensions are not configured for 1/10 mm (see above).
               For this reason, shape dimensions that are sent in 1/10 mm in the interface are only rounded or
               taken over cut off. The standard behavior is that the places after the decimal point that are set are
               cut off. With the environment variables DFUE_PARAMETER_RUNDEN you can make the shape
               dimensions be rounded. This possibility already existed in the previous versions.

               If, however, the environment variable DFUE_NTEL_MM is active, the environment variable
               DFUE_PARAMETER_RUNDEN is not evaluated and the shape dimensions in 1/10 mm are also
               taken over. Similarly, the dimensions of the shape record are generally taken over in 1/10 mm if this
               is a step dimensioning.

           2. Muntin dimensions

               Muntin dimensions can be taken over in 1/10 mm regardless of the item dimensions. For this, the
               environment variable DFUE_SPROSSENMASS10 must be activated. This possibility already
               existed in the previous versions.

               If, however, the environment variable DFUE_NTEL_MM is active, the environment variable
               DFUE_SPROSSENMASS10 is not evaluated and the muntin dimensions in 1/10 mm are also taken
               over.

           3. Processing parameters

               Processing parameters for processings with A+W processing type that are sent via the B1 record
               can be taken over in 1/10 mm regardless of the item dimensions. For this, the environment variable
               DFUE_BEARBMASS10 must be activated. This possibility is new with this version.



A+W Software GmbH                             EN-A+W EDI Import.docx                                           99 / 162
                 If, however, the environment variable DFUE_NTEL_MM is active, the environment variable
                 DFUE_BEARBMASS10 is not evaluated and the processing parameters in 1/10 mm are also taken
                 over.

        Imperial system (Inch): Starting with interface version 02.2.025, the FH record was expanded to include the
"Fraction" field. The inch fraction is specified in this field. If the value is > 1, then the fields P1:Width and P1:Height,
S1:Thickness, M1 and B1 are interpreted as inch (Inch * fraction). This means for Fraction 64, for a width of 100
inches, the value "064000" must be transferred. The standard interface recalculates these values in mm by itself. In
the AWE tables, the mm are saved with 4 places after the decimal point regardless of DFUE_NTEL_MM.

4.7.4 Article names
        Within the P1 record, up to 3 customized article names can be delivered. Depending on the configuration,
        these names are transferred to the ALCIB order.

        ATTENTION: Only the first 30 characters will be adopted because the ALCIB data structure can handle
        only 30 characters for article names.

        By default, the names are adopted, being preceded by the customer article number, to kposex.exarttxt,
        where they are available for their own individual use (e.g. printing on customer documentation).

        Structure of the field "exarttxt"
        Customer article number of item article       20 characters
        Customer article number of 1st glass replacement     6 characters
        Customer article name 1                              14 characters
        Customer article number of 2nd glass replacement     6 characters
        Customer article name 2                              14 characters
        Customer article number of 3rd glass replacement     6 characters
        Customer article name 3                              14 characters

        If the environment variable DFUE_KUARTBEZ_TO_KPOSEX has been activated, only the customer
        article names are written to the "exarttxt" field.

        Structure of the field "exarttxt"
        Customer article name 1                                     30 characters
        Customer article name 2                                     30 characters
        Customer article name 3                                     20 characters

        Parallel to these two basic configuration options, there are another 2 customized applications for the
        delivered article names.

        If the environment variable DFUE_SCHOLL_GWTERM has been set, the customer article name 3 is
        adopted with 20 characters as the customer item number (kpos.kuposnr).

        At customer 12, customer article name 1 is adopted in the field kpos.private_char.

4.7.5 Color
        Starting with ALCIB Version 3.1 and with the interface version 02.02.014, there has been the following
        change:

        The P1 record generally analyzes the color field. The following definitions apply.

            a) A color name is sent in field "color" (e.g. white). The color number for this color name is
               determined in the ALCIB color keys (Master data - Keys - Product keys – Colors). The customer's
               language is used for the search at first. If this produces no results, the national language will be
               used for searching. If there is no result either, the default color (definition as per table exbartyp
               artyp= 10) is transferred to the order.

            b) If the first character in field "color“ is "@", a number is expected right after that (e.g: @2 or
               @002). This number is interpreted as the ALCIB color number. If @ is not followed by a valid


A+W Software GmbH                                 EN-A+W EDI Import.docx                                            100 / 162
               number, or if the number is no valid color in the ALCIB color keys (Master data - Keys- Product
               keys - Colors), the default color (defined in table "exbartyp" artyp= 10) is transferred to the order.

           c) More external information on colors can be processed in field "color". The structure
              "@@code@value" will be used for this. The first two characters are "@". They are followed by a
              character string which defines the external color information. This code ends with "@". The third
              @ is followed by the actual external color information (e.g @@RAL@9010;
              @@EAN@880110100003). To determine an ALCIB color number based on these two entries
              (code and color information), use the stored procedure cu_dfue_getfarbe() with the parameters:
              Code, color information, customer number, sequential order number, item number, customer
              article number, client number. This stored procedure determines the ALCIB color number. The
              codes "RAL" (Master data - Keys - Product keys - Colors) and "EAN" (Master data - Article -
              Menu - Colors/sizes - <MODE>) were implemented in the stored procedure. Other codes or the
              analysis of the EAN code from article/customer data can be individually added.If the EAN code
              has been transferred, it is possible that no customized article number was included in the
              transfer. In this case, the stored procedure determines the article number for the EAN code and
              uses it as a customized article number for order entry. Please take this into account when
              setting up the order transfer (Master data - Article - Menu - Market partner details and table
              exbartyp).

               If the stored procedure returns no valid color, the default color (definition in the table exbartyp
               artyp=10) is transferred in the order.

               If the system is configured for optimized BOM number, then for color items a new BOM number is
               also assigned if the color changes.

4.7.6 Dimensional variants
       Starting with ALCIB Version 3.2 and with the interface version 02.02.014, there has been the following
       change: the record structure of the P1 record was expanded to include the field 23 "dimension variant".

       ALCIB currently does not analyze the fields 20, 21 and 22.

       Field 23 "Dimensional variant" is analyzed as follows:

           a) Field "Dimensional variant" transfers a fixed number. Currently, the number "1" is implemented
              which means: If 1 is transferred in field 23, the import routine tries - by means of the sizes
              entered in field 8 "width" and 9 "height" - to determine the corresponding ALCIB variant number.
              For this purpose, the stored procedure cu_dfue_getbitnr() with the parameters: customer number,
              sequential order number, item number, customer article number, and client number is loaded.
              The Stored Procedure determines the ALCIB variant number. We currently assume that the
              variants for Size1 and Size2 were clearly defined. If this is not the case, the Stored Procedure
              can be adapted accordingly. The system also checks for the exact sizes that were delivered. A
              size tolerance can also be used. Please contact a consultant, or our customer service team.

               A template for the stored procedure is located at $ALCIBPRG/install/xsql/sp/.opt/df.

               Imperial System (Inch):

               If in the interface inches are transferred, then it must be noted that the dimensions in mm
               including 4 places after the decimal point are transferred. The transfer in mm is done because
               dimensions are in mm in the master data in the database.

               Dimensional precision 1/10 mm:

               If the data takeover in 1/10 mm is configured, the dimensions are transferred to the SP
               accordingly in 1/10 mm including one place after the decimal point.

           b) If the first character in field "Dimensional variant" is "@", the system expects this to be followed
              by a number (e.g: @2 or @002). This number is interpreted as the ALCIB variant number. If @ is
              not followed by a valid number, or if the number is no valid variant in the ALCIB variant keys
              (Master data - Keys- Product keys - Variants), the default variant (defined in table "exbartyp"


A+W Software GmbH                               EN-A+W EDI Import.docx                                               101 / 162
               artyp= 11) is transferred to the order.

               If in the variant field this detail is sent, the data in fields 8 and 9 (width and height) are ignored.

           c) External information on variants can be processed in field "Dimensional variant". The structure
              "@@code@value" will be used for this. The first two characters are "@". They are followed by a
              character string which defines the external variant information. This code ends with "@". After the
              third @ follows the actual external variant information (e.g @@EAN@880110100003). To
              determine an ALCIB variant number based on this information (code and variant information), the
              Stored Procedure cu_dfue_getvar() with parameters: code, color information, customer number,
              sequential order number, item number, customer article number, client number is loaded. This
              stored procedure determines the ALCIB variant number. The code "EAN" (Master data - Articles -
              Menu - Variants - <MODE>) has been implemented in the stored procedure. Other codes or the
              analysis of the EAN code from article/customer data can be individually added. Please contact
              your consultant or the ALCIB service team.

               If the EAN code was transferred, it is possible that no customer-specific item number is included.
               In this case, the stored procedure determines the article number for the EAN code and uses it as
               a customized article number for order entry. Please take this into account when setting up the
               order transfer (Master data - Article - Menu - Market partner details and table exbartyp). Please
               contact your consultant or the ALCIB service team.

               If the stored procedure returns no valid variant, the default variant (definition in the table exbartyp
               artyp=11) is transferred in the order.

               If in the variant field this detail is sent, the data in fields 8 and 9 (width and height) are ignored.

               A template for the stored procedure is located at $ALCIBPRG/install/xsql/sp/.opt/df



4.7.7 Customer item
       Currently, field 15 "Customer item" is transferred from the P1 record to the ALCIB item (field
       kpos.kuposnr).

       However, there is already one customized deviation (DFUE_SCHOLL_GWTERM) for which the first 20
       characters of field 5 "Name 3" are used as the customer item.



4.7.8 Special logic
       If the variables GLASMARKT=1 and GLASMARKT_SPEZIAL = FEBA are set, the fields after field 21 will
       be interpreted differently from the way defined in the interface description.

4.7.9 Free of charge flag ; Complaint
       Starting with version 2.02.029 the free of charge flag from P1/20 will be evaluated. If the flag is set to True
       and value K5/9 – document type is 2 (A+W Enterprise kaufart „free-of-charge“), the order is free-of-charge
       and the total item price will be zeroed.




A+W Software GmbH                                EN-A+W EDI Import.docx                                              102 / 162
4.8   Item extension (P2)
4.8.1 Document reference and item reference
       As of ALCIB version 2006 (4.0)
       The standard filter has been extended in preparation of returning status information.
       Fields 6 "Document reference" and 7 "Item reference" of record P2 are imported. The data are written in
       table kposzusatz in the fields "dokuref" and "posref". By default, these fields are not displayed in the order.
       They can be displayed via customizing, and are available for analysis and searching.

4.8.2 Complaint type
      # 258397

      The complaint information is taken over from the P2 set as at ALCIB version 2009 (Release November 2013)
      and interface version 2.2.023. As ALCIB does not carry it on a position level but on a process level, this
      results in some restrictions during the transfer.

      1. Only the complaint information found first shall be incorporated into the order.

      2. All items of an order must contain the same complaint information.

      If a complaint is sent in an interface in the P2 record, it is not mandatory that this is the ALBCI-internal type of
      complaint.

       If the first (!) character is @, the program expects a number after that. This number is interpreted as ALCIB-
       internal number for the type of complaint.

       If the first character is not an @, the complaint specification is transferred as a text and through the call of
       the customer-specific SP
       cu_dfue_getcompltype(p_custcompl CHAR(10), p_customer INTEGER, p_aufnr INTEGER, p_site SMALLINT)
       RETURNING SMALLINT;
       Parameter: complaint text sent in the interface
                  Customer number
       Order number
                  Site number
       Return value: ALCIB-type of complaint
       Translated into the ALCIB complaint type.

        Example:

       P2 …. Crash …..                => Call of the SP cu_dfue_getcompltype(‘Crash’,100001,1,45)

       P2 …. @25 …..        => Transfer of the number 25 without change



       The program checks whether the resulting type of complaint is available in the ALCIB master data. If it is not
       available, type of complaint 32000 (indication in order "****“) is transferred to the order and the order is not
       released.

      If items with different types of complaints are sent within an order, the first type of complaint is transferred to
      the order. At the same time, a process note with "high" priority is generated which points out to the user that
      several pieces of complaint information were sent in the order.

      Orders with type of complaint 32000 (default) or the process note regarding several pieces of complaint
      information are not automatically released.




A+W Software GmbH                                EN-A+W EDI Import.docx                                            103 / 162
       In this case, mail 71 - Note: Check external order entry with the text "Conflicts exist in the attached pieces of
       complaint information in order <order number> (customer <customer number>). The order was not released"
       is sent to a defined processor.

       Up to version 2011, mail no. 59 with the text "Order <order number> (customer <customer number>) contains
       a dummy article. The order is not released" Unfortunately, this is technically not possible any other way.

4.8.3 Place of complaint and reason of complaint
       Both fields can be transferred to A+W Enterprise as alpha-numerical or numerical fields, example Item record
       P2.

      In this case, reason of complaint refers to database table rspec. You can search for matching Reklamspec
      either via incomming text or for incoming numbers via EDI it will be checked whether a value is defined.
      Example: EXEC SQL select reklamspec into : sSelReklamgrundNr
from rspec where bez = :helpReklamgrund;
       For easier processing, always the numeric value is transferred to A+W Enterprise.

      Place of complaint is processed in the same manner. In this case it is compared with database table rort.
      Example: EXEC SQL select reklamort into : sSelReklamortNr
from rort where bez = :helpReklamort;
       Here, the numerical value is also transferred to A+W Enterprise.

       For both complaint data fields the system makes sure, that the same place and type of complaint is
       transferred for an order (as for type of complaint).

4.8.4 Complaint order (#455928)
        If the reason for complaint and/or complaint location should be set, then you can use a P3/2 reference to the PO
        number directly before to communicate the original order number. This order number is then written to the
        database field kauf.referenz and serves as reference to the original order. For correct assignment, in addition to
        the data field kauf.reference, the data fields kauf_refvorgang = 5 and kauf.refsubnr = 0 are set.


4.9    Item references (P3) (AWE 6)
       Generally, the sent values are taken over in the table kposref.ex*. Currently there is no display dialog for this
       table. However the data is available for individual transfer to the production, reports, and queries.

4.10 Item-related parameter (PA)
The extension for the item-related parameter was handled with case #377618. Now it will be possible to
communicate to A+W Enterprise item-related parameter lists, that is, parameters that are only required once per item
using this record type via EDI.

As first implementation, the window frame overlap (#377618) is accommodated with record type = 1. With this type, 4
parameters are expected. 1=bottom, 2=right, 3=top, 4=left. Thus the frame offset for each side is communicated to
A+W Enterprise. For this record type, the parameters C1 - 32 - Simulated Divided Lite Bar Size and P1 - 21 -
Simple Cutback are expected.




A+W Software GmbH                                EN-A+W EDI Import.docx                                            104 / 162
Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




Recognizable in the image are the cutback (SR), the sightline(offset 1-4, here naturally only one edge), and the
simulated muntin width(Simulated Divided Lite Bar Size).


                                                              Type                                                                    Name                                                                                                  Description


                                                                                                                                                                                                                                            The parameters are required in order to be able to install the
                                                              1                                                                       Window frame overlap(Offset)
                                                                                                                                                                                                                                            associated muntins symmetrically in the window frame.




4.11 Private tables (item-related) (PT)

4.11.1 Supported tables and parameters
For the writing of the table, pay attention to the precise spelling. Entries are case-sensitive. If another table than the
one listed above is transferred, the data record is ignored (log entry with WARNING). However, scheduling is still
done.



Table                                                                                                                                                                                                                       Parameter                               Comment

Kspectxt                                                                                                                                                                                                                    1 – texttype                            # 368658

                                                                                                                                                                                                                            2 – Text                                Please check text types with
                                                                                                                                                                                                                                                                    development and project
                                                                                                                                                                                                                            3 - sequence                            management.

                                                                                                                                                                                                                                                                    see also include/kspectxt.h and table
                                                                                                                                                                                                                                                                    documentation

                                                                                                                                                                                                                                                                    This record type is not supported for
                                                                                                                                                                                                                                                                    items, that refer to a product set (P1
                                                                                                                                                                                                                                                                    – record with @).




A+W Software GmbH                                                                                                                                                                                                                   EN-A+W EDI Import.docx                                         105 / 162
PTkspectxt               1010|Text1|1
PTkspectxt               1010|Text2|2
PTkspectxt               1010|Text3|3
PTkspectxt               1010|Text4|4


Text types 6000 to 6999 are reserved for "customer-specific text types to be used within external EDI". Currently,
there is no special treatment by A+W Enterprise for these text types.

Text types larger than 6999 are internal A+W Enterprise types and are declined during scheduling as errors and the
scheduling is canceled.

If invalid parameters are transferred within the data record, then the scheduling of the order is canceled.


4.12 Item document link PL
        From AWE 5.4, document links can be transferred via the external order interface. If the system is not
        configured for document links (environment variable DATEI_REF_PFAD), the order is imported, a
        process note is generated ("The order includes document attachments that cannot be processed") and
        the order is not released. In addition a corresponding note is shown in the interface protocol.
        WARNING: The system is not configered to support attachments to an order.
                     Please contact A+W implementation team.

        The sent document is expected in the same directory that includes the interface file. If the attached
        documents are saved in a sub-cirectory, a relative or absolute path must be specified in front of the file
        name. The path information must not include any server names. "/", as well as "\" are processed.

        The attached documents are copied to $DATEI_REF_PFAD/<auftrnr>/<posnr>. The original files remain
        in the transfer directory.

        (When configuring, please ensure that the trm_ctrl ftp has access to the server that is defined in the
        variables. You may want to use variable DFUE_DATEI_REF_PFAD.)


4.13 Item text record (T1)
        Within the standard filter, item texts can be transferred by using transfer record T1. When transferring
        orders into A+W Enterprise, the fields Text code, Type and Text No. are not analyzed.

        You cannot define within the transfer record onto which A+W Enterprise forms a text should be printed.




A+W Software GmbH                               EN-A+W EDI Import.docx                                        106 / 162
4.14 Bill of materials (BOM) (S1)
       For assigning the BOM number of an item, see separate documentation: EN-CONFIG-A+W Enterprise
       EDI.docx
       The transfer of an S1 record changes the standard product structure for the special item. This change is
       only permitted for regular items. A change of the product structure for so-called "fixed items" is not
       permitted and will be ignored. There is no error treatment.

       To change the product structure for product sets, see "Product sets – exchange"



4.14.1 Supported product types and groups
       Within the S1 record, a product type (field 16 from item 219) and a product group (field 17 from item 222)
       are transferred. The following product types are supported:


         Product         Description                   Comment
         type
         1               Single glass                  For exchange into multi-layer glass and product sets
         2               Tempered glass                For exchange into multi-layer glass and product sets
         3               LAMI                          For exchange into multi-layer glass and product sets
         10              Services/surcharges           Generation of a procedure note. Item is not adopted
         11              Muntins
         12              Shape/step                    Product group 50 – step, if product group = 0, then the
                                                       record is ignored. Shapes are only processed via the
                                                       M1 record
         13              Leaded designs                Generation of a procedure note. Item is not adopted
         14              Curved glass                  May 2021: Generation of a procedure note. Item is not
                                                       adopted
         20              Processing
         30              Inserts                       Product group 41 – Gas
         40              Other items                   Product group 3 – other items;
                                                       otherwise generation of a procedure note. Item is not
                                                       adopted
         50              Insulated Glass               Generation of a procedure note. Item is not adopted
         60              Spacer                        Product group 80 - Frame
         100             GDS                           Generation of a procedure note. Item is not adopted
         200             Boxes                         Generation of a procedure note. Item is not adopted

       ProductGroup
       410 – Pressure equalization (support currently only for special logic DFUE_ARTIKELBEZ)

       From A+W Enterprise release 6 patch 19.10.2017 and interface version 2.02.014 on, an automatic
       mapping of product type and product group was provided:

       Now it is possible in the S1 record to leave the fields S1/16 product type and S1/17 product group within the
       interface file for the standard interface empty. If both of these fields are empty, then the new logic of the
       automatic mapping runs automatically.

       For this, the following table must be heeded.

         Product           Description            A+W                   Note
         Type                                     Enterprise
                                                  item type




A+W Software GmbH                              EN-A+W EDI Import.docx                                            107 / 162
         Product              Description            A+W                  Note
         Type                                        Enterprise
                                                     item type

         1                    Single sheet           100, 110, 120,       Exchange for multiple sheet units or
                              glass                  130, 140, 160        product - sets

         2                    Toughened glass        150                  Exchange for multiple sheet units or
                                                                          product - sets

         3                    Laminated glass        170                  Exchange for multiple sheet units or
                                                                          product - sets

         11                   Georgian bars          230

         12                   steps                  510                  Product group 50 - steps

         20                   Processings            Teilflag=0

         20                   Processing List        594                  Product group 410 pressure compens.

         30                   Fillings               260                  Product group 41 - gas

         40                   Other articles         999                  Product group 3 – other articles

         60                   Spacer                 210, 211             Product group 80 - space



       If the two fields S1/16 and S1/17 should be empty, then first in the exchange/add-on rules (table kuaz)
        and after that in the item market partner details (table artkuzu) using the customer item number (S1/6 –
       product no.) there is a search for an appropriate A+W Enterprise item number. If no data for the individual
       incoming items is maintained in these tables, the execution will fail.

       Attention must be paid that the maintenance of different item data via prefix and the same item name e.g.
       iso1234 and bea1234 is not supported in this logic. If your customer item numbers are maintained this
       way, there will be a failure of the execution of the document. The customer item numbers must vary by
       prefix.

       If the standard mapping as in the table above does not fit for individual items, you can store another
       product type or product group for the desired item in A+W Enterprise under the item master data dialog
       (Master Data>Items). With [F4] on the item master data dialog, you can open the Configured fields dialog
       and maintain the fields PRODUKTART and PRODUKTGRUPPE with the combinations of product types
       and product groups specified above. Here it is important that both of these fields were created with the
       installation script /develop/globfiles/kflddef/artprvfld/set_ARTPROD.sql (artcomfld.fldnr in (-10003, -
       10004) and artcomfld.fldnrz in (-1003, -1004).

       If you fill the fields S1/16 and S1/17 as usual, the new logic will not be run through and the i000filter will
       function as usual.


4.14.2 Color
       Starting with ALCIB Version 3.1 and with the interface version 02.02.014, there has been the following
       change:

       The S1 record generally analyzes the color field. The following definitions apply.

              a) A color name is sent in field "color" (e.g. white). The color number for this color name is
                 determined in the ALCIB color keys (Master data - Keys - Product keys – Colors). The customer's
                 language is used for the search at first. If this produces no results, the national language will be

A+W Software GmbH                                EN-A+W EDI Import.docx                                          108 / 162
               used for searching. If there is no result either, the default color (definition as per table exbartyp
               artyp= 10) is transferred to the order.

           b) If the first character in field "color“ is "@", a number is expected right after that (e.g: @2 or
              @002). This number is interpreted as the ALCIB color number. If @ is not followed by a valid
              number, or if the number is no valid color in the ALCIB color keys (Master data - Keys- Product
              keys - Colors), the default color (defined in table "exbartyp" artyp= 10) is transferred to the order.

           c) More external information on colors can be processed in field "color". The structure
              "@@code@value" will be used for this. The first two characters are "@". They are followed by a
              character string which defines the external color information. This code ends with "@". The third
              @ is followed by the actual external color information (e.g @@RAL@9010;
              @@EAN@880110100003). To determine an ALCIB color number based on these two entries
              (code and color information), use the stored procedure cu_dfue_getfarbe() with the parameters:
              Code, color information, customer number, sequential order number, item number, customer
              article number, client number. This stored procedure determines the ALCIB color number. The
              codes "RAL" (Master data - Keys - Product keys - Colors) and "EAN" (Master data - Article -
              Menu - Colors/sizes - <MODE>) were implemented in the stored procedure. Other codes or the
              analysis of the EAN code from article/customer data can be individually added. Please contact
              your consultant or the ALCIB service team.If the EAN code has been transferred, it is possible
              that no customized article number was included in the transfer. In this case, the stored procedure
              determines the article number for the EAN code and uses it as a customized article number for
              order entry. Please take this into account when setting up the order transfer (Master data - Article
              - Menu - Market partner details and table exbartyp). Please contact your consultant or the ALCIB
              service team.

               If the stored procedure returns no valid color, the default color (definition in the table exbartyp
               artyp=10) is transferred in the order.

4.14.3 Frame / AIR
       As of ALCIB Version 3.1 and interface version 02.2.014 the following changes apply:

       Transfer of the AIR within the S1 record and a frame replacement are now possible.

       For this purpose, the S1 record was extended by field 19 - Thickness.

       For the implementation of the customer-specific frame item, an entry must exist in the customer-specific
       exchange/addition rules (table kuaz). Here, a customized article name for the frame can be defined, if
       required.

       If product type=60 and product group=80 in record S1, this record S1 will be interpreted as a frame in an
       IG unit. In this case, the product number is used as a customized frame article number, and the thickness
       is used as the airspace (AIR). Fields 4 "Level" and 5 "Position on level" define whether this is the first or
       second airspace. If level = 1 and position= 2, this is the first frame / AIR. If the level=1 and the position=4,
       this is the second frame/AIR.

       With this extension, a specific exchange of the first or second frame within a triple IG is now possible. For
       this purpose, it is absolutely required that the frame generally has an assembly position within the
       original BOM (also in the case of double IG).

       If a frame exchange is sent for an IG in which the assembly positions of the frame are not
       maintained, no frame exchange will be carried out!

       If frames shall not be exchanged, but the AIR shall be transferred, the product number field in record S1
       can be left blank. If both AIRs shall be changed, two S1 records with level=1 and position= 2 or 4 must be
       sent.

       For the frame exchange, it is necessary that the default item that was defined for frame has a correct item
       type within the ALCIB master data. A correct article type is 210 - frame or 211 - color frame.




A+W Software GmbH                               EN-A+W EDI Import.docx                                               109 / 162
        If the frame changes the AHAM via formula in its master data and this should also be done for external
        DFÜ, then the environment variable INTAUF_AHAM_TEST must be set.

        By default, the frame with the quantity 1 is exchanged in the BOM. Depending on the system, however, it
        can be necessary that the BOM quantity in the order should be 2 also for frame 2 (e.g. price calculation
        by linear meters.) If this should be achieved, then the environment variable DFUE_FRAME_KUAZ should
        be set. If the variable is set, the quantity is taken over from the S1 record as quantity 1. In addition, there
        is a check if the quantity 1 or quantity 2 is equal to 0 after importing of the interface file; then the quantity
        1 or 2 from the A/Z rules is taken over.

Imperial system (Inch): Starting with interface version 02.2.025, the FH record was expanded to include the
"Fraction" field. The inch fraction is specified in this field. If the value is > 1, then the fields P1:Width and P1:Height,
S1:Thickness are interpreted as inch (Inch * fraction). This means for Fraction 64, for a width of 10 inches, the value
"006400" must be transferred. The standard interface recalculates these values in mm by itself. In the AWE tables,
the mm are saved with 4 places after the decimal point regardless of DFUE_NTEL_MM.

4.14.4 Additional processing / miscellaneous articles
        Starting with ALCIB Version 3.1

        So far, the standard filter in the IG BOM could only be used to exchange lites or frames, and add
        "genuine" processing steps.
        ALCIB item types:

            o    BENDING

            o    ARCHING

            o    ANNEALING

            o    PARTIAL ANNEALING

            o    HANDLES

            o    COLOR APPLICATION

            o    ENAMELING

            o    ETCHING

            o    UV COVER

            o    INSIDE THREAD

            o    DISTORTION

            o    GLUING

            o    COATING

            o    SAND BLASTING

            o    SCREEN PRINTING

            o    FLUTED BEVELING

            o    MISCELL_PROCESS

            o    SPEECH

            o    DRILLING

            o    EDGING

            o    EDGE CUT-OUTS


A+W Software GmbH                                 EN-A+W EDI Import.docx                                             110 / 162
            o    GRINDING

            o    MITERS

            o    ARRISSING

            o    ROUNDED CORNERS

            o    NOTCHED CORNERS

            o    CORNER CUT-OUTS

        Processing steps with product type 20 were transferred within the interface.

        Now it is possible with the transfer of the product code 40 and the product groups three also to transfer
        other items for the BOM change. In this case, it is assumed that no additional parameters are required
        (no B1 record in the interface, no article dimensioning in ALCIB).

        The prefix for these products is the entry artyp=13 in control table 'exbartyp'. The customized
        exchange/supplement rules define whether the transferred article is added or whether there shall be an
        exchange:

        By default, the item with the quantity from the S1 record is taken over as quantity 1. In addition, there is a
        check if the quantity 1 or quantity 2 is equal to 0 after importing of the interface file; then the quantity 1 or
        2 from the A/Z rules is taken over.

        Table 'kuaz', menu: Master data -> Market partners, menu - Exchange/addition rules.

4.14.5 Price relevance
        Steps: The price code is always set

        Frame: By default, the price code is always set. If the environment variable DFUE_FRAME_KUAZ is
        active, the price code is set as below.

        Gas: By default, the price code is always set. If the environment variable DFUE_BEA_NEU is active, the
        price code is set as below.

        Various BOM items (product type 40 / product group 3): The price code is always set.

        Processings: By default, the price code is always set. If the environment variable DFUE_BEA_NEU is
        active, the price code is set as described below.

        Grid articles: The price code is always set

        Muntins: The price code is always set.


With set environment variable DFUE_BEA_NEU:
Whether the exchange/additional flag is set in the order BOM, and thus also an additional price is calculated is done
in 2 stages.
     1. If in the interface file the field S1:26 is filled and equal to 1, then the A/Z flag is set.
    2. If in the interface file the field S1:26 is not filled or if it is equal to 0, then the AZP flag from the A/Z rules is
       used.
The evaluation of the field S1:15 is done only starting with interface file version 02.2.022



4.14.6 Print flag
        Steps: The print flag is always set




A+W Software GmbH                                  EN-A+W EDI Import.docx                                               111 / 162
       Steps: By default, the print flag is always set. If the environment variable DFUE_FRAME_KUAZ is active,
       the print flag from the exchange/addition rules is used.

       Gas: By default, the print flag is always set. If the environment variable DFUE_BEA_NEU is active, the
       print flag from the exchange/addition rules is used.

       Various BOM items (product type 40 / product group 3 ): The print flag is always set

       Processings: By default, the print flag is always set. If the environment variable DFUE_BEA_NEU is
       active, the print flag from the exchange/addition rules is used.

       Grid articles: The print flag is determined from the article master data fields "Verkaufspapiere" and
       "Produktionspapiere."

       Muntins: The print flag is always set.

4.14.7 Gas
       As of ALCIB version 2006 (4.0)

       You can now also transfer gas. The gas article is transferred within an S1 record with product type 30 and
       product class 41.

       In order to implement the customized gas article, an entry must exist in the customized
       exchange/supplement rules (table kuaz). Here, a customized article name for the gas can be defined, if
       required.

       The prefix for these products is the entry artyp=9 in control table 'exbartyp'.

       There are three options to decide on which BOM level the gas shall be added or exchanged in the ALCIB
       BOM; these options are defined by environment variable DFUE_GAS_LEVEL.

       As for external order entry, this variable defines the level on which gas shall be added to the IG.

           o   1 - First level, next to frame

           o   2 - Second level, in frame

           o   3 - The level is defined in the interface file

           o   If this variable is not set, the gas will be added to the frame.

       1- First level: This means that the gas is positioned on the first BOM level, right next to the frame and the
       lites. If there is gas within the frame, this will be kept and will not be replaced.

       2- Second level means that the gas is positioned inside the frame. If there is also gas on the first level
       (next to the frame), this will be kept and will not be replaced.

       3- This level is defined in the interface file. There are several variants available:

       First, an S1 record for the gas is transferred, followed by an S1 record for the AIR or frame replacement.
       In this case the gas is added in the inside frame.

       Just one S1 record is transferred for the gas. In this case, field 4 "Level" of this S1 record is analyzed. If it
       shows 1, the gas will be added or replaced to/at the first BOM level (next to the frame). If it shows 2, the
       gas will be added/replaced to/at the second BOM level (inside the frame). If neither 1 nor 2 is transferred,
       the gas will be added or replaced to/at the second BOM level (inside the frame).

       First, an S1 record for gas is transferred, followed by an S1 record for the AIR or frame replacement. In
       this case, field 4 "Level" of this S1 record is analyzed for gas. If it shows 1, the gas will be added or
       replaced to/at the first BOM level (next to the frame). If it shows 2, the gas will be added/replaced to/at
       the second BOM level (inside the frame). If neither 1 nor 2 is transferred, the gas will be added or
       replaced to/at the second BOM level (inside the frame).



A+W Software GmbH                                EN-A+W EDI Import.docx                                            112 / 162
       ATTENTION: The sequence of the S1 records for gas and AIR/frame is decisive for the
       configuration DFUE_GAS_LEVEL=3.

       When transferring triple IG, it is currently impossible to define whether the gas shall be replaced or added
       in the first or second frame. Exchanges or additions are always made in both frames. However, this is
       only possible if both frames have the same structure, i.e. either the original BOM of both frames includes
       gas, or none of them. If the structure is different in this respect, the result is undefined.

       When creating the master data, pay attention to the following:

       Depending on the configuration (DFUE_GAS_LEVEL), there must be just one gas article per BOM level
       (frame or IG). If two or more gas articles exist simultaneously, only the first gas will be exchanged as a
       rule. In this case, you have to use a meta element for gas mixtures.

       If IG generally includes a frame without gas, and if this frame is replaced by a frame with gas in the order
       received, while extra gas is transferred on frame level for the same item, the additional gas will be added,
       not exchanged.

       If on the other hand IG generally includes a frame with gas, and if this frame is replaced in the order
       received by another frame without gas while extra gas is transferred on frame level for the same item, the
       additional gas will be ignored.

       Since the program cannot solve this conflict, you have the option to inform the employee in charge about
       this conflict by email. Message number 62 will be sent if frame replacement and gas are transferred
       together for an item.

       The subject line for this message is: "Note: Please check external order entry"

       The text: "When importing order 151515 / P.O. text 'gastest' the frame was exchanged in items 8, 9, 10,
       11, 12, 14 and gas was added. Please check the order."

       The order number - here 151515 - defines the serial number of the order on the current transfer list. The
       final order number is unfortunately not available. The P.O. text can be used to search for the order at
       order entry (key <DETAIL> in the empty order number field).

       It is also important that the article types of the default articles for frames and gas are correct. This is why
       message number 63 can be configured. This message is sent if the article types of the default articles for
       IG, muntins, frames, and gas are incorrect, or if no default articles were defined.

       The subject line of the message is: "Note: Incorrect master data definition for external order entry."

       The text: "Frame: The defined default article 110004 has the wrong article type 100 FLOAT glass FM.
       Please check the log >/usr1/alcibnet/proto/exbin_proto33<!"

       The word "frame" can be replaced by IG, muntins, or gas depending on which article is incorrect.

       If frame and gas are replaced at the same time, message 62 will be sent.


4.14.8 Glass replacement
4.14.8.1        Exchange of patterned glass/coated glass
       If no patterned side is defined in record S1 of the interface file, the patterned side will be transferred to
       ALCIB as being inside. The field 19 "Coating side" is not evaluated within the glass exchange.

        The definition of field 15 'Pattern side' is as follows:

       0 - no defined structure side - the EP "inside" is used
       1 - The structure points inwards. This means:
           Glass 1 = assembly position 2
           Glass 2 = assembly position 3
           Glass 3 = assembly position 5

A+W Software GmbH                                 EN-A+W EDI Import.docx                                         113 / 162
       2 - The structure points outwards. This means:
           Glass 1 = assembly position 1
           Glass 2 = assembly position 4
           Glass 3 = assembly position 6

       If no sense of pattern is transferred, the sense of pattern is adopted from the customized exchange/
       supplement rules. If no sense of pattern is defined there either, no sense of pattern will be transferred to
       ALCIB.

4.14.8.1.1 Evaluation of the assembly position
       Starting with interface status i000filter Build 13.04.2130 and trm_ctrl Build 13.04.2150, another
       evaluation of the assembly position for exchanged glass applies.

       If no patterned side is defined in record S1 of the interface file (field is empty or a 0 is transferred), the
       patterned side from article reference (exchange / additional rules) is used. If no assembly position is
       defined, the assembly position of the master data BOM is retained for multiple glasses (IG, LAMI). The
       field 19 "Coating side" is not evaluated within the glass exchange.

        The definition of field 15 'Pattern side' is as follows:

        Empty or 0 - no defined pattern side - The assembly position of the article referencing is adopted
       (kuaz.pos), if none is defined there, the assembly position of the master data BOM is retained.

       1 - The structure points inwards. This means:
           Glass 1 = assembly position 2
           Glass 2 = assembly position 3
           Glass 3 = assembly position 5
       2 - The structure points outwards. This means:
           Glass 1 = assembly position 1
           Glass 2 = assembly position 4
           Glass 3 = assembly position 6
       It is important that the article master data is created correctly. It is imperative that glasses always have an
       assembly position within an IG BOM. For LAMIs, an installation item must always be available if several
       fixed dimensions are on one BOM level. If there is no assembly position, no correct glass replacement
       can be performed by the external EDI.



       Insulated glass examples:

       In the item master data, the IG is created with 2 glasses, A and B, with the assembly positions 2 and 3.

       Now, a glass C is sent via interface as replacement for glass A. In the replacement rules, only the item
       implementation, but not the assembly position is defined.




A+W Software GmbH                                 EN-A+W EDI Import.docx                                         114 / 162
         Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




        Now there are 4 scenarios depending on which value is transferred in field 15 (structure side) of the S1
        record in the interface file.
Value in the                                                                              Assembly position of glass C in                                                                                                               Reasons
interface                                                                                 the order
00                                                                                        2                                                                                                                                             No AP was sent and none was defined in the E/A rules => AP from
                                                                                                                                                                                                                                        master data is retained
01 (inside)                                                                               2                                                                                                                                             Assembly position was sent via the interface
02 (outside)                                                                              1                                                                                                                                             Assembly position was sent via the interface
 <empty>                                                                                  2                                                                                                                                             No AP was sent and none was defined in the E/A rules => AP
                                                                                                                                                                                                                                        from master data is retained


        If this glass C is sent as replacement for glass B, then the table looks as follows
Value in the                                                                              Assembly position of glass C in                                                                                                               Reasons
interface                                                                                 the order
00                                                                                        3                                                                                                                                             No AP was sent and none was defined in the E/A rules => AP from
                                                                                                                                                                                                                                        master data is retained
01 (inside)                                                                               3                                                                                                                                             Assembly position was sent via the interface
02 (outside)                                                                              4                                                                                                                                             Assembly position was sent via the interface
 <empty>                                                                                  3                                                                                                                                             No AP was sent and none was defined in the E/A rules => AP
                                                                                                                                                                                                                                        from master data is retained


        Now, a glass D is sent via interface as replacement for glass B. In the replacement rules, the item
        implementation and the assembly position are defined.




A+W Software GmbH                                                                                                                                                                                                                    EN-A+W EDI Import.docx                                         115 / 162
Das verknüpfte Bild kann nicht angezeigt werden. Möglicherweise wurde die Datei verschoben, umbenannt oder gelöscht. Stellen Sie sicher, dass die Verknüpfung auf die korrekte Datei und den korrekten Speicherort zeigt.




                                                           Now there are 4 scenarios depending on which value is transferred in field 15 (structure side) of the S1
                                                           record in the interface file.
Value in the                                                                                                                                                           Assembly position of glass D in the                                    Reasons
interface                                                                                                                                                              order
00                                                                                                                                                                     4                                                                      No AP was sent and but AP 4 is was defined in the E/A rules
01 (inside)                                                                                                                                                            3                                                                      Assembly position was sent via the interface
02 (outside)                                                                                                                                                           4                                                                      Assembly position was sent via the interface
  <empty>                                                                                                                                                              4                                                                      No AP was sent and but AP 4 is was defined in the E/A
                                                                                                                                                                                                                                              rules
If on the left side an assembly position is also entered, then this rule is only applied if the glass to be replaced is
created exactly for this assembly position.

                                                           A glass D is sent via interface as replacement for glass A. In the replacement rules, the item
                                                           implementation and the assembly position also on the left side are defined.




Value in the                                                                                                                     Assembly position of                                                                       Reasons
interface                                                                                                                        glass D in the order
00                                                                                                                                                                                                                          No replacement occurs because the referencing is only defined for the assembly
                                                                                                                                                                                                                            position 4, but here a replacement for the assembly position 1 or 2 is sent.
    <empty>                                                                                                                      2                                                                                          No replacement occurs because the referencing is only defined for the assembly
                                                                                                                                                                                                                            position 4, but here a replacement for the assembly position 1 or 2 is sent.

4.14.8.2                                                                                                                    Exchange in product sets
                                                           Within the product set, the exchange of the header item is possible while retaining the processings
                                                           defined in the product set. For this, a S1 record with level = 0 (field 4) and product type = 1,2 or 3 (field
                                                           16) must be transferred.(for further explanations, see section "Product Type")

4.14.9 Muntins in triple IG (op. 118656)
                                               Different muntins can be replaced in the different frames of the triple IG by using the standard filter.
                                               The muntin records (S1, C1, CA) must follow directly after the respective frame replacement record (S1).
                                               If a muntin record is written without a preceding frame, then the muntin is always added to the first frame.
                                               In the S1 record of the frame, field 5 (position within the level) for the first frame must be occupied with value 2
                                               and for the 2nd frame with value 4.



A+W Software GmbH                                                                                                                                                                                                                EN-A+W EDI Import.docx                                             116 / 162
      In the S1 record of the muntin, field 3 (parent number) must refer to field 2 (number) of the frame S1 record.
      Field 5 (position within the level) specifies the order of the muntins within the frame.
      For muntin records without preceding frame record it is important that field 3 (parent number) is occupied with
      0 and field 4 (level) with 1. If different values are entered, the filter behavior has not been defined.

      Currently, muntins in the standard filter can only be added into the different frames if a frame record has been
      sent with the interface file.
      However, the RDT logic could also be extended at the cost of approx. 1 MD to the effect that muntin records
      would be allowed without frame records.



4.14.10        Steps (op. 220022)
      ALCIB version 2011 supports the import of steps. For this purpose, a defined S1 record followed by an M1
      record is analyzed.

      The step S1 record is marked by the combination of product type 12 + product class 50. The customer step
      article is transferred in field 6 (product number). Determination of the allocated ALCIB step article is described
      in the next chapter "Steps (M1)".




A+W Software GmbH                              EN-A+W EDI Import.docx                                           117 / 162
           Steps (M1)
      AWDesk 220022: Import of steps

      As of ALCIB version 2011, the shape record M1 can be used for step import. (see record description "Shape
      record (M1)").

      The parameters define the cutback with regard to the header article sizes for the corresponding edge, with
      outside view:

      Parameter 1 = bottom
      Parameter 2 = right
      Parameter 3 = top
      Parameter 4 = left

      The stepped lites are entered as bit vectors in field 12:
      1 = 1st lite stepped
      2 = 2nd lite
      4 = 3nd lite
      8 = 4nd lite
      etc.

      If the entry is 7 for instance, the first, second, and third lite will be stepped.


      Steps cannot be transferred for rectangular IG lites (no shapes). Steps in LAMI cannot be transferred yet.

      The step record is marked by the transfer of shape number 999.

      (Shapes with shape number 999 can still be transferred. The main thing is that the stepped M1 record is
      preceded by a S1 record with the correct product type and product group.)



      In ALCIB versions 2011 and 2012, import of steps must be enabled by environment variable
      DFUE_I000_STEP. Activation is not necessary in higher versions.

      An appropriate record for step import should be entered in table exbartyp. The default article entered there is
      used as a step article if no mapping for the transferred customer stepped article can be found by means of the
      R/A rules.

      Statement:
      INSERT into exbartyp (dfuetyp, artyp, prefix, defartnr) VALUES (19, 14, <Prefix>, <Default-Artikel>);

      The field for <Prefix> can remain blank.

      A replacement record is entered in customer R/A rules for the combination of <Prefix><Customer article>
      which is used for mapping the ALCIB article.

      During external order import, the default stepped article and the prefix (artyp 14) are selected from table
      exbartyp. If a R/A record is found by means of the combination <Prefix><Customer article> + <Customer>,
      the defined ALCIB article will be used as a stepped article. If no record is found, the default article from
      exbartyp will be used.



      Environment variable DFUE_DISTINCT_DEL_KUAZ must be set to make sure that the step record does not
      get lost during the import if glass replacement has been configured.

      If trm_ctrl detects that the resulting step article is 0 or does not have the correct article type (510), a warning
      will be issued in the exbin log. System message 63 will also be issued for information purposes. Order entry
      continues however, and the order is released.


A+W Software GmbH                                 EN-A+W EDI Import.docx                                           118 / 162
4.15 Processings (B1)
Imperial system (Inch): Starting with interface version 02.2.025, the FH record was expanded to include the
"Fraction" field. The inch fraction is specified in this field. If the value is > 1, then the fields P1:Width and P1:Height,
S1:Thickness, M1 and B1 are interpreted as inch (Inch * fraction). This means for Fraction 64, for a width of 100
inches, the value "064000" must be transferred. The standard interface recalculates these values in mm by itself. In
the AWE tables, the mm are saved with 4 places after the decimal point regardless of DFUE_NTEL_MM.

If a processing (e.g. sealing) changes the AHAM via formula in its master data and if this should also be done for
external DFÜ, then the environment variable INTAUF_AHAM_TEST must be set.

Whether for the B1 parameters these are in inches or not and thus there is a conversion depends on the A+W
processing type.


       As of version ALCIB 2008 (4.2) and higher the following A+W processing types are supported:

         ID                Processing Name                  Comment
         1000              Arrissing                        Just four edges, no shapes
         1005              Grinding                         Just four edges, no shapes

         1010              Polishing                        Just four edges, no shapes
         1030              Sawing

         1100              Drilling                         Only measurement type 0


       For drilling (1100), parameter 13 defines the measurement type. Currently, the measurement type is not
       analyzed because only measurement type 0 is supported.

       ALFAK writes the measurement types 1, 2, and 3. If they are to be analyzed in future, they will have to be
       mapped to A+W measurement types:

              o   1 -> 0

              o   2 -> 1

              o   3 -> 2


      ATTENTION!!
      As of version AWE 5.4 and interface version 2.2.023, a different analysis of the processing parameters
      applies.
      So far, there was no differentiation between blank parameters and 0. Due to the implementation of the A+W
processing catalog, there is now a distinction whether a parameter is transferred explicitly with 0 or whether the
parameter was not sent. If a parameter is not sent, the value from the AWE article master data or the
exchange/supplement rules is used.



      Starting with AWE Version 6 and interface version 2.2.023, the following A+W processing types are
supported:


4.15.1 Overview (starting with AWE version 6 and interface 2.2.023)

         ID                Processing Name                  Remark



A+W Software GmbH                                  EN-A+W EDI Import.docx                                            119 / 162
                                               Now with 8 edges and shape (parameter 1-8
                                               define the processed edge counter-clockwise).
        1000        Arrissing                  Only the parameters 1-8 are evaluated. All other
                                               parameters are ignored

                                               Now with 8 edges and shape (parameter 1-8
                                               define the processed edge counter-clockwise).
        1005        Grinding                   Only the parameters 1-8 are evaluated. All other
                                               parameters are ignored

                                               Now with 8 edges and shape (parameter 1-8
                                               define the processed edge counter-clockwise).
        1010        Polishing                  Only the parameters 1-8 are evaluated. All other
                                               parameters are ignored.


                                               With 8 edges and shape (parameters 1-8 define
                                               the edge processed counter-clockwise). Only
                                               the parameters 1-10 are evaluated. All other
        1015        Mitering                   parameters are ignored.
                                               The level is implemented as follows AWB:
                                               outside=1 => AWE: bottom = 2; AWB: inside=-1
                                               => AWE: top = 1).


                                               With 8 edges and shape (parameters 1-8 define
                                               the edge processed counter-clockwise). Only
                                               the parameters 1-11 are evaluated. All other
        1020        Facet                      parameters are ignored.
                                               The level is implemented as follows AWB:
                                               outside=1 => AWE: bottom = 2; AWB: inside=-1
                                               => AWE: top = 1).

                                               With 8 edges and shape (parameters 1-8 define
                                               the edge processed counter-clockwise). Only
                                               the parameters 1-8 are evaluated and 11 are
        1025        Edge stripping
                                               evaluated. All other parameters are ignored.
                                               The level is transferred by the data record S1
                                               field 18 "Coating side".

        1030        Sawing

                                               Now with 8 edges and shape (parameter 1-8
                                               define the processed edge counter-clockwise).
        1090        Other edgework
                                               The level is transferred by the data record S1
                                               field 18 "Coating side".



        1100        Drilling                   See extended description

        1110        Countersunk hole           See extended description

        1120        Stepped drilling           See extended description

                                               The diameter is transferred in parameters 1,6,9
        1190        Other Drilling
                                               or 12. There is no further dimensioning



A+W Software GmbH                      EN-A+W EDI Import.docx                                     120 / 162
                                                      Currently, the file name cannot be taken over
        1200        Coating                           yet.
                                                      See extended description

                                                      Currently AWE does not support dimensioning
        1203        Edge Deletion                     types #353845
                                                      See extended description
                                                      Currently, the file name cannot be taken over
        1205        Matting                           yet.
                                                      See extended description
                                                      Currently, the file name cannot be taken over
        1210        Sandblasting                      yet.
                                                      See extended description
                                                      Currently, the file name cannot be taken over
        1215        Coloring                          yet.
                                                      See extended description
                                                      Currently, the file name cannot be taken over
        1220        Enameling                         yet.
                                                      See extended description
                                                      Currently, the file name cannot be taken over
        1225        Silk screen printing              yet.
                                                      See extended description
                    Grooving
        1230                                          See extended description


        1235        Bending                           Not currently supported



        1240        Spherical bending                 Not currently supported


        1245        Alarm net                         See extended description

        1250        Stamp                             See extended description

        1255        Logo                              See extended description



        1300        Corner cut-out                    See extended description

        1305        Corner cut-off                    See extended description

        1310        Rounded corner                    See extended description



        1400        Edge cut-out                      See extended description

        1402        Arc-shaped edge cut-out           See extended description

        1405        Speak-thru                        See extended description

        1410        Handle                            See extended description



A+W Software GmbH                             EN-A+W EDI Import.docx                                  121 / 162
        1415         Inner cut-out                       See extended description


        1520         Heat Soak

        1650         Enameling / UV protection           As of March 2021 see extended description
        1661         Filled corner                       As of March 2021

        1662         Capillary tubes                     As of March 2021

                                                         Edge quality and own macro file is currently not
        1900         Macro                               transported via the interface.
                                                         See extended description


4.15.2 Drillings
4.15.2.1        Drilling (awtyp 1100)
       Parameter 13 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

       If no parameter 13 is sent, then the transfer is carried out in accordance with the old logic (only dimensioning
with respect to corner 1 and all values originate from the interface).
       Here it must be noted that the parameter must be empty (1) or have a value between 1 and 3. If a value
outside of this range is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

       Parameter                         Meaning
       1                                 Item x drilling position 1
       2                                 Item y drilling position 1
       3                                 Diameter of drilling 1
       4                                 Item x drilling position 2
       5                                 Item y drilling position 2
       6                                 Diameter of drilling 2
       7                                 Item x drilling position 3
       8                                 Item y drilling position 3
       9                                 Diameter of drilling 3
       10                                Item x drilling position 4
       11                                Item y drilling position 4
       12                                Diameter of drilling 4
       13                                Dimensioning type (1, 2, 3)
       14                                Reference corner drilling 1 X
       15                                Reference drilling 1 Y (only for dimensioning types 2+3)
       16                                Reference drilling 2 X
       17                                Reference drilling 2 Y (only dimensioning type 2+3)
       18                                Reference drilling 3 X
       19                                Reference drilling 3 Y (only dimensioning type 2+3)
       20                                Reference drilling 4 X
       21                                Reference drilling 4 Y (only dimensioning type 2+3)
       22                                Relief cut (0, 1)
       23                                Edge quality

       Dimensioning type 1: Reference X = reference corner, Reference Y = empty
       Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2


A+W Software GmbH                               EN-A+W EDI Import.docx                                          122 / 162
       Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

       Reference corners:
       The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
       begins in the lower left corner and is incremented counter-clockwise.

       Edges and corners are numbered counterclockwise.
       If the dimensioning type 2 (dimensioning with respect to 2 edges) is sent, then it must be noted that the edge
       sequence (parameter 14/15, 16/17, 18/19, 20/21) must be entered counterclockwise.
       For example
       Correct                                          Incorrect
       Parameter 14: 000030                             000040
       Parameter 15: 000040                             000030

       Parameter 14: 000040                               000010
       Parameter 15: 000010                               000040

       Parameters that contain only empty spaces will be taken over from the AWE master data.

       B1000500000400000100000000000000000000000000000000000000000000000000000001000003

       When this record is loaded, 4(!) drillings are included, where 3 drillings have a diameter of 0 and are located
       directly on the glass edge.

       If you only want one drilling, then the record must look as follows.

       B1000500000400000100                                          000001000003



4.15.2.2        Countersunk hole (awtyp 1110)
       Parameter 12 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2


        If no parameter 12 is sent, there is no scheduling!
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

       Parameter                         Meaning
        1                                Position x
        2                                Position y
       3                                 Diameter (inside)
       4                                 Hole depth (top)
       5                                 Hole depth (bottom)
       6                                 Angle (top)
       7                                 Angle (bottom)
       9                                 Diameter (top)
       10                                Diameter (bottom)
       12                                Dimensioning type          (1, 2, 3)
       13                                Reference drilling 1 X
       14                                Reference drilling 1 Y (only dimensioning type 2+3)
       15                                Relief cut (0, 1)
       16                                (FREE)
       17                                Position drilling 2 X

A+W Software GmbH                                EN-A+W EDI Import.docx                                         123 / 162
      18                               Position drilling 2 Y
       19                              Reference drilling 2 X
      20                               Reference drilling 2 Y (only for dimensioning types 2+3)
      21                               Position drilling 3 X
      22                               Position drilling 3 Y
       23                              Reference drilling 3 X
      24                               Reference drilling 3 Y (only for dimensioning types 2+3)
      25                               Position drilling 4 X
      26                               Position drilling 4 Y
       27                              Reference drilling 4 X
      28                               Reference drilling 4 Y (only for dimensioning types 2+3)
      29                               Edge quality


      Dimensioning type 1: Reference X = reference corner, Reference Y = empty
      Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
      Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

      Edges and corners are numbered counterclockwise.
      If the dimensioning type 2 (dimensioning with respect to 2 edges) is sent, then it must be noted that the edge
      sequence (parameter 13/14, 19/20, 23/24, 27/28) must be entered counterclockwise.
      For example
      Correct                                          Incorrect
      Parameter 13: 000030                             000040
      Parameter 14: 000040                             000030

      Parameter 13: 000040                              000010
      Parameter 14: 000010                              000040

      Parameters that contain only empty spaces will be taken over from the AWE master data.

      Reference corners:
      The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
      begins in the lower left corner and is incremented counter-clockwise.



4.15.2.3       Stepped drilling (awtyp 1120)
       Parameter 14 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

       If no parameter 14 is sent, there is no scheduling!
       Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
       is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
       value and then the following parameter assignments apply:

      Parameter                        Meaning
       1                               Position x
      2                                Position y
      3                                Reference drilling 1 X
       4-13                            Diameter 1-10 (one diameter per lite in the BOM)
       14                              Dimensioning type          (1, 2, 3)
       15                              Reference drilling 1 Y (only for dimensioning types 2+3)
       22                              Relief cut
       17                              Position drilling 2 X
       18                              Position drilling 2 Y

A+W Software GmbH                              EN-A+W EDI Import.docx                                         124 / 162
         19                             Reference drilling 2 X
        20                              Reference drilling 2 Y (only for dimensioning types 2+3)
        21                              Position drilling 3 X
        22                              Position drilling 3 Y
         23                             Reference drilling 3 X
        24                              Reference drilling 3 Y (only for dimensioning types 2+3)
        25                              Position drilling 4 X
        26                              Position drilling 4 Y
         27                             Reference drilling 4 X
        28                              Reference drilling 4 Y (only for dimensioning types 2+3)
        29                              Edge quality

Dimensioning type 1: Reference X = reference corner, Reference Y = empty
Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

Edges and corners are numbered counterclockwise.
If the dimensioning type 2 (dimensioning with respect to 2 edges) is sent, then it must be noted that the edge
sequence (parameter 3/15, 19/20, 23/24, 27/28) must be entered counterclockwise.
        Correct                                          Incorrect
        Parameter 19: 000030                             000040
        Parameter 20: 000040                             000030

       Parameter 19: 000040                              000010
       Parameter 20: 000010                              000040

Reference corners:
The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.

Parameters that contain only empty spaces will be taken over from the AWE master data.

4.15.3 Surface processings
4.15.3.1        Decoating (1203)
       Parameter 1 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

        If no parameter 1 is sent, there is no scheduling!
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

       Parameter                       Meaning
1                               Dimensioning type         (1, 2, 3)
        2                              angle
        3                              Reference edge
        4                              Reference point
        5…8                            (free)
        9                              Parallel elongation
        10                             Perpendicular elongation
        11                             Position X
        12                             Position Y
        13                             Reference X
        14…15                          (free)


A+W Software GmbH                               EN-A+W EDI Import.docx                                           125 / 162
        16                               Reference Y (only for dimensioning types 2+3)
        17…29                            (free)

       Dimensioning type 1: Reference X = reference corner, Reference Y = empty
       Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
       Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

       Edges and corners are numbered counterclockwise.
       If the dimensioning type 2 (dimensioning with respect to 2 edges) is sent, then it must be noted that the edge
       sequence (parameter 13/16) must be entered counterclockwise.
       Correct                                          Incorrect
       Parameter 13: 000030                             000040
       Parameter 16: 000040                             000030

       Parameter 13: 000040                               000010
       Parameter 16: 000010                               000040

       Reference corners:
       The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
       begins in the lower left corner and is incremented counter-clockwise.

       Parameters that contain only empty spaces will be taken over from the AWE master data. This also applies to
       the edge quality that is currently not transported via the interface.
       The level is transferred by the data record S1 field 18 "Coating side" (01 - inside = bottom, 02 - outside = top).


4.15.3.2        Coating (1200)

4.15.3.3        Matting (1205)

4.15.3.4        Sandblasting (1210)

4.15.3.5        Coloring (1215)

4.15.3.6        Enameling (1220)

4.15.3.7        Screen printing (1225)


       Parameter 1 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

        If no parameter 1 is sent, there is no scheduling!
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

       Parameter                        Meaning
1                                Dimensioning type         (1, 2, 3)
        2                               angle
        3                               Reference edge
        4                               Reference point
        5..8                            (free)
        9                               Parallel elongation


A+W Software GmbH                                EN-A+W EDI Import.docx                                          126 / 162
        10                                Perpendicular elongation
        11                                Position x
         12                               Position y
        13                                Reference X
        14                                Shift number
        15                                Saturation
        16                                Reference Y
        17                                Scaling (0-free, 1 – proport. width, 2 – proport. height, 3 - fix)
        18                                Mirror (0 – no, 1 - yes)

       Dimensioning type 1: Reference X = reference corner, Reference Y = empty
       Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
       Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

       Edges and corners are numbered counterclockwise.
       If the dimensioning type 2 (dimensioning with respect to 2 edges) is sent, then it must be noted that the edge
       sequence (parameter 13/16) must be entered counterclockwise.
       Correct                                          Incorrect
       Parameter 13: 000030                             000040
       Parameter 16: 000040                             000030

       Parameter 13: 000040                                000010
       Parameter 16: 000010                                000040

       Reference corners:
       The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
       begins in the lower left corner and is incremented counter-clockwise.

       Parameters that contain only empty spaces will be taken over from the AWE master data. This also applies to
       the edge quality that is currently not transported via the interface.
       The level is transferred by the data record S1 field 18 "Coating side" (01 - inside = bottom, 02 - outside = top).

       The color is transferred via the data record S1 field 8 "color".

       Currently, the file name is not yet read in.

4.15.3.8        Enameling / UV protection (1650)
        Parameter                         Meaning
        1..8                              Edge 1 - 8
        9                                 -Depth (width of processing)
        10                                Distance to edge
The level is transferred by the data record S1 field 18 "Coating side" (01 - inside = bottom, 02 - outside = top)
Per B1 record, only one edge (parameters 1-8) may count as processed! If several edges are marked as processed,
there is no scheduling.
4.15.3.9        Fluted bevel (1230)
       Parameter 22 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

        If no parameter 22 is sent, there is no scheduling.
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:



A+W Software GmbH                                 EN-A+W EDI Import.docx                                         127 / 162
       Parameter                         Meaning
       1..8                              Edge 1 - 8
       9                                 Distance to the edge
       10                                Distance to the corner
       11..18                            Length on edges 1-8
       19                                width
       20                                bevel number
       21                                Reference corner / edge (dimensioning type 2 + 3)
       22                                Dimensioning type (1, 2, 3) – currently not supported by A+W Business
       23                                Reference edge
       24                                Reference point
       25                                Angle of rotation

       The parameters 22 ff. are not currently supported by A+W Business.

       Reference corners:
       The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
       begins in the lower left corner and is incremented counter-clockwise.

      Per B1 record, only one edge (parameters 1-8) may count as processed! If several edges are marked as
processed, there is no scheduling.


4.15.3.10       Stamp (1250)

4.15.3.11       Logos (1255)
       Parameter 7 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

        If no parameter 7 is sent, there is no scheduling.
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

Parameter                        Meaning
1                                Distance A
2                                Distance B
3                                Reference corner
4                                Logo number
5                                Reference edge
6                                Type (1-4) – is not supported during import into A+W Enterprise
7                                Dimensioning type (1, 2, 3) – currently not supported by A+W Business
8                                Width (parallel)
9                                Height (perpendicular)
10                               Reference point
11                               Reference edge
12                               Angle of rotation
18                               Mirror around center point (#456954) (not supported by AWB)

The parameters 7 ff. are not currently supported by A+W Business.

The level is transferred by the data record S1 field 18 "Coating side". (01 – inside = bottom; 02 – outside = top)
Reference corners:



A+W Software GmbH                               EN-A+W EDI Import.docx                                           128 / 162
The reference corners are NOT zero-based. That is, for corner 1, a 1 is written, for corner 2 a 2, etc.The numbering
begins in the lower left corner and is incremented counter-clockwise.



4.15.4 Corner processings
Parameters that contain only empty spaces will be taken over from the AWE master data.



4.15.4.1        Corner cutouts (1300)

Parameter                       Meaning
1..8                            Corner 1 – 8
9                               Distance A
10                              Distance B
11..18                          (free)
19                              Cutout edge A (vert./parallel)
20                              Cutout edge B (vert./parallel)
21                              Radius outer corner
22                              Radius inner corner
23                              Edge quality
The parameter 23 is not currently supported by A+W Business.



4.15.4.2        Corner cutouts (1305)

Parameter                       Meaning
1..8                            Corner 1 – 8
9                               Distance A ( width )
10                              Distance B ( height )
11                              Edge quality

The parameter 11 is not currently supported by A+W Business.


4.15.4.3        Rounded corners (1310)

Parameter                       Meaning
1..8                            Corner 1 – 7
9..10                           (free)
11                              Radius
13                              Edge quality

The parameter 13 is not currently supported by A+W Business.


4.15.5 Complex geometric processings

Parameters that contain only empty spaces will be taken over from the AWE master data.
4.15.5.1        Edge cutouts (1400)

Parameter                       Meaning
1..8                            Edge 1 - 8


A+W Software GmbH                              EN-A+W EDI Import.docx                                         129 / 162
9                               Length ( width )
10                              Depth ( height )
11..18                          free
19                              Distance to the corner
20                              Reference corner
21                              Radius outer corner
22                              Radius inner corner
23                              Edge quality

Reference corners:
The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering begins
in the lower left corner and is incremented counter-clockwise.



The parameter 23 is not currently supported by A+W Business. Parameter 30 is not evaluated by A+W Enterprise.


4.15.5.2         Arched edge cutouts (1402)

Parameter                       Meaning
1..8                            Edge 1 – 8 on which the cutout is made (only for type 1)
9                               Drilling radius
10                              Chord length (only for type 1)
11                              Distance to the corner (only type 1)
12                              Position x (only type 0)
13                              Position y (only type 0)
15                              Type (x/y = 0, Chord/Radius = 1)
19                              Reference corner
21                              Radius outer corner
22                              Edge quality
30                              Entry type (1 = Multi, 2 = Single)

The parameter 22 is not currently supported by A+W Business. Parameter 30 is not evaluated by A+W Enterprise.


4.15.5.3         Speaker holes (1405)

4.15.5.4         Interior cutouts (1415)
         Parameter 14 defines the dimensioning type
         1 – dimensioning with respect to corner => alcib mtyp = 0
         1 – Dimensioning with respect to 2 edges => mtyp = 1
         3 – dimensioning with respect to corner and edge => mtyp=2

        If no parameter 14 is sent, there is no scheduling!
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

Parameter                       Meaning
      1                                 Position x
 2                              Position y
3..8                            (free)
9                               width
10                              height
11                              Reference corner

A+W Software GmbH                               EN-A+W EDI Import.docx                                         130 / 162
12                              Reference edge (dimensioning type 2 + 3)
13                              Inner radius
14                              Dimensioning type       (1, 2, 3)
15                              Angle of rotation
16                              Edge (alignment)
17                              Object reference point
18                              Edge quality

       Dimensioning type 1: Reference X = reference corner, Reference Y = empty
       Dimensioning type 2: Reference X = reference corner1, Reference Y = referenceedge2
       Dimensioning type 3: Reference X = reference corner, Reference Y = reference edge

       Reference corners:
       The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
       begins in the lower left corner and is incremented counter-clockwise.

The parameter 18 is not currently supported by A+W Business. Parameter 30 is not evaluated by A+W Enterprise.


4.15.5.5        Handles (1410)
       Parameter 22 defines the dimensioning type
       1 – dimensioning with respect to corner => alcib mtyp = 0
       1 – Dimensioning with respect to 2 edges => mtyp = 1
       3 – dimensioning with respect to corner and edge => mtyp=2

        If no parameter 22 is sent, there is no scheduling!
        Here it must be noted that the parameter must have a value between 1 and 3. If a value outside of this range
is sent, there is no scheduling!

       If the dimensioning type is sent in the interface, only the parameters are taken over that contain a numeric
value and then the following parameter assignments apply:

Parameter                       Meaning
1..8                            Edge 1 – 8 (only dimensioning type 2+3)
9                               Length ( width )
10                              Depth ( height )
19                              Reference corner
20                              Distance to the corner
21                              Distance to the edge
22                              Dimensioning type        (1, 2, 3)
23                              Angle of rotation
24                              Edge (alignment)
25                              Object reference point

       Reference corners:
       The reference corners are zero-based. That is, for corner 1, a 0 is written, for corner 2 a 1, etc.The numbering
       begins in the lower left corner and is incremented counter-clockwise.


4.15.6 Other processings
4.15.6.1        Macro (awtyp 1900)
       The following parameter mappings apply:

       Parameter                        Meaning
       1..8                             Edge 1 - 8
       9..10                            (free)
       11                               Distance


A+W Software GmbH                               EN-A+W EDI Import.docx                                         131 / 162
       12                                Alignment (0 = right, 1 = left)

        Analogous to edge processing, the edge number is not transferred in the interface, but instead the parameter
is assigned (greater than zero) whose edge is processed. If the macro is placed at edge 3, in parameter 3 "000010"
must be transferred. The alignment defines whether the macro is dimensioned up to the right (0) or left (1) corner.
The edges are counted counter-clockwise.
        The examination left/right is always done as if the glass is standing on the reference edge (e.g. edge 1 right
means corner 2; edge 1 left means corner 1; edge 4 right means corner 1)


4.15.6.2        Parametric macro (awtyp 1920) / parametric surface macro (awtyp 1930)
        The import is (as of 09/11/2020) not implemented.

        The bit vector that indicates whether or not a parameter is to be converted is really transferred as bit
        vector.

        Example: there are 3 parameters; of these, parameters 1 and 3 with conversion. This results in the
        sequence "101". In the interface, the value "5" is transferred in the bit vector parameter.

4.15.7 Dimensional precision (AWE 6)

        Previously, the external standard interface could be configured so that muntin dimensions in 1/10 mm were
        taken over.
        The item dimensions, shape dimensions and processing parameters, by contrast, could only be taken over in
        full mm. Starting with this version (AWE 6), the function for storage has been expanded.
        In order to be able to enter item dimensions in the manual transaction entry/changing in 1/10 mm, the system
        must in principle be configured for 1/10 mm. For this, the environment variable IMP_CTRL_NTEL_MM must
        be set. Within the standard interface, the environment variable DFUE_NTEL_MM is evaluated. If the
        variable DFUE_NTEL_MM is active, then all dimensions are taken over from the standard interface in 1/10
        mm.

        If the variable DFUE_NTEL_MM is not active, it is possible to control the individual dimensions separately.

        Processing parameters

                Processing parameters for processings with A+W processing type that are sent via the B1 record
                can be taken over in 1/10 mm regardless of the item dimensions. For this, the environment variable
                DFUE_BEARBMASS10 must be activated. This possibility is new with this version.

                If, however, the environment variable DFUE_NTEL_MM is active, the environment variable
                DFUE_BEARBMASS10 is not evaluated and the processing parameters in 1/10 mm are also taken
                over.


4.16 Barcode (BC)
The BC record is written to the table kposzusatz by default. Here, the first 20 characters in the field barcode_char
and the first 80 characters in the field txt are transmitted. The data from the table kposzusatz is not displayed in the
order entry.

Starting in November 2024/i000 filter - 13.04.10324

The content of the BC record can also be taken over as item text. In which sequence the BC record is taken over
depends on whether it is transferred before of after the T<n> records.

The takeover is controlled by the client-specific environment variable "DF"UE_BCAST1". If the variable is activated
with the value "ON," the content of the BC record is taken over unchanged. If the variable is activated with another
value, then this value (maximum 5 characters) is used as prefix for the barcode.



A+W Software GmbH                                EN-A+W EDI Import.docx                                           132 / 162
If the barcode (including prefix) is longer than 80 characters, then there is a line break after 80 characters. The new
lines no longer include the prefix.


4.17 Muntins (C1)

4.17.1 Muntin symmetry / Calculation type
        The definition of the values for the muntin symmetry is different within the interface definition of the
        default filter than it is in ALCIB. Therefore it is required to convert the values. (Implemented in ALCIB –
        version 3.1, and as of ALCIB – version 4.0)

        For the simple transfer of values from the C1 record, the following problem occurs:

        Calculation type in C1 record             ALCIB

        0 = Drill-point symmetrical      not defined

        1 = Field symmetrical            Field symmetrical.

        2 = Drill point-asymm.                    field symmetrical + Editor

        3 = Field-asymm.                                  drilling point symmetrical

        If the system is configured accordingly (environment variable DFUE_SPROSSSYMKZ), the calculation
        type from record C1 will be converted to the correct ALCIB values.

        DFUE_SPROSSSYMKZ
        At external order entry, this variable controls the muntin symmetry code.
                      o 1 – The code that is delivered in the interface is converted to ALCIB values
                      o 2 – The code that is delivered in the interface is not changed
        If this variable has not been set, 2 (field-symmetrical + editor) will always be transferred.
        This has no effect on the actual muntin structure.

        Generally, everywhere where GLASMARKT is defined, the variable DFUE_SPROSSSYMKZ=2 should be
        set. As of ALCIB 4.0 only DFUE_SPROSSSYMKZ is analyzed.

        ATTENTION: For all users for which the environment variable GLASMARKT has been set for order
        entry via standard filter:

        If you request an unchanged transfer of the muntin calculation type, you must set environment
        variable DFUE_SPROSSSYMKZ=2. As of version 4.0, the environment variable GLASMARKT is no
        longer analyzed if the muntin symmetry code is filled.

        The muntin calculation type or code has no effect on the actual muntin structure.


        Currently it is not possible to transfer different calculation types within an item for vertical and horizontal
        muntins. Similarly, it is not possible if different muntins are transferred with the same orientation within an
        item. Generally, the calculation type of the first C1 record of an item is used.

4.17.2 Muntin parameters
        Up to 12 muntin parameters are processed within the C1 record. These parameters are always drill hole
        sizes of the muntins. The dimensions in all parameter fields must be transferred as absolute dimension
        from the origin!

        If no muntin parameters are transferred, it is assumed that the muntin structure is "drill hole symmetrical".
        The muntin calculation type (symmetry code) is not analyzed for this purpose.

        However, if environment variable DFUE_SPROSSSYMKZ=1 has been set (see section "Muntins (C1)",
        Section "Muntin Symmetry"), calculation of the drill holes is executed field-symmetrical for calculation



A+W Software GmbH                                EN-A+W EDI Import.docx                                            133 / 162
        types " 1 - Field sym." and "3 - Field asym.", and the symmetry code "field-symmetrical" is transferred. In
        all other cases, the calculation is executed drill hole symmetrical and transferred as a symmetry code.

        Since the calculation "field symmetrical" depends on the settings within the ALCIB articles, the final
        calculation of the drill points is only executed when the muntin documents are printed.

Imperial system (Inch): Starting with interface version 02.2.025, the FH record was expanded to include the
"Fraction" field. The inch fraction is specified in this field. If the value is > 1, then the fields are interpreted as inch
(Inch * fraction). The standard interface recalculates these values in mm by itself. In the AWE tables, the mm are
saved with 4 places after the decimal point regardless of DFUE_NTEL_MM.

4.17.3 Dimensional precision (AWE 6)

        Previously, the external standard interface could be configured so that muntin dimensions in 1/10 mm were
        taken over.
        The item dimensions, shape dimensions and processing parameters, by contrast, could only be taken over in
        full mm. Starting with this version (AWE 6), the function for storage has been expanded.
        In order to be able to enter item dimensions in the manual transaction entry/changing in 1/10 mm, the system
        must in principle be configured for 1/10 mm. For this, the environment variable IMP_CTRL_NTEL_MM must
        be set. Within the standard interface, the environment variable DFUE_NTEL_MM is evaluated. If the
        variable DFUE_NTEL_MM is active, then all dimensions are taken over from the standard interface in 1/10
        mm.

        If the variable DFUE_NTEL_MM is not active, it is possible to control the individual dimensions separately.

        Muntin dimensions

                 Muntin dimensions can be taken over in 1/10 mm regardless of the item dimensions. For this, the
                 environment variable DFUE_SPROSSENMASS10 must be activated. This possibility already
                 existed in the previous versions.

                 If, however, the environment variables IMP_CTRL_NTEL_MM und DFUE_NTEL_MM are active, the
                 environment variable DFUE_SPROSSENMASS10 is not evaluated and the muntin dimensions will
                 be taken over in 1/10 mm.


4.18 Muntins (CA)
If no CA record is written, the function for optimizing the BOM headers (DFUE_OPT_POSKONR) cannot work
correctly. The case of 2 C1 records with the same muntin item number (vertical and horizontal Georgian bar), there
is also no combination of the data records for the AWD BOM. This has direct effects on the texting, price calculation
and the AWE-internal order generation.


4.19 SN template (V1)

This record type is only supported by A+W Enterprise.

Previously, control is implemented through the variable MODUL_SN_TEMPLATE. With an activated variable, the
   parameter string is interpreted by numeric values of the format 7.1. The parameters transferred (maximum 73) are
   saved in the table kpostemplate.

Imperial system (Inch): Starting with interface version 02.2.025, the FH record was expanded to include the
"Fraction" field. The inch fraction is specified in this field. If the value is > 1, then the individual parameters are
interpreted as inch (Inch * fraction). Whether an individual parameter is interpreted as inch and thus converted into
mm depends on the master data definition of the template parameter (table xtempparam.convert; menu: "Master
data - Keys - Product - Template parameter"). The standard interface recalculates these values in mm by itself. In
the AWE tables, the mm are saved with 4 places after the decimal point regardless of DFUE_NTEL_MM.



A+W Software GmbH                                   EN-A+W EDI Import.docx                                              134 / 162
With the use of templates, the M1 record is also required. The template name is transported in the M1 record. For
the use of the M1 record as template name without shape parameter, a modelnumber=0 is permitted.

For detailed information, see the "Template" section of "DE-CONFIG A+W Enterprise EDI"




4.20 Environment variables


    •   DFUE_BEARBMASS10 (section: Dimensional precision)
        If the environment variables DFUE_NTEL_MM or IMP_CTRL_NTEL_MM are not set, this variable controls
        the takeover of the dimension parameters within the external default interface. If the variable is set, then the
        processing parameters will be taken over in 1/10 mm. The variable is not set, the parameters will be taken
        over in mm and any places after the decimal point will be cut off. #350104

    •   DFUE_ERROR_SUBPATH
        In this variable, a subdirectory can be specified into which the incorrectly processed file should be moved.
        The path specification is relative to the initial directory. If the subdirectory is parallel to the initial directory,
        then it must be specified with " ".. (e.g. ../error).
        Currently the variable is only evaluated by the default filter
        see also DFUE_SUCCESS_SUBPATH, Extern_Leitfaden_externe_Auftragsübertragung.doc

    •   DFUE_EXREF_FILE (section: external P.O. text)
        If set, the name of the interface file is written to kauf.exaufnr otherwise to kauf.exbez1. (see also
        DFUE_POTEXT)
    •   DFUE_GAS_LEVEL (section: Gas)
        The variable defines for the external order scheduling on which level gas is attached in the IGU.
             o 1 - First level, next to frame
             o 2 - Second level, in frame
             o 3 - The level is defined in the interface file
             o If this variable is not set, the gas will be added to the frame.

    •   DFUE_ITEM_SPLITT (section: Item split)
        If the variable is set to 1, sent items are split according to an individually-defined criterion (#337294)


    •   DFUE_KUARTBEZ_TO_KPOSEX                       (section: item designation)
        If the variable is set, the data that the filter writes in fields artbez1-3 of the intermediate table _ialf_kpos is
        written to kposex.exarttxt.

    •   DFUE_NTEL_MM (section: Dimensional precision)
        If the variable is set, all (defined) dimensions are taken over in 1/10 mm. For details, see the individual
sections (#350104)

    •   DFUE_OHNE_ARTKUZU
        Within the external DFÜ, for each customer who sends orders via external DFÜ a conversion of the
        customer item number into an AWE item number is stored (artkuzu). If the customer already makes a
        conversion and sends AWE item numbers, then setting this environment variable means that there does
        not have to be a repeated assignment in ALCIB.
        This means that if the conversion is stored in AWE, it is used. If no conversion is stored, the number sent
        is used as ALCIB number. Currently this only works for header items and muntins without prefix.
    •   DFUE_ONLINE_TYP



A+W Software GmbH                                   EN-A+W EDI Import.docx                                               135 / 162
       The variable controls the scheduling of orders via the default interface. If the variable, then an order will
       not be marked as Entry "DFÜ", but rather
       as entry "ONLINE". The variable currently includes 2 values, which are separated by '|' (<type>|<value>).
       Currently supported is:
       Type = 1 => if <value> = <transferred A/Z debtor> => entry = Online
   •   DFUE_OPT_POSKONR
       CAUTION: If the DFUE_OPT_POSKONR variant greater than 1 is used, an interface version greater than or
       equal to 2.2.014 is assumed.
       This variable controls the number of BOM headers for orders that are scheduled via external EDI.
       If the variable is set to 1, then the following is checked between 2 items
       next to one another:
           AIR/AIR2,2 spacer, spacer color,2 muntins, muntin color, item color
       If the variable is set to 2, then stamps are also checked.
       Additional explanation: EN-CONFIG-A+W Enterprise EDI.docx
       Alt: Additional explanation: Extern_Leitfaden_externe_Auftragsübertragung.doc

       CAUTION: If the DFUE_OPT_POSKONR variant greater than 1 is used, an interface version greater
       than or equal to 2.2.014 is assumed.

   •   DFUE_POTEXT(section: external P.O. text)
       Within the default filter (i000filter), this variable controls the evaluation
       of the fields K1: POtext1 and K1: POtext2
       for a precise description of the variants see interface documentation
       the interface documentation (see also DFUE_EXREF_FILE)
   •   DFUE_SCHOLL_GWTERM              (section: item designation / customer item)
       Special logic for the assignment of some fields for the importing of orders via the default filter:
           o    P1 record:Fld 15 (Itm 363) => Fld 5 (Itm.147) ==> 20 digits after kupos
           o    P1 record:Fld 14 (Pos 283) => Fld 22 (Pos.422) ==> 70 characters after kommtxt

   •   DFUE_SUCCESS_SUBPATH
       In these variables, a subdirectory can be specified into which the successfully processed file should be
       moved. The path specification is relative to the initial directory. If the subdirectory is parallel to the initial
       directory, then it must be specified with " ".. (e.g. ../archive).
       Currently the variable is only evaluated by the default filter
       see also DFUE_ERROR_SUBPATH, Extern_Leitfaden_externe_Auftragsübertragung.doc

   •   DFUE_ SPROSSSYMKZ               (section: muntin symmetry / Georgian bar parameters)
       Within the external order scheduling, the variable controls the assignment of the Georgian bar identifier.
           o 1 – The code that is delivered in the interface is converted to ALCIB values
           o 2 – The code that is delivered in the interface is not changed
           o If this variable has not been set, 1 (field-symmetrical) will always be transferred. This has no
               effect on the actual muntin structure.

   •   GLASMARKT
       This variable controls various special logic, which gradually should be made independent of it if
       necessary.
           o   Variable INDIR must be set

           o   Check of IN-directory based on the "receiving company number" that has been transferred in the
               FH record

           o   Special solution for frame replacement
   •   INDIR (within the interface only with set variable GLASMARKT)
       The variable defines the incoming directory for the external order interface. The external EDI expects the



A+W Software GmbH                                 EN-A+W EDI Import.docx                                               136 / 162
       transfer files in this directory. The directory has to have a sub-directory "Save". After successful
       processing, the transfer files are moved to the sub-directory.

   •   INTAUF_AHAM_TEST
       If an order is scheduled via external interface, the background process INTAUF calculates the
       resulting SR using the master data.
       #365411




A+W Software GmbH                               EN-A+W EDI Import.docx                                        137 / 162
5 A+W Enterprise export-specific field notes
5.1       Supplier configuration
       If in the following section discussion is of "supplier configuration," this is a setting in A+W Enterprise. For
more precise information about this, see "EN-CONFIG-A+W Enterprise EDI.pdf".

      For which data records are currently being exported, see the Data record overview at the start of the
document.

          NIU = Not In Use

        Among other things, the supplier configuration defines whether the export is to A+ W Business (supplier
configuration ID 66):


5.2       File header record FH
See also: AWB File header record




      No.     Name                                   ALCIB note                                     IV         PS


      1       Record type                            FH
                                                                                                    2.2.000    6.0

      2       Version number                         nn.mm.zzz (Supplier configuration ID 49)
                                                                                                    2.2.032
                                                     (default 02.2.032)
      3       Total characters                       Number of bytes of export file.                2.2.000
      4       Sending company number                 Default: 0
                                                     During export to AWB:                          2.2.010
                                                     (Supplier configuration ID = 67)
      5       Receiving company number               Default: 0
                                                     During export to AWB (supplier                 2.2.010
                                                     configuration: ID 68)
      6       Inch-Fraction                          Default 1 – metric (Supplier configuration
                                                                                                    2.2.025    6,0
                                                     ID 51)
      7       User-defined field                     SP: cu_edi_cust_record_fh
                                                     Parameter: auftrnr int, vorgang smallint,
                                                     subnr smallint, still smallint
                                                     Return-Wert: char(100)
      8       Coding                                 Default coding: UTF-8 (Supplier                2.2.033    6.0
                                                     configuration ID 53)
      7       Filler


          Table: File header record


Version number: currently, only Version 02.2.032 is supported



A+W Software GmbH                                EN-A+W EDI Import.docx                                              138 / 162
Inch fraction: inch fraction, e.g. 16 / 32 / 64

Accepted entries: ISO8859-1, ISO8859-2, ISO8859-15, UTF-8, 819(like ISO-1), 1250(like ISO-2), 1252(like ISO-
15), 57372(like UTF-8)




A+W Software GmbH                                 EN-A+W EDI Import.docx                                 139 / 162
5.3    General header record K1
See also 2.2 AWB "Header record general"



                                                                         AWE Database

No.   Name                 AWE note                                                                     IV        PS


1     Record type          K1                                                                           2.2.000

2     Document type        5                                             Based on Kauf.vorgang          2.2.015
                                                                         Kauf.vorgang=2 => document
                                                                         type = 5


3     Mode                 1 = New                                       See K1 mode                    2.2.000
                           2=change
                           3=cancel
4     Customer no.         External customer number in supplier          mp.extkundnr where mp.mpnr =   2.2.000
                           master                                        kauf.kunr and mp.kuliflag=1
                           (My customer number at the supplier)
5     Delivery date        Date requested by customer                    kauf.ltplan                    2.2.000
6     P.O. date                                                          bauf.bdat                      2.2.000

7     Purchase text 1      External number                               kauf.exaufnr                   2.2.000


8     Purchase text 2      Purchase information                          kauf.exbez1                    2.2.000

9     Predefined           Number of the PO. in A+W Enterprise           kauf.auftrnr                   2.2.000
      document number
10    Bill of landing      NIU                                           0                              2.2.000
      number
11    Site number          NIU                                           0                              2.2.000
12    Height above nn      NIU                                           0                              2.2.000
      (in meters)
13    Status               0000                                          Fix                            2.2.001
14    KZ locked            NIU                                           0                              2.2.001
15    Delivery code        0=no direct delivery                          kauf.geschart                  2.2.003
                           1 =direct delivery by supplier
                           2 = pick-up by customer


16    User-defined field   SP: cu_edi_cust_record_k1                                                    2.2.015
                           Parameter: auftrnr int, vorgang smallint,
                           subnr smallint, still smallint
                           Return-Wert: char(100)
17    Priority             0 = Standard; 1 = Urgent, 9 = Call            Eilt: kauf.schnell = 1 UND     2.2.023
                                                                         kauf.abruf=2
                                                                         Abruf: kauf.abruf=1



A+W Software GmbH                               EN-A+W EDI Import.docx                                       140 / 162
                                                          AWE Database

No.   Name            AWE note                                           IV        PS


18    Object                                              kauf.objnr     2.2.023
19    Architect       NIU                                                2.2.023
20    Delivery date   NIU                                                2.2.027
21    Production      NIU                                                2.2.028
      preparation
22    Business type   NIU                                                2.2.028
23    Filler          NIU




A+W Software GmbH                EN-A+W EDI Import.docx                       141 / 162
5.4    General header K2
No.   Name                     AWE note                                 AWE Database                    IV   PS
1     Record type              K2
2     Customer address -       Customer's address, not that of the      Mp.name
      name 1                   supplier
3     Customer address -       The customer arises from xhaus.kunr      Mp.vname
      name 2                   where xhaus.hnr=kauf.hausnr
4     Customer address -       with xhaus.kunr, you then go to          Mp.zhd
      name 3                   mp.mpnr where kuliflag = 0
5     Customer address -                                                Mp.str
      street
6     Customer address -                                                Mp.ort
      city
7     Customer address - zip                                            Mp.plz
      code
8     Customer address -                                                Mp.postfach
      post box
9     Customer address -                                                Mp.pfplz
      post box - zip code
10    Customer address -       Default:                                 Default:
      country code             Country code                             mp.kfzcode where mp.mpnr =
                                                                        kauf.kunr and mp.kuliflag=1
                               Export to AWB:
                               (delivery configuration ID 66):          Export to AWB:
                               IG country code                          xxland.iso where xxland.kfz =
                                                                        mp.kfzcode
11    Customer address -       NIU
      province/state
12    Customer address - fax                                            Mp.faxnr
13    Customer address -                                                Mp.telefon
      phone
14    Customer address -       NIU
      employee
15    Filler




A+W Software GmbH                              EN-A+W EDI Import.docx                                   142 / 162
5.5    General header K3
       Table: General header record

See also AWB "Delivery Address" and AWE section 4 " insert segmentsDelivery Address"


No.   Name                            AWE note                                 AWE Database                  IV   PS
1     Record type                     K3
2     Shipping address - no.          NIU
3     Shipping address -              Shipping address for the customer, not   Adr.adrname
      name 1                          that of the supplier
4     Shipping address -              The supplier address arises from         Adr.adrvname
      name 2                          kauf._ladrnr=adr.adrnr
5     Shipping address -                                                       Adr.zhd
      name 3
6     Shipping address -                                                       Adr.str
      street
7     Shipping address - city                                                  Adr.ort
8     Shipping address - zip                                                   Adr.plz
      code
9     Shipping address -              NIU
      province/state
10    Shipping address -              IG country code                          xxland.iso where xxland.kfz
      country code                                                             = adr.kfzcode
11    Delivery request                NIU
                                      The prior use of the field "abruf" is
                                      actually in K1/17 - priority
12    Shipping address -                                                       Adr.telefon
      phone
13    Shipping address -              NIU
      employee
14    Filler




A+W Software GmbH                                    EN-A+W EDI Import.docx                                  143 / 162
5.6    Document link DL
This item record is always written if documents were attached on PO header level (kaufref.posnr=0)

                                                                                       AWE Database

No.    Name                                      ALCIB note                                             IV          PS


1      Record type                               DL                                                     2.2.018     2011
2      Description of document link              NIU                                                    2.2.018     2011
3      Relative link to linked document                                                Kaufref.datei
                                                                                       where
                                                 <document                             auftrnr=<docum
                                                 number>_>document                     ent> and         2.2.018     2011
                                                 type>_<item>_file name                vorgang=<docu
                                                                                       ment type> and
                                                                                       posnr=0
4      Filler



5.7    Text record T2
This record type is not always written. It is only written if the following texts exist for the PO:
        - Manual PO header texts
        - Manual PO footer text
        - Supplier texts (SP)

The precise description of the stored procedure (SP) is in "EN-CONFIG-A+W Enterprise EDI.pdf".

                                                                                    AWE Database

No.    Name                                      ALCIB note                                             IV          PS


1      Record type                               T2                                                     2.2.005     3.1
2      Type                                      1 - Header texts
                                                 2 – Footer texts                                       2.2.005     3.1

3      Text identifier                           Only via SP                                            2.2.005     3.1
4      Text                                                                                             2.2.005     3.1
5      Filler



5.8    Item record P1
This record type exists once in every item; if it is repeated, a new item is created; it must be preceded by a K1
record.

See also AWE „Item record P1“


No.   Name               AWE note                                                            AWE Database         IV      PS
1     Record type        P1


A+W Software GmbH                                  EN-A+W EDI Import.docx                                         144 / 162
2    Product no.      SP: cu_edi_prodnr_record_p1                               Default kpos.artnr
                      Parameters: auftrnr int, aufnr int, posnr smallint
                      Return value: char(64)
3    Description1                                                               kpos.artbez1
4    Bezeichnung2     NIU
     (designation2)
5    Bezeichnung3     NIU
     (designation3)
6    Color                                                                      poszu.txt where
                                                                                tnr=999 or tnr=1
7    Short Name       NIU
8    Width                                                                      kpos.laenge
9    Height                                                                     kpos.breite
10    Quantity                                                                  kpos.menge
11   Item price                                                                 kpos.nstpreis
12   Sense of         0=none, 1=horiz., 2=vert., 3=irrelevant                   aufstrukt.strukthb
     pattern                                                                    0 - none 1 - horiz.
                                                                                2-vertic. 3 -
                                                                                diagonal
13   Pattern side     0=none, 1=inside, 2=outside                               aufstrukt.einbaupos
14   Reference        komm.kommnr where aufnr=kpos.aufnr and                    komm.kommtxt
                      kommnr=kpos.kommnr
15   Customer                                                                   kpos.kuposnr
     item
16   Total            ktechw.dicke is used for glass as item                    ktechw.dicke
     installation                                                               kpos.szr
                      kpos.szr is used for spacer orders
     thickness        (see “EN-CONFIG-A+W Enterprise EDI”
                      See also the environment variable RAHMEN_BESTELLUNG_SZR


17   Edge             NIU
     protection
18   Tight size                                                                 kauf._falzmass
19   KZ locked        NIU
20   Free             0 – no                                                    If kauf.kaufart=2
                      1 – yes
21   Single                                                                     kpos.aham/2
     cutback
22   Coated side      0=none, 1=inside, 2=outside                               aufstrukt.einbaupos
23   Dimensional      NIU
     variant
24   Procurement      NIU
     type
25   Price            NIU
     relevance
     identifier
26   Price type       NIU
27   Item number      NIU



A+W Software GmbH                                EN-A+W EDI Import.docx                               145 / 162
28    Filler

        Table: General item record


1)


5.9    Item record P2



No.    Name                          AWE note                                        AWE Database               IV   PS
1      Record type                   P2
2      Logo no.                      NIU
3      Logo position                 NIU
4      Rack Type                     NIU
5      Lites per rack                NIU
6      Document reference                                                            Kpos.aufnr
7      Item reference                                                                Kpos.posnr (not lfdpos!)
8      Item group of order                                                           Kpos.kuposnr
9      Item text 1                   NIU
10     Item text 2                   NIU
11     Item text 3                   NIU
12     Item text 4                   NIU
13     Item text 5                   NIU
14     Edge decoating                NIU
15     Foreign key for               Caution: the field is only 6 characters long.   rart.bez where
       complaints                    If the text is longer, it will be cut off       kauf._reklamart =
                                                                                     rart.reklamart
16     Restriction check for         NIU
       alternative products
17     User-defined field            SP: cu_edi_cust_record_p2 Parameter:
                                     auftrnr INT, aufnr INT, posnr SMALLINT
                                     RETURNING CHAR(100);
18     Reason for complaint                                                          rspec.bez where
                                                                                     kauf._reklamart =
                                                                                     rspec.reklamspec
19     Complaint place                                                               rort.bez where
                                                                                     kauf._reklamort =
                                                                                     rort.reklamort
20     Supplier of item              NIU
21     Confirmed delivery            NIU
       date
22     Filler




A+W Software GmbH                                     EN-A+W EDI Import.docx                                    146 / 162
5.10 Item record P3
The P3 record is not always exported. It is only exported if it is an order-related PO.

                                                                                             AWE
                                                                                             Databa
No.    Name                                    A+W Enterprise note                           se       IV         PS


1      Record type                             P2                                                     2.2.000
2      Reference for previous P.O.
                                               NIU                                                    2.2.000
       number
3      Reference for previous item
                                               NIU                                                    2.2.000
       number
4      Reference for shipping order
                                               kposref.orgauftrnr                                     2.2.000
       number
5      Reference for the shipping item
                                               kposref.orgposnr                                       2.2.000
       number
6      Reference for end customer's
                                               kauf.exaufnr                                           2.2.000
       P.O. number
7      Reference for end customer's
                                               NIU                                                    2.2.000
       item number
8      Filler



5.11 Document link PL
This record type is always written for attached documents on item level (kaufref.posnr!=0)

                                                                                    AWE Database

No.    Designation                             ALCIB note                                             IV         PS


1      Record type                             PL
2      Description of document link            NIU
3      Relative link to linked document                                             Kaufref.datei
                                                                                    where
                                               <document                            auftrnr=<docme
                                               number>_>document                    nt> and
                                               type>_<item>_file name               vorgang=<docu
                                                                                    ment type> and
                                                                                    posnr=<item>
4      Filler




5.12 Bar code record BC
This record type is not compulsory. This record type is currently only analyzed by A+W Enterprise.

The record is only written it the Stored Procedure „cu_edi_barcode_record_bc“ returns a corresponding value.



A+W Software GmbH                                EN-A+W EDI Import.docx                                         147 / 162
                                                                                             AWE
                                                                                             databa
No.       Designation                          A+W Enterprise note                           se       IV         PS


1         Record type                          BC                                                     2.2.000
2                                              Stored procedure
                                               cu_edi_parcode_record_bc (key_auftrnr
          Barcode                              INT, key_aufnr INT, key_posnr                          2.2.000
                                               SMALLINT)
                                               RETURNING CHAR(500);
3         Filler




5.13 BOM record S1
Each M1 record for steps assumes an S1 record. If an S1 record and an M1 record are written for stepped glass,
then for each stepped glass an individual S1 and M1 are written, even if all the glass is stepped identically.

Not all BOM elements are exported:
    •      Glass: For multiple glasses, the glass of the first BOM level is always exported. If the first BOM
           level is a stock size (e.g. LAMI), then the 2nd BOM level is exported.
    •      Foils: Foils are only exported if the EA flag is set.
    •      Frame/spacer: Frames are always exported
    •      Muntins: Muntins are always exported
      •    Accessory: Accessories are only exported with set EA flag
      •    Processings: Processings are only exported if the EA flag is set.
      •    Steps are always exported
      •    Gas: always exported (see "EN-CONFIG-A+W Enterprise EDI.pdf")

      •    Shapes: if configured via special shape S1 record SP (see "EN-CONFIG-A_W Enterprise EDI.pdf")

5.13.1 Product Types
            Product         Description                 Comment
            type
            1               Single glass                Product group is not assigned
            2               Tempered glass              Product group is not assigned
            3               LAMI                        Product group is not assigned
            11              Muntins                     Product group is not assigned
            12              Shape/step                  Product group 50 – step, 5 - shape
            20              Processings                 Product group is not assigned
            30              Inserts                     Product group 41 – Gas
                                                        Product group 42 - foil
            40              Other items                 Product group 3
            60              Spacer                      Product group 80 - Frame



A+W Software GmbH                                EN-A+W EDI Import.docx                                         148 / 162
                                                                          AWE database

No.     Designation                      A+W Enterprise note                                      IV            PS


1       Record type                      S1                               Table aufstrukt         2.02.000
2       Number (number)                  Is filled according to chapter   aufstrukt.tnr -1        2.02.000
                                         "2.19.1 Details about BOM
                                         structure".
3       Parent number (0=main product)   Is filled according to chapter   aufstrukt.parent -1     2.02.000
                                         "2.19.1 Details about BOM
                                         structure"
4        Level                                                            Glass etc. directly     2.02.000
                                                                          under the header
                                                                          article = 1
                                                                          Gas in the frame
                                                                          would be = 2
5       Position within level            Logic different depending on     Export (default) (not   2.02.000
                                         whether or not the export to     AWB!):
                                         AWB happens.                     Frame/foil with
                                         ---                              EP=1 =>2…
                                         Export to AWB:                   Frame/foil with
                                                                          EP=2 => 4
                                         Is filled according to chapter
                                                                          for glass EP 1/2 =>
                                         "2.19.1 Details about BOM
                                                                          1
                                         structure"
                                                                          for glass EP 3/4 =>
                                         ---                              3
                                         Export (default):                for glass EP 5/6 =>
                                         Presently not filled for         5
                                                                          for glass EP 7/8 =>
                                         • Gas                            7
                                         • Offset
                                         • Muntins
                                         • Processing steps
                                         • Accessories
                                         • Shapes
6       Product no.                      SP: cu_edi_prodnr_record_s1      Aufstrukt.artnr         2.02.000
                                         Parameter: auftrnr, aufnr,
                                         posnr, poskonr, tnr
                                         Return-Wert: char(64)

                                         CREATE PROCEDURE
                                         cu_edi_prodnr_record_s1
                                         (key_auftrnr INT, key_aufnr
                                         INT, key_posnr SMALLINT,
                                         key_poskonr SMALLINT,
                                         key_tnr SMALLINT)
                                         RETURNING CHAR(64);
7       Description                                                       aufstrukt.artbez1       2.02.000
8       Color                                                             Poszu.txt               2.02.000
9       Short Name                       NIU                                                      2.02.000
10      Width (mm)                       NIU                                                      2.02.000



    A+W Software GmbH                          EN-A+W EDI Import.docx                                        149 / 162
                                                                           AWE database

No.   Designation                        A+W Enterprise note                                     IV            PS


11    Height (mm)                        NIU                                                     2.02.000
12    Quantity                                                             aufstrukt.anz1 /      2.02.000
                                                                           poszu.panz1
13    Unit price (do not multiply with                                                           2.02.000
      main quantity)
14    Sense of pattern                   0=none, 1=horiz., 2=vert.,        aufstrukt.strukthb    2.02.000
                                         3=irrelevant                      0 - none
                                         Meaning                           1-vertical
                                         has to be implemented             2-horizontal
                                                                           3-diagonal

15    Pattern side                       This has to be determined         Aufstrukt.einbaupos   2.02.000
                                         from the installation position.
                                         0=none, 1=inside, 2=outside


16    Product type                       Mapping                                                 2.02.000
17    ProductGroup                       Mapping                                                 2.02.007      3.1
18    Coated side                        This has to be determined         Aufstrukt.einbaupos
                                         from the installation position.
                                         0=none, 1=inside, 2=outside                             2.02.009      3.1


19    Thickness (mm)                     For product type =60 and          Kpos.szr
                                         product group=80 (IG spacer),
                                                                           Kposp.szr2
                                         the thickness is interpreted as                         2.02.012      3.1
                                         the airspace.                     Kposp.szr3


20    Vector for production BOM                                                                  2.02.015      NR
21    User-defined field                 SP: cu_edi_cust_record_s1
                                         Parameter: auftrnr, aufnr,
                                         posnr, poskonr, tnr
                                         Return-Wert: char(100)

                                         CREATE PROCEDURE
                                         cu_edi_cust_record_s1                                   2.02.015      NR
                                         (key_auftrnr INT, key_aufnr
                                         INT, key_posnr SMALLINT,
                                         key_poskonr SMALLINT,
                                         key_tnr SMALLINT)
                                         RETURNING CHAR(100);


22    Procurement type                   NIU                                                                   NR
23    BOM number from main article       NIU                                                                   NR
24    Price printing code                NIU                                                                   NR
25    Modification code                  0 - not changed                   1 if
                                         1 changed                         aufstrukt.zusatz!=0                 NR

26    Price relevance identifier         NIU                                                                   AWE
                                                                                                 2.02.022
                                                                                                               6
27    Vector for production BOM 2        NIU

 A+W Software GmbH                             EN-A+W EDI Import.docx                                       150 / 162
                                                                            AWE database

No.    Designation                         A+W Enterprise note                                     IV           PS


28     Price type                          NIU
29     Supplier of part                                                     Aufstrukt.linr
30     Confirmed delivery date             NIU
31     Link ext. P.O./Order GUID (OMS)     NIU
27     Filler



 5.14 Shape record M1 (shape)
                                                                            AWE database

 No.     Designation                         A+W Enterprise note                                   IV         PS


 1       Record type                         M1                                                    2.2.000
 2       Shape number/ 999=steps                                            kpos.modnr             2.2.000
 3       SN name                             Shape designation              Kposparam.param99      2.2.000
 4       Parameter 1 (mm)                                                   kmodparam.param1       2.2.000
 5       Parameter 2 (mm)                                                   kmodparam.param2       2.2.000
 6       Parameter 3 (mm)                                                   kmodparam.param3       2.2.000
 7       Parameter 4 (mm)                                                   kmodparam.param4       2.2.000
 8       Parameter 5 (mm)                                                   kmodparam.param5       2.2.000
 9       Parameter 6 (mm)                                                   kmodparam.param6       2.2.000
 10      Parameter 7 (mm)                                                   kmodparam.param7       2.2.000
 11      Parameter 8 (mm)                                                   kmodparam.param8       2.2.000
 12      Reference lite for steps            NIU                                                   2.2019
 13      Rotation                            NIU
 13      Filler



 5.15 Shape record M1 (step)
 Each M1 record for steps assumes an S1 record. If an S1 record and an M1 record are written for stepped glass,
 then for each stepped glass an individual S1 and M1 are written, even if all the glass is stepped identically.



                                                                            AWE database

 No.     Designation                         A+W Enterprise note                                   IV         PS


 1       Record type                         M1                                                    2.2.000



 A+W Software GmbH                               EN-A+W EDI Import.docx                                      151 / 162
                                                                                 AWE database

No.       Designation                          A+W Enterprise note                                   IV         PS


2         Shape number/ 999=steps              999                                                   2.2.000
3         SN name                                                                                    2.2.000
4         Parameter 1 (mm)                     Bottom                            kstufparam.diff1    2.2.000
5         Parameter 2 (mm)                     Right                             kstufparam.diff4    2.2.000
6         Parameter 3 (mm)                     Top                               kstufparam.diff3    2.2.000
7         Parameter 4 (mm)                     left                              kstufparam.diff2    2.2.000
8         Parameter 5 (mm)                     NIU                                                   2.2.000
9         Parameter 6 (mm)                     NIU                                                   2.2.000
10        Parameter 7 (mm)                     NIU                                                   2.2.000
11        Parameter 8 (mm)                     NIU                                                   2.2.000
12        Reference lite for steps             Bit vector                                            2.2019
13        Rotation                             NIU
13        Filler



5.16 Muntin record C1


    No.    Description               AWE note                                       AWE Database          IV    PS


    1      Record type               C1
    2      Type                      NIU
    3      Calculation type          0 = drilling point sym.                        ksprosas.symkz
                                     (kspross.symkz=3)

                                     1 = field sym. (kspross.symkz=1) ,
                                     2 = drilling point asym.(kspross.symkz=4)

                                     3 = field asym. (kspross.symkz=2)

                                     4 = same bar length (NIU)
                                     5 = drilling point sym. glass edge (NIU)
                                     6 = drilling point asym. glass edge (NIU)
    4      Direction                 0 - horizontal                                 Ksprpar.swflag
                                     1 - vertical
    5      Parameter 1 (mm)          Dimensional precision                          Ksprpar.bohrp
    6      Parameter 2 (mm)
    7      Parameter 3 (mm)
    8      Parameter 4 (mm)
    9      Parameter 5 (mm)
    10     Parameter 6 (mm)


A+W Software GmbH                                EN-A+W EDI Import.docx                                        152 / 162
  No.       Description                   AWE note                               AWE Database        IV     PS


  11        Parameter 7 (mm)
  12        Parameter 8 (mm)
  13        Parameter 9 (mm)
  14        Parameter 10 (mm)
  15        Parameter 11 (mm)
  16        Parameter 12 (mm)
  17        Parameter 13 (mm)             NIU
  18        Parameter 14 (mm)             NIU
  19        Parameter 15 (mm)             NIU
  20        Parameter 16 (mm)             NIU
  21        Parameter 17 (mm)             NIU
  22        Parameter 18 (mm)             NIU
  23        Parameter 19 (mm)             NIU
  24        Parameter 20 (mm)             NIU
  25        Number of muntins                                                    kspross.anzahl1 /
                                                                                 anzahl2

  26        Muntin pads code              NIU
  27        Bit vector diagonal bars      NIU
  28        AWDesign filename             NIU
  29        Color code of muntin in
                                          NIU
            AWDesign file
  30        Muntin color name in
                                          NIU
            AWDesign file
  31        Dimension type of the
            drilling dimension
  32        Simulated Divided Lite
                                          NIU
            Bar Size
  33        Filler


For field symmetrical muntins, the parameters are 1 – 20 „000000“.


5.17 Muntin record CA
                                                                              AWE Database
       N
             Name                    ALCIB note                                                 IV    PS
       o.


       1     Record type             CA
       2     Direction               0=horizontal 1=vertical                  Ksprpar.swflag


A+W Software GmbH                                    EN-A+W EDI Import.docx                                153 / 162
                                                                                   AWE Database
     N
          Name                    ALCIB note                                                          IV   PS
     o.


     3    1. Muntin code
     4    2. Muntin code
     5    3. Muntin code
     6    4. Muntin code
     7    5. Muntin code
     8    6. Muntin code
     9    7. Muntin code
     1    8. Muntin code
     0
     1    9. Muntin code
     1
     1    10. Muntin code
     2
     1    11. Muntin code
     3
     1    12. Muntin code
     4
     1    13. Muntin code         NIU
     5
     1    14. Muntin code         NIU
     6
     1    15. Muntin code         NIU
     7
     1    16. Muntin code         NIU
     8
     1    17. Muntin code         NIU
     9
     2    18. Muntin code         NIU
     0
     2    19. Muntin code         NIU
     1
     2    20. Muntin code         NIU
                                                                                                           3.1
     2
     2    Filler
     3



5.18 Item text record (T1)
This record type is not always written. It is only written if the following texts exist for the PO:
        - Manual item texts
        - Manual article texts
        - Supplementary article texts (SP)


A+W Software GmbH                                  EN-A+W EDI Import.docx                                        154 / 162
        -       Project article texts (SP)
        -       Supplier article texts (SP)

The precise description of the stored procedure (SP) is in "EN-CONFIG-A+W Enterprise EDI.pdf".

                                                                                      AWE Database

No.    Name                                        ALCIB note                                           IV         PS


1      Record type                                 T1                                                   2.2.000
2      Text identifier                             Empty for manual item and
                                                   article texts
                                                   For the SP-controlled texts, the                     2.2.000
                                                   flag comes from the SP - return
                                                   parameter 3
3      Type ( 1=before item, 2=after item,         For SP – return parameter 1
                                                                                                        2.2.000
       3=product)
4      Text                                        For SP – return parameter 2                          2.2.000    3.1
5      Text number                                 NIU                                                  2.2.006    NR
6      Filler



5.19 Item record P9 (not implemented yet)

Writing this record type is not mandatory; it must be written after a P1 record. This record type is not supported in the
standard export.

                                                                      AWE Database

                                No.    Designation       AWE note                      IV   PS


                                1      Record type       NIU
                                2      Additional text   NIU
                                3      Filler            NIU

       Table: Item record supplement


    2) Individual additional text to be filled (only export)




A+W Software GmbH                                    EN-A+W EDI Import.docx                                       155 / 162
6 A+W Enterprise-specific function description
6.1     K1 mode
The mode is not evaluated by all receiving systems. Therefore, this is currently preset as follows
1 - new - no record in ottransferok or no export file exists
2 - change Record exists in ottransferok or export file
3 - cancel - kauf.still > 0 and record in ottransferok or export file exists
If no record exists in ottransferok, it is checked whether an export file exists. If an export file exists, the flag is set as if a
record were present in ottransferok.

When exporting to A+W Bussines (supplier setting ID 66) mode = 1 is always sent.


6.2     Export of processings (B1 record)
A+W standard processings (artikel.awtyp > 0) are exported.

6.2.1 B1 record for A+W standard processings
An A+W standard processing is marked with artikel.awtyp > 0.

Attention: This chapter is not yet complete. It is in processing with AWDesk #422752.

 Name                       Data mapping                                                      Description
 Seaming (1000)             Parameter 1 – 8: Converted edge from                              Edges see chapter notes
 Grinding (1005)            poszu.bearbvekt
 Polishing (1010)

 Mitering (1015)            Parameter 1 – 8: Converted edge from                              Edges see chapter notes
                            poszu.bearbvekt
                            Parameter 9: angle from poszu.dmess1
                            Parameter 10: converted level from poszu.ebene
 Faceting (1020)            Parameter 1 – 8: Converted edge from                              Edges see chapter notes
                            poszu.bearbvekt
                            Parameter 9: depth from poszu.dmess2
                            Parameter 10: angle from poszu.dmess1
                            Parameter 11: converted level from poszu.ebene
 Edge                       Parameter 1 – 8: Converted edge from                              Edges see chapter notes
 stripping(1025)            poszu.bearbvekt
                            Parameter 11: Depth from poszu.dmess1

 Other edge work            Parameter 1 – 8: Converted edge from                              Edges see chapter notes
 (1090)                     poszu.bearbvekt

 Drilling (1100)            Parameter 1: Position X from poszu.mass1
                            Parameter 2: Position Y from poszu.mass2
                            Parameter 3: Diameter from poszu.dmess1
                            Parameter 13: Dimensioning type
                            Parameter 14: Reference corner/edge 1
                            Parameter 15: Reference edge 2
                            Parameter 22: Relief cut from poszu.dmess2
                            Parameter 23: Edge quality
 Countersunk hole           Parameter 1: Position X from poszu.mass1
 (1110)                     Parameter 2: Position Y from poszu.mass2
                            Parameter 3: Diameter from poszu.dmess1


A+W Software GmbH                                      EN-A+W EDI Import.docx                                                   156 / 162
                       Parameter 6: top angle from poszu.dmess4
                       Parameter 7: bottom angle from poszu.dmess7
                       Parameter 11: Type (-> 0=diameter/1=depth)
                       Parameter 12: Dimensioning type
                       Parameter 13: Reference corner/edge 1
                       Parameter 14: Reference edge 2
                       Parameter 15: Relief cut from poszu.dmess2
                       Parameter 29: Edge quality

                       For type "Diameter":
                       Parameter 9: top diameter from poszu.dmess2
                       Parameter 10: bottom diameter from poszu.dmess5

                       For type "depth":
                       Parameter 4: top depth from poszu.dmess3
                       Parameter 5: bottom depth from poszu.dmess6

 Stepped drilling      Parameter 1: Position X from poszu.mass1
 (1120)                Parameter 2: Position Y from poszu.mass2
                       Parameter 3: Reference corner/edge 1
                       Parameter 4: Diameter from poszu.dmess2
                       Parameter 5: Diameter from poszu.dmess3
                       Parameter 6: Diameter from poszu.dmess4
                       Parameter 7: Diameter from poszu.dmess5
                       Parameter 8: Diameter from poszu.dmess6
                       Parameter 9: Diameter from poszu.dmess7
                       Parameter 10: Diameter from poszu.dmess8
                       Parameter 11: Diameter from poszu.dmess9
                       Parameter 12: Diameter from poszu.dmess10
                       Parameter 14: Dimension type
                       Parameter 15: Reference edge 2
                       Parameter 16: Relief cut from poszu.dmess1
                       Parameter 29: Edge quality
 Coating (1200)        Parameter 1: Dimensioning type                    Input type see notes
 Matting (1205)        Parameter 2: Angle from poszu.dmess7
 Sandblasting (1210)   Parameter 3: Reference edge (rotation) from
 Coloring (1215)       poszu.dmess6
 Enameling (1220)      Parameter 4: Inner reference corner from
 Screen printing       poszu.dmess5
 (1225)                Parameter 9: Width from poszu.dmess1
                       Parameter 10: Height from poszu.dmess2
                       Parameter 11: Position X from poszu.mass1
                       Parameter 12: Position Y from poszu.mass2
                       Parameter 13: Reference corner/edge 1
                       Parameter 14: Coating/screen number from
                       poszu.dmess3
                       Parameter 15: Saturation from poszu.dmess4
                       Parameter 16: Reference edge 2
                       Parameter 17: Mode from poszu.dmess8
                       Parameter 18: Mirror flag from poszu.dmess9
                       Parameter 30: Input type multi/single
 Decoating (1203)      Parameter 1: Dimension type                       Input type see notes
                       Parameter 2: Rotation angle from poszu.dmess5
                       Parameter 3: Reference edge (rotation) from
                       poszu.dmess4
                       Parameter 4: Inside reference corner from
                       poszu.dmess3
                       Parameter 9: Width from poszu.dmess1
                       Parameter 10: Height from poszu.dmess2

A+W Software GmbH                           EN-A+W EDI Import.docx                              157 / 162
                       Parameter 11: Position X from poszu.mass1
                       Parameter 12: Position Y from poszu.mass2
                       Parameter 13: Reference corner/edge 1
                       Parameter 16: Reference edge 2
                       Parameter 30: Input type multi/single
 Fluted bevel (1230)   Parameter 1 – 8: Converted edge from
                       poszu.bearbvekt
                       Parameter 9: Position Y from poszu.mass2
                       Parameter 10: Position X from poszu.mass1
                       Parameter 11 – 18: Width per edge from
                       poszu.dmess1
                       Parameter 19: Height from poszu.dmess2
                       Parameter 20: Grind ID from poszu.dmess3
                       Parameter 21: Reference edge 2
                       Parameter 22: Dimension type
                       Parameter 23: Reference edge (rotation) from
                       poszu.dmess5
                       Parameter 24: Inside reference edge from
                       poszu.dmess4
                       Parameter 25: Rotation angle from poszu.dmess6
 Alarm net (1245)      Parameter 1 – 8: Converted edge from
                       poszu.bearbvekt
 Stamp (1250)          Parameter 1: Position X from poszu.mass1         Parameter 6: Stamp type
                       Parameter 2: Position Y from poszu.mass2         (1-4), evaluated only in
                       Parameter 3: Reference corner/edge 1             AWB. Meaning still unclear.
                       Parameter 4: Stamp number from poszu.dmess1      Parameter 18: Mirroring is
                       Parameter 5: Reference edge 2                    not evaluated in AWB
                       Parameter 6: <EMPTY>
                       Parameter 7: Dimension type
                       Parameter 8: Width from poszu.dmess2
                       Parameter 9: Height from poszu.dmess3
                       Parameter 10: Inside reference corner from
                       poszu.dmess4
                       Parameter 11: Reference edge (rotation) from
                       poszu.dmess5
                       Parameter 12: Rotation angle from poszu.dmess6
                       Parameter 18: Mirror around center point from
                       poszu.dmess7
 Logo (1255)           Parameter 1: Position X from poszu.mass1         Parameter 6: Logo type (1-
                       Parameter 2: Position Y from poszu.mass2         4), evaluated only in AWB.
                       Parameter 3: Reference corner/edge 1             Meaning still unclear.
                       Parameter 4: Logo number from poszu.dmess1       Parameter 18: Mirroring is
                       Parameter 5: Reference edge 2                    not evaluated in AWB
                       Parameter 6: <EMPTY>
                       Parameter 7: Dimension type
                       Parameter 8: Width from poszu.dmess2
                       Parameter 9: Height from poszu.dmess3
                       Parameter 10: Inside reference corner from
                       poszu.dmess4
                       Parameter 11: Reference edge (rotation) from
                       poszu.dmess5
                       Parameter 12: Rotation angle from poszu.dmess6
                       Parameter 18: Mirror around center point from
                       poszu.dmess7
 Corner cut-out        Parameter 1 – 8: Converted edge from
 (1300)                poszu.bearbvekt
                       Parameter 9: Width from poszu.dmess2
                       Parameter 10: Height from poszu.dmess1
                       Parameter 12: Dimension type


A+W Software GmbH                           EN-A+W EDI Import.docx                                    158 / 162
                       Parameter 19: Orientation to reference edge 1
                       (height) from poszu.dmess3
                       Parameter 20: Orientation to reference edge 2
                       (width) from poszu.dmess4
                       Parameter 21: Outside radius from poszu.dmess6
                       Parameter 22: Inside radius from poszu.dmess5
                       Parameter 23: Edge quality
 Corner cut-off        Parameter 1 – 8: Converted edge from
 (1305)                poszu.bearbvekt
                       Parameter 9: Width from poszu.dmess1
                       Parameter 10: Height from poszu.dmess2
                       Parameter 11: Edge quality
                       Parameter 12: Dimension type
 Rounded corner        Parameter 1 – 8: Converted edge from
 (1310)                poszu.bearbvekt
                       Parameter 11: Radius from poszu.dmess1
                       Parameter 13: Edge quality
 Edge cut-out (1400)   Parameter 1 – 8: Converted edge from                 Input type see notes
                       poszu.bearbvekt
                       Parameter 9: Width from poszu.dmess1
                       Parameter 10: Height from poszu.dmess2
                       Parameter 19: Distance to corner from poszu.mass1
                       Parameter 20: Reference corner
                       Parameter 21: Outside radius from poszu.dmess4
                       Parameter 22: Inside radius from poszu.dmess3
                       Parameter 23: Edge quality
                       Parameter 30: Input type multi/single
 Arc-shaped edge       Parameter 1 – 8: Converted corners from              Input type see notes
 cut-out (1402)        poszu.bearbvekt
                       Parameter 9: Drilling radius from poszu.dmess1
                       Parameter 10: Chord length from poszu.mass2 (for
                       dimension to two edges)
                       Parameter 11: Distance to corner from poszu.mass1
                       (for dimension to two edges)
                       Parameter 12: Horizontal distance from poszu.mass1
                       (for absolute dimension)
                       Parameter 13: Vertical distance from poszu.mass2
                       (for absolute dimension)
                       Parameter 15: „0“ for absolute dimension, “1” for
                       dimension to two edges
                       Parameter 19: Reference corner
                       Parameter 21: Outside radius from poszu.dmess2
                       Parameter 22: Edge quality
                       Parameter 30: Input type multi/single
 Speaker's hole        Parameter 1: Position X from poszu.mass1             Input type see notes
 (1405)                Parameter 2: Position Y from poszu.mass2
                       Parameter 9: Width from poszu.dmess1
                       Parameter 10: Height from poszu.dmess2
                       Parameter 11: Reference corner/edge 1
                       Parameter 12: Reference edge 2
                       Parameter 14: Dimension type
                       Parameter 15: Rotation angle from poszu.dmess5
                       Parameter 16: Reference edge (rotation) from
                       poszu.dmess4
                       Parameter 17: Inside reference corner from
                       poszu.dmess3
                       Parameter 18: Edge quality
                       Parameter 30: Input type multi/single
 Handle (1410)         Parameter 1 – 8: Converted edge from                 Input type see notes


A+W Software GmbH                           EN-A+W EDI Import.docx                                 159 / 162
                    poszu.bearbvekt
                    Parameter 9: Width from poszu.dmess1
                    Parameter 10: Height from poszu.dmess2
                    Parameter 11 – 18: Width per edge from
                    poszu.dmess1
                    Parameter 19: Reference corner/edge 1
                    Parameter 20: Position X from poszu.mass1
                    Parameter 21: Position Y from poszu.mass2
                    Parameter 22: Dimension type
                    Parameter 23: Rotation angle from poszu.dmess5
                    Parameter 24: Reference edge (rotation) from
                    poszu.dmess4
                    Parameter 25: Inside reference corner from
                    poszu.dmess3
                    Parameter 30: Input type multi/single
 Internal cut-out   Parameter 1: Position X from poszu.mass1            Input type see notes
 (1415)             Parameter 2: Position Y from poszu.mass2
                    Parameter 9: Width from poszu.dmess1
                    Parameter 10: Height from poszu.dmess2
                    Parameter 11: Reference corner/edge 1
                    Parameter 12: Reference edge 2
                    Parameter 13: Inside radius from poszu.dmess6
                    Parameter 14: Dimension type
                    Parameter 15: Rotation angle from poszu.dmess5
                    Parameter 16: Reference edge (rotation) from
                    poszu.dmess4
                    Parameter 17: Inside reference corner from
                    poszu.dmess3
                    Parameter 18: Edge quality
                    Parameter 30: Input type multi/single
 Macro (1900)       Parameter 1 – 8: Converted edge from                Input type see notes
                    poszu.bearbvekt
                    Parameter 11: Distance to corner from poszu.mass1   Orientation left/right see
                    Parameter 12: Orientation left/right                notes
                    Parameter 30: Input type multi/single
 Surface macro      Parameter 1: Position X from poszu.mass1            Input type see notes
 (1910)             Parameter 2: Position Y from poszu.mass2
                    Parameter 11: Reference corner/edge 1
                    Parameter 12: Reference edge 2
                    Parameter 14: Dimension type
                    Parameter 15: Rotation angle from poszu.dmess2
                    Parameter 16: Reference edge (rotation) from
                    poszu.dmess1
                    Parameter 30: Input type multi/single
 Parametric macro   Parameter 1 – 8: Converted edge from                Input type see notes
                    poszu.bearbvekt
                    Parameter 11: Distance to corner from poszu.mass1   Orientation left/right see
                    Parameter 12: Orientation left/right                notes
                    Parameter 13: Number of parameters
                    Parameter 14: Bit vector for inch conversion,       Parametric macros/surface
                    currently always <EMPTY>                            macros are only exported if
                    Parameter 15: Parameter from poszu.dmess1           the export is not done in
                    Parameter 16: Parameter from poszu.dmess2           "inches". See chapter
                    Parameter 17: Parameter from poszu.dmess3           notes.
                    Parameter 18: Parameter from poszu.dmess4
                    Parameter 19: Parameter from poszu.dmess5
                    Parameter 20: Parameter from poszu.dmess6
                    Parameter 21: Parameter from poszu.dmess7
                    Parameter 22: Parameter from poszu.dmess8
                    Parameter 30: Input type multi/single

A+W Software GmbH                        EN-A+W EDI Import.docx                                       160 / 162
 Parametric surface     Parameter 1: Position X from poszu.mass1                Input type see notes
 macro (1930)           Parameter 2: Position Y from poszu.mass2
                        Parameter 11: Reference corner/edge 1                   Parametric macros/surface
                        Parameter 12: Reference edge 2                          macros are only exported if
                        Parameter 14: Dimension type                            the export is not done in
                        Parameter 15: Rotation angle from poszu.dmess2          "inches". See chapter
                        Parameter 16: Reference edge (rotation) from            notes.
                        poszu.dmess1
                        Parameter 17: Number of parameters
                        Parameter 18: Bit vector for inch conversion,
                        currently always <EMPTY>
                        Parameter 19: Parameter from poszu.dmess4
                        Parameter 20: Parameter from poszu.dmess5
                        Parameter 21: Parameter from poszu.dmess6
                        Parameter 22: Parameter from poszu.dmess7
                        Parameter 23: Parameter from poszu.dmess8
                        Parameter 24: Parameter from poszu.dmess9
                        Parameter 25: Parameter from poszu.dmess10
                        Parameter 30: Input type multi/single
 Edge silk screening    Parameter 1 – 8: Converted edge from
 (1970)                 poszu.bearbvekt
                        Parameter 11: Depth from poszu.dmess1
                        Parameter 14: Silk/type from poszu.dmess2
                        Parameter 15: Saturation from poszu.dmess3

6.2.1.1 Notes

6.2.1.1.1 Dimension Type
The dimensioning type of the interface is determined from poszu.mtyp.


6.2.1.1.2 Reference corner/edge
The reference corners/edges are determined depending on the dimensioning type from poszu.bearbvek and
poszu.ecknr.

6.2.1.1.3 Edges
Processed edges are marked with a "1" in the parameter; non-processed edges with a "0".

6.2.1.1.4 Input type multi/single
1=multi, 2=single
For export currently always 2=single.

6.2.1.1.5 Macro – Orientation/alignment left/right
The orientation/alignment defines whether the macro is dimensioned up to the right (0) or left (1) corner. The edges
are counted counter-clockwise.
The examination left/right is always done as if the glass is standing on the reference edge (e.g. edge 1 right means
corner 2; edge 1 left means corner 1; edge 4 right means corner 1).

6.2.1.1.6 Parametric macros/surface macros
Parametric macros/surface macros are only exported if the export is not done in "inches". In AWE, currently the
information whether or not a parameter is to be converted is not included. That's why the export can only be done
unconverted. As a result, the bit vector that normally marks the conversion of the parameters is empty and not
meaningful. The scheduling system may therefore not undertake any conversion.




A+W Software GmbH                              EN-A+W EDI Import.docx                                         161 / 162
6.2.2    (No!) B1 record for A+W Enterprise processings (without A+W-processing type)
An A+W Enterprise processing is marked with artikel.teilflag = 0 & artikel.awtyp = 0 & artikel.atyp > 0.

The export of A+W Enterprise processings is (with AWDesk #422752) not implemented and the implementation is
not currently intended. It is urgently recommended that you set up the system used with A+W standard processings.




A+W Software GmbH                               EN-A+W EDI Import.docx                                     162 / 162

