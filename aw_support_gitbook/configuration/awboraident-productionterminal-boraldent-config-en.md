---
title: "A+W Production Terminal - Boraldent Laserbird Interface Configuration"
source: "EN-CONFIG-A+W Boraldent LaserBird.docx"
tags: ["A+W", "Production Terminal", "Boraldent", "Laserbird", "Interface", "Configuration", "Glass Processing", "Hegla", "Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This internal document provides configuration instructions for the interface between the A+W Production Terminal and the Hegla Boraldent Laserbird machine. It details the setup required in A+W Business and the A+W Production Terminal to enable the lasering of bird-friendly patterns onto glass."
long_description: "This document serves as a technical guide for configuring the connection between an A+W Production Terminal and a Hegla Boraldent Laserbird machine. The Laserbird machine is used to laser specific patterns onto glass for bird protection. The guide covers the necessary setup within the A+W software ecosystem. It begins by explaining how the bird-friendly pattern process is managed in A+W Business, where it is treated as a 'logo processing' type. It then details the required components and configuration steps for the A+W Production Terminal, including the creation of a new button, the implementation of a special panorama script ('ProcessingWithLaserBird.cs'), and the setup of an XML file for parameter templates. The document also addresses the handling of different glass shapes, mapping between A+W and Hegla catalogues, and a special procedure for shapes requiring a frame. Finally, it mentions the Hegla LaserBird Simulator tool for testing the interface communication. The configuration involves setting IP addresses, ports, and file paths in the A+W Parameter Administrator."
---

# A+W Production Terminal - Boraldent Laserbird Interface

---
## Change history

| Date       | Author      | Comments            | Version |
| :--------- | :---------- | :------------------ | :------ |
| 2024-02-21 | Peter Kühn  | First Draft Version | 1.0     |

## 1. General

This document is about the configuration of the connection between an A+W Production Terminal Processing and the Hegla Boraldent Laserbird.

The LaserBird machine is able to laser different pattern into the glass for bird protection.

This Feature is developed in DevOps Feature: 101781 / PF Ticket: [AW-143731]

## 2. Configuration

### 2.1. A+W Business

In A+W Business, the LaserBird is treated with the processing Logo.

