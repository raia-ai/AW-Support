---
description: "EN CONFIG A+W Enterprise Customizing"
---



# EN CONFIG A+W Enterprise Customizing

         Configuration


Customizing




                                                                     english




   A+W Software GmbH                                         - -INTERNAL-
                       EN-CONFIG-A+W Enterprise Customizing.docx     1
Change history


           Date         Author                Comments                               Version
           2003-09-01 Frauke Ruppert          Initial version includes description of 3.1
                                              the cases: 70269, 32231, 27350, 75678
           2023-01-04 Ina Seifert             Takeover from various individual
                                              documents




Content

1.   Log                                                                                    5
2.   Overview                                                                                6
     2.1. Benefits                                                                           6
     2.2. Drawbacks                                                                          6
     2.3. Contents                                                                           6
3.   Customizing screen                                                                      8
     3.1. Start screen                                                                       8
     3.2. Mode screen                                                                        9
          3.2.1. Anchor                                                                      9
          3.2.2. Execution                                                                  10
     3.3. Customizing actions                                                               12
          3.3.1. SQL                                                                        12
          3.3.2. SPL                                                                        13
          3.3.3. AdhocSQL                                                                   14
     138233: Call of SQL queries from the customizing with parameter transfer               15
          3.3.4. AdhocSQL selo                                                              15
          3.3.5. Shell                                                                      15
          3.3.6. Perform                                                                    16
          3.3.7. Error                                                                      17
          3.3.8. YN-Quest / NY-Quest                                                        17
          3.3.9. Selo                                                                       18
          3.3.10. Formula                                                                   19
          3.3.11. Key                                                                       19
          3.3.12. SqlSelo                                                                   22
          3.3.13. FE-EXEC                                                                   23
          3.3.14. L-MSG / C-MSG / FFLASH                                                    24
     101975: Prompt line / Fill Flash line dynamically                                      24
     3.4. Special customizing action                                                        24
          3.4.1. Accessing higher-priority screens                                          24
          3.4.2. Suppressing system reports                                                 25
          3.4.3. Default answer for JN message                                              25
          3.4.4. Suppress message                                                           26
          3.4.5. Field pre-population                                                       27
          3.4.6. Keyboard customizing                                                       28


A+W Software GmbH           EN-CONFIG-A+W Enterprise Customizing.docx                            2
          3.4.7. Call up own/new dialog                                      28
          3.4.8. Follow-up events                                            29
     3.5. Limits                                                             30
     3.6. Possibilities                                                      30
4.   Set jump marks and hide field contents                                  32
5.   SQL queries                                                             33
     5.1. Definition of a query                                              33
          5.1.1. Dialog titles                                               34
          5.1.2. Selos and lookup fields                                     34
          5.1.3. Dialog tabs / tab                                           35
          5.1.4. Graphic fields on the results dialogs                       35
          5.1.5. Handling of invisible fields                                36
          5.1.6. Tooltip texts for fields                                    36
     5.2. Statements                                                         36
          5.2.1. Substatements                                               37
          5.2.2. Reference to field contents in sub-statements               38
          5.2.3. Jump to the document entry directly from the hit quantity   39
          5.2.4. Detailed example for ADHOC-SQL                              39
          5.2.5. Formatting of sub-statements                                40
     5.3. Hit dialog                                                         41
     5.4. SQL menu                                                           41
     5.5. ADHOC SQL env variables                                            42
6.   Ad hoc SQL tool                                                         44
     6.1. Configuration                                                      44
7.   Print format templates                                                  45
8.   Configurable fields                                                     46
     8.1. Data structures                                                    46
     8.2. Master data maintenance                                            46
     8.3. Fixed sets                                                         48
          8.3.1. Delivery time – Set 2 - kaufprvfld                          48
          8.3.2. Delivery note printing – Set 10 - kaufprvfld                48
9.   Transfer to Excel                                                       49
     9.1. General                                                            49
          9.1.1. Configuration                                               49
     9.2. Process                                                            49
     9.3. Excel Transfer with Template                                       50
     9.4. Example of an Excel Transfer:                                      51
     9.5. Important Information                                              52
     9.6. Adjustment of the "Page Layout" Dialog                             53
10. Individual Programs                                                      54
         10.1.1. Use of subdirectories                                       54
11. Vorgangs_sql                                                             55
12. SPs and shell scripts                                                    56
13. DFUE_Nachbearb                                                           57



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx           3
14. Documentation                                                    58
    Document 18670: Documentation of customizing                     58
15. Table of figures                                                 59




A+W Software GmbH        EN-CONFIG-A+W Enterprise Customizing.docx        4
1. Log
The customizing log can be switched on with system menu (CTRL+F4) – CTRL+K. The level of the
log - support or development - can be selected. The log is written to
$PROTOPFAD/cust<pid><mmdd><hhmm>.
If no log file can be written, there will be an error file in directory /tmp, called cust_err.




A+W Software GmbH           EN-CONFIG-A+W Enterprise Customizing.docx                            5
2. Overview
   2.1.        Benefits
1. Adjustment available directly
2. Adjustment can be developed on-site in cooperation with the customer
3. Customer workflow can be mapped directly
       a. Small adjustments can make a big difference with problems that occur over and over
4. No discussion of the required work if the development is done on-site


   2.2.        Drawbacks
5. Support can be difficult
       a. Sometimes it is not clear that a problem was caused by customizing - detailed docu
          necessary!
       b. For DB triggers, unexpected SQL codes can be reported
6. No standard
       a. Must be checked with version update
       b. Adjustments must be transferred manually


   2.3.        Contents
   ■   Adjustments outside the program code
   ■   No customizing STD functions
   ■   Interfaces in the program necessary
           ‒   Customizing screens
           ‒   Implementation of field attributes (defstyp)
           ‒   Shell scripts/SPs
                   •   Document SQL
                   •   OrderXML – SPs
           ‒   SQL queries with call from
                   •   Start dialog
                   •   Menus
                   •   Value import
   ■   Screen customizing
   ■   Print format templates



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                        6
           ‒   Excel transfer
   ■   Individual programs
   ■   Configurable fields (private fields, config. fields in the master and in the document)
   ■   Configurable texts
   ■   Exception DB triggers
           ‒   Use sooner only as protocol trigger




A+W Software GmbH            EN-CONFIG-A+W Enterprise Customizing.docx                          7
3. Customizing screen
Call of the customizing screen is only possible within a screen and here via the system menu
<Ctrl+F4>=>System Configuration=>Customizing actions. The call is controlled by the environment
switch CUSTOMIZING (ON).
These are event-oriented actions that can be defined for any ALCIB screens and fields. This
happens in that you save the assignments between screen, field, event, and actions in a database
table ('alcust'). When the user edits the screen field in question and the defined event occurs, the
corresponding actions are executed.


    3.1.        Start screen
On the header screen of the start screen, the specification for the screen is entered (with pre-
population of the values for the current screen field) into which the customizing should be
inserted. In addition to the specification of the screen and field names, the variant (in which mode
screen you are) and transaction level (Chap. 3 Limits) are specified.
On the rump screen, the stored customizing actions for the screen field are combined in a
summarized view.




Figure 1-1 Customizing main screen

The rump screen of the start page has a limited number of fields, so that the creation and
maintenance of the customizing actions should be done on the 1st mode screen. This mode
screen will be described below.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                            8
    3.2.           Mode screen




Figure 1-2 Customizing mode screen


        3.2.1.          Anchor
The Anchor area describes, like the header screen, the situation in which the defined customizing
action is called.


        Field name                   Value
        Inactive                     If the field is empty, the customizing is switched on. If there is a 1 in the
                                     field, the customizing action is switched off.
        Condition                    A p or a can be entered in this field.
                                     p means pre-event : the customizing action is called before the regular
                                     event handling
                                     a means after-event : the customizing action is called after the regular
                                     event handling
        Event                        In this field, the triggering event – that is, with which event should the
                                     customizing be done - is specified. If the event specified in the field
                                     defined in the header screen occurs here, the customizing action
                                     defined below is executed. However, only if the field inactive is empty.
                                     The selection for the Event field is made via <F9> (or <A9>) – only
                                     "positive" Eventids and via <F9> (or <A9>), then <F8> (or <A8>) key
                                     sequence – for all Eventids.
                                     The following events are currently supported in customizing:
                                     Field-related events:
                                     TESTFIELD            When leaving a field; not, however for <F12> (or
                                     <A43>) "Field back"
                                     EXPAND When leaving a field; however only if "touched"; a field is
                                     touched if the field content was changed by the user.
                                     ENTERFIELD           When entering a field
                                     RETURN               When pressing <Return>;
                                     START With triggering of <A39> <Start>


