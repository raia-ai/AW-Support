---
description: "EN INST A+W Enterprise B2B Service"
---



# EN INST A+W Enterprise B2B Service

          Installa�on Instruc�ons

          A+W Enterprise 6 B2B Service

   Change history:

    Date           Edited by               Remarks                                              Version
    2016-04-22     MP                      New crea�on                                          1.0
    2016-09-29     SVH                     Addi�on                                              1.1
    2016-12-13     MP                      AutoUpdate                                           1.2
    2017-05-04     MP                      Mul� database conﬁgura�on                            1.3
    2017-05-10     SVH                     Conﬁgura�on of openTRANS export
    2018-06-06     SVH                     Conﬁgura�on Hornbach export / Mail dispatch
    2020-05-12     SVH                     Conﬁgura�on A+W EDI Export (AWDesk #422752)
    2023-09-01     SVH                     Maintenance Se�ngs
    2024-06-25     SVH                     [AW-111997] – e-invoicing




     The installa�on instruc�ons will assist the planner with the installa�on and conﬁgura�on
     process for the so�ware named. Please proceed in the following sequence:



     1.      Check the installa�on requirements.

     2.      Compile the required data, addi�onal programs, drivers, etc.

     3.      Note or determine the �me required.




07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                         1
Content

   1         Installa�on of A+W Enterprise 6 B2B Service ................................... 3
   1.1       Overview and the basics ...................................................................................................... 3

   1.2       Time requirement ................................................................................................................ 3

   1.2.1     Installa�on �me for the so�ware ........................................................................................ 3

   1.3       Requirements....................................................................................................................... 4

   1.3.1     Windows Server Version ...................................................................................................... 4

   1.3.2     Network ............................................................................................................................... 4

   1.3.3     So�ware ............................................................................................................................... 4

   1.4       Procedure............................................................................................................................. 4

   1.5       Incompa�bili�es ................................................................................................................ 21

   1.6       Directory structure............................................................................................................. 21

   1.7       Result of the installa�on .................................................................................................... 21

   1.8       Conﬁgura�on ..................................................................................................................... 21

   1.9       Tips and tricks .................................................................................................................... 21

   1.9.1     AutoUpdate........................................................................................................................ 21

   1.9.2     Known errors and workarounds ........................................................................................ 21

   1.10      Uninstalling ........................................................................................................................ 21




07.03.2025                                   EN-INST-A+W Enterprise B2B Service.docx                                                                2
1 Installa�on of A+W Enterprise 6 B2B Service
The following installa�on instruc�ons assume that there is no previous version installed.
An update of an earlier release version of the A+W Enterprise 6 B2B Service is executed precisely like
a new installa�on.
An update of an earlier version of the B2B Service, e.g. from ALCIB 2011 B2B Service to A+W
Enterprise 6 B2B Service is not possible. Only one version of the B2B Service should be installed.
This document describes only the installa�on and conﬁgura�on of the A+W Enterprise 6 B2B
Service. In case of ques�ons about the installa�on or conﬁgura�on of dependent set-ups/disk sets,
please see the installa�on instruc�ons for these products.

1.1 Overview and the basics
The following list provides and overview of the work that must be done during installa�on:
    -   Installa�on and conﬁgura�on of the Informix driver via setnet32.exe
    -   Crea�on of the necessary set-ups/disk sets
             o     A+W Enterprise 6 B2B Service
             o     A+W Infrastructure 6 Collector Services
             o     A+W Infrastructure 6 Middleware
             o     Java 7 Update 51
             o     A+W Setup Launcher
    -   Installa�on of the B2B Service and the dependent disk sets with the Setup Launcher
    -   Conﬁgura�on of the B2B Service with the ConﬁgTool

1.2 Time requirement
If all requirements are checked and fulﬁlled, the following �mes are required for the installa�on and
the conversion of the exis�ng data:

1.2.1   Installa�on �me for the so�ware
Depending on the computer, storage space, and conﬁgura�on, the installa�on �mes will vary for
diﬀerent computers. The installa�on �me speciﬁed was determined using a reference device with
the following characteris�cs:
    -   Processor: 3000 Mhz
    -   RAM: 4 GB
    -   Other: /
For an ini�al or new installa�on, an installa�on �me of 5 minutes must be an�cipated for the
reference device. For higher or lower-power hardware, shorter or longer installa�on �mes must be
an�cipated.



07.03.2025                          EN-INST-A+W Enterprise B2B Service.docx                              3
1.3 Requirements
1.3.1   Windows Server Version
Supported opera�ng systems:



    •   Windows 2008 Server R2 32/64bit.
    •   Windows 2012 Server R2 32/64bit.


1.3.2   Network
For the installa�on itself, no network access is necessary.
For the opera�on of the service, there must be a connec�on to the A+W Enterprise DB Server and
the company network.

1.3.3   So�ware
It is assumed that the following disk sets were already installed and conﬁgured BEFORE the
installa�on of the A+W Enterprise 6 B2B Service disk set.



    •   Informix Client SDK 3.5 TC9 (or newer)
    •   Microso� .NET Framework 4.5.1 SDK

For the opera�on of the A+W Enterprise 6 B2B Service, access to an installed A+W ERP Web Service
6 is required. This must absolutely e installed on the same computer as the B2B Service.



    •   A+W ERP Web Service 6



1.4 Procedure
For the installa�on, please proceed in the following sequence:

        1. Use setnet32.exe to conﬁgure the database server and hosts. This assumes that an IBM
           Informix Client SDK was installed (see so�ware requirements).

        2. Installa�on of the A+W Enterprise 6 B2B Service with the Setup Launcher

    On the Component Selection dialog on the A+W Enterprise node, select the "A+W Enterprise 6
    B2B Service" module. This automa�cally selects all dependent set-ups.




07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                          4
     3.          A�er the successful installa�on, the B2B Service is conﬁgured with the Conﬁg Tool.

          3.1.      Common Se�ngs




07.03.2025                            EN-INST-A+W Enterprise B2B Service.docx                         5
        3.1.1.   Polling Interval

                 In the Polling Interval (Seconds) ﬁeld, the number of seconds is set that the service
                 waits un�l it checks the ottransfer transfer table again for new data records. The
                 default value is 60 seconds.

        3.1.2.   Internal Invoice/Dispatch Transfer

                 If this checkbox is ac�ve, the B2B Service processes otransfer entries with interface
                 = „INVOIC“ or „DELIVE“. (Logic of internal calcula�on, crea�on of INVOICE- and
                 DISPATCHNOTIFICATION documents in AW extended openTRANS format)

        3.1.3.   Dorma Orders

                 If this checkbox is ac�ve, the B2B service processes otransfer entries with interface
                 = „INVOIC“ (Dorma P.O.)

        3.1.4.   openTRANS Document Export

                 If this checkbox is ac�ve, the B2B Service processes the otransfer entries with =
                 „OTDOC“ (user-speciﬁc export of openTRANS documents)



07.03.2025                          EN-INST-A+W Enterprise B2B Service.docx                              6
        3.1.5.   A+W EDI Export (P.O. export)

                 If this checkbox is ac�ve, the B2B Service processes otransfer entries with interface
                 = „EDIEXP“ (A+W standard export)

        3.1.6.   Export of E-Invoice

                 If this checkbox is ac�ve, the B2B Service processes otransfer entries with interface
                 = „E-INV“ (export of electronic invoices)




        3.1.7.   Protocol-Buton

                 With the Protocol buton, you can reach the Protocol Conﬁgura�on dialog. This
                 automa�cally selects all dependent set-ups. On the ﬁrst tab, the trace categories for
                 the frontend are conﬁgured; on the following tabs, the tracing of dependent
                 modules and programs can be ac�vated if necessary.




07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                                7
             The following trace levels are dis�nguished:

             o   Fatal
             o   Error
             o   Warning
             o   Info
             o   Debug

             With the Protocol buton, you can reach the Protocol Conﬁgura�on dialog. If, for
             example, the Info level is ac�ve, trace messages of the type Error and Warning will also
             be writen into the tracing ﬁle.

             The tracing ﬁle is always in the directory %ProgramData%\A+W\Log. The ﬁle name
             consists of the service name, the current date and the process number and ends with
             .awtrc.

             The A+W Enterprise B2B Service currently uses no log protocol.


07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                               8
    3.2. ERP Webservice Se�ngs

        This dialog only opens if at least one of the Internal Invoice/Dispatch Transfer or Dorma
        Orders checkboxes were ac�vated in the Common Settings.




        3.2.1.   ERP Web Service URL

        3.2.2.   Export Path

                 Enter the Root path in which the exported openTRANS xml ﬁles are saved.

                 The internal logic completes the directory <site number> and <customer number> in
                 the path speciﬁed here.

                 The exported ﬁle is saved with the name: openTRANS_<process type>_<site
                 number>_<customer number>_<process number>_<process sub-number>.xml

                 Example:

                 The ﬁle export path „D:\openTRANS“ is entered in the Conﬁg tool.



07.03.2025                       EN-INST-A+W Enterprise B2B Service.docx                             9
                 The created openTRANS invoice ﬁle of invoice 776655 for customer 1234 in site 10 is
                 saved in:

                 D:\openTRANS\10\1234\openTRANS_INVOICE_10_1234_776655_0.xml

                 If errors occur during crea�on of export ﬁle, the records remains in table otransfer
                 with an error ﬂag. The A+W Enterprise B2B Service currently uses no log protocol.

                 If for some reason the ﬁle genera�on for a transac�on is started again even though
                 a ﬁle has already been generated, the exis�ng ﬁle is overwriten by the newly-
                 generated one.




    3.3. Cantor Export – openTRANS 2.1 Se�ngs

        This dialog only opens if the openTRANS Document Export checkbox was ac�vated in the
        Common Settings.




        3.3.1.   Ac�ve


07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                          10
                 The checkbox enables the export.



        3.3.2.   Export Root Path

                 Enter here the basic path in which the export ﬁles are saved. Below this basic path
                 the B2B Service automa�cally creates sub-directories for site numbers and customer
                 numbers in which the export ﬁles are saved.




    3.4. Hornbach export – openTRANS 2.1 se�ngs

        This dialog only opens if the openTRANS Document Export checkbox was ac�vated in the
        Common Settings.




07.03.2025                          EN-INST-A+W Enterprise B2B Service.docx                       11
        3.4.1.   Ac�ve

                 The checkbox enables the export.



        3.4.2.   Export Root Path

                 Enter here the basic path in which the export ﬁles are saved. Below this basic path
                 the B2B Service automa�cally creates sub-directories for site numbers and customer
                 numbers in which the export ﬁles are saved.



    3.5. A+W EDI Export Se�ngs

        This dialog only opens if the A+W EDI Export checkbox was ac�vated in the Common
        Settings.




        3.5.1.   Ac�ve



07.03.2025                          EN-INST-A+W Enterprise B2B Service.docx                       12
                 The checkbox enables the export.



        3.5.2.   Export Root Path

                 Enter here the basic path in which the export ﬁles are saved. Below this basic path
                 the B2B Service automa�cally creates sub-directories for site numbers and supplier
                 numbers in which the export ﬁles are saved.

                 This conﬁgura�on can be overridden by a supplier-speciﬁc conﬁgura�on in A+W
                 Enterprise. For a detailed descrip�on of overriding, see the conﬁgura�on document
                 "A+W Enterprise EDI."

    3.6. E-Invoice Export Se�ngs

        This dialog only opens if the E-Invoice Export checkbox was ac�vated in the Common
        Settings.




        3.6.1.   Ac�ve

                 The checkbox enables the export.


07.03.2025                          EN-INST-A+W Enterprise B2B Service.docx                       13
        3.6.2.   Export Root Path

                 Enter here the basic path in which the export ﬁles are saved.
                 The path is only used, if the export ﬁles were generated manually. For a detailed
                 descrip�on, see the B2B Service conﬁgura�on instruc�ons.



    3.7. Database se�ngs

        On this dialog, all database-precise se�ngs are conﬁgured, star�ng with the database itself.




             o   With the New buton, you can edit an exis�ng conﬁgura�on.
             o   With the Edit buton, you can delete an exis�ng conﬁgura�on.
             o   With the Copy buton, you can copy an exis�ng conﬁgura�on.
             o   With the Delete buton, you can delete an exis�ng conﬁgura�on.




07.03.2025                          EN-INST-A+W Enterprise B2B Service.docx                            14
07.03.2025   EN-INST-A+W Enterprise B2B Service.docx   15
        3.7.1.   With the New or Edit butons or with a double-click on a row in the table, you reach
                 the Site Proper�es dialog. Here, all database-dependent se�ngs can be made.




        3.7.2.   Database se�ngs
             o   The database server is entered in the Server Name ﬁeld. Via the combo box, all DB
                 servers entered in the setnet32 can be selected.
             o   If the ﬁelds Server Name, User Name, and Password are ﬁlled with valid values, the
                 Database Name combo box already contains all available database names of the
                 database server.
             o   The appropriate locale se�ngs are entered in the Client Locale and DB Locale ﬁelds.
                 The combo boxes already contain most values used. If it is necessary to enter
                 devia�ng values, this is also possible manually.

        3.7.3.   DB Func�ons

07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                          16
             o   With the Start Setnet32 buton, it is possible to start the setnet32.exe program
                 directly; with it, database server/hosts can be set up.
             o   With Check Alenv you can check the A+W Enterprise environment variables for this
                 service and view the current database conﬁgura�on. Since this dialog is only for
                 checking purposes, it will not be described in any more detail. The se�ngs of the
                 Alenv variables are made in A+W Enterprise.
             o   The Test Connection buton allows you to check the current values of the database
                 conﬁgura�on. If a database connec�on can be established with this values, you will
                 see the following message box; otherwise an error message.




07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                             17
    3.8. Maintenance Se�ngs




On the Maintenance Settings dialog, it is conﬁgured when successfully processed transfer records
from the archive table and incorrect records from the transfer table are deleted.

    o   Clean Up Time Success (Days): number of days a�er which successfully processed records
        are deleted from the table otransferok.

    o   Clean Up Time Error (Days):     number of days a�er which records that encountered an
        error are deleted from the table otransfer.




07.03.2025                      EN-INST-A+W Enterprise B2B Service.docx                        18
    3.9. E-Mail Se�ngs




        Use dialog E-Mail Settings to conﬁgure whether and to which recipients the error messages
        can be sent via email.

             o   SMTP Server: The name of the SMTP server
             o   Port:           (op�onal) devia�ng SMTP port
             o   From:           Email address of the sender
             o   To:             Email address of the recipient. Several recipient addresses
                                 can be speciﬁed separated by semicolons.
             o   CC:             Email address of the CC recipient. Several recipient addresses
                                 can be speciﬁed separated by semicolons.
             o   Encoding:       Coding of E-mail. Default: u�-8.
             o   Enable SSL:     Ac�vate SSL encryp�on (Y/N)


             o   Authen�ca�on: Ac�vate authen�ca�on (Y/N)
                          Account:                  Domain account for the authen�ca�on
                          Password:                 Password


07.03.2025                            EN-INST-A+W Enterprise B2B Service.docx                     19
                       Conﬁrm password:         Conﬁrma�on of the password




    3.10.       Service conﬁgura�on




        The service users are stored on the Windows Service Conﬁguration dialog. These are
        Windows users who are used to access external objects such as network paths, etc. This
        user must have the appropriate rights.

        With the Pick user... buton it is possible to select a domain user.

        If no network domain is available, e.g. because the service was installed on a PC, the value
        "." can be entered in ﬁeld Domain.

        If no user is available, the service can also run under "LocalSystem" in case of emergency.
        This is the default services user in a Windows system.




07.03.2025                        EN-INST-A+W Enterprise B2B Service.docx                          20
        4. Now the A+W Enterprise 6 B2B Service is ready and it writes a log into the directory
           named above.

        5. Se�ng of A+W Enterprise environment variables.



1.5 Incompa�bili�es
        No incompa�bili�es are known.

1.6 Directory structure


1.7 Result of the installa�on
If the service could be started, the installa�on was successful. Otherwise, the trace log is available
for determining possible problems.

1.8 Conﬁgura�on
For addi�onal conﬁgura�ons, please see the B2B Service documenta�on.

1.9 Tips and tricks
1.9.1   AutoUpdate

        In order to be able to install the service via AutoUpdate, the setup must have been
        installed successfully at least once with the Setup Launcher and conﬁgured with the
        ConﬁgTool.

1.9.2   Known errors and workarounds

        -

1.10 Uninstalling
You can uninstall the program as usual via Control Panel -> Programs and Func�ons.




07.03.2025                         EN-INST-A+W Enterprise B2B Service.docx                               21
Note: The conﬁg ﬁle is not deleted automa�cally. For a ﬁnal uninstalla�on, the program directory of
the A+W Enterprise B2B Service must be deleted manually.




07.03.2025                       EN-INST-A+W Enterprise B2B Service.docx                              22

