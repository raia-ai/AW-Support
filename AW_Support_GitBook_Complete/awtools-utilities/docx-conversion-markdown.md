---
title: "AUW_Description_AWPLogoTableEditor"
source: "AUW_Description_AWPLogoTableEditor.docx"
tags: ["docx-conversion", "markdown", "AUW", "AWP Logo Table Editor", "user-guide", "documentation", "tables", "vector-store", "technical-writing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Description AUW AWPLogoTableEditor History Content A+W Production Logo Table Editor The AUW tool AWPLogoTableEditor connects to the LOGO table of an A+W Production database."
long_description: "Description AUW AWPLogoTableEditor History Content A+W Production Logo Table Editor The AUW tool AWPLogoTableEditor connects to the LOGO table of an A+W Production database. With the tool you can edit or delete existing logos and add new logos. Copy the Tool into a directory on a PC with an installed database driver and start AWPLogoTableEditor.exe. It doesn’t work with Windows XP. Each logo has a unique numeric ID, a numeric type to group logos, a comment and the logo itself. With the wrench button you can edit the database connect information, this is need to be done at the first start of the tool. DBType: Informix or SQLServer DBServer: Name of the Server. In INFORMIX the SETNET32 setting, in SQLServer <Server PC>\\<SQLServer Name> or only <Server PC> (depends on the configuration of the SQLServer. DBName: Name of the A+W Production database on the DB Server. DBUser and DB Password: Login information to connect to the database. Windows authentication for SQLServer isn’t supported. DBLocale: need only for Informix, e.g.: Client Locale=en_US.UTF8; Database Locale=en_US.UTF8 Trace information will be stored in a trace file and you can show it in a trace dialog. Open and hide the trace dialog with the trace dialog button Add Logo Enter new ID, logo type, logo comment: Select an image file, support format BMP, JPG, PNG, GIF, TIFF. In our standard we use BMP or JPG, this works with CrystalReports, other format isn’t tested. Edit Logo Click on the edit button behind the fields and the same dialog as in “Add Logo” opens to edit the field. Delete Logo With the delete button you can delete the selected logo. Save Image You can save a selected image to a file with the floppy disk button behind the image. It check the image type and if it is one of the supported ones (BMP, JPG, PNG, GIF, TIFF) you can save it."
---

## Description AUW AWPLogoTableEditor

History



| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 2015.09 | DLA | Issue | 1.0 |
|  |  |  |  |



Content



## A+W Production Logo Table Editor

The AUW tool AWPLogoTableEditor connects to the LOGO table of an A+W Production database. With the tool you can edit or delete existing logos and add new logos.

Copy the Tool into a directory on a PC with an installed database driver and start AWPLogoTableEditor.exe. It doesn’t work with Windows XP.

Each logo has a unique numeric ID, a numeric type to group logos, a comment and the logo itself.

With the wrench button you can edit the database connect information, this is need to be done at the first start of the tool.

DBType: Informix or SQLServer

DBServer: Name of the Server. In INFORMIX the SETNET32 setting, in SQLServer <Server PC>\<SQLServer Name> or only <Server PC> (depends on the configuration of the SQLServer.

DBName: Name of the A+W Production database on the DB Server.

DBUser and DB Password: Login information to connect to the database. Windows authentication for SQLServer isn’t supported.

DBLocale: need only for Informix, e.g.: Client Locale=en_US.UTF8; Database Locale=en_US.UTF8



Trace information will be stored in a trace file and you can show it in a trace dialog. Open and hide the trace dialog with the trace dialog button

### Add Logo

Enter new ID, logo type, logo comment:

Select an image file, support format BMP, JPG, PNG, GIF, TIFF. In our standard we use BMP or JPG, this works with CrystalReports, other format isn’t tested.

### Edit Logo

Click on the edit button behind the fields and the same dialog as in “Add Logo” opens to edit the field.

### Delete Logo

With the delete button you can delete the selected logo.

### Save Image

You can save a selected image to a file with the floppy disk button behind the image. It check the image type and if it is one of the supported ones (BMP, JPG, PNG, GIF, TIFF) you can save it.