A+W Software GmbH            EN-CONFIG-A+W Enterprise Customizing.docx                                          9
                                  ALCIB-KEYS           All available ALCIB function keys
                                  CU_EVENT1-4 These are the events that can be sent by a screen
                                  customizing and to which in the screen field in which they are received
                                  can be reacted => two-level customizing, e.g. after Y/N questions. If Yes,
                                  send CU_EVENT1 and show another warning message; if No, set the
                                  current screen field to NO EXIT. Since there are several events available,
                                  a more-than-two-level customizing is even possible.
                                  In particular, for a screen field sequence, several multi-level
                                  customizings can be defined since the event sequence can be varied
                                  (1,2 ; 3,4 ; 4,1 ; etc.). This is very helpful, for example for the header of
                                  the KAUF screen since there are only a few screen field sequences there
                                  that allow a multi-level customizing.
                                  MSG_EVENT            Default answer for JN messages
                                  Screen-related events:
                                  FETCHED              When retrieving the data
                                  START With triggering of <A39> (or <Start>)
                                  LEAVEOBJECT          When leaving the screen
                                  ENTEROBJECT When entering the screen
                                  LEAVERECORD When leaving the current tuple on multi-record
                                  screens
                                  ENTERRECORD When entering the current tuple on multi-record
                                  screens
                                  DELETE               <A7> This way it is possible to react to deletion actions
                                  with the help of customizing and possibly to avoid inadvertently
                                  triggered deletion.
        Variant                   Here it is stored on which (mode) screens the customizing is active. -1
                                  means that is valid for all variants.
Example
The event DELETE in connection with the action ERROR and the entry L_STAY in the field !-0
causes <A7> to have no effect. This can also be commented with a message stored in the error
text field.
With the actions YN-QUEST and NY-QUEST it is also possible to provide the deletion with security
queries.


        3.2.2.          Execution
The "Execution" area describes a customizing action. Meanwhile, the "Customizing" tool offers a
whole lot of possibilities for realizing customer-specific requests. This complexity is reflected in
the structure of the Execution area. It is possible to change to different script languages, to add
screens, to define field properties, re-control screen behavior, manipulate value specifications,
etc.
Before we discuss individual customizing possibilities in more detail, the individual fields of the
Execution area will be described briefly below


      Field name                Value
      action                    Here you can store which action should be executed after the triggering
                                event. The following actions are available:
                                SQL                         Execute SQL statement
                                SPL                         Execute Stored Procedure (SP)


A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                                     10
                      AdhocSQL                    Starts an existing Adhoc-SQL
                      Shell                       Execute shell script
                      Perform                     Screen call
                      Error                       Trigger error case
                      YN-Quest                    Field-related user query
                      NY-Quest                    Field-related user query
                      Key                         Key sequences can be recorded by the
                      system and played back.
                      Selo                          The standard selo for a field can be
                                                    exchanged or a selo can be added to a field.
                      Formula                      Field value check/calculation
                      SqlSelo Dynamic selo from the Adhoc SQL
                      FE-EXEC                      Front end execute (start Windows programs)
                      L-MSG                        Output message on the 38th line
                      C-MSG                        Delete message on the 38th line
                      FFLASH                      Message on the 38th line until keypress
    Statement         In this field, statements can be stored depending on the action (action
                      field). If, for example, SQL was selected in action, there is a SQL
                      instruction in the Statement field.
    Error text        If the specified action (combined from action and statement)
                      encounters an error, the specified error text is output in this field.
    Settings          Here a field can be specified that the setting affects, which is specified
                      in the fields successaction and erroraction.
                      If you let a value be determined with the action, then the value is
                      transferred into the specified field.
    SUCCESSACTION     If the specified action delivers a zero value (=0), then the specified
                      settings are triggered.
                      The following settings are available:
                      SET_FIELD_REQUIRED            the current field is assigned a mandatory
                      input
                      SET_FIELD_NO_REQUIRED                  Mandatory input cancelled
                      SET_NO_EXIT                   The cursor lands again in the field from which
                      the customizing was started. Depending on the triggering event and the
                      action type, it is possible to make it so that a field can only be corrected
                      or exited forwards.
                      SET_VALUE           a field value already initialized can be overwritten
                      SET_DEFAULT_VALUE             Set default value
                      SET_FIELD_VERIFY                       The current field is assigned a
                      repeated input
                      SET_FIELD_NO_JUMP                      The current field is assigned a jump
                      end mark
                      SET_FIELD_JUMP Cancel existing jump end mark
                      SET_FIELD_UPPERCASE The current field is entered in upper-case
                      letters.
                      SET_FIELD_NO_UPPERCASE                 Cancel existing property UPPERCASE
                      SET_FIELD_NO_DELIMITER                 The current field includes no field
                      delimiters ("[...]" or "deeper"        font)
                      SET_FIELD_DELIMITER           Display field delimiters
                      SET_FIELD_INVISIBLE                    The field content of the current field
                      is hidden
                      SET_FIELD_VISIBLE             Make invisible field visible
                      SET_FIELD_NOMOD                        The current field is locked for
                      changes
                      SET_FIELD_MOD Make non-changeable field changeable



A+W Software GmbH   EN-CONFIG-A+W Enterprise Customizing.docx                                     11
                                 SEND_EVENT                  In case of success or error, the specified event
                                 is sent to actionevent
                                 SEND_EVENT_NO_EXIT                   In case of success or error, the
                                 specified event is sent to actionevent and stops on the current field
                                 SET_FIELD_DBMUST                     The current field contains the
                                 property          DBMUST. The specified value has to be present in the
                                 database table. DBMUST must only be used in connection with a selo.
                                 MSG_ANSWER_J                With this, the answer to the event
                                           MSG_EVENT is given
                                 MSG_ANSWER_N                         With this, the answer to the event
                                           MSG_EVENT is given

      ERRORACTION                If the specified action delivers a value that is not equal to zero (!=0),
                                 then the specified settings are triggered
      Actionevent                If the setting SEND_EVENT was selected in the fields
                                 SUCCESSACTION/ERRORACTION, it is specified in this field which event
                                 should be sent.
      Prompt    : Ctrl-U         Here, a text for a prompt message for the event "721 CUSTMENU" can
                                 be stored. The prompt is only displayed for the CUSTMENU event.


    3.3.        Customizing actions
Different types of actions are supported in the ALCIB customizing tool. This chapter will explain
the individual actions and provide application examples. Even if the individual actions are
discussed in more detail here, it is not possible to depict the complexity that the event-oriented
customizing covers. The use of the customizing tool assumes that you are familiar with ALCIB and
FIX and have extensive database knowledge.
All customizing scripts are in the CUST area (that is, $ALCIBPRG/cust). The customizing program
seeks here for the function or script call entered in the "Statement" field.


        3.3.1.             SQL
If the action "SQL" is selected, a SQL instruction has to be inserted in the field statement. In the
where clause, it is possible to reference screen fields. The result of the select is written to the
screen field that is in the "Settings" field or the return value or this action is intercepted in a
subsequent one.
In the example displayed below, the selected value (SUCCESSACTION=131072) is written to the
field KAUF_PRIVATE_LONG2 in case of success. In case of error, the message "An error has
occurred. Please contact support" is output.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                                      12
Figure 2-3 Example of a SQL action


        3.3.2.           SPL
