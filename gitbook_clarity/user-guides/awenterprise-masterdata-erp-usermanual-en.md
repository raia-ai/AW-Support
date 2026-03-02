---
description: "EN-UM-AWEnterprise_5"
---


# Software Reference

---
## Article

### Alternative type
If you have selected a muntin construction type in the **Muntin Type** field, you can enter a second type here.
If different muntins are to be fit into an IG unit, A+W Enterprise will check at order entry whether the types of the muntins are compatible. If not, A+W Enterprise will check if the defined Alternative type is compatible. If not, A+W Enterprise will issue a message.
**Technical info:** numeric field, `<F9>`, DB field: artikel.sprfor

### Production doc.
In this field, you can select whether or not the print code should be pre-populated in the BOM at document entry when an article is replaced.
- Print code will be pre-populated in the BOM at document entry when the article is replaced.
- Print code will be pre-populated in the BOM at document entry when the article is replaced.

**Technical info:** toggle field, DB field: artikel.pdruckkz

### Spacer text no.
If **Article type IG** has been entered, you can enter the spacer text number.
The text formula is entered on the **Text management > Text creation > Text formula** menu. This formula is analyzed when text is created at order entry, and will be printed on the spacer.
**Technical info:** numeric field, DB field: artikel.rahmtextnr

### Can be label.
In this field you can select if a label can be created for the article.
- Article can be labelled.
- Article cannot be labelled.

**Technical info:** toggle field, DB field: artikel.barcflag

### LAMI/CR inheritance
If the selected Article type is **Processing for LAMI** or **Cast resin**, you can choose LAMI/cast resin inheritance. For production, processing steps have to be defined for the individual lites. To make order entry for cast resin and LAMI units easier, you can set the inheritance code here. This way, the processing can be entered on the top BOM level, and will be automatically inherited to the elements below. Processing will not be inherited to the commercial area or to pricing.
The following options are available for selection:
- **Yes:** The processing will be inherited to the BOM.
- **No:** The processing will not be inherited to the BOM.

**Technical info:** toggle field, DB field: artikel.bearbcopy

### Item text
In this field, you can select if the article appears in the item text at document entry.
- Article will appear as item text.
- Article will not appear as item text.

**Technical info:** toggle field, DB field: artikel.poskompltxt

---
*A+W Enterprise Master Data*
*B-401*

## Prices

**Master Data > Article > Prices tab**

