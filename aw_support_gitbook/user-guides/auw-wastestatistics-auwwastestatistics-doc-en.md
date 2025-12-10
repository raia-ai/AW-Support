---
title: "AUW_Description_WasteStatistics"
source: "AUW_Description_WasteStatistics.docx"
tags: ["A+W Production", "Waste Statistics", "AUW_WasteStatistics", "Jumbo", "Lot", "JumboSize", "DYNOPT", "A+W Realtime Optimizer"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document describes the standard A+W Production waste statistics reports AUW_WasteStatistics_Lot, AUW_WasteStatistics_Jumbo, and AUW_WasteStatistics_JumboSize. It explains where the Crystal Reports files are located, how to integrate them, and the parameters that drive each report, including optional grouping, table-specific filtering, and top-N glass type selection. It details the AUW_WasteStatistics_Lot evaluation methods, the data sources and views used, and A+W Realtime Optimizer and DYNOPT interactions. Guidance is provided for configuration (e.g., MINRESTBLATT and WriteStockPlateStatistic), version prerequisites, and for understanding key metrics such as surface, rejects, lites, and yield."
long_description: "This document provides a comprehensive description of the A+W Production waste statistics, covering three standard Crystal Reports: AUW_WasteStatistics_Lot.rpt, AUW_WasteStatistics_Jumbo.rpt, and AUW_WasteStatistics_JumboSize.rpt. It begins with version history and then clarifies where the reports are installed (P:\Reports\) and how they are typically integrated into A+W Production. Because AUW-delivered report files are overwritten during setup, any customer-specific adaptations must be saved under a different name that replaces the “AUW” prefix with a customer-specific tag.

The document outlines the runtime parameters common to the statistics: the evaluation period, grouping mode, optional cutting table filtering, and limiting the number of glass types per group to a top-N subset ranked by area. For AUW_WasteStatistics_Lot specifically, an additional evaluation method parameter is supported. Two distinct approaches are described: “Planned yield,” which reflects the detailed scheduling lots as assigned to cutting tables (including manual cutting, with special handling for lots without a table or those spanning multiple tables), and “Closest true yield,” which attempts to mirror actual production by including what was cut through A+W Realtime Optimizer and assuming remaining lots were cut elsewhere. Important caveats are called out for table optimization, table 9 logic, and differing optimizer parameters that complicate direct comparisons between the two methods.

Data lineage is explained for each report. AUW_WasteStatistics_Lot is driven by table XOPT_STATISTIK via the pre-compressing view AUW_WasteStatistics_Lot. It records one row per cutting lot (optimized, manual, or table optimization). Detailed scheduling writes the initial results; A+W Realtime Optimizer then updates records during cutting with timestamps and events (e.g., breakage, rush orders), while the original scheduling results remain available. Because DYNOPT marks lots as resolved without writing its detailed results to XOPT_STATISTIK, this report is not suitable when DYNOPT is in use.

AUW_WasteStatistics_Jumbo focuses on stock plates. Up to version 5.4 it included only A+W Realtime Optimizer data; from version 5.5 onward, detailed scheduling also populates the statistics. Residual plates cut via a remaster (connected to A+W Realtime Optimizer) are excluded from the remainder. Residual plates not cut via a remaster are split into “Loss” (smaller than a configurable minimum length) and “Potentially usable” (greater than or equal to the minimum). The minimum length is controlled by the MINRESTBLATT parameter (in micrometers, default 1,200,000) in AUW_SETTINGS, which must be defined for the report to return data. The report also indicates the proportion of DYNOPT for each glass type in a gray line. For A+W Realtime Optimizer, the XOPTON.CFG setting WriteStockPlateStatistic determines when entries are written to XOPT_STATISTIK_JUMBO (modes 0–3).

AUW_WasteStatistics_JumboSize provides the same statistics as Jumbo but grouped by stock plate size. Residual plates are summarized per glass type and can be optionally hidden; to align comparisons with the Jumbo report, residual plates should be shown. Data collection uses the AUW_WasteStatistics_JumboSize view, and DYNOPT results are not shown separately. This report is available from version 5.5.

Finally, the document explains how to interpret key measures: Surface (including residual plate losses), Rejects, Manual Entry, Lites, and Yield, and clarifies how gray versus black lines represent DYNOPT-only versus total results, respectively."
---

# Description Waste Statistics

Description Waste Statistics

## History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 11.04.2014 | DLA | Issue | 1.0 |
| 13.05.2014 | DLA | Adaptation | 1.1 |
| 30.01.2015 | DLA | New report AUW_WasteStatistics_JumboSize | 1.2 |
| 15.09.2015 | DLA | Translation | 1.3 |
|  |  |  |  |

## Content

## Where can the waste statistcs be found?

In A+W Production we have three standard waste statatistcs reports AUW_WasteStatistics_Lot.rpt, AUW_WasteStatistics_Jumbo.rpt and AUW_WasteStatistics_JumboSize.rpt. The reports are located in P:\Reports\ and can be integrated in A+W Production list or reports.

Like all AUW reports files, they will be overwritten during setup. So don’t change the reports, for a custoimizing vesion save the report with a name where the AUW short cut AUW is replaced with a short cut of the customer.

## What are the parameters required by the waste statistics?

The following parameters will be used in the reports:

**Period of time**

date range in which the data are determined.

**Group**

Selecting a grouping mode for the determined data:
[table], [table/year/month], [year/month], [glass/thickness]
Within the group the data are sorted in descending order according to area.

**Table ID**

Entering the ID of a cutting table is available as an option. Without this the data of all tables in the specified period of time are displayed.

**x types of glass**

Will you not see all types of glass, you can limit the selection with this parameter. Per group so many types of glass displayed as entered. These are the first types of glass of the group, thus with the largest area.

AUW_WasteStatistics_Lot.rpt has one more parameter: Evaluation method.

## AUW_WasteStatistics_Lot

The report AUW_WasteStatistics_Lot.rpt has two evaluation methods:

**Planned yield (Geplante Ausbeute)**

This method displays the result of the detailed scheduling lots where cutting tables are assigned. Manual cutting lots are considered. Lots without an assigned cutting table are suppressed and lots with several tables (e.g. table 9 logic) are grouped under table id ---.

**Closest true yield (Realitätsnahe Ausbeute)**

This method displays all what is cut through A+W Realtime Optimizer and all that has not been cut. It is assumed that lots not cut through A+W Realtime Optimizer where cut anywhere, e.g. on a cutting table where no A+W Realtime Optimizer exist. So it could happen that in statistic of yesterday the result of detailed scheduling is calculate if the lots will be cut with A+W Realtime Optimizer tomorrow. In the statistic table the cutting time is the time of detail scheduling until the lot is cut with A+W Realtime Optimizer.

The direct comparison of both methods works only if no table optimization is in use. For table optimization the original statistic records are mark as resolved in table optimization and a new record for table optimization are inserted. The cutting timestamp of the resolved and the cut records are different so a direct comparison is not possible. Also the use of table 9 logic in detailed scheduling or the use of different optimization parameter in A+W Realtime Optimizer make a direct comparison difficult.

### Where the data come from?

The report AUW_WasteStatistics_Lot.rpt gets its data from table XOPT_STATISTIK. To display the VIEW AUW_WasteStatistics_Lot is used which already pre-compressed the data.

In this table for each cutting lot a record is stored, whether optimized, manual cutting or table optimization. The detailed scheduling store the result in the table and A+W Realtime Optimizer manipulates the records during cutting (cutting time, breakage, rush orders,…), the original detailed scheduling results are still to be found. Different stock plate sizes are not considered in this table.

Is DYNOPT in use, this report can not be used. The lots which are cut with DYNOPT are marked as resolved, but the DYNOPT result isn’t stored in this table, it would be too inaccurate.

### Examples

## AUW_WasteStatistics_Jumbo

This Report is exactly to stock plates. Up to version 5.4 you found only data of A+W Realtime Optimizer, but since version 5.5 the detailed scheduling also stores its data for this report.

Residual plates which are cut over a remaster (connected to A+W Realtime Optimizer) are been excluded from the rest. Residual plates which are not cut over a remaster are displayed in two categories on the report: Loss and potentially usable. Loss are residual plates which are smaller than the minimum length and potentially usable are residual plates which are greater than or equal than the minimum length. The minimum length is a global AUW parameter in micrometer, standard value is 1200000. This parameter must exist, without these no data are displayed.

The report indicates the proportion of DYNOPT in an additional line for each glass type in gray font. Has the complete glass type produced via DYNOPT, one grey line is shown.

### Where the data come from?

The report AUW_WasteStatistics_Jumbo.rpt gets ist data from table XOPT_STATISTIK_JUMBO. To display the VIEW AUW_WasteStatistics_Jumbo is used which already pre-compressed the data.

```sql
SELECT parameter_value FROM auw_settings WHERE module_name = 'REPORT' AND parameter_name = 'MINRESTBLATT';
UPDATE auw_settings SET parameter_value = '1200000' WHERE module_name = 'REPORT' AND parameter_name = 'MINRESTBLATT';
```

In the statistics data you find data for each stock plate. You see which stock plate size was used and which are reused with a remaster.

For A+W Realtime Optimizer you have to configure in XOPTON.CFG how the statistics data should be written:

```ini
[Cutting] WriteStockPlateStatistic = <INTEGER> [0,1,2,3] Default=0
```

- 0 : No information for cut Stockplate will be written to table XOPT_STATISTIK_JUMBO.
- 1 : information for cut Stockplate will be written to table XOPT_STATISTIK_JUMBO if the pattern is shown by XTV.
- 2 : information for cut Stockplate will be written to table XOPT_STATISTIK_JUMBO if the pattern isconfirmed by XTV.
- 3 : information for cut Stockplate will be written to table XOPT_STATISTIK_JUMBO if the transfer of the cutting code has been started for the pattern. You may use this mode if no XTV is installed.
### How are the data to be understood?

Surface is the total area including the residual plates of the loss column. Rejects and Manual Entry are included in Surface and Lites, it is used for identify how big the corresponding proportion is. For Yield the Surface with Lites is set in relation.

Result in gray are the results from DYNOPT, results in black is the total result. If there is only black result, there is no DYNOPT. With only gray result for this type of glass just DYNOPT exists.

### Examples

## AUW_WasteStatistics_JumboSize

These statistics correspond to the statistics AUW_WasteStatistics_Jumbo grouped by stock plate size. Residual plates are summarized in one line for each type of glass and can be hidden optional. If you want to compare this list with AUW_WasteStatistics_Jumbo, you have to show the residual plates, since otherwise the result would be falsified.

For data collection the VIEW AUW_WasteStatistics_JumboSize is used. DYNOPT results are not displayed separately. This list is available since version 5.5.

### Examples
