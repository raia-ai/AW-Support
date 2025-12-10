---
description: "EN CONFIG A+W Enterprise Print Service"
---



# EN CONFIG A+W Enterprise Print Service

      Configuration Instructions


A+W Enterprise Print Service




                                      english




                              - -INTERNAL-
Change history


Date          Author                  Comments                                   Version
2018-04-26 MP                         Document created                           1.0
2019-04-26 MP                         Organization                               1.1
20.02.17      ALW                     2.2. Form parameter – Field                1.2
                                      Archiving of lists + logic change of the
21.06.21      ALW                                                                1.3
                                      archiving
21.09.02      ALW                     Point 7 started                            1.4
22.09.08      ALW                     Troubleshooting                            1.5
23.11.13      JMI                     Troubleshooting entry made                 n/a
24.05.14      ALW                     Crystal Report Engine                      1.6
                                      Chapter Invoice, credit note, and
24.07.10      ALW                                                                1.7
                                      printing collective invoices




Contents

1.   General Information                                                                    6
     1.1. Installation                                                                      6
          1.1.1. Installation instructions                                                  6
     1.2. Documents                                                                         6
     1.3. Version update                                                                    6
          1.3.1. 2024/02 - Quality Release March 2024                                       6
2.   Report management                                                                      7
     2.1. Forms vs. lists                                                                   7
     2.2. Form parameters                                                                   8
     2.3. Form types                                                                        9
          2.3.1. Form types (forms)                                                         9
          2.3.2. Form types (lists)                                                        11
     2.4. Text generation                                                                  12
          2.4.1. reptzui                                                                   12
          2.4.2. repmix                                                                    12
     2.5. Other fields                                                                     12
          2.5.1. REPID                                                                     12
          2.5.2. Form group                                                                13
          2.5.3. Keys                                                                      13
          2.5.4. Subart                                                                    13
          2.5.5. Subnrflag                                                                 13
          2.5.6. Archives                                                                  13
