---
description: "AUW_Description_IG_Breakage"
---


# IG-Breakage in case of not assembled subcomponents (concept)

## History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 04.05.2017 | PK | First release | 1.0 |

## Content

- [Introduction](#introduction)
- [Goal](#goal)
- [Precondition](#precondition)
- [Solution](#solution)
  - [Installation](#installation)
  - [Configuration](#configuration)

## Introduction

There are situations during the production of insulating glass, in which the IG is not produced by the A+W Production Terminals in the IG line. There are several reasons for this:

- The IG needs to be reproduced very quickly
- It is not possible to produce the IG via the IG line (physical restrictions)
- …

If such an insulating glass is booked as breakage, the system cannot know which subcomponents have to be reproduced, because there is no link between the IG and the subcomponents. Because each part has to be tracked in the system separately, a unique barcode is assigned to each part in the bill of material. Therefore the system cannot just use subcomponents by random for the reproduction.

The result is:

The employee who triggers the booking has no information about the fact that his booking does not trigger any subsequent production.

The employee at the cuttingtable, spacer bender or Georgian bar-production has no information, the he need to reproduce something

If there are purchased parts involved, nobody will be informed, that there is something to reorder

The same situation will happen, if a laminated glass is not correctly booked via the A+W Production Terminals LG. Also here the system need to know, which parts are assembled in the LG to create correct remakes.

This document describes how to close this functional gap.

## Goal

The described solution is intended to ensure that a postproduction is reliably started even if no subcomponents are assembled in the IG. It is designed to help users find the right parts and take appropriate action.

## Precondition

- Minimum: AWProduction Release 5.4 last patches
- All necessary printers have to be installed and configured on the Process-Server (where AlcimBooking and the Process-Manager are running) for the “awservices”-Account
- For sending a report as email, you need to have a PDF printer, which can send mails directly (e.g. “eDocPrinter”). The Printer needs to be setup at the Process Server where the AlcimBooking and the Process-Manager are running.
- Since release v6 Update 3 it is possible to send mails directly, without using the eDocPrinter. This functionality is actually not usable for this solution, because there is no possibility to check if there are subcomponents assembled or no before sending the mail.
## Solution

Each breakage booking of an IG or LG (coming from scanner or Production Terminals) triggers a report to a specified printer. This report can contain information about the scheduled subcomponents, which should be reproduced.

AlcimBooking creates an entry in the table PROZESSE. The process-manager grab this entry and start the reporting with the Reportname, Printername and the parameter “BARCODE”. The report is designed, that it only give a result if there are no subcomponents assembled. So for a “normal” IG breakage with subcomponents there will be no printer output.

In the parameter it is possible to configure several reports depends on their needs:

- a report for the cutting table
- a report for purchased parts
- a report for spacer bender
- a report for Georgian bars
### Installation

The installation should be done on the process-server with the setuplauncher. The following modules and its dependencies are necessary:

- AlcimBooking
- Process-Manager
- eDocPrinter (to send reports via mail)
### Configuration

The main configuration is described in the document:

There are separate parameters necessary to trigger a report for IG or LG:

### Breakage of IG

Report is printed on a separate printer it the broken glass is an IG unit

Object Type: 1

Where clause: POOL_TEILE.BESCHAFFUNGSART=1 and POOL_TEILE.TTYP=7

Status Type: 4 (breakage)

RegPoint Type: 0

### Breakage of lami

Report is printed on a separate printer it the broken glass is a lami

Object Type: 1

Where clause: POOL_TEILE.BESCHAFFUNGSART=1 and POOL_TEILE.TTYP=8

Status Type: 4 (breakage)

RegPoint Type: 0
