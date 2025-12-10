---
title: "EN-INST-AW_Softlock"
source: "EN-INST-AW_Softlock.pdf"
tags: ["A+W", "Softlock", "License Management", "Software Licensing", "Gemalto Sentinel", "License Server", "Rehosting", "Dongle", "Technical Guide"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical presentation by Jürgen Makowka from A+W, dated January 19, 2018, introducing 'Dongle News' and the A+W Softlock system. It covers the basics, advantages, disadvantages, and workflows for initial installation, updates, and moving (rehosting) the software-based license."
long_description: "This document is a presentation titled 'Dongle News' by Jürgen Makowka of A+W, dated January 19, 2018. It details the transition to and implementation of the A+W Softlock system, a software-based licensing solution powered by Gemalto Sentinel. The presentation contrasts this new system with traditional hardware dongles, outlining the pros and cons. Key topics include the introduction of 'Softlocks', improved license file request processes via a new website, and new administration tools. It provides detailed workflows for the first installation, license updates, and moving a license to a new machine (rehosting). The document explains critical concepts such as machine 'fingerprinting', the non-recyclable nature of softlocks, and the precise order required for license updates. It also specifies which system changes (e.g., renaming a computer) might invalidate a softlock and which are non-critical. The presentation is aimed at installation personnel (IP) and internal sales, providing step-by-step instructions, file paths for necessary tools, and links to the license provider portal."
---

# Dongle News
**Jürgen Makowka**
**Pohlheim, January 19, 2018**

**Software for Glass and Windows**

---

---
## Bedenket, worum Ihr bittet ...

> Bedenket worum Ihr bittet,
> Es könnte Euch gewährt werden

*(Consider what you ask for, it could be granted to you)*

---

## Be Careful What You Wish For

> Be careful what you wish for,
> for the gods may grant you!
>
> — Marion Zimmer Bradley: “The Mists of Avalon"

---

## What's New?

-   **'Softlocks' supported**
    -   Gemalto Sentinel Software Licenses
-   **Improved requesting of license files**
    -   Website for requesting license files
        > #### A+W License Provider
        > This tool allows installation personnel at a customer's site to receive an appropriate license update file for the customer's license server at any time.
        >
        > **Dongle**
        > - **A+W Softlock/Dongle number:** 1000201
        > - **Type:** SoftLock
        > - **License date:** 25.1.2018, 14:47:54 (Latest)
        > - **Comment:** Additional Business licenses
        >
        > **Softlock settings**
        > - [ ] Standard method
        > - [x] By update counter: 0
        > - [ ] By fingerprint
        > - [ ] By info file
        >
        > `Download license`
-   **New administration tools for Internal Sales**

---

## A+W Softlock Basics

-   **Gemalto Sentinel Software License combined with the A+W License Server**
    -   Gemalto > SafeNet > Aladdin > Fast
-   **A Softlock has an A+W Dongle no**
    -   Number range 1000000 to 8999999
-   **A Softlock is bound to its physical or virtual machine**
    -   'Fingerprint' of the machine must be collected
        -   Initial installation only!
    -   License file creation requires the fingerprint (unless the softlock is known)
-   **Creating a softlock with a fingerprint causes expenses for A+W**
    -   Creating a softlock is about as expensive as buying a new hardware dongle
-   **Softlocks cannot be recycled**
    -   They can be re-located to another machine ('Rehosting')

---

## A+W Softlock Advantages & Disadvantages

### Advantages

-   **No hardware module**
    -   No shipment required
    -   Cannot break
    -   Cannot get lost
    -   Doesn't require USB over LAN connection when used in datacenter
    -   Can be used in cloud (Azure, AWS)

### Disadvantages

-   **No hardware module**
    -   No sticker, dongle no cannot be easily identified
-   **More cumbersome handling**
    -   Requires fingerprint collection before license file creation
    -   Cannot be moved easily from one machine to another
    -   License update may require additional steps
-   **Less secure**
    -   Not bound to hardware (not even the host machine's)

---

## A+W Softlock Workflow (First Installation)

-   IP* requests compilation of license (from `dongle@a-w.com`), based on a PO+
    -   (Some head start appreciated)
-   Internal Sales compiles the license and assigns a new A+W Softlock no
    -   The license, together with the A+W Softlock no is stored in a database
-   At installation time IP makes sure the target machine is in its final state
    -   Final machine name
    -   Final domain membership
    -   Final DNS properties
-   IP installs the 'SoftlockPreparePackage' on the target machine
    -   `\\jupiter\Doku_DocuWare\AWEnterprise\LicenseServer\!General\FAQ_Tips_Tricks\Softlock\SoftlockPreparePackage.zip`
-   IP collects the target machine's fingerprint
-   IP uses `https://www.a-w.com/licenseprovider` to download license file
    -   Fingerprint enters here
-   IP installs A+W License Server on target machine, using downloaded license file

\* IP = Installing Person
\+ PO = Purchase order

---

## A+W Softlock After Installation

### Critical changes (virtual machines, may invalidate A+W Softlock)
-   Rename computer (does always invalidate)
-   Change computer's domain membership
-   Change computer's DNS environment (may include ip address of DNS server)

### Non-critical changes (virtual machines)
-   Change Memory
-   Change no of processor cores
-   Migrate VM within the same network
-   Change 'physical' network adapter
-   Change 'physical' disk

### Other
-   More restrictive checks can be imposed on VMs, but are not by default
-   **Different with physical machines**
    -   Avoid to change any hardware component

---

## A+W Softlock Initial Installation (Demo)

This section indicates a demonstration was performed.

---

## A+W Softlock Initial Installation (More Info)

-   The fingerprint can be sent to `dongle@a-w.com`. Internal Sales will send back the license file.
    -   There are possible delays because of time zone differences and office hours
-   **Reading Material**
    -   `\\jupiter\Doku_DocuWare\AWEnterprise\LicenseServer\!General\FAQ_Tips_Tricks\Softlock`
    -   General hints for using A+W Softlocks (PDF file)
    -   Checklist for installing an A+W Softlock (PDF file)

---

## A+W Softlock License Update Workflow

-   IP request license modification (from `dongle@a-w.com`), based on PO
-   Internal Sales modifies license and stores the result
-   At installation time IP uses `https://www.a-w.com/licenseprovider` to download the new license
    -   Multiple options, depending on situation
-   IP uses 'A+W LicenseServices Config Tool' to activate the new license

---

## A+W Softlock License Update (Demo)

This section indicates a demonstration was performed.

---

## A+W Softlock Update (Things to Know)

-   **A+W Softlock updates have a precise order**
    -   An update targeted to a different value of the update counter cannot be activated
        -   You cannot go back to an older license version just by re-installing the older license file
    -   An update can be activated only once
-   **Update download options**
    -   Standard (for most recent known value of UC)
    -   By UC value
    -   By A+W Softlock information file
    -   Previous license versions

---

## A+W Softlock Activate Older License (Demo)

This section indicates a demonstration was performed.

---

## A+W LicenseProvider Web App (Things to Know)

-   Licenses can be downloaded for A+W Softlocks and A+W Dongles.
-   Licenses cannot be downloaded for the older HARDLOCK (OEM license files).
-   Permission to use the A+W LicenseProvider Web App is maintained by ICT.
    -   Permission is granted by the A+W departments' directors.
    -   Specific roles imply download permission.
    -   Permission check is based on AWAGDOM group membership.
-   The A+W LicenseProvider Web App does not (and will never) enable the user to change the contents of a license.

---

## Q&A

Any questions so far?

---

## A+W Softlock Move (Rehosting)

-   A+W Softlock can be moved from one machine to another.
-   **Softlock must be 'rehostable'**
    -   Internal Sales can prevent this when defining the license.
    -   Whether or not a customer gets rehosting permission is decided by A+W management.
    -   Default is that the A+W Softlock is rehostable.
-   Moving requires that both machines are simultaneously available.
    -   However, a direct connection is not required.
-   The target machine of the move must be in its final state.
-   The license can be moved along with the A+W Softlock.
-   **Moving is a multistep process**
    -   The part pertaining to the Gemalto Sentinel Software License is called 'Rehosting'.

---

## A+W Softlock Move Workflow

1.  IP ascertains that target machine is in its final state.
2.  IP installs SoftlockPreparePackage on target machine.
3.  IP uses 'A+W Softlock Tool' to create `.awtmid` file.
4.  IP transfers `.awtmid` file to source machine.
5.  IP stops and disables A+W License Server on the source machine.
6.  IP uses 'A+W Softlock Tool' to remove A+W Softlock and create `.awrhif` file.
    -   `.awrhif` may include the current license.
    -   After this operation A+W License Server no longer works on source machine.
    -   A+W License Server may be uninstalled at this time.
7.  IP transfers `.awrhif` file to target machine.
8.  IP uses 'A+W Softlock Tool' to install A+W Softlock on target machine.
    -   License may be installed if it was included in the `.awrhif`.
9.  IP installs A+W License Server on target machine (unless already present).
10. IP optionally requests and installs new license (if license was not transferred).

---

## A+W Softlock Move (Demo)

This section indicates a demonstration was performed.

---

## A+W License (Additional Information)

-   A+W Softlock live from February 12, 2018.
-   **Minimum requirements**
    -   Gemalto Sentinel Runtime version 7.54 or above ('A+W Distribution for Gemalto Sentinel Runtime').
    -   A+W License Server version v6.4 with latest patches.
        -   Older license clients will work with that version.
-   **There are options for specific situations**
    -   Options are always controlled by Internal Sales.
    -   For virtual machines the A+W Softlock can be bound to the virtualization hardware.
        -   Prevents cloning.
        -   Failover and Migration not possible.
    -   Moving the A+W Softlock can be prevented.
        -   Re-locating the A+W License Server to another machine requires a new A+W Softlock.
-   **There is a Dongle mode which is similar to the A+W Softlock**
    -   Works with our standard dongles.
    -   License updates bound to Update Counter as with the A+W Softlock.

---

## Q&A

Any questions left?

---

## The End

Thank you for your patience!