3.   Printer                                                                               14
     3.1. Printer setup                                                                    14
          3.1.1. Escape sequence                                                                14
          3.1.2. Output (drucker.faxflag)                                                       14
          3.1.3. Page length (drucker.pagelen)                                                  14
          3.1.4. Use of the page format for the PDF export (#413469)                            16
     3.2. PDF export                                                                            16
     3.3. General file export (#416295)                                                         16
          3.3.1. Description                                                                    16
          3.3.2. Possible file export formats                                                   17
     3.4. Empty printer (#404613)                                                               17
     3.5. PDF via e-mail to the current employee (#292850, #394372)                             18
     3.6. External PDF printer (#413469)                                                        18
          3.6.1. Configuration of the PDF printer                                               19
          3.6.2. Configuration of the Print Service                                             19
          3.6.3. Requirements for the external PDF tool                                         19
          3.6.4. Description of the flow                                                        20
          3.6.5. Internal working directory                                                     20
          3.6.6. Example of an external PDF tool: Foxit reader                                  21
4.   Form printing or e-mail                                                                    23
     4.1. Printed or sent documents                                                             24
     4.2. reptmp/ repform                                                                       24
     4.3. Additional forms ([AW-73668])                                                         24
     4.4. E-mail dispatch                                                                       25
          4.4.1. Determination of the e-mail addresses                                          25
          4.4.2. Determining the sender's address                                               26
          4.4.2.1. Use of a stored procedure for e-mail determination                           26
          4.4.3. Mail server configuration                                                      27
          4.4.3.1. Mail server for error notification                                           27
          4.4.3.2. Mail server for the mail dispatch                                            27
          4.4.4. SMTP port (#425282)                                                            27
          4.4.5. Display of a clear name (#415664)                                              28
          4.4.6. Merge of file attachments (#293039)                                            28
          4.4.7. Additional e-mail to the e-mail sender [AW-74765]                              29
          4.4.8. Naming of file attachment                                                      29
     4.5. PDF copy as transaction document                                                      30
5.   Print list                                                                                 31
6.   (Preliminary) delivery note printing in dispatch control                                   32
     6.1. Print additional forms if (advance) delivery note printing is triggered in dispatch
     (#327461)                                                                                  32
     6.2. Acceptance test certificate for delivery note generation (#440096)                    32
     6.3. Dividing up advance and/or delivery notes for a route into several print jobs
     ([AW-151256])                                                                              34
7.   Invoice, credit note, and printing collective invoices                                     35
     7.1. eInvoicing (XRechnung, ZUGFeRD)                                                       35
          7.1.1. Process                                                                        35
          7.1.2. Master data                                                                    37
          7.1.3. Archiving                                                                      39
          7.1.3.1. E-invoice                                                                    39
          7.1.3.2. ZUGFeRD archiving                                                            40


A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                             3
          7.1.4. Documentation generation of e-invoice                         40
8.   Document attachments                                                      41
     8.1. Send LE documents (#274142/#274577)                                  41
     8.2. Send file attachments (#250359)                                      41
     8.3. Embedding additional files in PDF                                    44
          8.3.1. Creating a dossier list                                       44
9.   Printing sketches                                                         46
     9.1. SNLive & AWBom sketches (#185271)                                    46
     9.2. AWDesign sketches (#118996)                                          46
          9.2.1. Muntin pattern for insulated glass with AWD file              47
     9.3. Sketch attachment for REPGO printing (#211903)                       47
     9.4. Printing of schematic diagrams on Crystal Report forms (#257788)     49
10. Archiving                                                                  50
    10.1. Archiving adjustment ([AW-77175])                                    50
    10.2. Archiving of lists [AW-77175]                                        51
    10.3. Archiving with the Print Service (#234872)                           52
    10.4. ARCHIV_FORMULARE                                                     53
    10.5. Watermarks in archiving #374635                                      55
11. Print Service – general                                                    56
    11.1. Print status check                                                   56
    11.2. Status flags                                                         56
          11.2.1. Status 0 – 99: progress status                               56
          11.2.2. Status 100 – 149: general error or incorrect configuration   57
          11.2.3. Status 150 – 199: incorrect printtransfer data               59
          11.2.4. Status 200 – 249: incorrect printparam data                  60
          11.2.5. Status 250 – 299: Crystal Reports error                      61
          11.2.6. Status 300 – 349: incorrect mailparam data                   62
          11.2.7. Status 350 – 399: incorrect printfiles data                  63
          11.2.8. Status 400 – 449: error in the archive process               65
    11.3. Configuration instructions                                           65
          11.3.1. Temporary status list                                        65
    11.4. Logs / Tracing                                                       65
12. Print Service – Maintenance --ToDo--                                       66
    12.1. Motivation and goals of this development                             66
    12.2. Special terms                                                        66
    12.3. Limitations, delimitation, validity                                  66
    12.4. Installation/configuration, environment variables                    66
    12.5. Functional description                                               66
          12.5.1. Master Data                                                  66
13. Troubleshooting                                                            67
    13.1. Exception: net_io_connectionclosed                                   67
    13.2. Resetting print job                                                  68
    13.3. Print job is not processed by the print service                      68
    13.4. Printer not found after printer driver updating                      69
14. Report content                                                             71
    14.1. AWP SubReports (#334410)                                             71


A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx            4
     14.2. Crystal Report Stored Procedures                                    71
     14.3. Problems with ReportDocument content                                72
     14.4. Sketch display suppression (e.g. A+W Design)                        72
15. Crystal Report Engine                                                      74
    15.1. Discontinuation of CR engine 2008                                    74
    15.2. Logging/ Tracing                                                     74
    15.3. Troubleshooting                                                      75
          15.3.1. Slow processing of the print service/Crystal Report engine   75
          15.3.2. Error in the Crystal Report engine during PDF creation       76
          15.3.3. General Crystal Engine error (error code 250)                77




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx            5
1. General Information
The A+W Enterprise Print Service was conceived and developed for NSG with case #145096 in
Version 2008.2. Since then, the Print Service has been enhanced continuously. The specification
was that all print functions that were possible with the REPGO environment should also be
possible with Crystal Reports.


1.1. Installation
        1.1.1.           Installation instructions
ALCIB 2011 Print Service: D-ALCIB_2011_Print_Service_Installationsanleitung.docx
A+W Enterprise 5 Print Service: EN-INST-A+W Enterprise Print Service.pdf
A+W Enterprise 6 Print Service: EN-INST-A+W Enterprise Print Service.pdf


1.2. Documents
Over time, a whole series of documents have been created. For information that didn't make it
into this document, please note the following links.
Documentation: Original PrintService specification
FAQs: Print Service FAQs
References: Print Service - References


1.3. Version update
Critical update for version closing via quality release


        1.3.1.           2024/02 - Quality Release March 2024
In Quality Release 2024/03 the Crystal Report Engine up to Version 13.0.35 was made usable.
With this expansion, the outdated Crystal Report Engine 2008 no longer supported by SAP is
terminated. The Print Service now draws the Crystal Report Engine automatically and thus needs
no setting via the Config Tool.
With a version update, attention must be paid that the customer is not working with the old
Crystal Report Engine 2008. Before the update, for customers who are using the old engine, a
newer engine must be installed and tested properly.
Please note that the old engine A+W Report Runtime is uninstalled!




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                         6
2. Report management




2.1. Forms vs. lists
Within A+W Enterprise, there is a distinction between forms and lists. Here are a few reference
points for distinguishing when a form and when a list is meant.
 Form                                             List
 Fixed number of parameters                       Variable number of parameters
 Reference to kauf document                       Reference to any DB tables
 Usually for external use                         Usually for internal use
 Can be accessed in                               Can be accessed via
     -   form printing (SA/PU)                           -   Print list
     -   Email dispatch (SA/PU)                          -   Special menu elements in alcib,
                                                             lapool, lager, etc.
     -   (Preliminary) delivery notes in
         dispatch



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                          7
          -    Direct printing in the order entry
    Several report calls are possible within a print       Always just precisely one report call per print
    job                                                    job




2.2. Form parameters
The number of parameters of forms is fixed (=6) and cannot be changed since this would have
wide-ranging adjustments in the whole Enterprise system as a consequence.
General comm. forms
              Parameter                       Field                             ALCIB type     Crystal type
     1.       Document number                 kauf.auftrnr                      numl           Number
     2.       Document type                   kauf.vorgang                      numl           Number
     3.       Sub number                      kauf.subnr                        nums           Number
     4.       Process number2                 rep.formart+                      numl           Number
                                              printtransfer.pid
     5.       Output type                     printtransfer.outputflag          nums           Number
     6.       Form type3                      rep.formart3                      nums           Number


Preliminary delivery note (dispatch)
              Parameter                       Field                             ALCIB type     Crystal type
     1.       Order number                    lapool.auftrnr                    numl           Number
     2.       Delivery date                   lapool.ltplan                     Date1          Date
     3.       Route number                    lapool.routenr                    nums           Number
     4.       Process number2                 rep.formart+                      numl           Number
                                              printtransfer.pid
     5.       Output type                     printtransfer.outputflag          nums           Number
     6.       Form type3                      rep.formart3                      nums           Number


1
 With #439427 it was determined that the parameter type has converted itself from date to
datetime. The PS6 was adjusted so that both parameters of type date as well as datetime can be
processed.
2
    Process number is composed of <rep.formart>< printtransfer.pid >
3
    Here the basic form type is written:
    Form type                                              Basic form type
    12, 128, 146, 147, 912                                 12 (collective invoice)
    23, 28, 38, 133, 177, 923, 928                         23 (preliminary delivery note)


A+W Software GmbH                  EN-CONFIG-A+W Enterprise Print Service.docx                               8
 27, 31, 132, 142, 927                                  27 (work order)
 86                                                     86 (advance delivery note purchase order)
 Rest                                                   If a document type is present, the document
                                                        type is written. If there is no document type
                                                        present, the form type is written.



2.3. Form types
Form types are managed and assigned in development. Via the program pr_repverw, entries can
be searched for in the table by the same name and completed.
      -   The range from 700 to 850 is reserved for customer-specific reports.
      -   The range from 900 to 998(!) is reserved for temporary forms.
              o       Example: 905 for a temporary OC, 904 for a temporary quotation, etc.
              o       Temporary means for a time and NOT forever!
      -   The form type 999 is reserved as anchor for the printer/form assignment.
The following form types are already assigned and can be used accordingly if they are not yet
used for other purposes.


          2.3.1.             Form types (forms)

 Form             Document         Name                            Special features
 type
 1                1                Inquiry
 2                2                Purchase order
 4                4                Quotation
 5                5                OC
 6                6                Delivery note                   rep.subnrflag = 2 (deliver)
 7                7                Individual invoice
 9                9                Credit note
 12               7                Collective invoice              rep.subnrflag = 1 (Coli)
 16               7                Cash invoice                    Use in sales counter printing
 18               4                Check quotation
 20               5                Check OC 2
 21               5                Check OC
 22               5                Pro forma invoice
 23               5                Preliminary delivery note SA



A+W Software GmbH                 EN-CONFIG-A+W Enterprise Print Service.docx                           9
27        5         Work order
28        5         Preliminary delivery note       Access in dispatch.
                    dispatch
                                                    Text generation for form type = 23
29        5         Correction form N
30        5         Correction form 2
31        5         Work Sheet                      Work order
35        6         DN including prices             rep.subnrflag = 2 (deliver)
36        2         Purchase order without
                    prices
37        4         Check quotation 2
38        5         PDN (special)
39        5         OC as purchase order
86        2         Preliminary delivery note       #227069
                    dispatch for receipt of goods
89        2         Purchase order copy
126       6         Fax delivery note               rep.subnrflag = 2 (deliver)
127       7         Fax invoice
128       7         Fax collective invoice          rep.subnrflag = 1 (Coli)
129       9         Fax credit note
130       9         Credit note 2
131       1         Inquiry 2
132       5         Work order (job)
133       5         Boxes - PDNlap
134       6         Boxes delivery note             rep.subnrflag = 2 (deliver)
138       5         Cancel OC
139       2         Cancel purchase order
140       4         Cancel quotation
141       5         Boxes OC
142       5         Boxes work order
143       7         Boxes invoice
144       9         Boxes credit note
145       7         Boxes invoice 2
146       7         Collective invoice copy         rep.subnrflag = 1 (Coli)
147       7         Total account
149       5         Pro forma invoice 2



A+W Software GmbH   EN-CONFIG-A+W Enterprise Print Service.docx                      10
150        5                  Pro forma invoice 3
177        5                  Counterfoil                      PDN (Lapool)
180-189    As required        CR sketches forms



       2.3.2.          Form types (lists)
Form       Name                              Special features
type
44         Orders not invoiced
83         Loading list PU                   #227069
114        Loading list
115        Supplementary loading list
154        ykowgpos                          Statistics list
155        yag                               Statistics list
156        yuwg                              Statistics list
157        yowg                              Statistics list
158        yb                                Statistics list
159        yvb                               Statistics list
160        yvuwg                             Statistics list
161        yvowg                             Statistics list
162        ykvowg                            Statistics list
163        ykund                             Statistics list
164        ykuwg                             Statistics list
165        ykowg                             Statistics list
166        kuwgums                           Statistics list
167        kowgums                           Statistics list
168        yauwg                             Statistics list
169        provab                            Statistics list
195        LEOutput                          Declaration of performance
214        Product stock label
220        Component
230        Invoiced construction site
250        Receipt of racks                  Rack list
251        Rack out                          Rack list
252        Rack list                         Rack list



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx      11
 253          Rack Customer                     Rack list
 255          Rack Company                      Rack list
 256          Rack master                       Rack list
 257          Rack comparison                   Rack list
 259          Rack reminder                     Rack list
 361          StackLab




2.4. Text generation
The text generation, that is, the document-precise preparation of the document and master data
texts for a report call, is done with two different functions. In the REPGO environment, these
functions are offered as stand-alone programs: repmix and reptzui.
Here, documents and master data texts are collected whose form vector fit the current form.
These include, among others,
    -   Header and footer texts
    -   Article and item texts
    -   Current texts
    -   Group texts
Product group texts
For additional documentation about text generation and reptzui/repmix, see:
\\jupiter\Doku_DocuWare\ALCIB-PMS\DRUCK\Installation_Configuration


        2.4.1.           reptzui
This function collects the texts for all quotations, OCs, individual invoices, credits, and
(preliminary) delivery notes. The texts are available in the table reptexte.


        2.4.2.           repmix
This function collects the texts for all POs, inquiries, and collective invoices. The texts are available
in the table reptxt.
TODO: relationship of printparam.pid <-> reptexte.pidno


2.5. Other fields
        2.5.1.           REPID
In the Repid field, for which there is no DB field, the customer is coded. The value is composed of
the UserID and "00". The value 9900 stands for all customers and is used for Std.Reports.



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                             12
The value comes from the environment variables REPID.


        2.5.2.          Form group
The form group generally has the value 1. If there is precisely one set of reports for the forms, this
is completely sufficient.
If there is more than one form set, additional values can be stored via Master Data > Division in
the form group field. Thanks to the assignment of a division in the employee master data, this
form group is assigned an employee, who from now on will only see forms of this group.


        2.5.3.          Keys
The Keys field is composed of the values REPID, form group, form type, and a sequential number
in order to generate a unique key for the table repparam. The REPID is only found in the field
rep.schuessel[1,4] and it is used in four places in the program and in environment files.


        2.5.4.          Subart
In form printing, it is possible to select several forms (up to 7) with the same document type
(rep.vorgang) together. The subart can be defined as another criterion. Only such forms with the
same subart can be printed together.


        2.5.5.          Subnrflag
Using the setting in the rep.subnrflag field, it is defined how subnumbers of a document are
handled. The settings are 0 – none, 1 – collective invoice, 2 – delivery note.
With the value 2 (= delivery note), the Subnummer field is released in form printing and e-mail
dispatch.
For the value 1 (=collective invoice), the Subnummer field is assigned the value 1 and it cannot be
changed.


        2.5.6.          Archives
With this check box, the archiving for lists or forms is activated by Crystal Report reports. This
logic was introduced with ticket [AW-77175].




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            13
3. Printer
3.1. Printer setup
The set-up of the printers available in A+W Enterprise is done under System > Print management
> Printer.




          3.1.1.         Escape sequence
ALWAYS set the ESQ sequence to "noesc". This demonstrates at some points that this is a printer
that is suitable for the Print Service.


          3.1.2.         Output (drucker.faxflag)
 Type          Meaning                                                                  Outputflag
 Printer       This is a physical printer                                               1
 Fax           Irrelevant in the CR environment Not supported                           -
 File          PDF or file export                                                       4
 Office        Irrelevant in the CR environment                                         -
 E-mail        PDF export with e-mail dispatch                                          2
 PDFPrn        Physical printer that is called from a PDF printer tool.                 6



          3.1.3.         Page length (drucker.pagelen)
In connection with Crystal Reports, this field is interpreted as page format, e.g. A4, letter.
Generally the value 0 = default size should be used.
 PageSize ID              Format
 0                        Default
 1                        Letter
 2                        LetterSmall
 3                        Tabloid



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            14
4                   Ledger
5                   Legal
6                   Statement
7                   Executive
8                   A3
9                   A4
10                  A4Small
11                  A5
12                  B4
13                  B5
14                  Folio
15                  Quarto
16                  10x14
17                  11x17
18                  Note
19                  Envelope9
20                  Envelope10
21                  Envelope11
22                  Envelope12
23                  Envelope14
24                  Csheet
25                  Dsheet
26                  Esheet
27                  EnvelopeDL
28                  EnvelopeC5
29                  EnvelopeC3
30                  EnvelopeC4
31                  EnvelopeC6
32                  EnvelopeC65
33                  EnvelopeB4
34                  EnvelopeB5
35                  EnvelopeB6
36                  EnvelopeItaly
37                  EnvelopeMonarch
38                  EnvelopePersonal
39                  FanfoldUS



A+W Software GmbH        EN-CONFIG-A+W Enterprise Print Service.docx   15
 40                      FanfoldStdGerman
 41                      FanfoldLegalGerman
 256                     User Defined



        3.1.4.    Use of the page format for the PDF export
            (#413469)
On the Setup printer dialog, a different page format can be stored in the SL (=page length) field.
The value 0 means that the page format of the CR report is used. Previously, this field was only
evaluated for output on a physical printer. In the course of this case, this value is now also
considered for the PDF export.


3.2. PDF export
For a printer that generates a PDF date as output, you use "crpdfexport".
Example:




3.3. General file export (#416295)
        3.3.1.          Description
Via the printer configuration on the System > Print management > Printer dialog, individual printers
can be created for the desired file formats. In the Pfad field, "crexportprinter #ID" is specified for
this. #ID stands for a value from the table below, e.g. the value 3 for the Word export. The output
type is "File".

Example: Word export




For the output of a report via the A+W Enterprise 6 Print Service, the same configurations are used
for the output path and the file name as for the PDF export. The exception is the file extension; this
is selected appropriate to the output type.

If a form for which a document archiving is configured is output via file export, an archive copy is
created in the archive directory in the same format.

For some of the file formats, the reports must be adjusted under some circumstances in order to
generate sensible outputs. We can make no guarantee that existing reports are suitable for every
file format.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                             16
        3.3.2.           Possible file export formats
The possible values for #ID are:
 Value Enum                                 Suffix     CR              Comment
                                                       Runtime
 1         CrystalReport                    .rpt       CR 2008
 2         RichText                         .rtf       CR 2008
 3         WordForWindows                   .doc       CR 2008         Microsoft Word (97-2003)
 4         Excel                            .xls       CR 2008         Microsoft Excel (97-2003)
 5         PortableDocFormat                .pdf       CR 2008
 6         HTML32                           .htm       CR 2008
 7         HTML40                           .htm       CR 2008
 8         ExcelRecord                      .xls       CR 2008         Microsoft Excel (97-2003),
                                                                       data only
 9         Text                             .txt       CR 2008
 10        CharacterSeparatedValues         .csv       CR 2008
 11        TabSeperatedText                 .ttx       CR 2008
 12        EditableRTF                      .rtf       CR 2008
 13        Xml                              .xml       CR 2013
 14        RPTR                             .rpt       CR 2013         Like 1 – Crystal Report, but
                                                                       readonly
 15        ExcelWorkbook                    .xlsx      CR 2013         Microsoft Excel (2007), only
                                                                       data, but in xlsx format




3.4. Empty printer (#404613)
In A+W Enterprise, there has always been a file printer, dateidruck2, with which you can start a
printout for test purposes. The output for this is in a general file. Here, all print flags and log entries
are made in the database, as if you had printed out the file in question normally. This functionality
is only available in case the output is done via REPGO report. No test output via Crystal Reports is
provided; there is the PDF file printing for this.
For the delivery note generation in dispatch control, under some circumstances it may not be
desired that physical papers are printed since preliminary delivery notes can be taken to the
customer's. In this case, it absolutely makes sense to have a functionality to suppress the printing.
With this case, a printer configuration has been defined with which you can simulate an output
without creating a physical output or placing demands on the system (background processes,
Windows services). This printer functions both in the REPGO environment as well as in a
configuration with Crystal Reports.



A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                              17
For distinction: all actions, from scripts or stored procedures that take place AFTER the print job
generation (repspool/printtransfer) will no longer be executed with this special printer. All actions
that occur before this, e.g. entries to druckhist, will be executed. The print job itself - entry still
repspool - does not take place! Thus, this setting can NOT be used for internal transfer of purchase
orders.
In order to set up this printer, a printer must be set up on the System > Print management > Printer
dialog, with the specification "nooutputprinter" in the Pfad field.
Example:




3.5. PDF via e-mail to the current employee (#292850,
   #394372)
In A+W Enterprise, a special printer can be set up, which in connection with the A+W Enterprise
Print Service, generates outputs as PDF file and sends these to the employee who initiated the
output via e-mail. This logistics is available for all outputs for which a printer selection is necessary.
That is, in the form and list printing and for the (advance) delivery note printing in dispatch control.
Since #394372 also in direct printing from the order entry.
The set-up of the printer is handled in A+W Enterprise under System > Print management > Printer.
You select the appropriate printer during the printer query if a list or a form is printed. Then the
output is created as PDF file and sent as e-mail to the e-mail address of the respective employee
(MITARB.EMAIL) who initiated the printing. If no e-mail address is stored for the employee, it is not
possible to generate output with this printer.
Example:




3.6. External PDF printer (#413469)
The A+W Enterprise Print Service is conceived so that for each document an individual report call is
made, regardless of the type in which the output happens. When printing several documents, it can
therefore happen that output from other print jobs that are specified on the same printer can slide
in between.
The structure of the Print Service, the associated reports and the stored procedures cannot be
changed without risk; it also offers technical advantages that we cannot forego. We have therefore
decided on a customizing solution that can be set up as needed and that solves the problem
described above. The solution provides that the output is no longer done directly on the selected
printer, but instead, individual PDF files are created for each document. These are combined into an
individual PDF, which in turn is sent by an external PDF program to the selected printer.
The setup and functioning of such a PDF printer in A+W enterprise will be described below.




A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                             18
        3.6.1.           Configuration of the PDF printer
In A+W Enterprise under System > Print management > Printer, printers that should work as
described above should be configured for output = PDFPrn. With use of such a printer, the correct
output type (=6) is written to the field PRINTTRANSFER.OUTPUTFLAG.

Example:




If the output should be done in the duplex process, the option -DUPLEX must be specified in the Pfad
field next to the printer designation - separated by a space. This option causes an empty page to be
inserted for PDF files with an odd number of pages.


        3.6.2.           Configuration of the Print Service
In the Config Tool of the A+W Enterprise Print Service, an external PDF program or a Windows script
must be configured that should take over the output of the combined PDF file. Two fields are offered
on the External Tools page. In the first, the file name of the program or the Windows script is entered.
The call parameters of the program or script are configured in the second field. The placeholders
%PRINTER% and %PDFFILE% can be used here. These are replaced with concrete values when the
program is called.




 Placeholder           Description
 %PRINTER%             receives the release name of the printer from the field
                       PRINTTRANSFER.OUTPUTPATH, less any options.
 %PDFFILE%             receives the fully qualified file name of the combined PDF file.

It is expected that there is an entry in both Config fields, otherwise there will be an error during the
processing of such print jobs.


        3.6.3.           Requirements for the external PDF tool
The PDF program or Windows script that should be used for the further processing of the combined
PDF files must satisfy a few requirements since the call is made from a Windows service that is
running only in the background. If these requirements cannot be met, the program is NOT suitable
for use.

The PDF tool must offer the opportunity to output a PDF file silent via command line on a printer.
Silent means here that neither a dialog opens nor is the PDF display nor is any interaction expected.



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            19
After the output on the printer, the program must end again. It is recommended that you test this
manually on the command line in advance as service user.

The Print Service instance in question will wait for the end of this program call and evaluate a return
value. If you are working with a Windows script, let's assume a success if the return value is equal
to 0.


        3.6.4.           Description of the flow
The user selects the configured PDF printer - like other printers - in A+W Enterprise. From the print
call, the print job is prepared in the transfer tables PRINTTRANSFER/PRINTPARAM. The only
difference from an output on a normal printer is the output type in the
PRINTTRANSFER.OUTPUTFLAG field; here a "6" is entered instead of a "1".

If a Print Service processes a print job with the output type "PDF Printer", it is checked whether the
configuration of the PDF tool is complete, that is, whether the file is present and whether arguments
were specified. Furthermore, a valid printer must be specified. If one of these prerequisites is not
fulfilled, there is an error status.

After that, for each record in PRINTPARAM, a PDF export is written to the internal working directory.
If all PDF files have been created, the individual PDF files are combined page by page into a new PDF
file (merge). If the DUPLEX option was specified, an empty page is added to PDFs with an odd number
of pages in order to guarantee that the individual outputs are separated from one another. If the
number in PRINTPARAM.OUTPUTQTY is greater than 1, the PDF files are attached multiple times in
order to create the appropriate number of copies this way.

In case either the printer or the PDF tool cannot cope with the size of the PDF file created, you can
set the file size in Mbytes via the environment variable CR_MERGEPRINT_MAXSIZE. In this case it
can happen that more than one PDF file is created.

After the combination, the merge PDF files created this way are printed out one after another via
PDF tool. In the process, the parameters %PRINTER% and %PDFFILE% described above are
replaced by the concrete values and there is a program or script call. If there is an error here, a
corresponding error is returned to the Print Service.


        3.6.5.           Internal working directory
Starting with #413469, the Print Service will work with one internal working directory per print job.
Under %PROGRAMDATA%\A+W\A+W Enterprise 6 Print Service an individual directory will be
created for each print job (pid<pid>) in which all necessary files are created and saved temporarily.
The purpose of this intermediate storage is to simplify the flow of the Print Service and if necessary
to speed it up, since work is only done locally. Furthermore, necessary research should be simplified
with this.

If the print job was processed successfully, the directory will be deleted again. If, by contrast, there
is an error, the directory remains and a Trace subdirectory is created in which data is collected that
is intended for making troubleshooting go faster. Whether or not the directory should always be
deleted can be configured with the config tool. Furthermore, very old directories are deleted in
maintenance mode insofar as this is active. The internal directories are kept for a maximum of 3
days.



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            20
The subdirectories are used as follows.

-   The archive copies are stored in the archiv subdirectory, if necessary provided with a
    watermark, and then copied to the archive directory.
-   Sketch files are generated in the bitmaps subdirectory and copied to the directory
    CR_IMAGE_PATH BEFORE the report call.
-   PDF files for e-mail attachment, file exports and merge files are placed in the export
    subdirectory. For a file export, after the creation, the file is copied to the desired output
    directory.
-   Other e-mail attachments are saved in the files subdirectory in individual subdirectories
    according to sequence numbers and processed.
-   In the trace directory, files for the print job and the environment are collected and retained for
    research in case of error. This is data that can appear this way or in another form also in the
    trace file.

If the internal working directory could not be created, work will be done as previously with the
previous directories. Only such subdirectories will be created that are necessary for the print job. If
the archiving is not active or not necessary, no archiv directory will be created.


         3.6.6.             Example of an external PDF tool: Foxit reader
For our tests, we decided on the Foxit Reader in Version 6.2 since it fulfills all requirements.
Download link:
http://cdn01.foxitsoftware.com/pub/foxit/reader/desktop/win/6.x/6.2/enu/FoxitReader623.815_
enu_Setup.exe
Starting with Version 9.4, the silent print should work again, but that could not be verified thus
far. See also #439227.




Fig. 1: Foxit Reader Help




A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                           21
A+W Software GmbH   EN-CONFIG-A+W Enterprise Print Service.docx   22
4. Form printing or e-mail
Output of forms of a market partner either via form printing or sending via e-mail.
Both in form printing as well as in e-mail sending, you can load processes regardless of market
partner and output these according to module. If for a particular market partner and a particular
form a particular dispatch method is agreed upon, that is, for the invoice form particular
customers should always receive an e-mail, other market customers always receive a printed
copy, the user can no longer know this.

In order to assist the user here, a configuration possibility has been implemented in order to store
per market partner and form precisely whether particular forms should only be printed or
whether they may be mailed. The configuration is done via configurable fields in the market
partner master data and environment variables.

If for a market partner it was configured that his invoices may only be sent via e-mail, in form
printing the processes with vorgang=7 are no longer loaded for this customer. If for this customer
you enter an invoice number manually in form printing, you will see a message that the output via
this module is not allowed. Vice-versa, for all customers for whom the identifier is not set, the
invoice can no longer be sent via e-mail. For these customers, the process can only be output via
form printing.

In the form printing it is possible to print several form types together, e.g. order confirmation and
check OC. If now there is a configuration that limits the form printing for a form type, but not for
the other form type, the processes that would be affected by this are loaded nevertheless. If the
printing is initiated, each process is checked again against the market partner data and depending
on the configuration, it is output or not.

The limitations described also apply for file printing.

The configuration of this solution is done via configurable MP fields and environment variables. A
configurable MP field of the type "numeric" is created, which you could call "Invoice only via e-
mail," for example. You enter the field name in an environment variable
RESTRICT_EMAIL_DOCUMENT_<FORMART>. Here, <FORMART> is the form type of the report
whose output you want to limit. For example, for the individual invoice, the formart = 7, for the
collective invoice, the formart = 12. The form types can be looked up in the form management
(rep.formart).

In form printing and in e-mail dispatch, these settings are read out and evaluated as follows. For
the combination market partner and form type, the configurable MP field has the value

    -   0 -> Only printing allowed.

    -   1 -> Only e-mailing allowed.

If such an environment variable incl. conf. MP field has been created, the either-or principle
applies. Either printing is allowed or e-mailing. The file printing is also affected.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                          23
It is also possible to use the same conf. MP field for different form types if this is desired. For
example, for individual and collective invoice, a common field would make sense. Nevertheless,
an individual environment variable is required for each form type.

Delivery note: for the solution, the messages were expanded. These must also be delivered for
the start-up of the solution. There are texts in German and English.


4.1. Printed or sent documents
[AW-172160] / QR2406

Within the form output, forms can be printed or sent by mail. If forms are printed, they also
counted at the same time as send and vice-versa. To distinguish a control print from sending by
mail, previously 2 separate forms were required. This increased the maintenance and
administration effort.

Now, you can distinguish whether a document was printed or sent via e-mail. On both dialogs, the
date of printing and sending is visualized. This way, the printed documents do not automatically
count as sent. The option "all not yet output" refers to the relevant ID in each case. If you are
printing, then here only the selection "printed" ID is evaluate, not whether the form has already
been sent via mail and vice-versa.


4.2. reptmp/ repform
When creating a new kauf record, entries are generated in the table repform; using those in form
printing and e-mail dispatch, it is detected whether there has already been an output and when.
For each configured report in the table rep, with the appropriate values in the document, REPID,
and form group and active = 1, a corresponding record is generated in the table repform. If this
record is not present, the document can only be entered manually.


4.3. Additional forms ([AW-73668])
The following developments preceded this development: #327461 und #440096
With this development, the use of the environment variable
CR_ADDITIONAL_REPORT_[FORMART] was expanded. It is now possible to attach several
additional reports to a form type and thus to trigger automated form printing.


Example:
CR_ADDITIONAL_REPORT_6 maintained with "126, 996"
If a delivery note (form type = 6) is printed now, printparam database records are also generated
for the forms 126 and 996 and they are printed out with the delivery note print job.


Particularities that come from the original development:



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                              24
-        For the form types, a report in the table rep (System > Print management > Forms > Manage)
         must be created. This entry must correspond to [FORMART] entry in question. This must be a
         Crystal Report (rep.repart=1), it must be a form (rep.reptyp=1), the form must be active and
         have 6 parameters. Furthermore, it must have the same process type (rep.vorgang) as the
         original form.
-        The reports must have the same parameters as the [FORMART] report. This is especially
         important with the advance delivery note printing since it has other parameters than usual
         forms.
-        The logic only applies if as output type a printer was selected or during PDF export.
-        The solution considers the evaluation of the sketch print ID, the archiving, and the text
         generation for the additional report. For the additional report, the evaluation of the
         document types is not initiated.


4.4. E-mail dispatch
             4.4.1.          Determination of the e-mail addresses
In e-mail dispatch, there is a multi-stage logic in order to determine an appropriate recipient
address for a document. So that an e-mail address can be found, it is recommended that you store
a general address for the market partner in the market partner field.


    Step           Description
    -3             Call of the stored procedure rpmgetmailformsnddst (auftrnr, vorgang, subnr,
                   formart). This SP provides a sender and recipient address. If this SP returns
                   "STOP_ADDRESS_SEARCH" instead of a recipient address, the following steps are
                   not run through.
    -2             Call of the stored procedure rpmgetmailformsnddstccbcc (auftrnr, vorgang, subnr,
                   formart). This SP provides a sender and recipient, a CC and a BCC address. If this SP
                   returns "STOP_ADDRESS_SEARCH" instead of a recipient address, the following
                   steps are not run through.
    -1             If there is an e-mail address for the quotation (vorgang = 4) or the order
                   (vorgang=5) in the field kauf.orgemail. The sender's address is determined
                   separately.
    0              Is there an e-mail address for the contact person for the order (kauf.busr) in the
                   table anspr (anspr.email)? This stage is only active if the environment variable
                   AWMAIL_ANSPR is not set. The sender's address is determined separately.
    1              Is there an entry in xemail for the combination of market partner, user, and form
                   type of the document? QR2304 – with active internal client separation, the entry
                   can be made client-specifically. First the client of the document is searched for and
                   if no special entry is found for it, then client=0 [AW-108769]
    2              Is there an entry in xemail for the combination of market partner, department, and
                   form type of the document? QR2304 – with active internal client separation, the




A+W Software GmbH                 EN-CONFIG-A+W Enterprise Print Service.docx                           25
              entry can be made client-specifically. First the client of the document is searched
              for and if no special entry is found for it, then client=0 [AW-108769]
 3            Is there an entry in xemail for the combination of market partner and user of the
              document? QR2304 – with active internal client separation, the entry can be made
              client-specifically. First the client of the document is searched for and if no special
              entry is found for it, then client=0 [AW-108769]
 4            Is there an entry in xemail for the combination of market partner and department
              of the document? QR2304 – with active internal client separation, the entry can be
              made client-specifically. First the client of the document is searched for and if no
              special entry is found for it, then client=0 [AW-108769]
 5            Is there an entry in xemail for the combination of market partner and form type of
              the document? QR2304 – with active internal client separation, the entry can be
              made client-specifically. First the client of the document is searched for and if no
              special entry is found for it, then client=0 [AW-108769]
 6            Is there an entry in xemail for the market partner of the document? QR2304 – with
              active internal client separation, the entry can be made client-specifically. First the
              client of the document is searched for and if no special entry is found for it, then
              client=0 [AW-108769]
 7            Is there an e-mail address for the market partner in the MP master data? The
              sender's address is determined separately. This stage can be deactivated with the
              environment variables MAILFORM_NO_ADDRESS_FROM_MP.




        4.4.2.           Determining the sender's address
If the sender's address cannot be determined from the table xemail, there is a multi-stage
determination logic to determine the sender's address.
First it is checked whether REP_REPLYTO is set and has content. If this is the case, it is checked
whether an address was specified for the current employee (akt.manr) in mitarb.email and also
used as the sender. If in the employee master data no address is found, the content of the variables
REP_REPLYTO is used as the sender's address.
If REP_REPLYTO is not set or if it is empty, then the customer's e-mail address (mp.email) is used
that is entered in xhaus.kunr for the current site (akt.hnr). The site number corresponds to the value
from mitarb.hnr of the current employee.
If no sender could be determined, no e-mail can be sent! A corresponding message informs the user
about this circumstance in the e-mail dispatch. If a special e-mail printer is used for the Print Service,
there is a status flag = 302 (no sender found) and no valid value is present in mailparam.mailfrom.


             4.4.2.1. Use of a stored procedure for e-mail determination
If you want to determine your e-mail data via stored procedure: rpmgetmailformsnddst or
rpmgetmailformsnddstccbcc , then you must determine the sender's address by yourself.
There is no fallback to the table xemail for the SP variant.


A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                             26
If no proper sender e-mail comes back from the SP, then the determination logic mentioned under
6.2 is used.


        4.4.3.          Mail server configuration

            4.4.3.1. Mail server for error notification
Up to Version AWE5 (12.5), the mail server for the error notifications is configured on the
"More..." subdialog per database configuration.
Starting with Version AWE6 (13.9), there is an individual page per Print Service for the
configuration of the error notification incl. mail server setting.


            4.4.3.2. Mail server for the mail dispatch
Up to Version AWE5 (12.5), the mail server for the mail dispatch is transferred to the Print Service
via the field mailparam.mailserver. That is, the determination of the mail server was done in the
back end.
Starting with Version AWE6 (13.0), the mail server is determined in the Print Service. Depending
on whether or not the host portion of the recipient address (mailparam.mailto) is the fax domain
(REP_FAXDOMAIN), either the mail server from SMTP_FAX_SERVER or from SMTP_MAIL_SERVER
is taken.
The reason for the conversion was that with the logic from 12.5, the SMTP port could not be
transferred. (see 5.4)


        4.4.4.          SMTP port (#425282)
The configuration of a different SMTP port for e-mail dispatch in the Print Service was not
previously possible. This has now been adjusted.

There are two new environment variables SMTP_MAIL_SERVER_PORT and
SMTP_FAX_SERVER_PORT. The port in question, which should then be used in the Print Service,
can be entered here. If the variable is not set, port 25 is assumed as default value.

For A+W Enterprise 5 Print Service version, a config switch is used internally to determine the mail
server for error notifications, for example. Here there is no separate possibility to define an SMTP
port. In this case, the port can be appended to the mail server separated by a colon, e.g.
mailserver:2500. The port is extracted and used if present. Here, port 25 is also used as default
value.

To be sure that the configured port is being used, a corresponding trace message is output before
use.

Two new environment variables have been defined:

SMTP_MAIL_SERVER_PORT

SMTP_FAX_SERVER_PORT



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                          27
These contain the port to the respective server variable. If the variables are not set, the default port
25 is used.




        4.4.5.           Display of a clear name (#415664)
If an email was sent via the Print Service, the sender's address consisted only of the email address.
The existing logic, which can be configured with the environment variable
AWMAIL_MAILFROM_KLARNAME for the awmail, has not been considered so far. This has now been
adjusted.

The content of the environment variable AWMAIL_MAILFROM_KLARNAME (0-3) is interpreted as
follows:

0, OFF = without name

1 = "Mustermann, Max" (maname, mavname)

2 = "Mustermann Max" (maname mavname)

3 = "Max Mustermann" (mavname maname)

A record in the table mitarb is determined using the sender's address (for example
max.mustermann@muster.com), and the clear name is assembled from the last name and first
name of the employee according to the setting in the environment variable.

The logic is executed for all sender addresses. If there is more than one record in the employee table
with this email address, the first data record found is evaluated during the evaluation.

If configured accordingly (=3), the result looks like this:
Max Mustermann <max.mustermann@muster.com>


        4.4.6.           Merge of file attachments (#293039)
It is possible to set a dispatch type for every combination of recipients in the email master data
under Master data > Market partner > <F4> Menu > Contact details > Email addresses. The options
"0 - Standard" and "1 - Several PDF/one email" have long been supported by the Print Service;
however dispatch type "2 - One PDF for all" has not. This option has now been set-up in the Print
Service and is taken into account when it comes to dispatching emails.

The option "One PDF for all" means that all individual PDF forms that are to be sent to the same
recipient group are combined into one PDF document. Only this combined PDF file is then sent as
an email attachment.

Exceptions include declarations of performance and other procedure documents. These will
continue to be attached individually to emails.

Information regarding how the email attachments need to be grouped is passed on to the Print
Service via the new field MAILPARAM.ATTDISPTYPE. When it comes to determining the email


A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                           28
addresses, the value is either derived from XEMAIL.VERSANDART or from the new environment
variable CR_MAIL_DISPTYPE.
The individual options both for the field as well as for the environment variable:
0 – an e-mail is sent for each PDF attachment
1 – several PDF attachments to the same group of recipients (to, cc, bcc, from) are sent with one e-
mail.
2 – several PDF files to the same group of recipients (to, cc, bcc, from) are combined into one PDF
file and then sent with an e-mail.
Options 1 and 2 already existed. New now is option 2. Starting with A+W Enterprise 5, the file
MAILPARAM.MAILTO2 is added to the grouping.
The dispatch type does not exist for particular evaluation stages (see
\\jupiter\Doku_DocuWare\ALCIB-PMS\DRUCK\FAQ_Tips_Tricks\ MailFAQs.docx). In these cases,
the content of the environment variable CR_MAIL_DISPTYPE is used.
The field PRINTTRANSFER.SINGLEFLAG, via which it was previously controlled whether or not
grouping should be done, is now always set to the value 1 for e-mail dispatch.
The file name of the combined PDF file is composed as follows: att-<pid>-<sequential number>-
<date>.pdf
The logic also considers the maximum e-mail size (MAILPARAM.MAILSIZE or CR_MAILSIZE), so
that it can happen that several e-mails are sent although option 2 was selected. The files are only
combined so that the specified file size is not exceeded.
Important for the delivery is that information such as subject, e-mail text can only be taken from
one MAILPARAM data record, namely the last one within a group that belongs together. This must
be considered for the adjustment of the corresponding SPs, which determine these values.
However, from the beginning, these include the dispatch type as parameter. (see
\\jupiter\Doku_DocuWare\ALCIB-PMS\DRUCK\FAQ_Tips_Tricks\ Print Service - Referenzen.docx).
Furthermore, the declarations of performance and other transaction documents are considered.
These files are never combined since they do not absolutely have to be present as PDF file.
However, these files influence the maximum e-mail size and are considered accordingly.


        4.4.7.          Additional e-mail to the e-mail sender [AW-74765]
With this development, the possibility was created to send the e-mail sender an additional e-mail
copy of an e-mail print job to himself. This function is activated with the CR_REPLY_TO_SENDER
environment variable.


        4.4.8.          Naming of file attachment
In the Print Services, it is possible to name an e-mail file attachment with the stored procedure
"rpattfilename". This value is entered in the database column mailparam.attfilename and
completed by default in the Print Service with printtransfer.pid and printparam.seqnr. This is done
to guarantee uniqueness.
The adding of the Pid and sequence number can be blocked with the environment variable
REP_RPATTFILENAME_ONLY. If this logic is switched on, it must be noted that the naming from
the SP should be unique.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                         29
4.5. PDF copy as transaction document
Under the AWDesk case #439086 or Feature 20920, the reporting for A+W iQuote was developed.
For this, a PDF copy logic was installed, which does not absolutely have to be used with the A+W
iQuote.
This logic creates copies of print jobs and creates them as documents for the respective
transactions. This file can be viewed in the document overview of the transaction.
For configuration, you can read the configuration instruction EN-CONFIG-A+W Enterprise iQuote
Reporting chapter.




A+W Software GmbH           EN-CONFIG-A+W Enterprise Print Service.docx                      30
5. Print list




A+W Software GmbH   EN-CONFIG-A+W Enterprise Print Service.docx   31
6. (Preliminary) delivery note printing in
  dispatch control
6.1. Print additional forms if (advance) delivery note
   printing is triggered in dispatch (#327461)
A possibility was implemented so that during (advance) delivery note printing in dispatch, an
addition, other form can be output. This is comparable to the possibility in form printing to select
several forms and print them simultaneously. The solution is only intended for Crystal Reports
forms that are output with the A+W Enterprise Print Service.
The solution only exists in the dispatch control for the menu elements advance delivery note and
delivery note printing.

In the environment variables CR_ADDITIONAL_REPORT_[FORMART] ([FORMART] = 6 for delivery
note, 28 for advance delivery note), an additional form type is stored that should be printed in
addition to the (advance) delivery note. If the logic should be configured for the advance delivery
note, the form type 175 must be used.

For this form type, a report in the table REP (System > Print management > Forms > Manage)
must be created. This entry must correspond to the (advance) delivery note entry in question.
This must be a Crystal Report (REP.REPART=1), it must be a form (REP.REPTYP=1), the form must
be active and have 6 parameters. Furthermore, it must have the same process type
(REP.VORGANG) as the original form.

The report must have the same parameters as the (advance) delivery note report. This is
especially important with the advance delivery note printing since it has other parameters than
usual forms.

The logic only applies if as output type a printer was selected or during PDF export.

The solution considers the evaluation of the sketch print ID, the archiving, and the text generation
for the additional report. For the additional report, the evaluation of the document types is not
initiated.




6.2. Acceptance test certificate for delivery note
   generation (#440096)
Print of delivery note has been extended so that an acceptance test certificate can now also be
issued. If the new functionality has been configured, the system checks whether items relevant to


A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                          32
the inspection certificate exist during delivery note and partial delivery note generation. An
inspection certificate is generated for such items and attached to the delivery note.

Likewise, via the market partners e-mail address maintenance mask (Master data > Market
partners > [F4] > Contact data > E-mail addresses) of the new form type 126, a recipient can be
created who also receives the generated acceptance test certificates by e-mail.

Report management

The acceptance test certificate report must be created in the report management (System > Print
management > Forms > Manage ). This must be a Crystal Report form with form type 126. Form
type 126 can be archived.

Settings Relevant for the Inspection Logic of the Inspection Certificates

The inspection logic that decides whether a source inspection certificate is to be created consists
of two parts. First, the value of the field KAUF.PRIVATE_LONG2 is checked. If the value is "1", the
system also checks whether there are items that have been flagged as relevant for the inspection
certificate. This information is expected in the new set of configurable fields with Setid 1002 in
field LONGAVL1.

Configurable texts

Texts with the print position "Special1" can now be created in the text management (Master data
> Text management > Configurable texts). These texts can be evaluated in the inspection
certificate report.

Archiving of the PDF printer

The PDF printer, which is used to combine printouts, now archives the individual print jobs. No
combined printouts are archived; instead, the individual print jobs are.

Configuration:

Environment variable:

-   LAPOOL_PREFZEUGNIS (ON/OFF)  for logic activation
-   CR_ADDITIONAL_REPORT_6 = 126  Additional report for the delivery note with form type
    126.

ARCHIV_FORMULARE = digit 44 must not be equal to 0.  For the inspection certificates to be
archived.




A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                        33
6.3. Dividing up advance and/or delivery notes for a
   route into several print jobs ([AW-151256])
With the environment variable CR_SINGLE_PRINT_VLS for advance delivery notes or
CR_SINGLE_PRINT_LS for delivery notes, it can be activated that you divide up the printing of
advance and/or delivery notes for a complete route into several print jobs.
This logic thus generates a new print transfer record with its own print ID for each advance and/or
delivery note.
Reason for the implementation:
The customer controls a stapler function of its physical printer and this extension was
implemented so that the customer can combine the original and copy via external PDF tool and
send these together to his printer with stapler function.
The customer would like to staple the individual originals and copies of a delivery note and not a
complete route.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                         34
7. Invoice, credit note, and printing
  collective invoices
7.1. eInvoicing (XRechnung, ZUGFeRD)
With the development under DevOps Feature 104965, XRechnung and the Feature 138876 the
PDF extension ZUGFeRD will be incorporated into A+W Enterprise and the AWE Print Service.
This section will explain only the configuration for the print area and Print Service.
Configuration of XRechnung creation for the B2B Service is assumed; for more information about
this, see Feature 104965 and the A+W Enterprise B2B Config instructions.


        7.1.1.          Process
The A+W Enterprise B2B Service offers the opportunity to generate customer-specific electronic
invoices in the XRechnung format. This is an XML document.
The generation is triggered on invoice booking (if the invoice could be booked successfully). The
file generated is saved in the configured storage location.
The XRechnung generated is saved as file attachment of the AWE invoice.
For the invoice generation, a document type record is written for the created XRechnung in the
table kaufdokutype. (For the invoice printing, the required data from the kaufdokutype table is
checked and not from xdokutype.)
Print triggering in Sales > Forms > Print or E-Mail/Fax:
For Forms > E-Mail/Fax the new fields from MP master/invoices are displayed.




RV = e-invoice dispatch via e-mail
ER = electronic invoice (XRechnung)


A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                         35
For print triggering in Sales > Forms > Print:
With this print triggering, it is not ensured that the e-invoice will actually be sent via e-mail,
therefore a notice is displayed that asks the user to trigger printing via Sales > Forms > Email in
order to ensure e-mail dispatch.




After confirmation of the notice, the user will not be hindered from triggering printing via Sales >
Forms > Print.
The notice can be suppressed with customizing.



Checks for print triggering
    1. Document type with document type XRechnung (xdokutype.dokutyp = 5) maintained?
    2. MODUL_EINVOICING set?
    3. Database field printparam.einvoicing and printparam.einvoicingsendingtype present?
    4. Market partner maintained correct (mp.rechexport and mp.rechemail)?
    5. kaufdokutype filled and form vector (kaufdokutype.formular) correct for form invoice?
If everything matches, the database field printparam.einvoicing is assigned the mp.rechexport
value and printparam.einvoicingsendingtype is assigned the value mp.rechemail.
Takeover of the XRechnung XML document
After correct check, the information for the XRechnung XML document are collected in the e-mail
dispatch of the A+W Enterprise and entered in the table printfiles and processed by Print Service.
(mp.rechemail + mp.rechexport)
Only XRechnung (mp.rechexport=1 + mp.rechemail=0)
After the PDF invoice creation, the file attachment flow of the Print Service collects the
XRechnung XML document in DATEI_REF_PFAD and sends only the XRechnung file in attachment
to the e-mail recipient.
XRechnung + PDF (mp.rechexport=1 + mp.rechemail=1)
After the PDF invoice creation, the file attachment flow of the Print Service collects the
XRechnung XML document in DATEI_REF_PFAD and sends the PDF with the file in attachment to
the e-mail recipient.
ZUGFeRD (mp.rechexport=1 + mp.rechemail=2)
After the PDF invoice creation, the file attachment flow of the Print Service collects the
XRechnung XML document in DATEI_REF_PFAD and creates with the PDF and the XRechnung XML
document a ZUGFeRD PDF file. The file name of the ZUGFeRD file remains the same as the current
PDF creation.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                             36
        7.1.2.          Master data
Market partner master data (DB table mp)
Field            Type          Key              Description
                                                Document export type (e.g. XRechnung,
rechexport       smallint      no
                                                ZUGFeRD, …)
                                                Send type of the e-invoice (0 = Only e-invoice,
rechemail        smallint      no
                                                1 = E-invoice + PDF, 2 = ZUGFeRD)




(Master data > Market partners > Invoice)

For the market partner, an e-mail address must be entered in the master data.
Document set-up
A document type must be created for the e-invoice. This document type (table: xdokutype) is
created under Master Data > Keys > System > Document Types.




A+W Software GmbH           EN-CONFIG-A+W Enterprise Print Service.docx                       37
Document type must be set to e-invoice and type of output to e-mail and for forms the document
Invoice selected so that the print flow is executed correctly.
Type of output determines whether or not the invoice is sent by e-mail. This data is taken over
automatically into all documents and can be corrected in the process.
CAUTION: For the invoice printing, the required data from the kaufdokutype table is checked and
not from xdokutype.
This document type must then be assigned to the desired forms. Under System > Print
Management > Forms > Document Assignment, you assign the document type to the invoice
forms. (currently only invoice is possible)




The global setting can be overridden for each market partner. (Submenu in the market partner
texts/print -> Document types)
Document-related, the data is saved in the table kaufdokutype.
The document types in the invoice are always currently drawn from the master data and not
taken over from the order or delivery note.
If this document type is not found, no file is reserved and the following service has no information
for the assignment of the file.
Print table: printparem expansion



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                          38
Field                       Type          Key            Description
                                                         Document export type (e.g., XRechnung,
einvoicing                  SMALLINT no
                                                         ZUGFeRD, etc.)
                                                         Send type of the e-invoice (0 = Only e-
einvoicingsendingtype SMALLINT No                        invoice, 1 = E-invoice + PDF, 2 =
                                                         ZUGFeRD PDF)

The new printparam.einvoicing database field is required for forwarding of the document export
type to the Print Service. The data field reflects the value from the market partner field
mp.rechexport and will be set in the mail dispatch of the A+W Enterprise if the necessary settings
were checked positively.
Update according to ZUGFeRD development:
With the expansion of the table column printparam.einvoicingsendingtype, the database field
mp.rechemail from the market partner master data is reflected and then sent directly to the Print
Service.
Note:
So that the XRechnung as attachment is not zipped, the env variable
CR_FILES_MAXSIZE_UNZIPPED must be set to the value UNLIMITED.
After this adjustment, the AWE Print Service must be restarted so that the change takes effect.


        7.1.3.          Archiving

             7.1.3.1. E-invoice
The archiving analogous to the form archiving was developed for the e-invoice processing in the
Print Service. This functionality is available with QR [24/10].
If an e-invoice is configured for a market partner and the archiving is intended for its invoice form,
then the e-invoice is now also copied to the archiving path.
For configuration of the archiving with e-invoice, the stored procedure
rpeinvoicingarchivefilename must be created:
Parameter:
        pid INTEGER
        seqnr SMALLINT
        auftrnr INTEGER
        vorgang SMALLINT
        subnr SMALLINT
        hausnr SMALLINT
        formart SMALLINT
        kunr INTEGER
        einvfilename CHAR(256)


        Return value:


A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                           39
        archivefilename CHAR(256)
Please note that the print job fails if e-invoice + archiving is active, but the stored procedure
rpeinvoicingarchivefilename is missing or no correct archive file name comes back.
CAUTION: If only the XRechnung is sent, only the XRechnung is archived!


            7.1.3.2. ZUGFeRD archiving
The ZUGFeRD archiving is analogous to the current archiving. The created ZUGFeRD file is
archived if an archiving is configured for the invoice form.
It doesn't matter to the Print Service whether a ZUGFeRD PDF or a standard PDF was generated.


        7.1.4.          Documentation generation of e-invoice
Configuration and logic of e-invoice/XRechnung are described in the configuration document
"A+W Enterprise B2B Service".




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                            40
8. Document attachments
With ticket [AW-207440], the logic was adjusted a bit:
In the A+W Enterprise mail dispatch and printing, the logic for additional document attachments,
such as declarations of performance and e-invoice was reworked. For the e-mail dispatch
(Sales/Purchasing > Forms > E-mail/Fax) of document attachments, it is now no longer necessary
that the customer must have a maintained e-mail address in the master data; he should, however,
be selected during the document type assignment (System > Print management > Forms >
Document assignment) as recipient market partner. For printing (Sales/Purchasing > Forms >
Print), an e-mail address in the market partner master data is still required. This can still be
entered on the 1st tab. If this is not desired, it is now possible to maintain an entry in the e-mail
address management (Market partner > Context menu > Contact data > E-mail addresses). So that
the document attachment logic can draw the right e-mail address from the e-mail address
management, an entry with the right form type and the e-mail address must be present. Site,
employee number, and department must be empty.


8.1. Send LE documents (#274142/#274577)
With the cases mentioned above, the activation in A+W SLT and Sommer Informatik was
implemented.


8.2. Send file attachments (#250359)
In A+W Enterprise, the possibility was created to send file attachments to transactions via e-mail.
This was previously only possible if declarations of performance were also processed.
With the new version, it is possible for the user to decide precisely for a file attachment whether a
file should be transferred to production via OrderXML or sent via e-mail in connection with
particular forms to the customer or supplier or employee. The basis for this is the configuration of
the document types in the master data.
Configuration of the document types
Under Keys > System > Document types any desired document types can be defined. A document
includes information about whether it should be sent via e-mail, with which forms processing
should take place, and whether there should be a transfer to production.
Under Market partner > [F4] > Texts/Print > Document types the information can be adjusted
precisely for the market partner. No additional document types can be entered here.
Configuration of the forms
Under System > Print management > Forms > Document assignment, you define the concrete
reports for which during output it should be checked whether or not corresponding assigned
documents should be processed. Here it is also set whether the e-mail should be sent to the
customer and/or to the employee.
Example:
There is a document type "Sketches" with the form selection "Order confirmation+Invoice" and
output type "via e-mail". In the document assignment, only the invoice form was assigned for this


A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                          41
document type. During printing of the order confirmation, this document type is not checked;
only with the output of the invoice is it checked whether or not file attachments with the
corresponding document type occur in a transaction.
If there is a report invoice and a report invoice copy, in the configuration described, the
evaluation of the transactions is only undertaken for the report invoice, but not for the invoice
copy.
Use in transaction recording
In the transaction entry, it is possible via [Shift]+[F4] > Document types for the document types for
which the identifier VF was set in the master data to view and configure them precisely to the
transaction. For all other document types, the values from the master data apply.
If now you attach a new file to a transaction in the header or in the items, you select a document
type and the values for "type of output" form, and production are pre-populated according to
their configuration. The user now has the opportunity to adjust these settings.




File attachments for reference
If reference is made to a transaction, the files are not copied; instead they are taken over as a link
to the original file. Via a reference key, the actual file can be found on the file server.


A+W Software GmbH              EN-CONFIG-A+W Enterprise Print Service.docx                          42
Sending file attachments via A+W Enterprise Print Service
As already is the case of declarations of performance, for other document types during form
printing, e-mail dispatch and (advance) delivery note printing, it is checked in dispatch whether
there is a corresponding document type assignment for the current form. If this is the case, it is
checked for the transactions to be output whether there are appropriate documents. For this, the
type of output and form vector are checked. Only if an output via e-mail is set and the form vector
fits the current form is a processing initiated.
For the file attachments found this way, appropriate data records are created in the transfer
tables of the print service. Depending on the type of output of the form - print, file export, e-mail
dispatch - the recipient data is taken from the dialog or read from the master data. If the output is
not done via the print service, an individual "print job" is generated for the print service that is
only responsible for sending the files.
In the print service, the concrete files are first copied to the server and combined into one or
several Zip archives. Here, attention is paid to the maximum size for file attachments. The
resulting e-mail contains, depending on the output type, the PDF with the form output, the
declarations of performance, and the associated Zip archive.
Since in A+W Enterprise there is no limitation for particular file types that you attach to a
transaction, it was decided to combine the files in a Zip archive into a package. The recipient of
the e-mail thus only has to permit this file type as file attachment in his firewall and on his e-mail
server, and not an arbitrary number. These Zip archives can be searched via virus scanner and
offer the advantage that the file attachments can be compressed if necessary.
The logic described assumes the A+W Enterprise Print Service in the Version 6.4 and the reworked
bin files alcib and lapool.
The environment variable DATEI_REF_PFAD must be set. The path specified there must be
accessible from the server on which the print service is installed. The print service user must have
sufficient access rights to this path.
The following new environment files must be installed for the logic, and the last version in
alcibversion must be 13.0.4.

$ALCIBPRG/schlue/cho/formchoice.cho

$ALCIBPRG/schlue/cho/formchoice.dat

$ALCIBPRG/schlue/pan/formchoice.pan

$ALCIBPRG/schlue/mfo/xdokutype64.mfo

$ALCIBPRG/schlue/pan/xdokutype64.pan

$ALCIBPRG/kauf/cho/formchoice.cho

$ALCIBPRG/ kauf /cho/formchoice.dat

$ALCIBPRG/ kauf /pan/formchoice.pan

$ALCIBPRG/kauf/mfo/kaufdokutype64.mfo

$ALCIBPRG/kauf/pan/kaufdokutype64.pan


A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                           43
$ALCIBPRG/kauf/mfo/kaufref64.mfo

$ALCIBPRG/kauf/pan/kaufref64.pan

The SP rpattfilename is used in order to determine a name for the file attachment even if the
form is output on a printer or as PDF attachment.


8.3. Embedding additional files in PDF
With the dossier list logic [AW-177854], the possibility was created to embed additional files in a
PDF. Currently (02/05/2025), this logic is only possible for the dossier list.


        8.3.1.          Creating a dossier list
The dossier logic is activated with the environment variable MODUL_DOSSIER. If the logic is
activated, there is always an attempt in the Print Service to create a dossier list from the dossier
numbers of the document.
For this, the stored procedure "cu_getdossiernumbers" is required. The SP is called in the Print
Service.

 Name                               Parameter & return values

 cu_getdossiernumbers               Parameter:
                                    p_auftrnr INTEGER,
                                    p_vorgang SMALLINT,
                                    p_subnr SMALLINT,
                                    p_formart SMALLINT


                                    Return value:
                                    dossiernumber CHAR (256),
                                    errorcode INTEGER


In the stored procedure, the dossier numbers are determined via the kaufprvfld with Setid=11.
The SP is called in a loop and always returns a dossier number text line and an error code.
The dossier number should be comma-separated and can contain any information. The text lines
are each written on individual lines in the CSV file.
Example:
<Dossiernummer>,<Dossierbezeichnung>":

Example:
  1234568,Dossierbezeichnung1


A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                           44
  1234569,Bez2
  1234570,Bezeichnung3
The error code should return 0 if everything is OK. If the error code is not 0, the list is not created.
This way, you can block the dossier list for various forms.
If one or several dossier number(s) could be determined, a CSV file with the dossier numbers is
generated comma-separated. The name of the CSV file is the same as the PDF export name. The
export name is determined by the respective print variants.
For example:
E-mail: Stored procedure rpattfilename
PDF export: You assign the name yourself
If a copy of a printout should be generated, the ATTACH_PRINTOUTS_TO_DOCUMENT logic can
be set up for this (EN-CONFIG-A+W Enterprise iQuote). In the logic, the PDF export name for the
dossier logic can be changed. For this, the existing stored procedure "rppdfcopyfilename" is
required.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                             45
9. Printing sketches
9.1. SNLive & AWBom sketches (#185271)

9.2. AWDesign sketches (#118996)
A+W Enterprise 5 now integrates the effective, fully graphic grill pattern display of A+W CAD
Designer; like the A+W CAD Designer display of processings, this provides an even more realistic
visual impression of complex grill pattern constructions, both for rectangular and shaped sheets.
At grill pattern entry or on the item list – direct visualization allows direct control of the defined
grill pattern and helps to avoid errors. These grill patterns can be printed to pass order details on
to your customers or suppliers.
Document entry

The grill pattern dialog has been extended; the AWDesign sketch for the defined grill patterns is
displayed. For IG units with several grid patterns, grill patterns for the grill are displayed that is
active in the table (bottom part of the dialog). The sketch is updated with each change of the
number of bar or color. The sketch appears true to scale, taking the shape of the item into account.
Auxiliary bars are still entered in the old grill pattern editor (rectangular view).

In the order item, the AWDesign sketch appears instead of the shape sketch. If there are several
grids, the grid of the first spacer is displayed.

ALCIB 2012.1 Print Service

With this Version, AWDesign permits the printing of sketches on forms. Prerequisite for this is that
the ALCIB 2012.1 Print Service and Crystal Reports are used in connection with AWDesign. This
configuration is similar to the one that is necessary to enable SNLive sketches.

The forms on which sketches shall be printed in general have to be configured accordingly in
ALCIB. The sketch code must be enabled in System > Print management > Forms > Manage.
Please note that only reports that have been defined as forms can be used for printing sketches.

At ALCIB order entry, the 'Print shapes' code must be enabled on the Properties tab in the order
header to make sure that sketches can be printed at all for this order. On item level, the user can
define the type of sketch that shall be printed for the item in question. The appropriate setting for
this is found on item level on the Properties tab, Print sketches field. This field permits selection
from SNLive, AWDesign, and the glass structure (AWBom) the sketch types that shall be printed.
An environment variable can be used to define the default setting for the 'Print sketches' field.

The AWDesign switch must be enabled in the Config tool of the Print Service; the Crystal Report
forms have to be adapted for printing AWDesign sketches.

Document entry

The environment variable used to enable the grill pattern display in AWDesign is called
AWDESIGN_SPROSSEN_ANZEIGE. If this variable has not been set, the former ALCIB display will
be kept.


A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            46
The environment variable for presetting the field kpos.imagedrkz is KPOS_IMAGEDRKZ_DEFAULT.
Please enter the bit vector to be used by default.

    1.   digit: SNLive
    2.   digit: AWBom
    3.   digit: AWDesign


Print Service

Configuration is done in the same way as in SNLIve and AWBom, only that there are special
switches for AWDesign.

The Print Service evaluates the following environment variables especially for AWDesign sketches.

CR_IMAGE_FORMAT_AWDESIGN: File format of the AWDesign sketch. BMP or EMF are valid.
Other types are not supported.

CR_IMAGE_SIZE_AWDESIGN: Size of the resulting image; this is not necessarily the size in which
the image is displayed. The definition is „Width,height“, e.g. „200,200“.

The ConfigTool offers a new switch for switching the AWDesign module on or off.

Unlike version 2011, the Print Service only creates the sketches that were selected in
kpos.imagedrkz. The previous version used to create all sketches by default.

The file name of the AWDesign sketch is principally structured like the names of the other sketch
types except for the type. AWDesign is encoded with an A:

image-<pidno>-<auftrnr>-<posnr>-<type>.<format>


         9.2.1.            Muntin pattern for insulated glass with AWD file
For insulated glass, currently (status as of 06/16/2025), only the muntin pattern is generated via
AWD file of the topmost muntin. It is not yet possible with insulated glass with more than 2 lites to
generate several A+W Design images if there should be muntins between several lites.


9.3. Sketch attachment for REPGO printing (#211903)
REPGO reports can now be printed with SN sketches. This applies to the printing of forms (SA/PU)
and to email dispatch (SA/PU) in ALCIB and to the printing of delivery notes and preliminary delivery
notes at shipping. Apart from the creation of special sketch reports and installation of the ALCIB
2011 Print Services on a Windows server, this requires settings in ALCIB and its environment.
The environment variable MODUL_PRINTSERVICE has to be set to 2 to be able to print Crystal
Reports in ALCIB in the first place.
Whether or not SN sketches shall be printed for a certain form, e.g. for order confirmations is defined
in report management. The code Sketches = Yes is set for the report.
At least one Crystal Reports sketch report has to be set up in System > Print management > Forms
> Manage .



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                           47
You should pay special attention to the following settings:

    •   File name: File name of the report without file suffix
    •   Path: UNC path of the report
    •   REPID: Only customer REPIDs will be analyzed. 9900 is not meant for sketch reports!
    •   Form type: The form types 180 - 189 are reserved for CR sketch reports.
    •   Form group: 1
    •   Document: 0
    •   Repart: Crystal Reports
    •   Reptype: Form
    •   Active: Yes
    •   Number of parameters: 6
    •   Sketches: Yes
    •   Text creation: No

The sketch report to be used for the corresponding printout is defined by the environment variables
REP_CRMODRPT, REP_CRMODRPT_<formart>, and REP_CRMODRPT_28 . They include the form
type of the CR sketch report to be used.
The program first checks whether a special CR sketch report has been defined for the form type of
the form to be printed, e.g. if the order confirmation format is formart=5. In this example,
REP_CRMODRPT_5 would be checked first. If this variable has not been set, the general
variable REP_CRMODRPT will be analyzed. The resulting form type can be used to determine the
corresponding CR sketch report in table REP .
For preliminary delivery notes issued in the shipping area, only the environment variable
REP_CRMODRPT is analyzed. If SN sketches are to be printed for this form, a special CR sketch
report will be necessary, using special parameters.
Whether sketches shall be printed at all, is defined by the settings for the report to be printed, and
by the correctly configured sketch report. Printing of forms still permits to print several matching
forms together, e.g. order confirmation and control order confirmation. The configuration of every
form type will be checked separately.
The codes KAUF.MODDRKZ and KPOS.IMAGEDRKZ define whether SN sketches can be printed for a
certain order. This permits control of the printing of sketches in general (KAUF.MODDRKZ) or by
item (KPOS.IMAGEDRKZ). KPOS.IMAGEDRKZ is a byte vector the first digit of which represents
SNLive sketches and the second digit, the icons of the BOM structure (AWBOM).
If these settings define that sketches have to be printed for a certain form and a certain order, the
entry in table REPSPOOL is made as Status = -99 . repspool for this record will not be processed at
first. Entries are also made in the transfer tables of the print service (PRINTTRANSFER and
PRINTPARAM).
After the print service has created the output PDF file in the directory defined in
CR_REP_EXPORT_PATH , the record in REPSPOOL is updated to Status = 0, and via socket
communication, the command D0B is transmitted to the control server. The socket call is based on
the environment variables AWC_ALCIB_SERVER and AWC_PORT_CONTROL_SERVER .
The Print Service issues a PDF file, which has to be copied to the UNIX server. The above-mentioned
path has to be a UNC path for a Samba released on the UNIX servers so that the PDF file can be
included in the common print process.
If the output of the CR sketch report has to be archived, the environment variables
ARCHIV_FORMULARE must be configured correctly, and in CR_REP_EXPORT_PATH , the output
path (UNC path for a Samba release) for the PDF output must be defined.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                           48
As the print service is going to use the same number area as the former REPGO printout, you have
to make sure that the transfer tables PRINTTRANSFER and PRINTPARAM are empty! Otherwise,
there could be a clash of the codes used. The tables include mere booking data which can be restored
by repeating the printout.
The actual printing of forms is started by the script call of repspool. The created PDF files are
integrated in the print stream and are printed via ghost script.
To determine whether printing was started in printing of forms for in email dispatch, there are two
versions of the output flag. 7 for printing via printing of forms or shipping, and 8 for email dispatch.
This information is passed on as a parameter to the report for analysis.




9.4. Printing of schematic diagrams on Crystal Report
   forms (#257788)
At order entry, you can use the item details in field 'print sketches' to define the type of sketches to
be printed on Crystal Report forms. This selection has been extended by the option "Principle" now,
which stands for the so-called schematic diagrams. This means that the schematic diagrams used
in ALCIB can be printed if the ALCIB Print Service is used for printing, and the Crystal Reports
forms are configured accordingly.


CR forms must be capable of printing schematic diagrams. These sketches must be saved in the
directory defined in CR_STATIC_IMAGE_PATH.
In Version 4.5 (ALCIB 2011) we recommend using a transaction SQL for initializing the field
kpos.imagedrkz. Apart from that it is useful to set the byte vector in the transaction SQL because
the Print Service will not be able to decide whether or not a certain flag makes sense.
The points are
    1.   SNLive
    2.   AWBom
    3.   AWDesign (from Version 2012.1)
    4.   Schematic diagrams.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            49
10. Archiving
The archiving logic with environment variable <ARCHIV_FORMULARE> became obsolete with
ticket [AW-77175]. It still serves as a fallback if the new logic was not maintained.


10.1.           Archiving adjustment ([AW-77175])
With the development [AW-77175], the archiving in A+W Enterprise was changed. The logic
ARCHIV_FORMULARE thus becomes obsolete, but it can still be used. New developments will no
longer be made for the old logic. The new logic can only be used with Crystal Reports.
In order to be able to use this logic, a system update of the state of the release notes of the
above-mentioned ticket has to be made. To activate the archiving, the environment variables
CR_ARCHIVE and CR_ARCHIVE_PATH have to be set.
For the new logic, it is necessary to activate the reports that should be archived in the report
management (System > Print management > Forms > Manage) with the archive check box
(rep.archiveflag).




If the archive check box is not set, then the environment variable ARCHIV_FORMULARE is checked
as a fallback to the old logic.



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                           50
10.2.           Archiving of lists [AW-77175]
With the development mentioned above, the archiving of lists is enabled. The configuration has to
be done as under Archiving adjustment ([AW-77175]) and the respective lists activated via check
box for the archiving.
Similarly, two new stored procedures have to be included in the database.

 Name                              Parameter & return values

 rparchivelistfilename             Parameter:
                                   pid INTEGER
                                   seqnr SMALLINT
                                   hausnr SMALLINT
                                   formart SMALLINT
                                   paramlist CHAR(256)


                                   Return value:
                                   archivefilename CHAR(128)

 rpfilllistindexparam              Parameter:
                                   pid INTEGER
                                   seqnr SMALLINT
                                   hausnr SMALLINT
                                   formart SMALLINT
                                   paramlist CHAR(256)


                                   Return value:
                                   SQL-Result INTEGER


The rparchivelistfilename serves to generate the file name, which is used to generate the
archive copy. (printparam.archivefile)
The rpfilllistindexparam fills the Indexparam table with values so that the A+W Print
Service can create an index file. Do not forget that for this, CR_ARCHIVE has to be on 2.
The A+W Print Service includes the complete form archiving functionality for the list archiving. For
additional information about archiving, see Archiving with the Print Service (#234872).




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                         51
10.3.           Archiving with the Print Service (#234872)
The Print Service was extended with the case mentioned to include archiving functions. For form
printing and e-mail dispatch, now, depending on the configuration, PDF copies are created and
stored in an archive directory from which they can be picked up by the archiving system. In addition,
it is possible to create so-called index files if the archiving system needs these.
The archiving function of the Print Service is intended for form printing, the e-mail dispatch of
forms, and the (preliminary) delivery note printing in dispatch. In this case, as for REPGO archiving,
the environment variable ARCHIV_FORMULARE is checked; if it contains the form type that was just
output, archiving is necessary. This logic was changed by Archiving adjustment ([AW-77175]) and
now lists can also be archived.
The archiving function itself is controlled via CR_ARCHIVE. If this variable has the value "0" there is
no archiving; if it has the value "1," only the PDF copy is placed in the archiving directory; and if it
has the value "2" an index file is created in addition.
The environment variable CR_ARCHIVE_PATH includes the UNC path to which the archive copies
are stored. This variable must absolutely be set.
The SP rparchivefilename determines the name of the archiving file and must be created by the
customer if CR_ARCHIVE was set to "1" or "2".
rparchivefilename (pid, seqnr, auftrnr, vorgang, subnr, hausnr, formart)
Return value: char(128)
If a file was determined successfully, printparam.archiveflag is set to "1" and the file name is written
to printparam.archivefile.
If an index file is necessary for the archiving, CR_ARCHIVE has the value "2", then the SP
rpfillindexparam must be created.
rpfillindexparam (pid, seqnr, auftrnr, vorgang, subnr, hausnr, formart)
Return value: integer (0 = SUCCESS, SC value in case of error)
This SP fills the new table indexparam. From this table, the index file is build later on, in that for a
key (PID, SEQNR), the individual lines are written in sequence to a text file. The name of the index
file is the same as that of the archive PDF file, where by the file extension can be configured with
the environment variable CR_INDEXFILE_EXTENSION. By default, ".txt" is used. The index file is also
stored in the directory from CR_ARCHIVE_PATH.
If there is an error during archiving, the print job is still processed. This corresponds to the previous
program behavior in the REPGO environment. The error is noted in the log and the user who
initiated the print job gets an e-mail about which document (auftrnr, vorgang, subnr) in which the
error was encountered.
If there is an error on the back end side, a new system message (79 - "Incorrect archiving") is sent
to the configured user.


In A+W Enterprise 5, the release of the archiving solution comes with Service Pack 3; it includes all
DB changes, etc. Only the correct Print Service version must be used.
For the start-up under ALCIB 2011, the scripts from the directory /develop/sql_scripts/4/archiv
must be used. Furthermore, alcib and lapool must be updated on the back end side, a new version
of the Print Services is required, and last but not least, new texts (messages, fx_texte) are required.


A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                             52
In ALCIB 2009, there is no back end side for an implementation of the archiving function. However,
as ALCIB 2011 print service is applied for this ALCIB version, the above mentioned SQL scripts also
have to be executed in ALCIB 2009 if a new print service is supplied; otherwise, database errors
may occur.
In ALCIB 2011 the field printparam.archiveflag didn't exist yet; in this version, printparam.sfill1 is
used.


10.4.           ARCHIV_FORMULARE
Which forms should be archived must be configured with the Alenv variable
ARCHIV_FORMULARE. Example:
„ANG:AUF:SAM:REC:GUT:0:0:0:0:VLS:0:0:BAG:0:0:0:0:0:0:0:0:0:PRD“
In the REPGO environment, the text is used as prefix for the archive files. In the CR environment, a
"1" would suffice. Currently, 43 different form types are considered.
Here is the set-up of the flag that is used in ARCHIV_FORMULARE.

 Position             Form type                Description

 1                    4                        Quotation

 2                    5                        OC

 3                    12                       Collective invoice

 4                    7                        Invoice

 5                    9                        Credit note

 6                    29                       Kontr.AB1

 7                    30                       Kontr.AB2

 8                    2                        Purchase order

 9                    6                        Delivery note

 10                   23                       Preliminary Delivery Note

 11                   1                        Supplier inquiry

 12                   21                       Erf.Prot. OC3

 13                   20                       OCnP OC4

 14                   27                       Work order



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                           53
15              28                   PDN Lopool

16              22                   Proforma RE AB5

17              36                   OO no prices

18              904                  Test quotation

19              905                  Test OC

20              912                  Test collective invoice

21              907                  Test invoice

22              909                  Test credit note

23              16                   Cash invoice

24              310                  Production documents

25              127                  Invoice2

26              128                  Collective invoice2

27              130                  Credit note2

28              906                  Test delivery note

29              38                   PDN special

30              31                   PO special

31              89                   Purch. special

32              180                  CRSKETCH1

33              181                  CRSKETCH2

34              182                  CRSKETCH3

35              183                  CRSKETCH4

36              184                  CRSKETCH5

37              185                  CRSKETCH6

38              186                  CRSKETCH7



A+W Software GmbH     EN-CONFIG-A+W Enterprise Print Service.docx   54
 39                    187                      CRSKETCH8

 40                    188                      CRSKETCH9

 41                    189                      CRSKETCH10

 42                    175                      PDNLAP - copy

 43                    86                       PDN - PO

 44                    126                      Fax delivery note
                                                "Acceptance test certificate" (#440096)



10.5.           Watermarks in archiving #374635
If forms are added to an archive system as PDF, it is now possible to provide these archive copies
with a configurable watermark. For this logic, the A+W Enterprise Print Service must be
configured appropriately.
To activate this logic, the ALENV variable CR_ARCHIVE_WATERMARK (ON/OFF) has to be set to
the value ON. Via the variable CR_ARCHIVE_WATERMARK_TEXT it is possible to configure the
watermark text. If this variable is not set, the default value "COPY" will be used.
Prerequisite for this logic is that CR_ARCHIVE >= 1, that is, that an archiving via the print service
has been configured.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                               55
11. Print Service – general
      11.1. Print status check
Print jobs that have encountered an error remain in the system with the corresponding
status. It is now possible to check these print jobs via a dialog and to present them again
for printing. The associated dialog is under System > Print Management > Check Print
Status. When starting in an internal client separation, first the site is queried from which
the incorrect print jobs should be displayed. If you do not specify a company number,
then all data is obtained. Depending on the configuration of the client separation, the
employee-company assignment is also considered.

With F5/"Detail", you can display all elements of the print job. Thus far, it has not been
possible to change the parameters on this dialog, however.
The fields also cannot be changed directly on the overview of print jobs. With the "Reset"
or "Reset all" button, you can delete the status and ServiceID. The record is then marked
right away for renewed transfer.

On the bottom area of the dialog, the description of the error status is displayed. Please
note that the description is displayed in English here, as is the case in the system message
that is sent to the responsible employee via e-mail.

For this functionality, the employee needs the separate right REER. Here, there is no
distinction made between "read" and "write". Even if the user only has the read right, he
can reset the status of a print job.



11.2.          Status flags
        11.2.1.       Status 0 – 99: progress status

  No.       Status                                 Description

  0         NotReady                               New print job

  1         Waiting                                Print job ready to print

  2         Progress                               Print job in process

  3         ReadyForOutput                         PDF file was generated successfully but the
                                                   file was not yet sent via e-mail (#404875)

  99        Success                                Print job executed successfully



A+W Software GmbH          EN-CONFIG-A+W Enterprise Print Service.docx                           56
       11.2.2.    Status 100 – 149: general error or incorrect
           configuration

 No.     Error                                   Description

 100     Error                                   General error

 101     TextGeneratorError                      Error during the text generation in
                                                 the ALCIB back end

 102     NoEMailPathError                        No path for the temporary PDF files
                                                 was found.

 103     EmailPathWrongError                     The path for the temporary PDF
                                                 files does not exist

 104     NoArchivePathError                      No archive path was specified.

 105     ArchivePathWrongError                   The archive path does not exist.

 106     NoPDFExportPathError                    In the configuration, no default PDF
                                                 export path was specified.

 107     PDFExportPathWrongError                 The default PDF export path does
                                                 not exist.

 108     NoRepPDFExportPathError                 The Rep PDF export path is missing.

                                                 This is expected in
                                                 CR_REP_EXPORT_PATH

 109     RepPDFExportPathWrongError              The Rep PDF export path does not
                                                 exist.

 110     NoRepPDFArchivePathError                The Rep PDF archive path is
                                                 missing.

                                                 This is expected in
                                                 CR_REP_ARCHIVE_PATH

 111     RepPDFArchivePathWrongError             The Rep PDF archive path does not
                                                 exist.

 112     FileSystemCopyError                     There was an error during copying.


A+W Software GmbH   EN-CONFIG-A+W Enterprise Print Service.docx                         57
 No.     Error                                    Description

 113     NoAlcibServerName                        No ALCIB server was specified in
                                                  the configuration.

 114     NoCtrlServerPort                         The port of the control server was
                                                  not specified.
                                                  (AWC_PORT_CONTROL_SERVER)

 115     ExportFileDoesNotExist                   The export file that should be
                                                  processed further does not
                                                  exist.

 116     CouldNotCopyFileToDestination            A file could not be copied into
                                                  the target directory.

 117     CouldNotUpdateXlesprzu                   A record in xlesprzu could not
                                                  be updated.

 118     DocumentBasePathIsMissing                The alenv DATEI_REF_PFAD is
                                                  missing, is not set or is empty.

 119     NoPdfPrinterToolError                    Tools/PDFPrinterTool      is
                                                  empty. Starting with AWE6

 120     PdfPrinterToolNotExistError              Tools/PDFPrinterTool does
                                                  not exist in the file system.
                                                  Starting with AWE6

 121     PdfPrinterNoArguments                    Tools/PDFPrinterArguments
                                                  is empty. Starting with AWE6

 122     PdfPrinterError                          There was an error when
                                                  executing the PDFPrinter
                                                  tools. Starting with AWE6

 123     PdfCopyCreateDirError                    PDF copy logic No export
                                                  target path could be created
                                                  (DATEI_REF_PFAD)

 124     PdfCopyCopyFileError                     PDF copy logic Copying of the
                                                  PDF file into the export path
                                                  failed (DATEI_REF_PFAD)




A+W Software GmbH    EN-CONFIG-A+W Enterprise Print Service.docx                       58
 No.     Error                                       Description

 125     PdfZUGFeRDCreationError                     PDF ZUGFeRD creation failed



       11.2.3.      Status 150 – 199: incorrect printtransfer data

 No.      Error                                Description

 150      PrinttransferDataError               General data error, cause unknown.

 151      NoPrinterError                       No printer was specified

 152      PrinterNotExistError                 Printer does not exist or unknown

 153      NoExportPathError                    No export path was specified

 154      ExportPathWrongError                 Export path does not exist

 155      NoExportFileNameError                No file name for the export file was
                                               specified

 156      OutputFlagError                      Output option unclear/not defined

 157      NoPDFPrinterPathError                No printer path was specified.
                                               /* OBSOLET */

 158      PDFPrinterPathWrongError             The path for the job<pid>.txt files
                                               does not exist.
                                               /* OBSOLET */

 159      NoLenrError                          In printtransfer.exportfile, the LE
                                               number is expected.

 160      ExportFormatNotAvailable             The selected export format
                                               (printtransfer.sfill1) does not exist
                                               or it is invalid.

 161      ExportFormatNotSupported             The CR Runtime version used does
                                               not support the selected export




A+W Software GmbH       EN-CONFIG-A+W Enterprise Print Service.docx                    59
       11.2.4.      Status 200 – 249: incorrect printparam data

 No.      Error                                         Description

 200      PrintparamDataError                           General data error, cause
                                                        unknown.

 201      NoSeqnrError                                  No data records found in
                                                        printparam

 202      NoReportFileError                             Report file does not exist

 203      ReportFileWrongError                          The report name does not
                                                        exist

 204      NoReportPathError                             No report path was found

 205      ReportPathWrongError                          The report path does not
                                                        exist

 206      PreSpError                                    Error in pre_sp

 207      PostSpError                                   Error in post_sp

 208      ParamCntError                                 Number of parameters
                                                        transmitted does not
                                                        match      the  report
                                                        parameters

 209      ParamCntFormError                             None or too few form
                                                        parameters      were
                                                        transferred.

 210      NoParameterError                              No parameters were
                                                        specified,      although
                                                        paramqty    >     0    or
                                                        parameters were specified
                                                        even though paramqty = 0

 211      NoValidFormParameterFound                     No form parameters could
                                                        be extracted from the
                                                        parameter string although
                                                        it is a form.




A+W Software GmbH      EN-CONFIG-A+W Enterprise Print Service.docx                   60
 No.      Error                                         Description

 212      CouldNotAdjustVlslapParameter                 #441607
                                                        In the case that a vlslap
                                                        report has a datetime
                                                        parameter instead of a
                                                        date parameter, but the
                                                        parameter list could not
                                                        be adjusted, this status is
                                                        set.



       11.2.5.      Status 250 – 299: Crystal Reports error

 No.     Error                                               Description

 250     CrError                                             General       Crystal
                                                             Reports error

 251     CrLoadError                                         Error when loading
                                                             the report

 252     CrDbConnect                                         Error in the database
                                                             connection

 253     CrExportError                                       Error during export,
                                                             not yet used

 254     CrPrintError                                        Error during printing

 255     CrExportOptionsError                                Export options are
                                                             incorrect and cannot
                                                             be processed.

 256     CrDataSourceError                                   Error with       data
                                                             source.

 257     CrParameterTypeError                                The data type of the
                                                             transferred
                                                             parameter is not OK.
                                                             Another data type is
                                                             expected.



A+W Software GmbH      EN-CONFIG-A+W Enterprise Print Service.docx                    61
 No.     Error                                                Description

 258     CrLoadReportError                                    Error when creating
                                                              the report object
                                                              with LoadReport()

 259     CrAssignParameterError                               Error        during
                                                              assignment of the
                                                              report parameters

 260     CrPrinterInReportError                               Error    occurs    if
                                                              problems occur with
                                                              the selected printer
                                                              within the report.
                                                              Previously      only
                                                              happened with CR
                                                              Runtime 2013.

 261     CrAccessedReportValueWasNullError                    Error during attempt
                                                              to determine a
                                                              ReportDocument
                                                              value. Value was
                                                              zero.



       11.2.6.      Status 300 – 349: incorrect mailparam data

 No.      Error                                 Description

 300      MailparamDataError                    General data         error,   cause
                                                unknown.

 301      NoMailServerError                     No mail server was defined

 302      NoSenderAdressError                   The sender's address (From) is
                                                missing

 303      NoReceiveAdressError                  No recipient address was
                                                specified. At least one To, CC or
                                                BCC address must be specified

 304      FromAdressWrongError                  The From address is not correct



A+W Software GmbH      EN-CONFIG-A+W Enterprise Print Service.docx                    62
 No.      Error                                 Description

 305      ToAdressWrongError                    The To address is not correct

 306      CCAdressWrongError                    The CC address is not correct

 307      BccAdressWrongError                   The BCC address is not correct

 308      MailtextFileWrongError                The file that should include the e-
                                                mail text does not exist.

 309      ToAdress2WrongError                   The mailto2 address is not correct

 310      NoMailparamDataFoundError             In the mailparam table, there is no
                                                data.

 311      AttDispTypeWrongError                 The             value               in
                                                mailparam.attdisptype has an
                                                incorrect value. Valid are 0, 1, 2.

 312      NoMailSubjectFoundError               No     subject   was      found.
                                                mailparam.mailsubject is empty.

 313      DBErrorWhileFetchMailparam            Database error when retrieving
                                                the mailparam data.

 314      MailparamDifferenceRowCount           Different number of mailparam
                                                and printparam records.

 315      MailparamMultiAttachment              An e-mail with several print job
                                                sequence numbers attached could
          DispTypeSequenceError
                                                not be sent because a processing
                                                of a sequence number was
                                                incorrect.



       11.2.7.      Status 350 – 399: incorrect printfiles data

 No.      Error                                 Description

 350      PrintfilesDataError                   General data         error,   cause
                                                unknown.




A+W Software GmbH      EN-CONFIG-A+W Enterprise Print Service.docx                       63
 No.      Error                                 Description

 351      FileDoesNotExist                      The file printfiles.filename does
                                                not exist.

 352      CouldNotCopyFileToServe               The file could not be copied to
          r                                     the server.

 353      CouldNotFoundMailparamD               There are no appropriate e-mail
          ata                                   addresses    in   the     table
                                                mailparam.

 354      CouldNotSendEmailToCust               Mail to the mailto address could
          omer                                  not be sent.

 355      CouldNotSendEmailToStaf               Mail to the mailto2 address
          f                                     could not be sent.

 356      CouldNotDeleteTemporaryPrin           The temporary files on the
          tfiles                                server could not be deleted.

 357      CouldNotCreateTemporaryFile           The directory for the temporary
          Directory                             files could not be created.
                                                (Starting with 6.4)

 358      FileEinvoicingMissing                 E-invoice files could not be
                                                found.

 359      CouldNotRetrieveEinvoicingA           E-invoice archive name could
          rchiveFilename                        not be determined.

 360      CouldNotRetrieveEinvoicingS           E-invoice send type could not be
          endingType                            drawn from mp table.

 361      CouldNotRetrieveCollectiveI           The     collective       invoice
          nvoiceSubnumbers                      subnumbers could        not be
                                                determined.

 362      FileCouldNotBeEmbedded                Additional file could not be
                                                added to the PDF.

 363      CsvFileCouldNotBeGenerated            The Excel (CSV) file creation
                                                encountered an error.




A+W Software GmbH      EN-CONFIG-A+W Enterprise Print Service.docx                  64
        11.2.8.         Status 400 – 449: error in the archive process

  No.         Error                                        Description

  400         ArchiveError                                 General data         error,    cause
                                                           unknown.

  401         CouldNotFindSourceFile                       Source PDF file not available

  402         ArchiveFilenameIsEmpty                       No name for the archive file was
                                                           specified

  403         CouldNotCreateArchiveCopy                    No copy for the archive could be
                                                           created

  404         NoIndexparamDataFound                        Despite configuration, there is
                                                           no data in the table indexparam

  405         CouldNotCreateIndexFile                      No index file could be created.

  406         CouldNotCreateAdditionalFil                  No archive file copy could be
              eArchiveCopy                                 created.

  407         CouldNotRenameEmbeddedFileF                  The embedded file in a PDF could
              romPdf                                       not be renamed.



11.3.           Configuration instructions
        11.3.1.         Temporary status list
Here stati can be entered, which under some circumstances no longer occur at a later point in
time and it is therefore worthwhile if the print job will be processed again at a later point in time.
A typical example is the status 152 – PrinterNotExistError. If the printer in question is not
currently available, e.g. due to network problems, this can be remedied at a later point in time,
frequently after just a few seconds.
As separator in the config-Feld, the Comma is expected if more than one status should be defined
as temp. Status.


11.4.           Logs / Tracing



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                           65
12. Print Service – Maintenance --ToDo--
12.1.       Motivation and goals of this development
AWDesk case: #404613


12.2.       Special terms

12.3.       Limitations, delimitation, validity

12.4.   Installation/configuration, environment
  variables


12.5.       Functional description
      12.5.1.       Master Data




A+W Software GmbH      EN-CONFIG-A+W Enterprise Print Service.docx   66
13. Troubleshooting
Here, known errors are document in order to prevent or reduce more research.


13.1.           Exception: net_io_connectionclosed
This error was discussed in the following cases: #430249 and #460026.
With an attempt to send e-mails to an e-mail address outside the internal network, there a
"net_io_connectionclosed" exception can occur. The following error message it output
accordingly in the Print Service log:
"SendErrorMail() Could not send E-Mail because
- Albwir.Basis.Exceptions.AWException: Error sending E-mail: Fehler beim Senden von Mail. --->
System.Net.Mail.SmtpException: Error sending e-mail. ---> System.IO.IOException: No data could be
read from the transmission connection: net_io_connectionclosed.“
A similar error message should also appear with the "Send Test Mail" call in the A+W Enterprise 6 Print
Service Config Tool.




Troubleshooting:
This error is with the customer's IT. Either a firewall is blocking the sending of the e-mail or the
server has not yet released the required port for communication. Note from David Gorr from case
#430249: "Add Server to RelayPerIP Connector in Exchange Server."




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                           67
13.2.           Resetting print job
If you want to re-print a print job at the customer's or for test purposes, but this print job is no
longer listed on the form printing or on the e-mail printing dialog since it was already printed
once. Then the repform.drflag can be set to 0. This way, you re-enable the print job and it appears
on the list again.


13.3.           Print job is not processed by the print service
[AW-164307] minara.95 Print job does not print


Print jobs that get stuck in the tables printtransfer or printparam, whose users are connected to
the correct printer, the printer also executes other print jobs and have statusflag=1, may have
been sent by a site/client whose printer is inactive.

Example Scholl – client 95:




Two print jobs are stuck in the print queue with statusflag=1. Printtransfer.hausnr states that
these print jobs are running via the client/site 50. This site 50 was inactive in the config tool.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                            68
Consult the customer to select another client/site for the print job or to set the printer to active if
the customer gives the OK for this.




13.4.                    Printer not found after printer driver updating
With a Project Facts Ticket [AW-145316] it was reported that the Print Service 6 can no longer
reach a printer. The customer has updated the printer used from a V3 type to a V4 type driver.
The following trace line was reported by the Print Service or the Crystal Report Engine:
023-06-12 09:40:38.819 | [6112] | [0x0000000D] | DEBUG | AWEPrintService                               | HOFFMANNGLAS\awservices-pe |    |
322332-1 | "OutputPrint() print logic " | " " | " " |
2023-06-12 09:40:38.819 | [6112] | [0x0000000D] | DEBUG | AWEPrintService                               | HOFFMANNGLAS\awservices-pe |       |
322332-1 | "PrintOutputControllerIntern() Start " | " " | " " |
2023-06-12 09:40:38.850 | [6112] | [0x0000000D] | ERROR | AWEPrintService           | HOFFMANNGLAS\awservices-pe |
| 322332-1 | "PrintOutputControllerIntern() TargetInvocationException occured: System.Runtime.InteropServices.COMException
(0x80000201):
Invalid printer specified.
cr_ho_ab 6112_21344_{C500BBCE-66A3-4BDF-982F-49CD0D3BA06D}.rpt
 for CrystalDecisions.ReportAppServer.Controllers.PrintOutputControllerClass.ModifyPrinterName(String newVal) " | " " | " " |
2023-06-12 09:40:38.850 | [6112] | [0x0000000D] | DEBUG | AWEPrintService                               | HOFFMANNGLAS\awservices-pe |       |
322332-1 | "ExamineInnerException() Start " | " " | " " |
2023-06-12 09:40:38.850 | [6112] | [0x0000000D] | ERROR | AWEPrintService                              | HOFFMANNGLAS\awservices-pe |    |
322332-1 | "ExamineInnerException() COMException detected " | " " | " " |
2023-06-12 09:40:38.850 | [6112] | [0x0000000D] | ERROR | AWEPrintService                              | HOFFMANNGLAS\awservices-pe |    |
322332-1 | "ExamineInnerException() Undefined COM Exception " | " " | " " |



And the following is generated in the ErrorAnalysis text file:
Error Analysis for print job 322332
----------------------------------------------------------------------------------------------------


seqnr = 1 --> statusflag = 250 (CrError)
----------------------------------------------------------------------------------------------------
Reason:
- General 'crystal runtime' error.
- This error status occurs when the problem has not yet occurred or was not expected to occur.
General Information:
- This error occurs when a Crystal Reports Runtime function is called.




A roll-back to the previous V3 type driver can eliminate the problem, but it makes no sense.
At the customer's, it has helped to open the individual Crystal Reports with the designer and to
check the "No printer" printer option under "File > Set up page".




A+W Software GmbH                             EN-CONFIG-A+W Enterprise Print Service.docx                                                69
A+W Software GmbH   EN-CONFIG-A+W Enterprise Print Service.docx   70
14. Report content
14.1.           AWP SubReports (#334410)
Crystal Reports generally supports the possibility of linking data from different databases within a
report. This was not previously considered in the print service, you could specify precisely one data
source.
For the application case that in a report, data from an ERP database should be linked to data from
a production database, an appropriate adjustment was made. Via the Print Service Config Tool, you
can specify for an ERP database configuration – also for internal sites – an additional Informix data
source consisting of ODBC name, database, user, and password.




Within a Crystal Report, the data of the second data source must be selected via so-called
subreports. These subreports must begin with the prefix "AWPSUB." For the AWPSUB subreports,
the print service exchanges the data source for the additional data source. All other database
objects are assigned the configured ERP data source.
For the use of reports with several data sources, it is not possible to prevent that data is loaded for
which the current user has no rights.


14.2.           Crystal Report Stored Procedures
For the standard Crystal Reports that are delivered via the Setup Launcher, some stored
procedures are required.



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                           71
For the initial set-up, you can obtain the most current stored procedures under
\\jupiter\ALCIB_Service\ALCIB-
AWE\Druck_Fax_Mail\Crystal_Reports\Albat_Wirsam_Standardreports.
The stored procedures are provided with date folder if there have been updates.


14.3.           Problems with ReportDocument content
With the replacement of the old Crystal Report Engine 2008 and the accompanying conversion to
the new CR engine, there were more crashes when processing the ReportDocument. Individual
elements on the ReportDocument are interpreted as NULL values. Since the engine was installed
with the reflection method, we cannot check these values in advance and there are NULL
exceptions right away.
With ticket [AW-213821] a solution was implemented so that the crashes were stopped and the
ReportDocument is re-loaded into the memory. Thus, the printing on the spot takes somewhat
longer, but it is executed successfully and the print job does not get stuck with an error status.


14.4.           Sketch display suppression (e.g. A+W Design)
The sketch display in the Crystal Report templates has a suppression check, so that really only the
A+W Design sketch is displayed in the muntin report.
Example:




With the introduction of the new A+W Design functionalities with QR 25/03, we have had
problems with customer reports that introduced expanded suppression formulas.
     if {cr_aw_rep_items_5.v_sprosym} = 0 // 0 is a-symetric
    then true
    else
       IF mid({cr_aw_rep_items_5.imagedrkz},3,1) <> '1' THEN true ELSE false
The case was treated under ticket [AW-224931].



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                         72
If you have problems with the display of sketches on reports, please check all formulas of the
subreports. And also check that the Suppress checkbox is checked.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                         73
15. Crystal Report Engine
15.1.           Discontinuation of CR engine 2008
With the Quality Release in March 2024, the Crystal Report Engine up to version 13.0.35 was
made usable. With this expansion, the outdated Crystal Report Engine 2008 no longer supported
by SAP is terminated. The Print Service now draws the Crystal Report Engine automatically and
thus needs no setting via the Config Tool.
With a version update, attention must be paid that the customer is not working with the old
Crystal Report Engine 2008. Before the update, for customers who are using the old engine, a
newer engine must be installed and tested properly.


15.2.           Logging/ Tracing
There is a possibility to log the processing of the Crystal Re.ort Engine. This is done with the
crlogger. The versions SAP Crystal Reports 2013, 2016, and 2020 and SAP Crystal Reports,
Developer for Visual Studio (all versions) are supported.
To activate the crLogger, the following Windows user environment variables must be set for the
user under whom the print service is running:
    LOGGING_DIR = path for Log files
    LOGGING_ENABLED_ASSERT = 1
    LOGGING_ENABLED_RUNTIME = 100




After setting the environment variables, the print service must be restarted.
The log files are stored in the LOGGING_DIR.




Note:



A+W Software GmbH             EN-CONFIG-A+W Enterprise Print Service.docx                          74
This functionality should only be switched on to search for errors. If the error has been
reproduced, the logging should be switched off again since it can compromise the performance
and generate very large log files.
To switch off, the environment variables can be removed or changed as follows:
      LOGGING_ENABLED_ASSERT = 0
      LOGGING_ENABLED_RUNTIME = 0
Source: https://userapps.support.sap.com/sap/support/knowledge/en/1603398


15.3.           Troubleshooting
        15.3.1.    Slow processing of the print service/Crystal Report
            engine
It can happen that the print service takes a very long time for particular print jobs that are
processed via the Crystal Report engine. This behavior was already checked under ticket [AW-
56208].
One case is that print jobs with PDF printing should be sent to the printer from the Crystal Report
engine. Here there are repeated queries of the Crystal Report engine to the printer. This looks as
follows in the log:
2020-11-03 11:48:13.949 | [18672] | [0x00000003] | DEBUG | AWEPrintService            |
SCHOLLGLAS\awadmin |                  |    | "OnElapsed() Timer elapsed. threadIsRunning =
True " | " " | " " |
A familiar problem with the Crystal Report engine is that it searches for updates on the Internet
during processing and if on the computer where it is installed there is no Internet access, the
engine goes in a circle, log error screen above.
So that this does not happen, the setting of a particular registry switch can help:
1. Open the Microsoft Windows Registry Editor (cmd > regedit)
2. Navigate to the following product:
        o   Crystal Reports 2008: \HKEY_LOCAL_MACHINE\SOFTWARE\Business Objects\Suite
            12.0\Crystal Reports
        o   Crystal Reports 2011: \HKEY_LOCAL_MACHINE\SOFTWARE\SAP
            BusinessObjects\Suite XI 4.0\Crystal Reports
        o   Crystal Reports 2013: \HKEY_LOCAL_MACHINE\SOFTWARE\SAP
            BusinessObjects\Suite XI 4.0\Crystal Reports

Note: if the product is installed on a 64-bit version of Microsoft Windows, the path is different
since the 32-bit software registry key is here: Wow6432Node. For example, for Crystal Reports
2011, HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\SAP BusinessObjects\Suite XI
4.0\Crystal Reports

3. saves a new "string value": DisableCheckForUpdates

4. Sets the value DisableCheckForUpdate to 1



A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                            75
https://answers.sap.com/questions/12106701/how-to-disable-internet-connection-from-sap-
crysta.html


        15.3.2.    Error in the Crystal Report engine during PDF
            creation
In the ticket [AW-120719], the following error was reported:
2022-09-06 11:33:36.358 | [20544] | [0x0000000C] | DEBUG | AWEPrintService            |
HOFFMANNGLAS\awservices-be |              | 126609-1 | "ExportToDisk() Export report to disk -
From now on in CR Runtime " | " " | " " |
2022-09-06 11:33:40.265 | [20544] | [0x0000000C] | ERROR | AWEPrintService       |
HOFFMANNGLAS\awservices-be |             | 126609-1 | "ExportToDisk()
TargetInvocationException occured: System.NullReferenceException: Der Objektverweis wurde
nicht auf eine Objektinstanz festgelegt.
  for
CrystalDecisions.ReportSource.EromReportSourceBase.ExportToStream(ExportRequestContext
reqContext)
  for
CrystalDecisions.CrystalReports.Engine.FormatEngine.ExportToStream(ExportRequestContext
reqContext)
  for CrystalDecisions.CrystalReports.Engine.FormatEngine.Export(ExportRequestContext
reqContext)
 for CrystalDecisions.CrystalReports.Engine.ReportDocument.Export(ExportOptions options) "
|""|""|


This error occurred during direct PDF export, no external tool such as the Foxit Reader is in
between. Print output was e-mail or pure PDF export.
After a longer search without success, we looked at the incorrect report again and experimented
with different settings in the Page menu element (File > Set up page). The lower figure reflects
approximately the previous settings at the customer's. There, we noticed the edge distance,
which seemed very unusual to us. We have set the edge distance for pixels to 100 everywhere
and after that, the report went through.
A suspicion is that the too-large edge took up the space of an image and that the report creation
was cancelled accordingly.
Similarly, you should watch out which printer you specify for the printer options. In the best case,
do not select a printer and let the report do the formatting work.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                          76
        15.3.3.         General Crystal Engine error (error code 250)
When working through print jobs in the A+W Enterprise Print Service, there were general Crystal
Reports errors with the error code 250. This error occurs in the Crystal Report Engine. You can get
additional information via the print service log.
In our case, we suspect that the simultaneous connection of two print services to one printer
blocked a print service print job. The same error situation could occur for network printers and
connection failures.
Therefore, we recommend using the Print Service Config Tool for the Print Services to include the
error code 250 in the temporary error list; increasing the maximum number of attempts, as well
as the time between attempts; as well as the time between them so that print jobs with this error
code can be executed again.




A+W Software GmbH            EN-CONFIG-A+W Enterprise Print Service.docx                           77
A+W Software GmbH   EN-CONFIG-A+W Enterprise Print Service.docx   78

