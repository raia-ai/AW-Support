---
description: "EN-CONFIG-AW_License_System_Bypass"
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

