---
title: "AUW_Configuration_FlipSheetsInProduction"
source: "AUW_Configuration_FlipSheetsInProduction.docx"
tags: ["configuration", "production", "flip-sheets", "AUW", "operations", "workflow", "SOP", "manufacturing", "setup", "process-control"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a structured configuration guide for managing Flip Sheets in a production environment at AUW. It outlines required settings, roles, workflows, and step-by-step procedures, including dependencies and validations. The content has been converted to clean, UTF‑8 Markdown with clear sections, lists, and tables to support search and retrieval in a vector store."
long_description: "This reference consolidates the complete configuration and operating guidance for Flip Sheets in the AUW production environment. It is intended for system administrators, process owners, and operations staff who configure, maintain, and execute Flip Sheet workflows. The material covers prerequisites, environment assumptions, and the underlying business rules that govern when and how Flip Sheets are created, validated, posted, and archived. It also captures field-by-field settings, role-based permissions, statuses and transitions, and any integration points with upstream and downstream modules (for example, inventory, scheduling, or quality). Where the source included tables, these have been rendered using GitHub-Flavored Markdown for clarity and fidelity; lists have been normalized to Markdown bullets and ordered steps, and headings have been standardized so that primary sections appear as level-2 headers and sub-sections as level-3 or emphasized text. In addition to configuration steps, the guide includes exceptions, validations, and decision points that affect the Flip Sheet lifecycle in production. The layout has been semantically reconstructed to preserve all original content while improving readability and consistency for downstream indexing. This file is suitable for programmatic ingestion into an embedding-based knowledge system and can serve as the authoritative reference for training, troubleshooting, onboarding, and audit support."
---

## Scheiben gewendet produzieren
### History

| Date | Author | Modification/remarks | Version |
| --- | --- | --- | --- |
| 2018-01-10 | DLA | Issue | 1.0 |
|  |  |  |  |

## Content

## Einführung
Stücklisten und SN Zeichnungen werden immer aus Ansicht Außen beschrieben. Bei der Produktion kann es vorkommen, dass Scheiben gewendet produziert werden. Dies beginnt beim Zuschnitt von Lagerplatten mit Beschichtung oder Struktur. Beschichtungen sind im Zuschnitt in der Regel oben und Strukturen unten. Hat eine Scheibe nun eine Beschichtung in Richtung der Innenseite oder eine Struktur in Richtung der Außenseite, dann muss die Scheibe im Zuschnitt gewendet werden.
Neben Beschichtung und Struktur gibt es noch die sogenannte Siebdruck-Funktion, wo Scheiben mit speziellen Bearbeitungen nach ihrer Luft- bzw. Zinnseite für den Zuschnitt gewendet werden können.

In diesem Dokument werden Funktionen beschrieben, die über das Wenden von Struktur, Beschichtung oder Siebdruck für den Zuschnitt hinausgehen. Dies betrifft das Wenden für andere Produktionsschritte, gewendete Bilder für die Papiere aber auch dauerhaftes Wenden direkt in den SN Zeichnungen für Maschinenansteuerungen.
Voraussetzung für diese Funktion ist eine SN Zeichnung an der Position. Zudem werden Scheiben für den gesamten Produktionsprozess gewendet und diese Wendung entspricht der Wendung im Zuschnitt.
Zusätzlich muss der Schalter [ALCIM_SHAPE / **SN_FLIPMODE] = 0** gesetzt werden, damit dies funktioniert. Dieser Schalter existiert aus Gründen der Rückwärtskompatibilität.
## Scheiben wenden für den Druck
Die Information ob eine Scheibe für den Zuschnitt gewendet wird oder ermittelt die Feinplanung und schreibt diese Information in das Feld FEIN_TEILE.CUTMIRROR. Zusätzlich wenn über ein BLOCK Eintrag optimiert wird, wird diese Information durch die Feinplanung in den BLOCK Satz geschrieben.
Wird nicht optimiert benötigt man eine Handzuschnittsliste, damit dort die SN Skizze gewendet dargestellt wird, muss ein gewendetes Bild erzeugt werden. Dazu kann über den Schalter [ALCIM_SHAPE / SKETCHFLIPPINGVIEWS] SN Konstruktions-Ansichten definiert werden, die nach den Regeln gewendet werden sollen.
Will man auch Bilder aus anderen Ansichten gewendet darstellen, können in diesem Schalter auch weitere Ansichten in eine kommaseparierten Liste aufgenommen werden.
Mögliche Werte: POINTS, SKETCH, GEOMETRY, EDGE, INCONT, TARGETPRODUCT, WORK, DRILL, DRILL2, DRILL3, DRILL4, DRILL5, GRIND, UNICUT, PACKET

## Scheiben wenden in SN Zeichnung
Für die Produktion nach dem Zuschnitt kann es vorkommen, dass eine Scheibe fest in seiner SN Zeichnung gewendet dargestellt werden muss. Dies ist nötig, will man im SN-Live Bild an einem A+W Production Terminal die Scheibe gewendet darstellen und soll die Scheibe an einer Bearbeitungsmaschine gewendet produziert werden. Voraussetzung für die Bearbeitungsmaschine, es muss sich um einen Treiber handeln, der über eine SN Datei gesteuert wird (z.B. BENTELER, INTERMAC,…).
Um die SN Ansichten zu bestimmen, die gewendet werden sollen, wird derselbe Schalter [ALCIM_SHAPE / SKETCHFLIPPINGVIEWS] verwendet. Zusätzlich wird über einen weiteren Schalter erzwungen, dass die Änderung auch in die SN Zeichnung zurück geschrieben wird: [ALCIM_SHAPE / **SN_CLOSEMODE]=4**.

Die Original SN Zeichnung wird umbenannt in *.org.sn und die Änderungen werden im Originalname gespeichert. Diese Sicherungskopie ist notwendig, da bei erneuter Geometrieberechnung diese herangezogen wird.
## Scheiben benutzerdefiniert wenden
Die aktuelle Lösung wendet Scheiben nach Beschichtung, Struktur oder Zinn-/Luftseite. Jetzt kann es aber vorkommen, dass die Gegenscheibe einer solchen Scheibe auch gewendet werden soll.
Dies ist notwendig um das spätere Handling zu vereinfachen. Scheiben werden gleich beim Zuschnitt gedreht und müssen im späteren Produktionsverlauf nicht erneut gedreht werden um somit Schäden vermeiden. Eine andere Anforderung wäre, für unbeschichtete Scheiben die Richtung der Senkung von Bohrungen so auszuwerten, dass im Zuschnitt eine Scheibe so gewendet wird, dass die Senkbohrungen von unten ausgeführt werden. Das hat den Vorteil, dass sich variierende Glasdicken nicht auf die Präzision der Senkbohrungen auswirkt (Bolzenhalterungen, die absolut plan zur Glasoberfläche gefertigt werden müssen).
Um dies zu erreichen, kann für jedes Teil der Stückliste über eine StoredProcedure ermittelt werden, ob dies gewendet werden soll. Das Ergebnis dieser SP wird nur dann verwendet, wenn das Stücklistenteil keine explizite Wendung oder Unterlassung vorschreibt. Damit nachfolgende Prozesse (Feinplanung, Reportdruck,…) auf das Ergebnis zugreifen können, kann das Ergebnis in das Feld **POOL_MODELL.SPIEGELUNG** geschrieben werden.
Aktiviert wird diese SP über den Schalter **[ALCIM_SHAPE / CALL_GEOMETRY_COMMAND]**
0 – SP wird nicht ausgeführt
1 – SP wird ausgeführt, POOL_MODELL.SPIEGELUNG wird geschrieben
2 – SP wird ausgeführt, POOL_MODELL.SPIEGELUNG wird nicht geschrieben
Wenn aktiviert wird folgende SP ausgeführt:
***cu_alcimsndraw_command** (**sp_auftnr** INT, **sp_pos** INT, **sp_u_pos** INT, **sp_teile_nr** INT) RETURNING INT*
Diese SP hat folgende Rückgabewerte:
0 - nicht ausgewertet (die Wendung ist unbestimmt, die interne Logik ist wirksam)
4 - es wird links nach rechts gewendet (wenn Scheibe unbeschichtet und strukturlos ist)
8 - es wird kopfüber gewendet (wenn Scheibe unbeschichtet und strukturlos ist)
12 - es darf nicht gewendet werden (wenn Scheibe unbeschichtet und strukturlos ist)

Damit das Ergebnis der SP auch von der Feinplanung verwendet wird, muss **POOL_MODELL.SPIEGELUNG** gesetzt werden und der versteckte Feinplanungsschalter **[FEIN_SPECIALS / USESPIEGELUNG]** aktiviert werden.
*INSERT INTO PARAMETER (**bereich**,** **eintrag**,** **nummer**,** **typ,** **text**) VALUES ('FEIN_SPECIALS',** **'USESPIEGELUNG'** **,0** **,0** **,1);*

Die Richtung einer erzwungenen Wendung aus der Zuschnittslogik wird über den neuen Konfigurationsparameter [ALCIM_SHAPE / SN_FLIPDIRECTION] festgelegt. Er hat folgende Werte
0 - nicht konfiguriert (wendet rechts nach links, wenn nötig)
1 - wendet rechts nach links, wenn nötig
2 - wendet kopfüber, wenn nötig
