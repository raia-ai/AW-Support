---
title: "AUW_Description_VBS_VB_Scripts_AWP"
source: "AUW_Description_VBS_VB_Scripts_AWP.docx"
tags: ["VBS", "VB.NET", "C#", "Crystal Reports", "ALCIMServer", "ALCIMBooking", "Detailed Scheduling", "Job Release", "Database", "A+W Production"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document describes how to implement and execute VBS, VB, and C# scripts in the A+W Production environment. It explains parameter passing from lists, reports, Detailed Scheduling, terminals, and server components; shows configuration options; and provides complete, runnable examples. Topics include reading and writing files, database access via ALCIMRUN and ADODB, calling Crystal Reports (including PPS WebService), registry access, tracing, and running scripts from Windows. Reference tables and revision history are included to support deployment and maintenance."
long_description: "This technical guide consolidates all guidance required to create, configure, and run custom scripts inside the A+W Production suite using VBS (VBScript), VB (Visual Basic), and C#.

It begins with a change history and then outlines how scripts are invoked from A+W Production lists and reports. For each integration point, the document specifies the exact calling convention and the parameter values that A+W passes to the script (for example VIEW, SPERRSTATIONPARAM, DBCONNECT, ALCIMWND, ROOTDIR, and SERVERDIR for list-based calls, and a reduced set for reports). Each section is paired with self-contained examples in VBS and VB that demonstrate how to read parameters, present diagnostic dialogs, and return control to the host application.

Subsequent chapters cover scripting from Detailed Scheduling, ALCIMBooking, ALCIMServer, the Production Terminal, and the job release dialog. Where configuration is required (e.g., enabling post-creation scripts or setting additional parameters), the steps and settings are described, alongside language-specific examples in VBS, VB, and, where applicable, C#.

A toolbox section deepens the practical coverage by showing common tasks: creating dialog boxes (MsgBox and InputBox in VBS as well as building custom dialogs), establishing database connections using both the ALCIMRUN helper and raw ADODB objects (with SELECT and UPDATE examples), and reading/writing files in VBS and VB. Reporting scenarios are documented in depth, including how to execute Crystal Reports, how to use the PPS WebService, export format constants, and how to execute reports on SQL Server without storing passwords in scripts. Additional utility patterns demonstrate starting external CMD scripts, reading and writing Windows Registry values, and implementing tracing so that scripts can log their progress and diagnostics.

Throughout, the document preserves clear sectioning with headings for parameter definitions, configuration instructions, and code examples. All code samples are provided as complete procedures or modules that can be copied into your environment. The closing sections emphasize good practices for maintainability, including consistent use of Scriptname/Scriptversion constants, return variables (e.g., IRESULT), and robust error handling and logging.

Collectively, these materials provide a reference and recipe collection for automating A+W Production workflows with scripts across the platform."
---

VBS, VB and CS Scripts in A+W Production
## History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 2015.08 | DLA | Issue | 1.0 |
| 2016.08 | DLA | Set addition parameter + 6.1 | 1.1 |
| 2016.10 | DLA | POSTIGU.VB | 1.2 |
| 2016.11 | DLA | VB Example for AWP Lists | 1.3 |
| 2017.02 | DLA | Deteailed Scheduling | 1.4 |
|  |  |  |  |


## Content

## Scripts from A+W Production lists and reports
Anders als unter ENABLE Skripten wird die Funktion MAIN mit den Übergabeparametern aufgerufen.
In Funktion MAIN muss eine Variable IRESULT definiert werden, ob diese ausgewertet wird ist unklar. Ist die Variable nicht definiert, kommt es zu einer Meldung.
Globale Konstanten SCRIPTNAME und SCRIPTVERSION müssen definiert werden, Inhalt egal. Sind diese nicht definiert kommt es zu einer Meldung.
### Parameter value for lists
Es werden 6 Parametern übergeben:
- Parameter 1 = VIEW
- Parameter 2 = SPERRSTATIONPARAM
- Parameter 3 = DBCONNECT, ODBC connect string
- Parameter 4 = ALCIMWND, ALCIM window ID
- Parameter 5 = ROOTDIR
- Parameter 6 = SERVERDIR
#### VBS Example
```vbscript
Option Explicit 
Const Scriptname = "TestListen.VBS"
Const Scriptversion = "1.0"

Sub Main (VIEW, SPERRSTATIONPARAM, DBCONNECT, ALCIMWND, ROOTDIR, SERVERDIR)
  MsgBox "VIEW=" + VIEW, 0, Scriptname
  MsgBox "SPERRSTATIONPARAM=" + SPERRSTATIONPARAM, 0, Scriptname
  MsgBox "DBCONNECT=" + DBCONNECT, 0, Scriptname
  MsgBox "ALCIMWND=" + ALCIMWND, 0, Scriptname
  MsgBox "ROOTDIR=" + ROOTDIR, 0, Scriptname
  MsgBox "SERVERDIR=" + SERVERDIR, 0, Scriptname
End Sub
```
#### VB Example
Aufruf erfolgt über die SUB oder FUNCTION Main.
```vb
Imports System
Imports System.IO
Imports Microsoft.VisualBasic

Module AWScript_TestListen
    Sub Main(VIEW As String, SPERRSTATIONPARAM As String, DBCONNECT As String, 
ALCIMWND As String, ROOTDIR As String, SERVERDIR As String)
       MsgBox("SPERRSTATIONPARAM=" & SPERRSTATIONPARAM)
	MsgBox("DBCONNECT=" & DBCONNECT)
	MsgBox("ALCIMWND=" & ALCIMWND)
       MsgBox("ROOTDIR=" & ROOTDIR)
       MsgBox("SERVERDIR=" & SERVERDIR)
    End Sub
End Module
```
### Parameter value for reports
Es werden 3 Parametern übergeben:
- Parameter 1 = DBCONNECT, ODBC connect string
- Parameter 2 = ROOTDIR
- Parameter 3 = SERVERDIR
#### VBS Example
```vbscript
Option Explicit 
Const Scriptname = "TestBerichte.VBS"
Const Scriptversion = "1.0"

Sub Main (DBCONNECT, ROOTDIR, SERVERDIR)
  MsgBox "DBCONNECT=" + DBCONNECT, 0, Scriptname
  MsgBox "ROOTDIR=" + ROOTDIR, 0, Scriptname
  MsgBox "SERVERDIR=" + SERVERDIR, 0, Scriptname
End Sub
```
#### VB Example
Aufruf erfolgt über die SUB oder FUNCTION Main.
```vb
Imports System
Imports System.IO
Imports Microsoft.VisualBasic

Module AWScript_TestBerichte
    Sub Main(DBCONNECT As String, ROOTDIR As String, SERVERDIR As String)
        MsgBox("DBCONNECT=" & DBCONNECT)
        MsgBox("ROOTDIR=" & ROOTDIR)
        MsgBox("SERVERDIR=" & SERVERDIR)
    End Sub
End Module
```
### Set additional Parameter
Will man weitere Parameter an das Skript übergeben, dann können diese in der Befehlszeile für den Skriptaufruf in der Konfiguration mit gegeben werden.
#### VBS Example
```vbscript
$SERVERDIR$\scripts\TestBerichte.VBS MyParam1=abc
```
…
```vbscript
Sub Main (MyParam1, DBCONNECT, ROOTDIR, SERVERDIR)
  MsgBox "MyParam1=" + MyParam1, 0, Scriptname

```
…
#### VB Example
```vb
$SERVERDIR$\scripts\TestBerichte.VB MyParam1=abc
```
…
```vb
Module AWScript_TestBerichte
    Sub Main(MyParam1 As String, DBCONNECT As String, ROOTDIR As String, 
SERVERDIR As String)
        MsgBox("MyParam1=" & MyParam1)
```
…
```vb

$SERVERDIR$\scripts\TestBerichte.VB MyParam1=123
```
…
```vb
Module AWScript_TestBerichte
    Sub Main(MyParam1 As Integer, DBCONNECT As String, ROOTDIR As String, 
SERVERDIR As String)
        MsgBox("MyParam1=" & MyParam1)
```
…
## Scripts from Detailed Scheduling
Beim Start der Feinplanung wird ein VORFEIN Skript und beim Speichern der Feinplanung ein SAVE Skript aufgerufen.
### Parameter value for lists
VORFEIN:
- Parameter 1 = Lauf
SAVE:
- Parameter 1 = Lauf
- Parameter 1 = ReleasePath
### VBS Example
```vbscript
VORFEIN:
Option Explicit 
Const Scriptname = "Vorfein.VBS"
Sub Main (Lauf)
	MsgBox "Batch " & Lauf, 0, Scriptname
End Sub

```
SAVE:
```vbscript
Option Explicit 
Const Scriptname = "Save.VBS"
Sub Main (Lauf, ReleasePath)
	MsgBox "Batch " & Lauf & " - ReleasePath=" & ReleasePath, 0, Scriptname
End Sub
```
### VB Example
```vb
VORFEIN:
Imports System
Imports System.IO
Imports Microsoft.VisualBasic

Module AWScript_Vorfein
Sub Main(Lauf As Int32)
		MsgBox("Batch=" & Lauf, 0, "Vorfein.VB")
End Sub
End Module

SAVE:
Imports System
Imports System.IO
Imports Microsoft.VisualBasic
Module AWScript_Save
Sub Main(Lauf As Int32, ReleasePath As String)	                        
		MsgBox("Batch=" & Lauf & " - ReleasePath=" & ReleasePath, 0, "Save.VB")
End Sub
End Module
```
### C# Example
VORFEIN:
```csharp
using System;
using System.Windows.Forms;
```
class AWScript
```csharp
{
static public void Main(int lauf)
{
MessageBox.Show("Batch=" + lauf.ToString(), "Vorfein.CS");
}
}

```
SAVE:
```csharp
using System;
using System.Windows.Forms;
```
class AWScript
```csharp
{
static public void Main(int lauf , string ReleasePath)
{
MessageBox.Show("Batch=" + lauf.ToString()+ " - ReleasePath=" + ReleasePath, "Vorfein.CS");
}
}
```
## Scripts from ALCIMBooking
Nach jeder Buchung kann ein Skript aufgerufen werden. Dazu muss neben dem Namen des Skripts auch das aufrufende Programm definiert werden, z.B. WSCRIPT.

Wird diese Funktion aktiviert, führt der Buchungsdienst dieses Skript für alle gebuchten Datensätze (AWBAR_BOOKING.STATUS = 1) aus. Nach erfolgreicher Ausführung wird der Status auf 2 gesetzt.
Damit nicht für alte Buchungen das Skript ausgeführt wird, muss vor Aktivierung des Skripts der STATUS von 1 auf 2 gesetzt werden: UPDATE awbar_booking SET status=2 WHERE status=1;

Dieses Skript bekommt alle Felder der Buchung aus der Tabelle ALCIM_BOOKING übergeben. Es wird beim Skriptaufruf keine Funktion aufgerufen, somit wird keine Funktion MAIN benötigt.
### Configuration

[ALCIMBOOK / POSTPROCESSSCRIPT] = WSCRIPT
[ALCIMBOOK / POSTPROCESSEXEC] = //B $SERVERDIR$\SCRIPTS\ALCIMBOOK.VBS
//B  verhindert im WSCRIPT die Ausgabe von Systemmeldungen, dies ist wichtig da das Skript im Hintergrund durch ein Dienst aufgerufen wird. Wird dies nicht angegeben, dann bleiben die WSCRIPT Prozesse hängen und warten auf eine Benutzereingabe.

ALCIMBook erzeugt hierzu folgenden Aufruf:
WSCRIPT \\localhost\Trans\Scripts\ALCIMBOOK.VBS station=“AW“ sequence=“4711“ timeregister=“30.05.2015 15:47:22“ …

Sollten auf einem 64-Bit OS 32-Bit Funktionen im Skript nötig sein, z.B. für Datenbankzugriffe oder eine 32-Bit ALCIM COM Objekt laden, dann muss die 32-Bit Version von WSCRIPT verwendet werden: C:\Windows\SysWOW64\wscript
### VBS example
```vbscript
Option Explicit 
Const Scriptname = "TestALCIMBook.VBS"
Const Scriptversion = "1.0"
Dim iResult

' Define variables for parameter of ACLIMBook
Dim station, sequence, timeregister, priority, info, status
Dim errorinfo, errordata,order, item, subitem, part
Dim unitbc, rackbc,regptbc, statusbc, staffbc, boxbc, materialbc, batchbc, quantity
Dim timeinsert, timesys, timebooking, lot_number, lot_type, lot_job, scannerid
Dim timeref, edited, chargeinfo, processlist, counter, eval_station, eval_process,
Dim ignoreuntil, bruchmodus, processinfo, buildintobc, errorregpt, kundennr, lieferort
Dim statuszeit, farbe_rgb, tisch_id, bruch_text 

' Set variables with parameter value
station = GetArgumentValue ("station")
sequence = GetArgumentValue ("sequence")
'...

iResult = 0

' Function to get parameter value
Function GetArgumentValue (ArgumentName)
  Dim i, iEqualPos, Argument
  GetArgumentValue = ""
  For i=0 To WScript.Arguments.Count - 1
    Argument=WScript.Arguments.Item(i)
    iEqualPos = InStr(1, Argument, "=", 1)
    If iEqualPos > 0 Then
      If Trim(Left(Argument, iEqualPos - 1)) = Trim(ArgumentName) Then
        GetArgumentValue = Trim( Mid(Argument, iEqualPos + 1 ))	
```
Exit For
End If
End If
```vbscript
  Next  
End Function
```
## Scripts from ALCIMServer
Bei der Archivierung kann ein allgemeines Skript aufgerufen werden. Es wird am Ende der Archivierung eines Auftrags ausgeführt. Dieses Skript darf keine Bildschirmausgaben produzieren, da es im Hintergrund über ein Dienst aufgerufen wird und sonst die Anwendung stehen bleibt.
### Parameter value
Im Skript wird eine Funktion ArchiveOrder aufgerufen, die 4 Übergabeparameter bekommt:
- Parameter 1 = ODBC connect string of production database
- Parameter 2 = ODBC connect string for archive database. This parameter is empty in the case AlcimServer is set-up to delete old records instead of archiving.
- Parameter 3 = batch number (number variable)
- Parameter 3 = order number (number variable)
### Configuration

[ALCIM_ARCHIV / SCRIPT]
### VBS example
```vbscript
Option Explicit 
Const Scriptname = "TestAlcimServer.VBS"
Const Scriptversion = "1.0"

Sub ArchiveOrder (Param1, Param2, Param3, Param4)
    Dim DbConnect, DbConnectArchive, Schedule, Order
    DbConnect = Param1
    DbConnectArchive = Param2
    Schedule = Param3
    Order = Param4
    '... 
End Sub
```
### Obsolete scripts
Der ALCIMServer führt die Skripte ArchiveSchedule.BAS, ArchiveOrder.BAS und SN_Archive.BAS aus, wenn diese vorhanden sind. Die ersten beiden Skripte sind abgekündigt, würden aber noch funktionieren. Für diese gibt es eine entsprechende Funktion im Programm. Für SN_Archive.BAS gibt es noch keine Funktion, diese sollte ab Version 6 zur Verfügung stehen.


## Scripts from A+W Production Terminal
Die in den A+W Production Terminals eingehängten Skripte werden auf dem PPSWebService ausgeführt, dieser muss das Skript über den definierten Pfad erreichen. Im Skript wird die Funktion MAIN mit einem Parameter aufgerufen. Bei dem Parameter handelt es sich um die SPERRSTATION, über die Daten aus der Tabelle SKRIPT_SELEKTION geladen werden können. Welche Daten das A+W Production Terminal in die SKRIPT_SELEKTION schreiben soll, wird Skriptkonfiguration des A+W Production Terminal Dialogs definiert. Nach Ausführung des Skripts werden die Daten wieder aus der SKRIPT_SELEKTION gelöscht.
### VBS example
```vbscript
Konfiguration und Skript welches Daten aus einem A+W Production Terminal Grid in eine Datei schreibt.

Option Explicit 
Const Scriptname = "TestToolTV.VBS"
Const Scriptversion = "1.0"

Function Main (ParamSperrstation)
  Dim FSO, oFile, oDB, sqlCommand
  Set FSO = CreateObject("Scripting.FileSystemObject")
  Set oFile = FSO.OpenTextFile("C:\Temp\TestToolTV.txt", 2, True)
  oFile.WriteLine(ParamSperrstation)

  Set oDB = CreateObject("AlcimRun.AlcimDB")
  sqlCommand = "SELECT wert1, wert2, wert3, wert4, wert5, wert6, wert7 "
  sqlCommand = sqlCommand & " FROM skript_selektion WHERE "  
  sqlCommand = sqlCommand & " sperrstation = '" & ParamSperrstation & "'"

  oDB.SelectExec(sqlCommand)
  While(oDB.SelectFetch())   	
    oFile.WriteLine(oDB.GetString(1))	
    oFile.WriteLine(oDB.GetString(2))
    oFile.WriteLine(oDB.GetString(3))
    oFile.WriteLine(oDB.GetString(4))
    oFile.WriteLine(oDB.GetString(5))
    oFile.WriteLine(oDB.GetString(6))
    oFile.WriteLine(oDB.GetString(7))	
  Wend
  oDB.SelectDone()
  oDB.Done()
  Set oDB = Nothing
  oFile.Close
  Main = 0
End Function

```
ACHTUNG:
```vbscript
Execute Local = True: Das Skript wird auf dem lokalen Rechner ausgeführt. D.h. es müssen alle nötigen Komponenten vorhanden sein, die im Skript verwendet werden (hier nur alcimrun.dll). Die Ausgabe erfolgt ebenfalls im lokalen Verzeichnis. Das Objekt oDB verwendet hier z.B. die Datenbank, die auf dem lokalen Rechner eingestellt ist. Diese könnte von der Datenbank des Web-Services abweichen!

Execute Local = False: Das Skript wird auf dem Rechner aufgerufen, auf dem Der Web-Service läuft. I.d.R. sind hier alle nötigen Komponenten für das Skript vorhanden. Die Ausgabe erfolgt nun auf dem Rechner, auf dem der WebServcie läuft. Bildschirmausgaben sind somit unmöglich.
```
## Scripts from release dialog (ALCIMJobRelease)
Individual scripts can be configured for the Release Dialog. It is possible to activate a script if you e.g. press a button, this is the same technic we have in A+W Production Terminal.
Here it is described how to configure a script run like all other actions with the process manager, this is only possible with VB (or CS) scripts. The easiest way is to configure in the parameters for the Release Dialog a new Simple On/Off Action. The Action has to be one of the RESERVED actions.


In the ReleaseDialog-Designer a new On/Off Checkbox with a link to the action can be defined.


### Parameter value
The script get 3 Parameter:
- Schedule  = batch number
- Params = semicolon separated list of parameter, each parameter has the syntax <ParameterName>=<ParameterValue>. Values can configured in the configuration of the “simple On/Off action”. At the end the parameter Visible is attached. 
If no parameter is configured and the script is running in foreground the Value is: ;Visible=True
- Modulname = <ProcessID>_<Name of Script>

### VB Example
```vb
Imports System
Imports System.IO
Imports Microsoft.VisualBasic
Imports System.Diagnostics

Module AWScript_ReleaseTestScript
    Function Main(Schedule As String, Params As String, Modulname As String) As Integer
        MsgBox("Schedule: " & Schedule, 0, Modulname)
        MsgBox("Params: " & Params, 0, Modulname)
        MsgBox("Param Visible: " & GetVariableFromParams(Params, "Visible"), 0, Modulname)
        Return 0
    End Function

    Function GetVariableFromParams(Params As String, VariableToSearch As String) As Object
        Dim retVal As Object = Nothing
        Dim delimiterStr As String = ",;"
        Dim delimiter() As Char = delimiterStr.ToCharArray()
        Dim pParams() As String = Params.Split(delimiter)
        Dim substring As String
        Dim split() As String
        For Each substring In pParams
            substring = substring.Trim()
            split = substring.Split("=")
            If (2 = split.Length) Then
                split(0) = split(0).Trim()
                ' compare case insensitiv!
                If (0 = String.Compare(VariableToSearch, split(0), True)) Then
                    retVal = split(1).Trim()
```
Exit For
End If
End If
```vb
        Next
        Return retVal
    End Function
End Module
```
### CS Example
```csharp
using System.Windows.Forms;
```
namespace ReleaseTestScript
```csharp
{
```
class AWScript_ReleaseTestScript
```csharp
  {
    static public void Main(string Schedule, string Params, string ModuleName)         
    {			
      MessageBox.Show(string.Format ("Schedule {0}, Params: {1}, ModulName: {2}", Schedule, Params, ModuleName));
    }
  }
}
```
### Execute Script as Report or Table
It is possible to execute a script as a report. If you do so, it is need to configure an existing report file in the report configuration, independent if you want use this report or not. If no existing report is configured, you get a message that report doesn’t exist. The parameter are the same like in a Simple On/Off action, but in variable Params more Information are transferred, e.g. you can transfer a printer selected in release dialog.
To execute a report you get a ComboBox with the Options “Off”, “Screen” and the “Printer” which has a fix value in configuration or in this example will be set with a defined global variable




MsgBox("Params: " & Params, 0, Modulname)

If you want switch only between On and Off without an option “Screen” but want select a special variable e.g. a printer, it is possible to execute the script as a table. In this example the printer variable is transfer to parameter XOPTB_PRINTER:



MsgBox("Params: " & Params, 0, Modulname)
## Scripts from XL_JOBRELEASE.CFG (PostCreationScript)
It is possible to execute a VB script as PostCreationScript for a JobRelease machine driver. In the configuration file the advanced scripting function needs to be enable.

[GENERAL]
UseAdvancedScripting=Y

[XL_ISO_LISEC_0]
OutputFile=LISEC.TRF
OutputFilePattern=LISxxxxy.TRF
WorkingDir=$USER$\Release\ISO\lisec
PostCreationScript==$ROOT$\Release\ISO\PostIGU.VB
### VB Example
```vb
Imports System
Imports System.IO
Imports Microsoft.VisualBasic
Module AWScript_PostIGU
    Sub Main (Job As Integer, Lot As Integer, FileName As String, 
		 WorkingDir As String, Section As String, Machine As String, 
		 FirstLot AS Integer, LastLot As Integer, PS As String)
	MsgBox("Job=" & Job & chr(13) _
	& "Lot=" & Lot & chr(13) _
	& "FileName=" & FileName & chr(13) _
	& "WorkingDir=" & WorkingDir & chr(13) _
	& "Section=" & Section & chr(13) _ 
	& "Machine=" & Machine & chr(13) _
	& "FirstLot=" & FirstLot & chr(13) _
	& "LastLot=" & LastLot & chr(13) _
	& "PS=" & PS, 0, "AWScript_PostIGU")
    End Sub
End Module

```
## Execute scripts direct from Windows
Sometime it is need to execute a script direct from windows without our applications. If you use our applications in the script, the script has to be execute in a 32-bit environment, like our applications.
### VBS Example
```vbscript
VBS scripts can be execute direct in Windows with the application wscript. If you use objects from a 32-Bit application like AlcimRun, execute the 32-bit version of wscript. The execution with wscript executes no function (e.g. main) in the script:
C:\Windows\SysWOW64\wscript Scriptname.vbs

If you want transfer parameter into the script, you can access to the parameter with the Arguments function of wscript.
C:\Windows\SysWOW64\wscript Scriptname.vbs Param1 Param2 Param3

Option Explicit
Dim Arguments, Counter
Arguments = WScript.Arguments.Count
If Arguments < 1 Then
  WScript.Echo "You have enter no arguments."
Else
  WScript.Echo "You have enter " & Arguments & " argument(s)."
  For Counter = 0 To (Arguments - 1)
    WScript.Echo "Argument[" & Counter & "]: " & WScript.Arguments(Counter)
  Next
```
End If
### VB Example
```vb
A VB script can be execute with the Albwir.Alcim.Basis.Awh.exe. To execute a script TestScript.VB with gets one parameter use the following Command:
"%ProgramFiles(x86)%\A+W\Techsoft\ProcessManager\Albwir.Alcim.Basis.Awh.exe" TestScript.VB "Hello World"

```
Here the example syntax of the test script:
```vb
Imports System
Imports Microsoft.VisualBasic
Module AWScript_TestScript 
  Function Main (Param1 As String) As Integer
    MsgBox (Param1)    	
    Return 0
  End Function
End Module

```
Attention:
```vb
VB or CS Scripts execute with AWH or direct in with Albwir.Alcim.Scripting.DLL need a module with a name starts with “AWScript” and need a function “main” which will be execute.

```
## Toolbox
In the toolbox you find some working examples of requirements which we have at customers.
### VBS DialogBox
```vbscript
In VBS gibt es 2 Standard Dialogboxen, MsgBox und InputBox. 
InputBox("Enter a number")  
MsgBox("Helle World!")
```
#### MsgBox
MsgBox(prompt[,buttons][,title][,helpfile,context])

Parameter Description
- prompt - A Required Parameter. A String that is displayed as a message in the dialog box. The maximum length of prompt is approximately 1024 characters. If the message extends to more than a line, then we can separate the lines using a carriage return character (Chr(13)) or a linefeed character (Chr(10)) between each line.
- buttons - An Optional Parameter. A Numeric expression that specifies the type of buttons to display, the icon style to use, the identity of the default button, and the modality of the message box. If left blank, the default value for buttons is 0.
- Title - An Optional Parameter. A String expression displayed in the title bar of the dialog box. If the title is left blank, the application name is placed in the title bar.
- helpfile - An Optional Parameter. A String expression that identifies the Help file to use to provide context-sensitive help for the dialog box.
- context - An Optional Parameter. A Numeric expression that identifies the Help context number assigned by the Help author to the appropriate Help topic. If context is provided, helpfile must also be provided.

The Buttonsparameter can take any of the following values:
- 0 vbOKOnly Displays OK button only.
- 1 vbOKCancel Displays OK and Cancel buttons.
- 2 vbAbortRetryIgnore Displays Abort, Retry, and Ignore buttons.
- 3 vbYesNoCancel Displays Yes, No, and Cancel buttons.
- 4 vbYesNo Displays Yes and No buttons.
- 5 vbRetryCancel Displays Retry and Cancel buttons.
- 16 vbCritical Displays Critical Message icon.
- 32 vbQuestion Displays Warning Query icon.
- 48 vbExclamation Displays Warning Message icon.
- 64 vbInformation Displays Information Message icon.

- 0 vbDefaultButton1 First button is default.
- 256 vbDefaultButton2 Second button is default.
- 512 vbDefaultButton3 Third button is default.
- 768 vbDefaultButton4 Fourth button is default.

- 0 vbApplicationModal Application modal. The current application will not work until the user responds to the message box.
- 4096 vbSystemModal System modal. All applications will not work until the user responds to the message box.

The above values are logically divided into four groups: The first group (0 to 5) indicates the buttons to be displayed in the message box. The second group (16, 32, 48, and 64) describes the style of the icon to be displayed, the third group (0, 256, 512, 768) indicates which button must be the default, and the fourth group (0, 4096) determines the modality of the message box.

Return Values:
- 1 - vbOK - OK was clicked
- 2 - vbCancel - Cancel was clicked
- 3 - vbAbort - Abort was clicked
- 4 - vbRetry - Retry was clicked
- 5 - vbIgnore - Ignore was clicked
- 6 - vbYes - Yes was clicked
- 7 - vbNo - No was clicked
#### InputBox
InputBox(prompt[,title][,default][,xpos][,ypos][,helpfile,context])

Return value for cancel is an empty string.

Parameter Description
- Prompt - A Required Parameter. A String that is displayed as a message in the dialog box. The maximum length of prompt is approximately 1024 characters. If the message extends to more than a line, then we can separate the lines using a carriage return character (Chr(13)) or a linefeed character (Chr(10)) between each line.
- Title - An Optional Parameter. A String expression displayed in the title bar of the dialog box. If the title is left blank, the application name is placed in the title bar.
- Default - An Optional Parameter. A default text in the text box that the user would like to be displayed.
- XPos - An Optional Parameter. The Position of X axis which represents the prompt distance from left side of the screen horizontally. If left blank, the input box is horizontally centered.
- YPos - An Optional Parameter. The Position of Y axis which represents the prompt distance from left side of the screen vertically. If left blank, the input box is vertically centered.
- helpfile - An Optional Parameter. A String expression that identifies the Help file to use to provide context-sensitive Help for the dialog box.
- context - An Optional Parameter. A Numeric expression that identifies the Help context number assigned by the Help author to the appropriate Help topic. If context is provided, helpfile must also be provided.
#### Create your own DialogBox
In VBS selbst gibt es nur die MsgBox, zur Ausgabe von Meldungen und Benutzerabfragen, und die InputBox, zur Eingabe eines Wertes. Einen komplexen Benutzerdialog kann über das InternetExplorer.Application Objekt erstellt werden.

Option Explicit
Dim objIEDialogBox, objShell, szNothing
Dim sValue1, sValue2, sPassword
' Get a reference to IE's Application object
Set objIEDialogBox = CreateObject("InternetExplorer.Application")
objIEDialogBox.Offline = True
objIEDialogBox.navigate "about:blank"

' This loop is required to allow the IE object to finish loading...
Do
WScript.Sleep 100
Loop While objIEDialogBox.Busy

objIEDialogBox.Document.body.Style.FontFamily = "Calibri"

' Inject the HTML code above into the IE object
objIEDialogBox.Document.Body.innerHTML = _
"<p><b><u>Example DialogBox:</u></b></p>" & _
"<p><b>Value 1:</b><br><input name='Value1' size='40' maxlength='512'></p>" & _
"<p><b>Value 2:</b><br><input name='Value2' size='40' maxlength='512'></p>" & _
"<p><b>Password:</b><br><input type=password name='Password' size='40' maxlength='512'></p>" & _
"<button name='OK' Onclick=document.all('ButtonHandler').value='OK';>OK </button>" & _
"<button name='Cancel' Onclick=document.all('ButtonHandler').value='Cancel';>Cancel</button>" &_
"<input name='ButtonHandler' type='hidden' value='Nothing Clicked Yet'>"

' Prevent the MenuBar, StatusBar, AddressBar, and Toolbar
' from being displayed as part of the IE window
objIEDialogBox.MenuBar = False
objIEDialogBox.StatusBar = False
objIEDialogBox.AddressBar = False
objIEDialogBox.Toolbar = False

' Set the initial size of the IE window
objIEDialogBox.height = 300
objIEDialogBox.width = 300

' Set the title of the IE window
objIEDialogBox.document.Title = "Test DialogBox"
objIEDialogBox.Visible = True

' This loop is required to allow the IE window to fully display before moving on
Do
WScript.Sleep 100
Loop While objIEDialogBox.Busy

' This code brings the IE window to the foreground.
Set objShell = CreateObject("WScript.Shell")
objShell.AppActivate objIEDialogBox.document.Title

' Once the dialog is displayed and has been brought to the foreground,
' set focus on a control
objIEDialogBox.Document.All("Value1").Focus

Do
' If the user closes the IE window by Alt+F4 or clicking on the 'X'
' button, we'll detect that here, and exit the script if necessary.
On Error Resume Next
Err.Clear
szNothing = objIEDialogBox.Document.All("ButtonHandler").Value
If Err.Number <> 0 Then Exit Do
On Error Goto 0

' Check to see which buttons have been clicked
Select Case objIEDialogBox.Document.All("ButtonHandler").Value
Case "Cancel" ' The user clicked Cancel. Exit the loop
objIEDialogBox.quit
Exit Do
Case "OK" ' The user clicked OK.
sValue1 = objIEDialogBox.Document.All("Value1").Value
sValue2 = objIEDialogBox.Document.All("Value2").Value
sPassword = objIEDialogBox.Document.All("Password").Value
MsgBox "Here is the information you entered..." & vbcrlf & vbtab & _
"Value1: " & sValue1 & vbcrlf & vbtab & _
"Value1: " & sValue2 & vbcrlf & vbtab & _
"Password: " & sPassword
' Now that we have closed the IE dialog, we can act on our data
objIEDialogBox.quit
Exit Do
End Select

' Wait for user interaction with the dialog...
WScript.Sleep 200
Loop
### Database connection
A database connection can be done with the ALCIMRUN object or with ADODB interface, if no A+W Production is installed.
#### VBS ALCIMRUN example SELECT
```vbscript
Dim oDB, sqlCommand, Wert1, Wert2  
Set oDB = CreateObject("AlcimRun.AlcimDB")
sqlCommand = "SELECT wert1, wert2 FROM Datenbanktabelle ..."
oDB.Init ("DEFAULT")
oDB.SelectExec(sqlCommand)
While(oDB.SelectFetch())   	
  Wert1 = oDB.GetString(1)
  Wert2 = oDB.GetString(2)
Wend
oDB.SelectDone()
oDB.Done()
Set oDB = Nothing
```
#### VBS ALCIMRUN example UPDATE etc.
```vbscript
Dim  oDB, sqlCommand, Wert1, Wert2, RowCount, lResult
Set oDB = CreateObject("AlcimRun.AlcimDB")
sqlCommand = "UPDATE Datenbanktabelle SET wert1='xxxx' AND wert2=5 ..."
oDB.Init ("DEFAULT")

' ANSI LOG
oDB.Transact sqlCommand, Clng(RowCount)

' Buffered LOG
lResult = oDB.TransactBegin (sqlCommand, Clng(RowCount))
oDB.TransactCommit (1)

' !!! RowCount bekommt keinen Rückgabewert aus der Transact Funktion, da dies von 
' VBS nicht unterstützt wird (es sei denn RowCount wäre vom Typ Variant) !!!

oDB.Done()
Set oDB = Nothing
```
#### VBS ADODB example SELECT
```vbscript
Const ConnectString = "DSN=alcimdb; UID=alcimdb; PWD=alcimdb;"
Dim  objConn, objRS, sqlCommand, Wert1, Wert2  
Set objConn = CreateObject("ADODB.Connection")
Set objRS = CreateObject("ADODB.Recordset")
sqlCommand = "SELECT wert1, wert2 FROM DatabaseTable "
objConn.Open ConnectString
objRS.Open sqlCommand, objConn  ' IsolationLevel ist CommittedRead bei INFORMIX
If NOT objRS.EOF Then
```
objRS.MoveFirst
Do until objRS.EOF
```vbscript
    Wert1 = objRS.Fields("wert1").Value
    Wert2 = objRS.Fields("wert2").Value
    objRS.MoveNext
```
Loop
```vbscript
  objRS.Close
```
End If
```vbscript
Set objRS = Nothing
objConn.Close	
Set objConn = Nothing
```
#### VBS ADODB example UPDATE etc.
```vbscript
Const ConnectString = "DSN=alcimdb; UID=alcimdb; PWD=alcimdb;"
Dim  objConn, objCommand, sqlCommand, Wert1, Wert2  
Set objConn = CreateObject("ADODB.Connection")
Set objCommand = CreateObject("ADODB.Command")
sqlCommand = "UPDATE Datenbanktabelle SET wert1='xxxx' AND wert2=5 "
objConn.Open ConnectString
objCommand.ActiveConnection = objConn
objCommand.CommandText = sqlCommand
objCommand.Execute
Set objCommand = Nothing
objConn.Close
Set objConn = Nothing
```
### VBS read and write files
```vbscript
Use the Scripting.FileSystemObject for reading and writing files. This example read a file and write the content in a second file.

Option Explicit
Dim FSO, TextStreamIn, TextStreamOut
Set FSO = CreateObject("Scripting.FileSystemObject")
Set TextStreamIn = FSO.OpenTextFile("C:\Temp\TestFileIn.txt", 1)
Set TextStreamOut = FSO.OpenTextFile("C:\Temp\TestFileOut.txt", 2, True)
Do While Not TextStreamIn.AtEndOfStream  
  TextStreamOut.WriteLine(TextStreamIn.ReadLine)
```
Loop
```vbscript
TextStreamIn.Close
TextStreamOut.Close
  
' FileSystemObject.OpenTextFile(fname,mode,create,format) 
' fname [Required] The name of the file to open 
' mode [Optional] How to open the file
'      1=ForReading - Open a file for reading. You cannot write to this file.
'      2=ForWriting - Open a file for writing.
'      8=ForAppending - Open a file and write to the end of the file.  
' create [Optional] Sets whether a new file can be created if the file does not exist. 
'        True indicates that a new file can be created
'        False indicates that a new file will not be created. False is default 
' format [Optional] The format of the file
'        0=TristateFalse - Open the file as ASCII. This is default.
'        -1=TristateTrue - Open the file as Unicode.
'        -2=TristateUseDefault - Open the file using the system default.
```
### VB read and write files
```vb
Imports System
Imports System.IO

Module AWScript_TestScript
  Sub Main()
    ' Open a new file in %TEMP% directory, exsiting file will be overwritten
    Dim filename As String
    filename = Path.Combine(Path.GetTempPath(), "NewFile.TXT")
    Dim fs As FileStream = New FileStream(filename, FileMode.Create, FileAccess.Write)
    Using sw As StreamWriter = New StreamWriter(fs)
      sw.WriteLine("Hello World!")
```
End Using
```vb
    fs.Close()

    ' Open file again and append 
    fs = New FileStream(filename, FileMode.Append, FileAccess.Write)
    Using sw As StreamWriter = New StreamWriter(fs)
      sw.WriteLine("...more text...")
```
End Using
```vb
    fs.Close()

    ' Open file and read content
    fs = New FileStream(filename, FileMode.Open, FileAccess.Read)
    Using sw As StreamReader = New StreamReader(fs)
      While Not sw.EndOfStream
        MsgBox(sw.ReadLine())
      End While
```
End Using
```vb
    fs.Close()
  End Sub
End Module
```
### Execute Crystal Report
Reports werden über das Objekt ALCIMRUN.ALCIMREPORT2 aufgerufen und können gedruckt, am Bildschirm angezeigt oder Exportiert werden.

Beim Export  wird ein Format angegeben. Die folgende Liste der Formate ist evtl. nicht vollständig und es können evtl. auch nicht alle Formate exportiert werden. Es sollten die Formate Exportiert werden, die man direkt aus dem CrystalReports Vorschaudialog exportieren kann.
Es wird empfohlen einen Textdateiexport (z.B. Kommaseparate Liste) nicht über einen Report zu exportieren, sondern wenn ein Skript aufgerufen wird dann kann das Skript die Datei selbst schreiben.
| crEFTNoFormat = 0 | crEFTCrystalReport = 1 | crEFTDataInterchange = 2 |
| --- | --- | --- |
| crEFTRecordStyle = 3 | crEFTRichText = 4 | crEFTCommaSeparatedValues = 5 |
| crEFTTabSeparatedValues = 6 | crEFTCharSeparatedValues = 7 | crEFTText = 8 |
| crEFTTabSeparatedText = 9 | crEFTPaginatedText = 10 | crEFTLotus123WKS = 11 |
| crEFTLotus123WK1 = 12 | crEFTLotus123WK3 = 13 | crEFTWordForWindows = 14 |
| crEFTExcel21 = 18 | crEFTExcel30 = 19 | crEFTExcel40 = 20 |
| crEFTExcel50 = 21 | crEFTExcel50Tabular = 22 | crEFTODBC = 23 |
| crEFTHTML32Standard = 24 | crEFTExplorer32Extend = 25 | crEFTNetScape20 = 26 |
| crEFTExcel70 = 27 | crEFTExcel70Tabular = 28 | crEFTExcel80 = 29 |
| crEFTExcel80Tabular = 30 | crEFTPortableDocFormat = 31 | crEFTHTML40 = 32 |
| crEFTCrystalReport70 = 33 | crEFTReportDefinition = 34 |  |

#### VBS example
```vbscript
Option Explicit
On Error Resume Next
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' ODBC Connect String 
' Informix und SQLBase: 	DSN=<dsn>; (DATABASE=<database>)
' SQLServer: 	DSN=<dsn>;UID=<benutzername>;PWD=<password>;(DATABASE=<database>)
Const Connect = "DSN=alcimdb;" 
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Dim oRPT, lRet, ReportName
Reportname = "P:\Reports\AUW_Rack_Organisation.rpt"

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' Create Object for Report
Set oRPT = CreateObject("AlcimRun.AlcimReport2")
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' [Optional] Set the Crystal Reports version, if not set the version from AWP DB will be used
' OLD: Version 9,10,11
' lRet = oRPT.SetCrystalVersion (11)
' NEW: 5 = 11NET, 6 = 12NET, 7 = 2016
' lRet = oRPT.SetCrystalVersionEx (6)
' Version ermitteln:
' MsgBox oRPT.GetCrystalVersion()
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' Open the Report
lRet = oRPT.OpenReport(ReportName, 99)
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' Set DSN
lRet = oRPT.LogOnServerEx ("", "alcimdbrep", Connect)
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' [Optional] Set Report Parameter
' lRet = oRPT.SetParameter("Parameter", "Wert")
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' [Optional] Set Printer
' lRet = oRPT.SelectPrinterByName("Drucker")
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' [Optional] Set Report Settings
' oRPT.SupressEmptyPages = 0
' oRPT.KeepReportSettings = 1 ' Aufruf nach dem setzen des Druckers!
' oRPT.Collated = 0 ' Sortierung beim Mehrfachdruck, Standard = 1 = sortieren
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' Report output on screen
lRet = oRPT.OutputToWindow (90)
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' Report output direct to the printer
' lRet = oRPT.OutputToPrinter2(0,1) ' (AskForPrinter, NumberOfCopies)
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' Report Output export in a file
' lRet = oRPT.SetExportFormatType (21)
' lRet = oRPT.SetExportFileName ("C:\public\test.xls")
' lRet = oRPT.Export (0) ' FormatType, 0 = crEFTNoFormat
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
' kill Report object
Set oRPT = Nothing
' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

If Err.Number <> 0 Then
  MsgBox Err.Description
```
End If
#### VB example
```vb
' Example VB.NET-Skript for Executing a Report
' Albwir.Alcim.Basis.AWH.EXE "<script>" "<schedule>" "<parameters>" "<modulename>"
Imports System
Imports System.IO
Imports System.Diagnostics
Imports Microsoft.VisualBasic
Imports Albwir.Basis.Tracing

Module AWScript_Report
  ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
  ' ODBC Connect String 
  ' Informix und SQLBase: 	DSN=<dsn>; (DATABASE=<database>)
  ' SQLServer: 	DSN=<dsn>;UID=<benutzername>;PWD=<password>;(DATABASE=<database>)
  Public Const DBConnect As String = "DSN=alcimdb;"
  ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

  ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
  ' Report name
  Public Const Reportname As String = "P:\Reports\AUW_Rack_Organisation.rpt"
  ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

  Function Main(Schedule As String, Params As String, Modulname As String) As Integer
    Dim Resultcode As Integer = 0 ' 0=Successful    
    Dim oRpt As Object = Nothing ' Interface AlcimRun.AlcimReport2
    Dim traceSwitch As New TraceSwitch("Albwir.Alcim.Scripting", "Tracing for Bsp_Execute_Report_VB.VB")

    Try
      AWTrace.WriteLineIf(TraceLevel.Info, traceSwitch, "Reportname = " & Reportname)
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' create the AlcimReport2-Interface:
      oRpt = CreateObject("AlcimRun.AlcimReport2")
      oRpt.ErrorReset()
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' [Optional] Set the CR version, if not set the version from AWP DB will be used
      ' OLD: Version 9,10,11
      ' Resultcode = oRPT.SetCrystalVersion (11)
      ' NEW: 5 = 11NET, 6 = 12NET, 7 = 2016
      ' Resultcode = oRPT.SetCrystalVersionEx (6)
      ' Version ermitteln:
      ' AWTrace.WriteLineIf(TraceLevel.Info, traceSwitch, "CrystalVersion = " 
      '                     & Convert.ToString(oRPT.GetCrystalVersion()))
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' Open the Report
      Resultcode = oRpt.OpenReport(Reportname, 2)
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' Set DSN
      Resultcode = oRpt.LogOnServerEx("ALL_REPORTS", "ALCIMDBREP", DBConnect)
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' [Optional] Set Report Parameter
      ' Resultcode = oRpt.SetParameter("Parameter", "Wert")
      ' e.g.: Resultcode = oRpt.SetParameter("schedule", Convert.ToInt32(Schedule))
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' [Optional] Set Report Settings
      ' oRPT.SupressEmptyPages = 0
      ' oRPT.KeepReportSettings = 1 ' Aufruf vor dem setzen des Druckers!
      ' oRPT.Collated = 0 ' Sortierung beim Mehrfachdruck, Standard = 1 = sortieren
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' [Optional] Set Printer
      ' Resultcode = oRPT.SelectPrinterByName("Drucker")
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' Report output direct to the printer
      ' Resultcode = oRPT.OutputToPrinter2(0,1) ' (AskForPrinter, NumberOfCopies)
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' Report output on screen
      Resultcode = oRPT.OutputToWindow(90)
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

       ' ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' Report Output export in a file
      ' Resultcode = oRpt.SetExportFormatType(21)
      ' Resultcode = oRpt.SetExportFileName ("C:\public\test.xls")
      ' Resultcode = oRPT.Export (0) ' FormatType, 0 = crEFTNoFormat
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Catch ex As Exception
      Resultcode = -1
      AWTrace.WriteLineIf(TraceLevel.Error, traceSwitch, ex.Message)
    Finally
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
      ' kill Report object
      If (oRpt IsNot Nothing) Then
        System.Runtime.InteropServices.Marshal.ReleaseComObject(oRpt)
```
End If
```vb
      oRpt = Nothing
      ' +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    End Try
    Return Resultcode
  End Function
End Module
```
#### Execute Report with PPSWebService
You can execute a report direct in a browser over PPSWebService with the function Albwir.Alcim.DataService/ViewReport.aspx.
##### VBS example
```vbscript
' Script for execute in ToolTV
Option Explicit 
Const Scriptname = "PPSWebViewReport.VBS"
Const PPSWebViewReport = "http://<ProcessServer>/Albwir.Alcim.DataService/ViewReport.aspx"
Const ReportLink = "\\<FileServer>\trans\Reports\BDE\AUW_OrderList_Status.rpt"
Const ParameterFix = "&Unterteile_anzeigen=1"
Function Main (ParamSperrstation)
  Dim oBrowser, url, ParameterOrder 
  ParameterOrder = InputBox("Order number: ",Scriptname, "700053")
  If ParameterOrder <> "" Then
    If IsNumeric(ParameterOrder) Then
      ParameterOrder = "&Auftrag=" & ParameterOrder    
      url = PPSWebViewReport & "?Report=" & ReportLink & ParameterFix & ParameterOrder
      ' Execute with Shell open web page in standard browser
      Set oBrowser = CreateObject("WScript.Shell")
```
oBrowser.Run url
```vbscript
      ' Execute direct with IE and customize options of IE window
      ' Set oBrowser = CreateObject("InternetExplorer.Application")
      ' Do While (oBrowser.Busy)
      '   Wscript.Sleep 250
      ' Loop
      ' oBrowser.TheaterMode = False
      ' oBrowser.AddressBar = False
      ' oBrowser.MenuBar = False
      ' oBrowser.StatusBar = False
      ' oBrowser.ToolBar = False
      ' oBrowser.Resizable = True
      ' oBrowser.Height = 100
      ' oBrowser.Width = 100
      ' oBrowser.Left = 0
      ' oBrowser.Top = 0
      ' oBrowser.FullScreen = True
      ' oBrowser.Silent = True
      ' oBrowser.Visible = True
      ' oBrowser.Navigate2 url
      Set oBrowser = Nothing
    Else
      MsgBox "ParameterOrder isn't numeric!", 16, Scriptname
```
End If
End If
```vbscript
  Main = 0
End Function
```
##### VB example
```vb
' Script for execute in ToolTV
Imports System
Imports System.Diagnostics
Imports Microsoft.VisualBasic
Module AWScript_PPSWebViewReport
  Const Scriptname As String = "PPSWebViewReport.VB"
  Const PPSWebViewReport As String = "http://<ProcessServer>/Albwir.Alcim.DataService/ViewReport.aspx"
  Const ReportLink As String = "\\<FileServer>\trans\Reports\BDE\AUW_OrderList_Status.rpt"
  Const ParameterFix As String = "&Unterteile_anzeigen=1"
  Function Main(ParamSperrstation As String) As Integer
    Dim url As String = ""
    Dim ParameterOrder As String = ""
    ParameterOrder = InputBox("Order number: ", Scriptname, "700053")
    If ParameterOrder <> "" Then
      If IsNumeric(ParameterOrder) Then
        ParameterOrder = "&Auftrag=" & ParameterOrder
        url = PPSWebViewReport & "?Report=" & ReportLink & ParameterFix & ParameterOrder
        Process.Start(url)
```
End If
End If
```vb
    Return 0
  End Function
End Module
```
### Execute Report on SQLServer without enter a Password in the script
If you execute a report with such a script on a SQLServer database, you have to enter the password for the database user every time you run the report. If you don’t want this, create a SQLServer ODBC database connection with trusted connection (Windows authentication), e.g. data source name alcimdbreptc. Create a report with this connection and it works.
One problem, the windows user who opens the report need the right to connect and read the database. So the use can connect with other tool (e.g. Excel) to the database, some customers don’t want such a security leak.
### VBS Start CMD script
Use the function run from object wscript.shell:
```vbscript
object.Run(strCommand, [intWindowStyle], [bWaitOnReturn]) 

```
intWindowStyle:
0 - Hides the window and activates another window.
```vbscript
1 - Activates and displays a window. If the window is minimized or maximized, the system restores it to its original size and position. An application should specify this flag when displaying the window for the first time.
```
2 - Activates the window and displays it as a minimized window.
3 - Activates the window and displays it as a maximized window.
```vbscript
4 - Displays a window in its most recent size and position. The active window remains active.
```
5 - Activates the window and displays it in its current size and position.
```vbscript
6 - Minimizes the specified window and activates the next top-level window in the Z order.
7 - Displays the window as a minimized window. The active window remains active.
8 - Displays the window in its current state. The active window remains active.
9 - Activates and displays the window. If the window is minimized or maximized, the system restores it to its original size and position. An application should specify this flag when restoring a minimized window.
10 - Sets the show-state based on the state of the program that started the application.

Dim oShell
Set oShell = createobject("WScript.Shell")
oShell.Run "scriptname.cmd", 1, True
```
### VBS Read and write Registry from
```vbscript
Use Interface AlcimRun.AlcimRegistry to get the Information from Registry need for A+W Production.

Option Explicit 
Dim oReg
Set oReg = CreateObject("AlcimRun.AlcimRegistry")
MsgBox "ConnectString: " & oReg.GetConnectString() & Chr(10) & Chr(13) _
     & "StationID: " & oReg.GetStationId() & Chr(10) & Chr(13) _
     & "RootDirectory: " & oReg.GetRootDirectory() & Chr(10) & Chr(13) _
     & "UserDirectory: " & oReg.GetUserDirectory() & Chr(10) & Chr(13) _
     & "ServerDirectory: " & oReg.GetServerDirectory() & Chr(10) & Chr(13) _
     & "ServerVolume: " & oReg.GetServerVolume() & Chr(10) & Chr(13)

```
Read a special Parameter:
```vbscript
MsgBox oReg.RegGetStringEx("HKEY_LOCAL_MACHINE\Software\Albat+Wirsam\Communication", "IceHost","String IceHost not exist")

The Function RegGetLongEx should do the same like RegGetStringEx, but it returns a number value, but this function doesn’t work right. Use the RegGetStringEx Function and convert it with the function Clng() or CInt() into a number.

To Set Parameter in [HKEY_CURRENT_USER\Software\Albat+Wirsam] you can use the following function:
oReg.RegSetCurrentUserString ("TestKey","Parameter1", "Value")
oReg.RegSetCurrentUserLong ("TestKey","Parameter2", 1234)


But to read this value doesn’t work with VBS, because it doesn’t work to give a C++ function a variable which get back the right return value. 
Dim lRet, ReturnValue
lRet = oReg.RegGetCurrentUserString ("TestKey", "Parameter", ReturnValue)

```
You can use the common registry function of VBS to around this problem:
```vbscript
Option Explicit 
Const RegKey = "HKEY_CURRENT_USER\Software\Albat+Wirsam\TestKey\Parameter3"
Dim oShell
Set oShell = CreateObject("WScript.Shell")
oShell.RegWrite RegKey, "Test"
On Error Resume Next
MsgBox oShell.RegRead(RegKey)
If err.number <> 0 Then
  MsgBox "Can't read registry " & RegKey
```
End If
### Tracing in Scripts
Activate Tracing in the configuration of the application which is executing the script. In a VB script the trace will be done with AlcimScripting and is find in .NET trace file (e.g. ALCIM.NET_....AWTRC), in VBS a script the trace is done AlcimShared (e.g. ALCIM_....AWTRC).
#### VBS example
```vbscript

Option Explicit 
' Trace Level 0-6
' 0/1 = Error
' 2 = Warning
' 3/4 = Info
' 5/6 = Debug
Sub Main (DBCONNECT, ROOTDIR, SERVERDIR)
  Dim oTrace, lRet
  Set oTrace = CreateObject ("AlcimTools.Trace")
  lRet = oTrace.SetDebug("TestVBSTrace")
  On Error Resume Next
  lRet = oTrace.Trace(2, "Trace Level Warning")
  lRet = oTrace.Trace(4, "Trace Level Info")
  lRet = oTrace.Trace(6, "Trace Level Debug")
  If Err.number <> 0 then
    lRet = oTrace.Trace(1, "Error code" & Err.Number)
    lRet = oTrace.Trace(1, "Error source: " & Err.Source )
    lRet = oTrace.Trace(1, "Error description: " & Err.Description )
```
End If
```vbscript
  Set oTrace = Nothing
End Sub
```
#### VB example
```vb

Imports System.Diagnostics
Imports Albwir.Basis.Tracing

Module AWScript_TestScript
    Function Main(DBCONNECT As String, ROOTDIR As String, SERVERDIR As String) As Integer
        Dim traceSwitch As TraceSwitch = Nothing
        traceSwitch = New TraceSwitch("Albwir.Alcim.Scripting", "")
        Try
            AWTrace.WriteLineIf(TraceLevel.Warning, traceSwitch, "Trace WARNING")
            AWTrace.WriteLineIf(TraceLevel.Info, traceSwitch, "Trace INFO")
            AWTrace.WriteLineIf(TraceLevel.Verbose, traceSwitch, "Trace VERBOSE")
        Catch ex As Exception
            AWTrace.WriteLineIf(TraceLevel.Error, traceSwitch, ex.Message)
        End Try
        Return 0
    End Function
End Module

```