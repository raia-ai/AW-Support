---
title: "EN_AWProduction_Terminal_1.50"
source: "EN_AWProduction_Terminal_1.50.pdf"
tags: ["A+W Production Terminal", "Software Manual", "Glass Manufacturing", "Window Production", "Door Manufacturing", "MES", "Production Control", "Tutorial", "Software Reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a user manual for the A+W Production Terminal, a software solution for managing production processes in the glass, window, and door manufacturing industry. It provides a detailed tutorial and software reference for various terminal modules."
long_description: "The A+W Production Terminal user manual serves as a comprehensive guide for operators and end-users of the A+W software suite. The document is divided into two main parts: a Tutorial and a Software Reference. The Tutorial section is designed for new users, offering a step-by-step introduction to the various production terminal modules, including Terminal IG (Insulating Glass), Manual Cutting, Georgian Bars, Order, Processing, TG (Toughened Glass), and LG (Laminated Glass). It explains the purpose of each terminal, its user interface, operating sequences, and how to handle common situations like material shortages or defects. The goal is to help users perform their work more efficiently by visualizing and controlling individual processing steps. The Software Reference section provides a detailed, technical breakdown of all software functions, dialogs, menus, and terms. It covers module operation, key combinations, reporting, and help functions. This part is intended as a quick reference for experienced users to look up specific functionalities like registering rejects, loading remakes, or changing machine statuses. The manual is published by A+W Software GmbH and is crucial for the effective operation of their production control system on the shop floor."
---

# A+W Production Terminal

A+W - Software for Glass, Windows and Doors

---
## Introduction

The introduction contains information on editorial notes.

### Revision Overview

| User Manual Version / Date | Description |
| :--- | :--- |
| 1.50 / 01-2023 | Various additions |
| 1.20 / 09-2014 | Part Georgian Bars added |
| 1.10 / 03-2013 | Part LG and Edit added |
| 1.00 / 01-2012 | Original Version |

### Editorial

The editorial contains information on the following topics:
- Remarks concerning this document
- Copyrights
- Trademarks
- Contact

#### Remarks concerning this document

This document is intended for end users of A+W Production Terminal.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation is only informative and is subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

The representation of this document requires full scope of A+W Production Terminal.

#### Copyrights

© 2023, A+W Software GmbH, any right, also the right of reprint, the production of copies and of the translation, is reserved.

The documentation must be copied, completely or in part, saved, or transferred only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH prior approval in writing.

#### Trademarks

Any designation of hardware and software being mentioned in the documentation can also be registered trademarks or other commercial rights of third parties being protected by law. Rights of third parties being protected by law are to be observed insofar.

#### Contact

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
- **Tel:** +49 6404 2051-0
- **Fax:** +49 6404 2051-877
- **Email:** zentrale@a-w.com
- **Web:** http://www.a-w.com

## Contents

- **Introduction**
    - Revision Overview
    - Editorial
    - Contents
- **Tutorial**
    - Overview
    - Documentation
    - Production Terminals
    - A+W Production Terminal IG - Overview
    - Using Terminal IG-In
    - Using Terminal IG-Assembly
    - Using Terminal IG-Out
    - Overview A+W Production Terminal Manual Cutting
    - The use of Terminal Manual Cutting.
    - Overview A+W Production Terminal Georgian Bars
    - The use of Terminal Georgian Bars.
    - Overview A+W Production Terminal Order
    - Using Terminal Order
    - Overview A+W Production Terminal Processing
    - Using Terminal Processing
    - Overview A+W Production Terminal TG
    - Using Terminal TG-In
    - Overview A+W Production Terminal TG-Out
    - Using Terminal TG-Out
    - Overview A+W Production Terminal LG
    - Using Terminal LG-In
    - Using Terminal LG-Assembly
    - Overview A+W Production Terminal Edit
    - Using Terminal Edit
- **Software Reference**
    - Module Operation
    - Closing the Program
    - General Overview
    - Overview: Terminal IG
    - Overview: Terminal Manual Cutting
    - Overview: Terminal Georgian Bars
    - Overview: Terminal Order
    - Overview: Terminal Processing
    - Overview: Terminal TG
    - Overview Terminal LG
    - Overview Terminal Edit
    - Reports
    - How to Use the Help Function
    - Log Entries for this Session
    - Language Selection
    - About A+W Production Terminal
- **Index**
    - Index

## Tutorial

### Overview

The training on the A+W Production Terminal modules is designed for employees working at the corresponding registration points on the shop floor.

We are going to convey to the users how our software shall help him perform his work more efficiently and more easily, and what to do in case of defects etc.

**Sets of Topics**
This tutorial offers the following sets of topics:
- Production Terminals
- A+W Production Terminal IG - Overview
- Overview A+W Production Terminal Manual Cutting
- Overview A+W Production Terminal Order
- Overview A+W Production Terminal Processing
- Overview A+W Production Terminal TG
- Overview A+W Production Terminal LG

> **Required knowledge**
> Basic IT knowledge and/or Windows knowledge are prerequisite for using the corresponding modules. The user has to know what the physical work processes and process steps at the terminal in question look like, and how to execute them.

### Documentation

The following documentation is available for this training:

| Type | Description |
| :--- | :--- |
| **Hand-out** | Printed training documentation for the participants |
| **PDF** | Complete documentation (Tutorial, Software Reference) |
| **Online help `<F1>`** | Context-sensitive dialog help for the software reference |

#### Tutorial Structure

This tutorial consists of sets of topics with several sessions each. Each session consists of the following elements:

- **Overview:** Each training session starts with an overview of the major topics:
    - Objectives: What shall be conveyed?
    - Benefit: What can this knowledge be used for?
    - Maxims: Which correlations are to be remembered?
- **Concepts:** Concepts and terms of the corresponding training session will be explained first. This is followed by examples and operating instructions.
- **Reading instructions:** The contents of a learning unit are based on the knowledge conveyed in the previous unit. We therefore recommend not to skip any learning units. If you are already familiar with a subject you should at least read the summary at the start of the session in order to bring the main details to mind.

### Display conventions

Individual elements of the sentences are displayed in a special form. Their meanings are:

| Convention | Meaning |
| :--- | :--- |
| *Italics* | marks character strings referring to software elements, e.g. the dialog *Vertical/horizontal pattern*. |
| **Bold** | marks phrases to be entered via keyboard, e.g. the number **0**. |
| `>` | shows the way to open a dialog, e.g. File > Import > Transfer file. |
| `[]` | Square brackets mark the buttons in the dialog, e. g. [OK] to save the data. |
| `<>` | Pointed brackets refer to keys or shortcuts on the keyboard, e. g. `<F1>` is used to open the online help. |

### Production Terminals

A+W Production Terminals are software modules of the production control system A+W Production which serve to check, enter, modify, control, and divert process steps in the work flow.

A+W Production Terminals visualize and control individual processing steps and can be configured individually. A+W Production Terminals can be used to print labels and reports online, and enter breakage including all necessary information. Operation of the production terminals is easy and uniform. These intelligent systems enable you to inform your customers of the current state of his products at any time.

Below please find a schematic diagram of a possible A+W Production Terminal landscape:

