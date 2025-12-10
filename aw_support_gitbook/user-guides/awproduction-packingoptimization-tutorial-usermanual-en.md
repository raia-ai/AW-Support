---
title: "EN_UM_AWProduction_11"
source: "EN_UM_AWProduction_11.pdf"
tags: ["A+W Production", "Packing Optimization", "Software Reference", "Tutorial", "Barcoding", "Master Data", "PackView", "Glass Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a user manual for A+W Production software, focusing on the Barcoding and Packing Optimization modules. It provides both a software reference and a step-by-step tutorial for managing master data, optimizing packing configurations, and visualizing results in the PackView tool."
long_description: "This comprehensive user manual covers two key modules of the A+W Production software suite: Barcoding and Packing Optimization. The first part of the document serves as a Software Reference for Master Data related to barcoding. It details the fields for employee information, barcodes, column assignments for processing stations, and a post-processing tool for correcting data errors. The second, more extensive part, is dedicated to the A+W Production Packing Optimization module. It begins with a tutorial that explains the basic concepts, master data setup (using *.RUL and *.VAL files), and various packing parameters. The tutorial then provides detailed, step-by-step instructions on creating and managing packing groups, running optimizations, and using the PackView visualization tool. PackView functionalities are thoroughly explored, including different views (3D, top, side), editing modes (full screen, editing, expert, free edit), and advanced operations like moving units/stacks, using the clip list, and handling invalid placements. The final section is a Software Reference for the Packing Optimization module, offering a systematic breakdown of all menus, dialogs, icons, and functions available in the software, from creating packing rules to interpreting the info line in PackView. The manual is intended for users who manage and execute packing operations in a glass, window, or door manufacturing environment."
---

# A+W Production Barcoding - Software Reference

---
## Master Data

**Name**
Enter the name of the employee in this field.
*Technical info: database field: PersonName*

**Description**
In this field you can enter additional information relating to the employee.
*Technical info: database table: Beschreibung*

**Employee no.**
Enter the employee number in this field. This number will be provided to you by the Payroll office or Accounting.
*Technical info: database table: PersonKey*

**Barcode**
Enter the barcode for the employee in this field. It is compiled from the number and the employee number. Example: There is a 9-digit barcode, the employee's number is 60 and the personnel no. is 51 - the barcode is then 600000051.
*Technical info: database field: Personbc*

**Additional information**
⇨ Tutorial, "Employee" on page H-929

