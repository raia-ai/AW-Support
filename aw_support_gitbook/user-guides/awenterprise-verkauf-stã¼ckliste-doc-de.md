---
title: "DE_AWEnterprise_Verkauf_4_5"
source: "DE_AWEnterprise_Verkauf_4_5.pdf"
tags: ["A+W Enterprise", "Verkauf", "Stückliste", "Software-Referenz", "Auftragserfassung", "Packmittelplanung", "Sprossenerfassung", "ERP", "Glasindustrie", "Bedienungsanleitung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist eine Softwarereferenz für das Modul A+W Enterprise Verkauf. Es beschreibt detailliert die Funktionalitäten rund um die Stücklistendarstellung, Auftragserfassung, Bearbeitungsparameter, Sprossenerfassung und Packmittelplanung. Es richtet sich an Anwender und Administratoren des Systems."
long_description: "Diese Softwarereferenz bietet eine umfassende Beschreibung des A+W Enterprise Verkaufsmoduls, Version 4.00/02-2020. Der Schwerpunkt liegt auf der Erstellung und Verwaltung von Stücklisten (Stückliste) und den damit verbundenen Prozessen in der Auftragserfassung. Das Dokument gliedert sich in mehrere Hauptbereiche. Zunächst wird die 'Stücklistendarstellung' erläutert, die den Produktaufbau und die Produktionsskizze umfasst und visuelle Darstellungen sowie Bemaßungen von Artikeln und Bearbeitungen zeigt. Es werden die verschiedenen Register wie 'Produktaufbau', 'Produktionsskizze' und 'Akt. Stücklistenebene' mit ihren jeweiligen Feldern und Funktionen detailliert beschrieben. Ein weiterer großer Abschnitt widmet sich den Bearbeitungsparametern, in dem Dialoge wie 'Alle Parameter/Skizze' erklärt werden. Hier können Benutzer spezifische Einstellungen für verschiedene Bearbeitungsarten wie Bohrungen, Kantenschliffe, Siebdruck und mehr vornehmen. Themen wie 'Kantenzuordnung', 'Einstand' und 'Stufenerfassung' für Spezialgläser werden ebenfalls behandelt. Das Dokument geht auch intensiv auf die 'Sprossenerfassung' ein, die die Konstruktion von Sprossen in ISO-Artikeln ermöglicht. Es werden der 'Sprosseneditor' und zugehörige Dialoge zur Definition von Bohrpunkten und Abstandsmaßen vorgestellt. Abschließend wird die 'Packmittelplanung' behandelt, mit der die benötigten Packmittel (z. B. Gestelle) für einen Auftrag automatisch geplant werden können, basierend auf verschiedenen Algorithmen und benutzerdefinierten Vorgaben. Ergänzt wird die Referenz durch eine Beschreibung der 'Anmerkungen'-Funktion, die es erlaubt, interne Informationen zu Vorgängen, Kunden oder Artikeln zu hinterlegen. Das Dokument dient als Nachschlagewerk für die tägliche Arbeit mit der Software und zur Konfiguration spezifischer Parameter."
---

# Softwarereferenz: Stückliste

Mit `<Shift>+<F2>` wechseln Sie zum Register Produktaufbau.
⇨ "Stücklistendarstellung - Produktaufbau" auf Seite D-199

---
## Register Produktionsskizze

Die Produktionsskizze zeigt die bemaßte Skizze der Position mit den Bearbei-
tungen. Mit Klick auf die Skizze öffnen Sie eine vergrößerte Ansicht der Skizze
im Dialog SNLive Zoom. In diesem Dialog können Sie Teile der Skizze weiter
vergrößern.

Je nach Konfiguration von A+W CAD Designer (Shapes) werden in der Skizze
Pfeile eingeblendet, die Richtung des Produktaufbaus in den Querschnitten
anzezeigen.

Die Bezeichnungen und Markierungen zeigen die Positionierung und die Be-
arbeitungsart an, z. B. welche Kanten einer Scheibe bearbeitet werden und ob
die Kanten geschliffen oder poliert werden, usw. Die Markierungen der Bear-
beitung, die im Register Parameter gewählt ist, werden in der Aufsicht-Skizze
rot hervorgehoben, z. B. Eckabschnitt.

**H, H(n)** Höhe der Scheibe. Je nach Modell existieren verschiedene Angaben
für die Scheibenseiten. *H* steht für die Gesamthöhe und *H(n)* für eine Teilhöhe
von H. Die Parameter sind durchnummeriert. Die Zahl in den eckigen Klam-
mern gibt die Höhe der Scheibenseite in Millimeter an.

**W, W(n)** Breite der Scheibe (aus dem Englischen: W = width = Breite). Je
nach Modell existieren verschiedene Angaben für die Scheibenseiten. *W* steht
für die Gesamtbreite und *W(n)* für eine Teilbreite von W. Die Parameter sind
durchnummeriert. Die Zahl in den eckigen Klammern gibt die Breite der Schei-
benseite in Millimeter an.

### Fußbereich

Die Schaltflächen im Fußbereich sind zum Dialog *Stücklistendarstellung –
Stücklistenaufbau* beschrieben.
⇨ "Stücklistendarstellung - Stücklistenaufbau" auf Seite D-196

---
*A+W Enterprise Verkauf, D-201, 4.00/02-2020*

---

# Stücklistendarstellung – Akt. Stücklistenebene

**Pfad:** Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld B.Art > `<F5>`

