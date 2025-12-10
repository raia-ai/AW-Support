---
title: "EN-CONFIG-AW_License_System_Bypass"
source: "EN-CONFIG-AW_License_System_Bypass.pdf"
tags: ["A+W", "License Bypass", "Software Configuration", "Emergency License", "LicenseClientServer.dll", "TOTP", "Internal Document", "Software for Glass"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Internal configuration instructions for bypassing the A+W License System. This document details an emergency 'back door' feature that allows unrestricted use of A+W software for a temporary period by granting all licenses to a client."
long_description: "This internal document provides detailed configuration instructions for utilizing the A+W License System bypass. This feature acts as an emergency 'back door' built into the `Albwir.CB.LicenseClientServer.dll` (version 13.4.2544 or higher). When activated, the bypass allows a client machine to grant any license request without contacting the license proxy or server. This permits unrestricted use of all A+W software modules in their highest variants. The guide outlines a two-step activation process: first, generating a time-based one-time password (TOTP) from an internal A+W web page, and second, using the `LicenseBypassManager.exe` tool to activate the bypass on the client machine with the generated code and a specified expiration date. It includes instructions for both GUI and command-line activation, technical notes for developers on the encryption mechanism, and troubleshooting for known problems like time synchronization issues."
---

# A+W Configuration Instructions: A+W License System bypass

**-INTERNAL-**

*A+W - Software for Glass*

---

---
## Change history

| Date       | Author | Comments         | Version |
| :--------- | :----- | :--------------- | :------ |
| 2022-11-4  | EB     | Original version | 1.0     |
| 2022-11-7  | PK     | Extensions       | 1.1     |

## Content

1.  **Use of A+W license system bypass**
    1.1. Introduction
    1.2. Prerequisite
2.  **A+W license system bypass manager**
    2.1. Creating a verification code
    2.2. Activating the license bypass
    2.3. Notes for developers
    2.4. Known Problems

---

## 1. Use of A+W license system bypass

### 1.1. Introduction

All licensed applications/modules communicate with the license proxy via the client component that is represented by `Albwir.CB.LicenseClientServer.dll`; the license proxy, in turn, communicates with the license server components.

