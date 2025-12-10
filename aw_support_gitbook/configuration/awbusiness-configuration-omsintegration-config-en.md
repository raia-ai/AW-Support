---
description: "EN-CONFIG-AW_Business-16-1"
---


# 21.8. Phase III (transfer of status changes to OMS)

At that moment, the EDI files are generated with the new workflow if the orders are in the correct status area.

---
### 21.8.1. Installation

The following packages must be installed:
- ALFAK 2011 Basis
- ALFAK 2011 French
- ALFAK 2011 Server
- Complete infrastructure and commercial (see Chapters 1-3)

All new formulas and triggers are in the subdirectory of the ALFAK 2011 installation `\Formula\SGGATP`.

### 21.8.2. Configuration

The database must be brought up to the current state (all scripts including `20170313a.sql`).

The database triggers `SQLBase BW_AUFTR_HIST OMS_Insert.sql` and `SQLBase BW_AUFTR_KOPF OMS Delete.sql` must be installed on the database.

**Before installation of the triggers, the architect number must be adjusted.**

The Webservice address must be entered on the eCommerce/OMS login dialog:

