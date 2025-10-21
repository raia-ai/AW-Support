---
title: "AW_Business_Pro_-_Mark_Longest_Edge_Version_1.01"
source: "AW_Business_Pro_-_Mark_Longest_Edge_Version_1.01.docx"
tags: ["AW Business Pro", "Mark Longest Edge", "business documentation", "procedures", "guidelines", "version 1.01", "operations", "reference", "SOP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This Markdown file is a structured conversion of the original DOCX document titled “AW_Business_Pro_-_Mark_Longest_Edge_Version_1.01.” It preserves the document’s headings, lists, and tables for reliable indexing in a vector store. Major sections include: A+W BUSINESS PRO - MARKING LONGEST EDGE ON PLANEDIT. The introduction begins: **A+W****BUSINESS PRO****-****MARK****LONGEST****EDGE**"
long_description: "This file provides a faithful, UTF-8–cleaned Markdown reconstruction of the source document “AW_Business_Pro_-_Mark_Longest_Edge_Version_1.01.docx.” The conversion process preserves the document’s logical structure, including hierarchical headings, bullet and numbered lists with nesting, and any tabular data transformed into GitHub Flavored Markdown tables. The content order follows the original, enabling accurate search, retrieval, and chunking for embedding-based systems.

Top-level sections identified in the document include: A+W BUSINESS PRO - MARKING LONGEST EDGE ON PLANEDIT.

Where the original layout implied structure—through typography, spacing, or list formatting—this Markdown expresses that structure using ## and ### headers, standard list syntax, and tables. Duplicated lines were removed where appropriate, stray control characters were eliminated, and common mojibake sequences were normalized for consistency. Inline emphasis such as bold and italics were retained where possible to reflect emphasis or sub-section cues present in the DOCX.

The resulting Markdown is intended for ingestion into OpenAI’s vector store or similar retrieval systems. By preserving semantic groupings and converting tables into machine-readable rows, this file supports fine-grained chunking, metadata tagging, and context-rich retrieval. It does not alter or interpret the substantive content of the original; rather, it provides a clean, standardized format that mirrors the source while being more interoperable with developer tooling and LLM pipelines.

Note: If the original document included embedded images, shapes, or complex numbering schemes, they are represented here in plain Markdown as text, lists, or notes, which ensures portability while maintaining the core informational content."
---





























**A+W****BUSINESS PRO****-****MARK****LONGEST****EDGE**

**INSTALLATION AND CONFIGURATION**

**A+W AUSTRALIA**



**PROJECTFACTS****TICKET -****[AW-102504]**









| **Date** | **Author** | **Modification/Remarks** | **Version** |
| --- | --- | --- | --- |
| 18/02/2022 | Juan Segovia | AWB Pro-Marking longest edge onPlanEdit | 1.00 |
| 24/02/2022 | Todd Leiseman | Formattingand Registry information | 1.01 |
|  |  |  |  |











## A+W BUSINESS PRO - MARKING LONGEST EDGE ON PLANEDIT



### CONFIGURATION

The steps to mark the longest edge on thePlanEditare the following ones:



1. Copy the files “XT_BEDGE.EXE” and “XT_BEDGE.CFG” located at folder:





2. File “XT_BEDGE.EXE”

Copy the file “XT_BEDGE.EXE” at folder:

C:\Program Files (x86)\A+W\Techsoft\Xopt



3. File “XT_BEDGE.CFG”

Inthe APPDATAfolderof the user, create manually the folder structure-C:\Users\<USERNAME>\AppData\Roaming\A+W\Techsoft\cuttv\xtvand copyinsidethe file “XT_BEDGE.CFG”.





Note -Itappearsthe “XT_BEDGE.EXE” was designed to work with XTV and it is reading the config file from this location. If the folder already exists, it contains the “XT_BEDGE.CFG”.



4.In thefolder P:\Common, edit the file “xrecalc.bat” andaddthe following line at sections XOPT and XOPTS:

***if exist "%******RootDir******%\******xopt******\XT_BEDGE.exe" "%******RootDir******%\******xopt******\XT_BEDGE.exe"***





5.Updatethe Windows Registryandset the key “ShowEdge” to 3to show the mark the longest edge

HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Albat+Wirsam\PlanEdit\Pattern

**Other****Known Registry Entry Options**

1 =No Marking, 2 =MarkShortest and 3 =MarkLongest





### A+W BUSINESS PRO EXAMPLE OF LONGEST EDGE











### DOCUMENTATION OF TOOL XT_BEDGE.EXE



Author: THG

Date: 12.04.2005



Requirements:

xT_BEDGE.CFG, Getfrm32.dll



Description:

XT_BEDGE determines the longest edge of a shape (also of rectangles) and writes this value back

to the opt2dat item 'lisealr'. Viewers like PLANEDIT or XPATDIS should be configured to display

the bottom-edge in Lenhard-Modecounterclockwise(0 bottom, 1 right, 2 top, ...). To configure this in

XPATDIS > editxpatdis.cfgand setdispedge=3.

PLANEDIT > edit registry and set HKEY_LOCAL_MACHINE\SOFTWARE\Albat +Wirsam\PlanEdit\Pattern >ShowEdge> 3.



History:

12.04.2005 THG - first release 1.0.0.1