With the stored procedure, the customizing behaves in a similar manner as with a SQL action. IN
the Action field, "SPL" is selected with the toggle, and the call of the saved function with transfer
values is written in the Statement field. The parameters refer to the screen fields. The SPL action
always expects the return of a value. To be noted is that error code evaluates the SC value and
not the return value of the stored procedure.
Useful trick: if a return value is needed, which cannot be procured with 'simple' SQL (e.g. due to
required IF branching), this problem can be solved by a SQL of the type
SELECT cu_sql_sp(#MaskenFeldInhalt1, ...) FROM alsysinfo
(the table alsysinfo always has precisely one line!)
The source code for the stored procedure has to be in the CUST area (that is, $ALCIBPRG/cust).




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                             13
Figure 2-4 Example of an SPL action

The return value of a stored procedure and the result of a select instruction can be evaluated in
another customizing action. With the action "Message" and through specification %s as format
string (same formatting possibilities as a string for the c-function printf) in the Statement field,
the return value is displayed in a dialog box.




Figure 2-5 Evaluation of a SQL return value in a formatted message


        3.3.3.           AdhocSQL
The tool AdhocSQL can be called in customizing. After selecting "AdhocSQL" in the action field,
the group number is specified as first value in the statement and separated with a space, the
value for the SQL query. If parameters are specified in the AdhocSQL, these can also be specified
with field reference. Sample statement: "2 201 #KAUF.KAUF_AUFTRNR|#KAUF.KAUF_KUNR"
would give the statement 2/201 the values from the fields KAUF_AUFTRNR and KAUF_KUNR from
the KAUF screen. The field references are composed of "#<Screenname>.<Fieldname>" (see
screen reference).




Figure 2-6 Example of an AdhocSQL action



A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                               14
138233: Call of SQL queries from the customizing with parameter transfer

In the customizing, it is now possible to call SQL queries with parameter transfer. Here, as
usual with the action "AdhocSQL" group both the ID and the SQLs to be called are
transferred. After the input of the ID, separated by the pipe character, parameters can be
transferred according to the question mark and $ variables in SQL.
If the user has decided for a parameter transfer, a value must be specified for each ? in the
corresponding SQL. Here it is possible, as usual in customizing, to specify field
references.
Example:
The customizing with action "AdhocSQL" and statement "10 12
#MITARB_MANR|#MITARB_HNR" in the employee master data calls the SQL of group
10 and ID 12 with the employee number and client number on the screen. The associated
select in the Adhocsql looks like this:
select auftrnr, vorgang, subnr, eusr, hausnr from kauf where eusr=? and hausnr=?;




        3.3.4.           AdhocSQL selo
horizontal
The logic "Adhocsql as selo" enables the dynamic addition of a selo to any field via adhocsql.
The action has to be created with action "SQLSelo". The additional parameters work analogously
to the ADHOCSQL action.
The Adhocsql screen now behaves like a selo. Only the first two columns are displayed, it is
positioned under the field and when return is pressed on a line, the value is taken over into the
original field. A value takeover is only possible if the data type of the first column of the
ADHOCSQL and the data type of the field match.


        3.3.5.           Shell
From the customizing, it is possible to call shell scripts. These shell scripts have to be stored in the
directory ./spec/cmd (cdscmd).
Return values of shell scripts cannot be evaluated, neither "calculated" values nor error codes




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                               15
Figure 2-7 Example of a shell action


         3.3.6.           Perform
With the action "Perform," customer-specific ALCIB screens can be added. The created mfo files
have to be stored in the directory cust/mfo. The call of the generate file in the customizing screen
is done with a relative path specification.




Figure 2-8 Example of a perform action

The entry in the field "Prompt         :Ctrl-U" is displayed in the lower area of the window as
information for the user.
When the keys <Ctrl+U> are pressed, the screen cu_versand opens.




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                         16
Figure 2-9 Prompt display for <Ctrl+U>


        3.3.7.            Error
An error case can be forced to trigger (e.g. to output a message or to essentially change the field
attribution).
In the example depicted, an error case is generated with <F3> (<START>) (Event: 324) and the
message "No problem!" is output.




Figure 2-10 Customizing action with an error message


        3.3.8.            YN-Quest / NY-Quest
Field-related, a defined YN message can be activated, which, for example, changes the default
behavior.
The difference between YN-Quest/NY-Quest is that in one case "yes" and in the other "no" is
specified as the default.
A particularity of this example is that the value "#ALL#" is in the "Feldname" field. This means that
this customizing action affects all fields of the screen.
The value 2 in Success Action means that in case of success, the screen is not exited.




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                          17
Figure 2-11 NY-Quest action


        3.3.9.            Selo
Additional selos can be added to screens. Selos are frequently used on customized screens. Since
here the screen is self-created, there are no selos on the fields. With this action type, it is possible
to add a selo. If for this you select the setting "SET_FIELD_DBMUST" in the Success Action field,
the request is fulfilled that the value has to come from the table - the selo.
Customized selos have to be stored in the directory CUST/sel. The selo is incorporated into the
screen with a relative path specification.




Figure 2-12 Example of a selo action




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                              18
         3.3.10.          Formula
With the action type "Formula," the formula interpreter is incorporated. It is possible to check
field values, calculate field values or store message texts.
An example for calculation of a field value: here, the field value #XXVAR_MAS1 is multiplied by
the field value from #XXVAR_MAS2 and the result is written into the field XXVAR_MAS3. The
specification for "Settings" has to be SET_DEFAULT_VALUE or SET_VALUE for this type of
customizing.
The field content is addressed with #.




Figure 2-13 Example of incorporation of the formula interpreter


         3.3.11.          Key
Here, key sequences and field assignments can be stored or recorded. The events are processed
in the appropriate sequence after triggering. If values should be stored, which are not assigned to
any event, then the field you have just entered is assigned this value (insofar as possible). Events
can be stored manually or automatically (via macrorecorder <CTRL+F9>).
With the customizing key it is not possible to record blank spaces since these are used as a
separator for the recorded keys. For the input of several blank spaces one after another, the
action is interrupted at this point since the keys after this can no longer be found.
The following keys are supported:


      Key                                     Code                Event


      <A38> or <F1>                           A38                 Help

      <A16> or <SHIFT F1>                     A16                 User help




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                          19
    <A18> or <CTRL F1>               A18                Define user help

    <A30> or <F2>                    A30                Mode

    <A80> or <SHIFT F2>              A80                Shift Mode

    <A39> or <F3>                    A39                Start

    <A31> or <SHIFT F3>              A31                Print

    <A1> or <F4>                     A1                 Supplementary menu

    <A51> or <SHIFT F4>              A51                Information menu

    <A21> or <CTRL F4>               A21                System menu

    <A5> or <F5>                     A5                 Detail

    <A55> or <SHIFT F5>              A55                Detail

    <A22> or <CTRL F5>               A22                Sort menu

    <A6> or <F6>                     A6                 Add record

    <A4> or <SHIFT F6>               A4                 Insert record

    <A7> or <F7>                     A7                 Delete record

    <A8> or <F8>                     A8                 First record

    <A19> or <SHIFT F8>              A19                Special 3

    <A60> or <CTRL F8>               A60                Special 1

    <A9> or <F9>                     A9                 Selo

    <A12> or <SHIFT F9>              A12                Extra 4

    <A62> or <CTRL F9>               A62                Extra 1

    <A10> or <F10>                   A10                Last record

    <A13> or <SHIFT F10>             A13                Extra 5

    <A63> or <CTRL F10>              A63                Extra 2




A+W Software GmbH          EN-CONFIG-A+W Enterprise Customizing.docx         20
      <A3> or <F11>                     A3                    Jump key

      <A13> or <SHIFT F11>              A13                   Extra 6

      <A64> or <CTRL F11>               A64                   Extra 3

      <A43> or <A12>                    A43                   Field back

      <A20> or <SHIFT F12>              A20                   Special 4

      <A61> or <CTRL F12>               A61                   Special 2

      <Page Up>                         PU

      <Page Down>                       PD

      CTRL U                            CTRL U

      CURSOR UP                         CU

      CURSOR DOWN                       CD

      RETURN                            RT                    Enter key



The key recorder is deactivated again with <Ctrl+F9>. Normally, the key recorder should always be
used to store the events. If, however, a key is already programmed so that the recording cannot
be done correctly, a manual entry of the appropriate coding is also possible. This is required for
the following keys:


      Key                               Code                  Event

      <A2> or <CTRL F3>                 A2                    Copy field content

      <A34> or <CTRL F6                 A34                   Insert row

      <Backspace>                       BS

      TAB                               TAB

      CURSOR RIGHT                      CR

      CURSOR LEFT                       CL




A+W Software GmbH            EN-CONFIG-A+W Enterprise Customizing.docx                         21
The following keys can be stored neither with the recorder nor manually:


      Key                                 Event

      <A17> or <CTRL F2>                  Previous field content

      <A42> or <SHIFT F7>                 Delete field content

      <A37> or <CTRL F7>                  Delete row



Example: for statement, the following entry has to be made if a customizing screen should be
opened: A21 CD RT CU RT


        3.3.12.          SqlSelo
A selo can be added to a field with SqlSelo. The difference from the selo action is that the selo is
not generated by a selo file, but rather by an AdhocSql. The action can be given three parameters.
Sql group and ID are mandatory. The query parameters are optional. The query parameters fill the
? in the Adhocsql and are specified separated with |. Example: "11 22 9911101|4711" would call
the Adhocsql group 11, ID 22, with the parameters 99111101 and 4711. The generated "selo"
positions itself under the current field.




Figure 2-14 SqlSelo displayed




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                        22
Figure 2-15 SqlSelo as replacement for the employee selo


        3.3.13.          FE-EXEC
The customizing is expanded to include the action FE-EXEC for the incorporation to archiving
systems. With this action, with use of FIXWIN, any Windows applications can be started.
Furthermore, with a field reference, it is possible to pass along data from the screen called up as
program parameters.


Since path specifications for the programs to be called can vary, there is also the possibility to
address alenv variables in the "statement" field. For naming, however, attention should be paid
that they start with CU_.


Example: The new environment variable CU_OFFICEPATH must be defined and activated with the
value "C:\Programme\Microsoft Office\Office". After that, a customizing action FE-EXEC must be
created with the statement "$CU_OFFICEPATH\winword.exe" in the desired place.


Example
In a field in MP master, the geocoordinates should be saved. With a hotkey, it should be possible
to call a browser that displays the associated place in Google Maps.
Shelexec starts the linked application under Windows (http-> browser, docx-> Word, etc.)
As parameter, Maps URL is transferred with the field #MP_BRANCHE as parameter


■       For screen MP and field MP_BRANCHE


A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                             23
■         Trigger-Event
■         721 – CTRL+U
■         Action FE-Exec
■         Statement
■         shelexec http://maps.google.com/maps?z=12&t=h&q=loc:#MP_BRANCHE


          3.3.14.           L-MSG / C-MSG / FFLASH
101975: Prompt line / Fill Flash line dynamically

Customising now allows to expansion of the fields in the 38th line on screen. For this, the ACTION
toggle on the Customizing screen is expanded to include the following versions:
1. L-MSG works analogously to the message version, only that the message is output on the 38th
screen line. This message is only deleted if an empty message is output.
2. C‐MSG With this action, messages that were output with the action L-MSG can be removed.
1. FFLASH works analogously to the message version, only that the message is output on the
38th screen line. This message disappears as soon as the user presses a key.




    3.4.           Special customizing action
          3.4.1.            Accessing higher-priority screens
Customizing can access screens of higher priority (e.g. from the screen `kpos' to `kauf'). The high-
priority screen field is addressed as follows: #Screenname.Fieldname
This does not work however if you want to access screens that have not been called yet, i.e. that
are after the customizing action in the sequence of events (example: from 'kauf' to 'kpos'). You
cannot access screens of higher priority if another menu was loaded in the meantime.
Screen name        SPROPR                      created: 20.10.2003
Field name                  SPROPR_VKPLM
Variant            00
Transactionlevel            01


-------- 1 of 2 -------------------------------------------------------=KPOS


Anchor
Inactive [_]
Condition          P
Event              721


A+W Software GmbH                 EN-CONFIG-A+W Enterprise Customizing.docx                       24
Variant : [-1]
Execution
Action             Formula
Statement          #SPROKL.SPROKL_SPRPKZ=2
Errortext
Settings           ____________________262144                        (returnvalue = 0
Actionevent        850                                      (returnvalue != 0)


-------- 2 of 2 ------------------------------------------------------|
Anchor
Inactive [_]
Condition          P
Event              850
Variant            [__]
Execution
Action             Message
Statement          The price for linear meters in the price list 2 may not be more than 10 €!


           3.4.2.            Suppressing system reports
Within A+W Enterprise, some reports are defined as so-called customized messages. These can be
suppressed via customizing, so that they are no longer presented to the user.

Customizing is done then:

• Determination of message number
  Using the customizing log (help level 3), the report RT_MSG_CU(2, 4711, "message text", ...)
  can be used to determine the message number (here: 4711).
• By customizing the formula for event 855, "§MSGNO=4711" can be used to check whether the
  message event for the customizing message has been triggered.
• To suppress this message, enter "MSG_ANSWER_J" for the SUCCESS action.
• In the following test, the fflash "CUST" should appear in the penultimate line instead of the
  report.


           3.4.3.            Default answer for JN message
It is possible for YN message in customizing to store a default answer. This means that the
question is ALWAYS answered in this way and no longer appears on the screen.




A+W Software GmbH                   EN-CONFIG-A+W Enterprise Customizing.docx                     25
Prerequisite is that the function jn_msg is replaced in the program by the new function
jn_msg_cu, as the new function will send the triggering event 855 (from version 3.1 partially
available in KAUF).




Figure 2-16 By storing a message number, the customizing default answer can be stored

The default answer is defined in the customizing screen by entering "MSG_EVENT“ as the
triggering event 855 and selecting the default answer "MSG_ANSWER_J" or "MSG_ANSWER_N" in
settings "Successaction / Erroraction". In "Statement" you need to enter the allermsg number of
the message to be answered by customizing. The statement creates a logical printout with the
determined number (see Figure 14). Further conditions can be linked to the customizing.
To determine the message number for the yes/no message, you can either search for the
message in file fx_texte, or define the following action in customizing. The triggering event is MSG
event "855"; SQL is selected as an action, and the following SQL instruction is defined as
"Statement": select §MSGNO from alsysinfo.
In a second customizing step, enter 855 again as the triggering event, and select “message” as an
action. For statement, just enter %s. When you trigger customizing now, the message box will
show a message number.
The easiest way of writing an f_test. Adopt the message number and message text from file *.test;
if this details are missing in f_test, the function was not changed.



        3.4.4.           Suppress message
Example
Order: message "Takeover of the FinAc debtor" should not appear
System menu > CTRL + K > SH F12 (Customizing log switched on)
Perform Action
Log cust<mmdd>:




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                         26
21.09.2018 15:04:45: no customizing action is defined for this screen 21.09.2018 15:04:45:
screenname: KAUF
21.09.2018 15:04:45: fieldname: KAUF_AUFTRNR
21.09.2018 15:04:48: message id: 30461 message: XALC16539 - There is a FinAc debtor: 100.
Invoice-relevant data of the FinAc debtgor will be taken over!


Ftest:
Search for event 855 (100855)
15:17:48 U Mask:KAUF          Fld:KAUF_KUNR     ( 12) Event:100855     T:0


CUSTOMIZING
For screen KAUF and field KAUF_KUNR
Trigger-Event
855 – MSG-Event
Action Formula
Statement §MSGNO=30461
= 0 -> MSG_ANSWER_J


         3.4.5.           Field pre-population
Example:
    ■    Pre-population of the abbreviation field in the MA master
    ■    Trigger enter the field
    ■    Only if not filled
    ■    First letter of the first name +
    ■    First letter of the last name
    1. Screen name : MITARB
    2. Field name: MITARB_ZEICHEN
    3. Event: -132 – ENTERFIELD
    4. Action SQL
    5. select substr( #MITARB_MAVNAME , 1, 1) || substr(#MITARB_MANAME, 1,1) from
       alsysinfo;
    6. Error text: "An error occurred during the pre-population of the abbreviation"
    7. =0                 8 – SET_DEFAULT_VALUE




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                     27
        3.4.6.           Keyboard customizing
With the customizing key it is not possible to record blank spaces since these are used as a
separator for the recorded keys. For the input of several blank spaces one after another, the action
is interrupted at this point since the keys after this can no longer be found.


Example
A particular submenu can only be reached with difficulty - but it is needed frequently.
Article prices in the order
Order > F4 > e price details > b order prices > a article prices
This should be called on project number with CTRL-u
    ■   For screen KAUF and field KAUF_OBJNR
    ■   Trigger event
    ■   721 – CTRL+U
    ■   Action Key
    ■   CTRL+F9 – Activate key interpreter
    ■   F4
    ■   e
    ■   b
    ■   A
    ■   CTRL+F9 – Deactivate key interpreter




        3.4.7.           Call up own/new dialog
It must always be possible to enter the first field of a customizing screen. If the
field cannot be entered, it is no longer possible to exit the screen with POS1 or
End.

Example
In dispatch, it should be possible to store additional information on the tour level
-   New table cu_versand
-   Generation of the associated dialog
        ■    Area CUST
        ■    MFO-File cu_versand.mfo
        ■    PAN-File cu_versand.pan



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                          28
        ■   If necessary, SELO files


    ■   LAPOOLTOU screen
    ■   LAPOOLTOU_ROUTENR field
    ■   Trigger event
    ■   721 – CTRL+U
    ■   Action Perform
    ■   Statement
    ■   Mfo/cu_versand.mfo
    ■   Update of the data directly for L_END
    ■   Caution:
    ■   The entry can be discarded in the order -- then this data/changes are retained.


        3.4.8.           Follow-up events
Example:
Event Action Statement      Error text =0 !=0
[P][_722][Formel__][#WLBV_NDBA_DIFF!=40][___________][262144][______]
[P][_850][Formel__][#WLBV_NDBA_DIFF +10][___________][131072][______]


The customizing described above is called via <CTRL-U> in the "Booking" field of the stock input
screen. Its effect is - if the field value of the "Booking" field !=40 - the event CU_EVENT1 is sent.
The second customizing reacts to this event, which then ensures that the field value is incremented
by 10. The behavior is such that with each press of the key combination <CTRL+U> 10 is added to
the current value. As soon as the "Booking" field has a value of 40, no more change is possible with
<CTRL+U>.


To be noted: The action SEND_EVENT only triggers customizing actions that were stored for the
same field or for the entire screen. Actions that were stored for another field and are also called by
CU_EVENT1 are not triggered.


When storing an action that triggers the event SEND_EVENT, attention must be paid that this can
also trigger actions that were stored earlier for the entire screen.
If several actions that are triggered by CU_EVENT1 are stored for the same field, then they will be
executed in the sequence in which they were stored (that is, from top to bottom).




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                            29
    3.5.        Limits
Within a header-rump screen, the "Overall transaction logic" applies:
    •   The discarding of the calling module leads (implicitly) to the discarding of the customizing
        actions.
    •   This is depicted on the customizing screen with the transaction level, which in case of an
        overall transaction logic is greater than zero.
Within a main table, there are separate read and write transactions:
    •   The discarding of the calling module therefore does not lead to the discarding of the
        customizing actions.
    •   This is depicted on the customizing screen with the transaction level "0".
    •   Order processing and PMS job creation are also modules with separate read and write
        transaction, although these are not main tables. Thus there is the problem that additional
        performed screens (that fill corresponding cu tables with data) are not reset with
        discarding of the job or the order!
Currently, the new alcib-even-control is not active everywhere:
    •   If a module still works with old event-control, then the creation of customizing actions is
        prevented.
    •   There can be no expansion into a field that can be entered
    •   Storing CU actions is only possible as user awserv!
    •   Only if env variable CUSTOMIZING is active
    •   Avoid field name = #ALL#
    •   Can influence performance
    •   Endless loops are possible via customizing
    •   Then the customizing must be set to inactive = 1 via update




    3.6.        Possibilities
Event-oriented customizing actions offer the following possibilities:
    •   Messages can be output; possibly conditionally
    •   STD answer to JN queries
    •   Suppress messages
    •   The field content of the current field can be checked
    •   The current field can be assigned a default value
    •   Fields can be given additional attributes
            o   Set field invisible



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                           30
           o   Do not allow manual field change
               See "Set jump marks and hide field contents"
   •   The standard behavior of the function keys can be started (or changed)
   •   At the touch of a button, a list (formulated with Adhoc-SQL) can be displayed
   •   Change of the STD selection (SELO)
   •   The print, mode, and menu functionality can be deactivated
   •   In addition to an existing ALCIB screen, additional data can be entered on user-specific
       screens
   •   Call of a new dialog (FIX knowledge required)
   •   Call of programs on the client PC
   •   Create keyboard shortcuts




A+W Software GmbH           EN-CONFIG-A+W Enterprise Customizing.docx                             31
4. Set jump marks and hide field contents
(SYSTEM MENU => SYSTEM CONFIGURATION => DEFINE JUMP END,
SYSTEM MENU => SYSTEM CONFIGURATION => CHANGE FIELD ATTRIBUTE)
If you change a jump mark or field display, you will be asked whether you want to execute
the particular action. This way, your changes are more transparent, especially if you define
different settings for different authorization groups. So that your changes become
effective, you must exit the selected screen saving the relevant field.
You can now select the authorization group that should apply for these settings via <SELO>.


The table "defstyp" in which the relevant information is stored has been changed. In the
course of the installation 2.10, an upd script handles the implementation of the existing
settings on the new data structure.
This new logic considers only the attributes INVISIBLE/NOMOD and NOJUMP. All additional
attributes that were previously changed by the field styp of the table "defstyp" must be
changed through customizing actions, effective immediately. The last especially affects
Pilkington! If a NOJUMP or INVISIBLE attribute has been removed by the customer, then this
cannot be considered during the automatic implementation.
In order to be able to detect customer-specific settings, the field styp remains in "defstyp"
and is not changed by the new logic.
AWDesk 8875.




A+W Software GmbH          EN-CONFIG-A+W Enterprise Customizing.docx                      32
5. SQL queries
The AWE SQL queries offer a variety of options for creating your own evaluations and thus
displaying any data from the database.
The aim of this document is to explain the functionality of SQL queries to the user using a few
examples.
The procedure can be divided into three logical steps:
    -   Definition of a query
    -   Formulating a statement
    -   Open the hit dialog
Before using this function, the SQL groups must be created in the master data. These can also be
managed in several languages and can be defined under Master data > Key
> System > Adhocsql groups. The SQLs of group 1 are delivered by A+W with the installation and
are therefore generally available. These SQLs are used in various places in A+W Enterprise and
therefore cannot be changed by the end user.


    5.1.        Definition of a query

Using the system menu <Ctrl+F4> > Change SQL queries > you can store new SQL queries or
change existing queries. The following describes which options A+W Enterprise offers for creating
an SQL query.




Figure 17: Example 1




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                         33
Figure 18: Example 2


        5.1.1.            Dialog titles
A title can be stored for the hit dialog. The field Title serves this purpose. In this field, both a text
and a message number can be entered. A message number must have a leading #. Only existing
message numbers can be used as message number (table errmsg).
In Figures 1 and 2, the titles are stored as text.
A value from the hit quantity of the query can also be entered as title.
Example: in the query, a customer number is queried. It should be depicted in the title of the
event dialog.
If the customer number is the first field in the query, then a $1 must be entered in the title field.
When executing the SQLs, in the title, the result of the first field of the query will appear in the
title instead of the $1.


        5.1.2.            Selos and lookup fields
Now selos incl. lookup fields can be used in the query. The selos used must be stored in the CUST
area in the directory "sel".
To attach a selo to a query field, in the Selection field of the SQL query, the name of the selo must
be entered. Input is done as usual separated with "|".
Example:         "mitarb.sel|abtnr.sel"
In this example, the selo "mitarb.sel" is added to the first field and the selo "abtnr.sel" is added to
the second query field.
If you would like to fill a lookup field via selo, this is identified in the Selection field next to the
selo name with "1".



A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                                  34
Example:          "mitarb.sel,1|abtnr.sel"
This example provides the same result as the previous result. In addition, however, a lookup field
will be generated next to the employee number field. This field is on the screen to the right of the
query field and reaches to the right edge of the query screen.
IMPORTANT: Only one lookup field is allowed per selo.


         5.1.3.            Dialog tabs / tab
Various tabs can also be defined on the hit dialog. In the Tab name field, the number and titles of
the tabs for the his dialog can be defined.
Tabs are only shown if the Tab name field is filled. The number of tab names there separated by
"|" determines the number of tabs. If there are more views than tabs, you can switch among
these with <F2>.




Figure 19: Example of a tab definition and the hit dialog.


         5.1.4.            Graphic fields on the results dialogs
It is now possible to display graphics fields in SQL statements. Possible graphics fields are
checkboxes and status lights. In addition, it is possible to switch fields so they are invisible. This
possibility has been present since Alcib version 2008.2.
For the definition of which column should be displayed as graphic field on the results screen,
there is a new field on the SQL dialog (Gfx fields). In this field, analogous to the specification of the
column titles (Spaltenbez) and column widths (Spaltenlän), a character string can be stored. The
separator symbol for columns is the pipe character "|" (<Alt Gr+|>).
Possible values for columns as graphics fields: status light:
    •        0 - green
    •        1 - yellow



A+W Software GmbH                EN-CONFIG-A+W Enterprise Customizing.docx                               35
    •         2 - red
    •         3 - white
    •         4 - blue
    •         5 - blue-red Checkbox:
    •         0 - unchecked
    •         1 - checked.


        5.1.5.            Handling of invisible fields
It is also possible in SQL statements to hide the fields required for the query in the display. Such
fields are called invisible. The identification is done via the keyword nodispl.
For invisible fields, it must be noted that they must be counted normally in the formatting of the
column titles and column widths.
Example:
Gfk fields:       "|status|nodispl|checkbox"
Spaltenbez:       "Auftragsnr.|Verarbeitungsstatus||Gebucht"
There are two pipes (||) between "Verarbeitungsstatus" and "Gebucht" since there is an invisible
field there, which must be counted when counting the titles.
In this example, first a normal field, a traffic light, an invisible field, and then a checkbox will be
displayed. There is an invisible field between the traffic light and the checkbox.
Attention: If additional views are available, invisible fields should be distributed to them. The case
that in a view no fields at all are displayed must be avoided since it can cause problems in the
program. The select statement and the GFX fields should be adjusted accordingly.


        5.1.6.            Tooltip texts for fields
In the GFX tooltip field, tooltips can be stored for fields on the results dialog. These can be direct
text or also a message number. Line breaks can be created by entering "\n" (without quotation
marks).
The entry of tooltips makes particular sense for graphic fields. Input is done as usual separated
with "|".
Example:          "#12345|red: negative margin, green: with profit|||#234566"


    5.2.          Statements
After specifying the basic conditions, the statements can now be stored. Use <F5? from the SQL
dialog to reach the SQL editor.
For the examples from chapter 3.1, the following statements are formulated:




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                                  36
Figure 20: Statement for example 1 in the figure




Figure 21: Statement for example 2 in the figure


         5.2.1.           Substatements
In the ADHOC-SQL, it is now possible to start SQL queries again for hit quantities (with displayed
dialogs).
Example:
The first statement is a "Select * from xhaus;" Now you would like to select a line and issue a
"Select * from ykund where haus = (selected query from previous
query").




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                         37
This can now actually be done. Queries that should refer to hit quantities from the previous
statement begin with {SUB1:}, whereby the second statement contains a "2".
ATTENTION: The following constellation is not directly possible:
    1. Select Statement
    2. Select into temp
    3. Substatement
So that this works, the "into temp" statement must also be formulated as sub-statement
(with {SUB:<Number>} at the beginning).


        5.2.2.            Reference to field contents in sub-statements
In order to refer to a record, it is possible, e.g. to refer to a column of the hit screen in the WHERE
condition. A reference to fields begins in the query with leading #.
Example:




Figure 22: Example of a SUB-select

The column #1000_5_0_haus is composed as follows:
#<ADHOCSQL Group>_<ADHOCSQL ID>_<Column No.>_<Column name>
On the his screen of "select * from xhaus;" you can display this name with <Shift-F5>:




Figure 23: <Shift+F5> on the hit dialog displays the column name that is needed for a SUB-select.

ATTENTION: Alphanumeric columns must be entered in the referencing with individual
apostrophes. Example "select * from xhaus where hname='#11_1_3_hname';"
Otherwise, SQL error 217 may occur.
Tip:      If the field to which reference should be made is a GFX field, that is, a traffic light or
checkbox, then reference may not be made to the field itself. ThThe GFX field itself is a lookup
field. It contains no "sensible" values. However, there is an invisible field in front of this field. This
contains the values of the GFX fields (e.g. 0 for green traffic light). Example: The status field is
called "#11_1_3_LUSTATUS", then the associated values field is called "#11_1_2_STATUS".



A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                               38
         5.2.3.     Jump to the document entry directly from the hit
             quantity
It is also possible to branch directly into the manual document entry and change. The following
conditions must be met:
       •    These fields must be present in the hit quantity. They may also not be provided with an
            alias in the select.
                –    Auftrnr
                –    Document
                –    Subnr
       •    No open transaction
                –    In change mode, from document entry or from another entry dialog, it is not
                     possible to start document entry.
This logic functions for all manual document dialogs, also for invoices and delivery notes.


         5.2.4.           Detailed example for ADHOC-SQL




Figure 24: Example of an Adhoc-Sql with sub-statement and a traffic light display (declaration)




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                          39
Figure 25: Example of an Adhoc-Sql with substatement and a traffic light display (formulation of the statement)




Figure 26: Example of an Adhoc-Sql with substatement and a traffic light display (hit dialog with the <F5>
indicator)


         5.2.5.            Formatting of sub-statements
The sub-statements can, like the main statement, be assigned formats.
If you are in the editor in a line with substatement flag (e.g. {SUB:1}), then you can enter the
subdialog with <F5> and store the necessary details in language-specific fashion there. The
evaluation of the language depends on the display later of the A+W Enterprise system language.



A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                                    40
    5.3.         Hit dialog
The execution of a query is done with the <F3> or via the System menu <Ctrl-F4> > SQL queries>
Execute




Figure 27: Result of the SQL 1000/3




Figure 28: Result of the SQL 1000/1



    5.4.         SQL menu
‒   Quick accessing of particular SQL queries
‒   SQLs of the group 1000
‒   SQL queries with IDs between 1 and 20
‒   SQL_MEN_GRP – Definition of other groups


A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                         41
    5.5.        ADHOC SQL env variables
The program execution of an ADHOC-SQL is done by activating an appropriate environment
variable. In order to activate an environment variable sensibly, the group and the ID of the
ADHOC-SQL must be stored separated by blank spaces. For example, the ADHOC-SQL with ID 87
of the group 1 as "1 87"
The document information is controlled by an ADHOC-SQL using an environment variable.
Order
Sales > Overview > Document Information
Sales > Order Entry > <Shift+F4 > Order Information, or <Shift+F10> > Status
Purchase Orders
Purchase > Overview > Purchase Information
Purchase > P.O. Management > Shift+F4 > P.O. Information, , or <Shift+F10> > Status




Figure 29: Document information

The "Int.Auftr." button is on the "Document information" dialog (on each tab).. Clicking this
button causes the appropriate ADHOC-SQL env variable stored on the tab to be queried and the
corresponding ADHOC-SQL to be carried out.
 Tab                    Env variable for „Int. Order“  Order / P.O.
 Document               VORGANGSSTATUS_ADHOCSQL / VORGANGSSTATUS_EK_ADHOCSQL
 Items                  POSITIONSSTATUS_ADHOCSQL / POSITIONSSTATUS_EK_ADHOCSQL
 Purchasing             EINKAUFSSTATUS_ADHOCSQL / EINKAUFSSTATUS_EK_ADHOCSQL
 Receipt of goods       WARENEINGANGSSTATUS_ADHOCSQL /
                        WARENEINGANGSSTATUS_EK_ADHOCSQL
 Production             PRODUKTIONSSTATUS_ADHOCSQL
 Dispatch               VERSANDSTATUS_ADHOCSQL / VERSANDSTATUS_EK_ADHOCSQL



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                        42
Barcoding           BDESTATUS_ADHOCSQL
Racks               GESTELLSTATUS_ADHOCSQL
Stock               LAGERSTATUS_ADHOCSQL / LAGERSTATUS_EK_ADHOCSQL
Linked prod.        LINKEDPRODSTATUS_ADHOCSQL




A+W Software GmbH       EN-CONFIG-A+W Enterprise Customizing.docx    43
6. Ad hoc SQL tool
   6.1.        Configuration
ADHOC SQL results screens can be presented for correction with the environment variable
ADHOCSQL_EDITMODUS = ON. Thus, rows can be deleted and fields changed.




A+W Software GmbH          EN-CONFIG-A+W Enterprise Customizing.docx                      44
7. Print format templates
   ■   Available in all tabular dialogs
   ■   Earlier only for printout, today also for Office transfer
   ■   For Office transfer -> Paper format "blank"
   ■   Definition
           ‒   Output only for printing = Y
           ‒   Titles
           ‒   Sequence
           ‒   Intermediate total (not for Excel transfer)
           ‒   Sorting




A+W Software GmbH            EN-CONFIG-A+W Enterprise Customizing.docx   45
8. Configurable fields
Time and again, customers have requested an option for saving additional information at
document entry, asking whether this could be applied to existing versions as well.
This is why version 2007 offers a general logic (#120277) that allows configuration of additional
fields in customer systems. These fields can be preset from master data.
Configurable fields in the order header allow entry of information about partners or about the
entire document.
 Additional information about the individual items such as the CE code can be saved in additional
fields on the item level.
It is also possible to link functions to configurable fields within the ALCIB program code.




    8.1.          Data structures
The tables involved are described briefly below. For a detailed description of the individual fields,
please use altab.
•       Master data
    •   kflddef
The additional fields on both document header level and item level are saved in this table.
Appearance, length, changeability, and possible presettings are defined here.
•       Transaction data
    •   kaufprvfld
Information on order header level are saved in this table.
    •   kposprvfld
Information on item level is saved in this table.


    8.2.          Master data maintenance
The fields that can be configured at document entry are set on the menu Master data > Field
configuration > Document field configuration.
First enter the name of the table whose fields you would like to configure:
•       for fields on item level, kposprvfld
•       for field on document header level, kaufprvfld


Now enter the number of the variable set to be configured. Every set of variables can contain up
to five fields of the data types char, decimal and integer. If the number of fields does not suffice,
you have to define an additional set of variables. The required sets are usually numbered, starting
from 1001.


A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                             46
The set numbers from 1 to 1000 are reserved for linking functions to the fields.
If records for the defined combination of table name and variable have been defined already,
these will be loaded now. A change of the field meaning, e.g. by amending the label, may cause
problems in existing documents.
To configure a field, first enter the menu name of the field. For both tables, this is:
•       longval1, ...., longval5
•       decval1, ..., decval5
•       charval1, ..., charval5


Now enter a group number. Using this number, ALCIB functions such as calculation can be linked
to the fields. This function has to be ordered separately if required.
The sequence number follows. It has to be between 1 and 20, and must be unique. This sequence
number defines the sequence of fields in transaction data. A gap in the sequence will cause a
blank line between the fields in the transaction data menu later on.
Next, you can enter the field label. It will be shown in front of the field in transaction data.
Use STYP to set the properties of the transaction data field.
You can also define a title for a group of fields by creating a record for a redundant field and
setting the STYP to 2056. Now set the field above the first field of the group and enter the
required group title in the label.
Enter the required field length in the Length field. It must not exceed the maximum length of the
field.


The last two fields of the screen are used for presetting.
The reference field allows entry of a database field ("<Table name>.<column name>“). The
configurable field will be preset with the entry in this field. Please note that for kposprvfld you can
only select database tables with field artnr as a key. For kaufprvfld you can use only tables with
the keys mpnr and kuliflag. Sales fields are always preset from customer master data and
purchasing fields, from supplier master data. Possibly existing projects will not be considered for
presetting. You can also enter a fixed default in this field. To make sure that the system realizes
that this is a default, the entry has to be preceded by a rhombus (e.g. #678 for a long field or #ABC
for a char field).
In the following field you can enter the number of a configurable master data field. For kposprvfld
this is item master data and for kaufprvfld , partner master data.


It does not make sense to enter both a reference field and a configurable master data field. In
these cases, the default setting always used the value of the configurable field from the master
data.
Only fields can be used as defaults that have the same data type.
Furthermore, you can use <F5> to branch into a screen on which you can specify language-
dependent labels. These will not be directly used in ALCIB but can be analysed by reports.




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                           47
<F2> brings you to a MODE menu. There you can define whether the field shall be included in
internal EDI, or if it will be preset anew at the recipient's end. Fields will always be preset anew
for external EDI. You can also define a selo to be added to the menu field in transaction data. The
selo name consists of "<area>/sel/<Selo name>" (e.g. "kauf/sel/kunr.sel"). If no area is defined
(e.g. "sel/custselo.sel"), the system will search the customizing area.


If the configurable fields contain information to be analyzed by reports, report amendments will
have to be ordered separately.
For reasons of performance, the information in table kflddef is saved in a cache. This is ALCIB has
to be rebooted after this table has been changed.
Setting of the document fields
The menu for editing configurable fields can be accessed via the Configurable fields menu.
If you load this from the document header, the configurable document fields will be displayed. If
you select this menu from an item, you will see the configurable fields on item level. When you
enter a new document with a reference, the system will adopt the entries from the old document.
They will not be preset anew.


    8.3.         Fixed sets
        8.3.1.           Delivery time – Set 2 - kaufprvfld
In this set, the delivery time in Group 2 in charval1 is entered. If a delivery time is entered, this is
displayed with a "*" in the document header in front of the customer's requested date. The
delivery time can be used for the discount calculation.
See “EN-CONFIG-A+W Enterprise” – “Discount logic 2005” – environment variable
RABATT_SP_KAUF_PARAMETER.
Furthermore, the field dateval1 is pre-populated with today's date. However, this is currently not
evaluated in the program.
For user 60, there are additional customer-specific functions for this set.



        8.3.2.           Delivery note printing – Set 10 - kaufprvfld
See „EN-CONFIG-A+W Enterprise“ – „Delivery note printing in dispatch depending on a configured
field in market partner master“




A+W Software GmbH              EN-CONFIG-A+W Enterprise Customizing.docx                               48
9. Transfer to Excel
    9.1.        General
The transfer of table contents to Excel(©) has been considerably extended since A+W Enterprise
6. It is now possible to specify an Excel template file for a style sheet. Using this template, pivot
tables, pivot charts and macros can be defined, which are called automatically updated after the
transfer. This allows a multitude of new displays of your data. Thus, for example, the incoming
order from a customer can be compared graphically with those from the previous year.
Such evaluations are possible in all table views of A+W Enterprise as well as in hit quantities of the
SQL queries.


        9.1.1.           Configuration
CIB2OFFICE_EXCELBASICPATH (client reference: no)
Basic path for the Excel templates for the CIB2OFFICE/spreadsheet. It must be a Windows path


    9.2.        Process
    •   Via a print format template, data is written to a file $REPTEMP/MPR*.
    •   datpgscr
            o   The datpgscr is with the following parameters:
                        MPR file
                        Desired file type (Excel = 102)
                        If necessary, path to template file
            o   If there is a customer-specific datpgscr under $ALCIBPRG/spec/cmd, this is called.
            o   The datpgscr adds a control instruction #Parameter.<Extension> that later causes
                the Cib2Office2 to generate the desired format.
            o   If a template file was specified, it is attached to the #Parameter line.
            o   The script now outputs the control line and the file content to STDOUT.
    •   Front end
            o   The front end now collects the data transferred to STDOUT in the "Output file"
                stored under Settings > Overview.
            o   After that, the program stored under filter is started with parameter "Output
                file".
            o   This generates in the %TEMP% directory a file called al*.<extension>. The
                extension is oriented according to the second parameter in datpgscr. Here, if the
                "CIB2OFFICE_CSV" variable is set, a csv format is generated. This is necessary if
                MS Office is not installed on the PC.



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                             49
    9.3.        Excel Transfer with Template
Creating the template file
A template file is created with Excel. For this, an existing worksheet is saved as a template. This
template can contain tabs for the transferred data with the predefined names.
Names of the current tabs for the transferred data:
       •   Data:
All data from the table to be passed is written to this tab. The first row contains the column
names.
       •   DataHeader:
On this tab, all header and footer lines are written in a fixed position. In A1 – A3 the 3 header lines
are written. In A4 and A5, the 2 footer lines are written.
Note: Both of these tabs may not contain important information since it will be overwritten
completely.
If these tabs are not found, they will be recreated.
Additional tabs can be filled at will.
(e.g. Pivot tables, diagrams, calculations)
All Pivot tables are, after the data tab was filled, updated automatically and their data sources are
adjusted to all of the data written.
After that, there is an attempt to execute the macro "AW_Autostart".
Excel templates are saved with the extension "*.xltx" or "*.xltm" (if it contains a macro).
Automatically starting macro
Templates can be provided with macros. The "AW_Autostart" macro is called automatically after
all data has been written and the pivot tables have been updated.
Excel transfer without template
If you do not specify a template, a new Excel folder is created. In it, a new tab is created on which
all data is written.



A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                               50
However, the header and footer lines are considered differently. These are written via the table.
Here the 1st header line is used as name of the tab. If the 1st header line should be too long for
the tab, only part of it is used as name of the tab and written over the table with all header and
footer lines. A free line is left between the header and footer lines and the table. The first line is
also boldfaced and the data is prepared visually with a table formatting.


    9.4.        Example of an Excel Transfer:

    1. Create print format template
    2. Paper forma "EMPTY"
    3. Set fields for transfer to Y
    4. Transfer to Excel
    5. Open %TEMP%/alxxxx.xlsx
    6. Rename tab Data
    7. Insert > Pivot table
    8. Save as Excel template under \\srvalcib\globusr\dokuserver\excelt
    9. Assign in print format template




Figure 30: Formulating a style sheet using an ADHOC-SQL.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                              51
Figure:31 Result of the transfer to Excel.



    9.5.          Important Information
Formatting
        •   Columns with a date format are formatted using the short data format for the system.
        •   Columns with decimal numbers are formatted with the same number of places after
            the decimal point.


Restrictions
        •   Totals are not considered
        •   Borders are not considered
        •   Page numbers are not considered
        •   The date is ignored
All pivot tables are adjusted to the new data.




A+W Software GmbH                EN-CONFIG-A+W Enterprise Customizing.docx                    52
Additional parameter
-noHeader:        all header and footer lines are ignored

-warnings:        Warning messages are output




Possible errors
If a field should be empty, this may be because in the print format template for this column, a
field length that is too small is entered. The field lengths for this column should be increased in
the print format template.
Date fields can, depending on the length set in the print format template, not contain a day. Here
the counting starts from the 1st of the month in question.
Tab:    designates a single table.
Worksheet:        designates a collection of tabs
Macro: program code in Visual Basic for Applications (VBA) that is executed within Excel.




    9.6.          Adjustment of the "Page Layout" Dialog
The Page Layout dialog has been restructured to make it easier for users to use.


The individual mode screens were provided with tabs and you can still flip through them with F2.
The tables for the column information are now switched on throughout. The header and footer
texts were placed on a single mode screen. In the area of the Excel mode screen you will find the
new Excel template data field, which allows you to save a template. The Excel templates are
selected via the file open dialog or can be entered manually. Please note that only the Excel
template and any existing subfolders may be entered in the data field, e.g. "AW_Autostart.xltm".
The base path for the Excel templates is set using an environment variable. With F5 you can now
open the dialog for the edge distances.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                               53
10. Individual Programs
    ■   Shell scripts ($ALCIBPRG/spec/prg)
    ■   Call via system > Individual programs > Execute
    ■   System > Individual programs > Parameters
            ‒    Definition of call parameters
                     •   Sequence
                     •   Data Type
                     •   Selo if desired
Possible areas of application:
    ■   Starting EDI storage/FinAc transfer
    ■   Interface generations
    ■   Query of system status information


        10.1.1.          Use of subdirectories
#449130 – 2019-09 – A+W Enterprise 6
It is now possible to create subdirectories in the menu System > Individual programs , for a better
grouping of the scripts. If, when selecting an element of the collection, it is recognized that this is
a subdirectory, the system branches to this directory and offers a listing of this directory.
Navigation back to the parent directory can be achieved by exiting the selection with END and
restarting the selection.

Only subdirectories to the individual path are possible (default: STD $ALCIBPRG/spec/prg).

When storing parameter queries via the menu path System > Individual Programs > Parameters, it
is assumed that the script names are unique. I.e. you can only create ONE parameter set per script
name.

To use this logic, it is necessary to update the privsyscall.mfo file ($ALCIBPRG/libs/cho directory)
on the client system.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                              54
11. Vorgangs_sql
For the set-up of customizing in the vorgangs_sql, you must absolutely pay attention to the fact
that this can influence the performance of production transfer. On the one hand, the
ORDDERXML file can only be written when the vorgangs_sql is finished and on the other hand,
during the reporting, the order is only released again if the vorgangs_sql is finished. Therefore,
you must consider for which intauf runs (still flag) which customizing is required.
The call of the Vorgangs_sql is made at various points in the process flow. Currently, these are:
    -   After saving in the foreground (0)
    -   Dispatch control (2)
    -   After processing by intauf (3). In particular here, attention must be paid that there are
        several different intauf run-throughs (still flag)
    -   Order release (4)
    -   Order booking (5)
The Vorgangs_sql works in an individual transaction and not in the original order transaction.
Which parameters the Vorgangs_Sql expects can be read in the script in the development
environment.
Tasks that can be done via the Vorgangs_sql are:
    -   Manipulation of data via update/insert
    -   Writing of interfaces
    -   Sending information via mail - awmail
Here too, it is important: documentation within the script With more extensive documentation,
reference to external documentation.




A+W Software GmbH               EN-CONFIG-A+W Enterprise Customizing.docx                            55
12. SPs and shell scripts
If you are working with your own SPs and shell scripts, these must absolutely be documented
inline. The purpose should also be documented.
SPs and scripts serve the purpose of data manipulation and if necessary the generation of
interface files.
Scripts should be stored in central places so that the colleagues and employees can find them
easily.
SPs in the course of the production transfer (OrderXML) is documented "EN-CONFIG-A+W
Enterprise Production Interface".




A+W Software GmbH           EN-CONFIG-A+W Enterprise Customizing.docx                           56
13. DFUE_Nachbearb
The special customizing in the course of internal and external EDI is documented in "EN-CONFIG-
A+W Enterprise EDI".




A+W Software GmbH           EN-CONFIG-A+W Enterprise Customizing.docx                         57
14. Documentation
Document 18670: Documentation of customizing
A documentation module was created so that, even some time after a customizing action, you can
still see what it does, and why it was created. Module alcustdoku can be used by the customer's
service-, project- and IT teams to record their customizing work on site. Customising in this
connection does not only mean the "actual" customizing via al_cust, but all amendments of the
database (SPs, trigger, synonyms, views) and the process (case Sql). A serial documentation
number in the main menu is automatically allocated if this field is left empty. This field also offers
a selo to view all customizing actions recorded so far. The fields user ID and client will be
automatically filled with the values from the environment variables USER_ID and HAUS when you
open the menu. The fields Action type and Section can be selected via toggle. Field Keyword is
mandatory. Field DB object must be filled if DB action was selected as the action type. Also, field
Starting point must be filled if Process action was selected as the type of action. Field Activation
date is mandatory. Date of change is automatically filled with the current date. The author's name
and first name, as well as the customer name, must be filled in. When you select the action type
Menu Customizing, you can switch to a mode menu which contains all fields of the Customizing
menu. The system automatically switches to this mode menu if you select the action type Menu
Customising, and the end of the main menu is reached. After filling in the fields menu name, field
name, and sequence via F3 in the mode menu, you can load the values from table alcust. The
corresponding descriptions can be defined in the footer. As for Customizing, the Customizing
documentation menu is accessed via the code SYCU.
In case of major changes of a menu customizing, you must update not only the documentation,
but also the Customizing section. This is done in the mode menu, in field Sequence, using <F3>.


Installing the module for Version 2.12 (for German clients only):
From directory /r3/kundinst/2.12 (on romulus), load nachcustdoku.z and transfer it. Unpacking: In
directory $ALCIBPRG gzcat <File name>, load | .suc tar xvf -; the files will be transferred to the sql
directory. Then, the following scripts must be executed:
alcustdokuk01.sql (create table alcustdokuk)
alcustdoku01.sql (create table alcustdoku)
nr_kreise03.upd (enter the corresponding number area)
ALso, transfer and install the binfile alcustdoku.
Please note: Since fx_texte is transferred again, the installation must not be done during
operation. Because of the new number area, the server must be rebooted after installation.
The necessary data for foreign versions will be created as required.
As from version 3.0, this environment is included in the ALCIB update routine;:you have to transfer
a new binfile to the customer's computer, however. Starting with Version 3.2, this will also be
automatic.




A+W Software GmbH             EN-CONFIG-A+W Enterprise Customizing.docx                             58
15. Table of figures
Figure 1-1 Customizing main screen .................................................................................................. 8
Figure 1-2 Customizing mode screen ................................................................................................. 9
Figure 2-1 Example of a SQL action .................................................................................................. 13
Figure 2-2 Example of an SPL action ................................................................................................ 14
Figure 2-3 Evaluation of a SQL return value in a formatted message.............................................. 14
Figure 2-4 Example of an AdhocSQL action ..................................................................................... 14
Figure 2-5 Example of a shell action ................................................................................................ 16
Figure 2-5 Example of a perform action........................................................................................... 16
Figure 2-7 Prompt display for <Ctrl+U> ........................................................................................... 17
Figure 2-8 Customizing action with an error message ..................................................................... 17
Figure 2-9 NY-Quest action .............................................................................................................. 18
Figure 2-10 Example of a selo action ............................................................................................... 18
Figure 2-11 Example of incorporation of the formula interpreter .................................................. 19
Figure 2-12 SqlSelo displayed........................................................................................................... 22
Figure 2-13 SqlSelo as replacement for the employee selo ............................................................. 23
Figure 2-14 By storing a message number, the customizing default answer can be stored ........... 26




A+W Software GmbH                        EN-CONFIG-A+W Enterprise Customizing.docx                                                      59

