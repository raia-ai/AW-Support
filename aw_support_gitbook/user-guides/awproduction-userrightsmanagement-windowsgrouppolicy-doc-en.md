---
title: "AW_Production_-_User_Rights_Management"
source: "AW_Production_-_User_Rights_Management.docx"
tags: ["A+W Production", "user rights management", "Windows Group Policy", "ADMX", "security", "access control", "roles and permissions", "IT administration", "gpedit.msc"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document explains how to enable and administer user rights management in A+W Production using the Windows Local Group Policy. It covers installing the A+W Software GmbH ADMX/ADML templates, opening gpedit.msc, and configuring policies under both Computer and User configurations. It describes global versus user-specific rights, policy states (Not Configured, Enabled, Disabled), and provides practical examples. An implementation outline recommends group-based access (Administrators, Power, Normal Users) and optional automation using registry export and logon scripts."
long_description: "This guide provides step-by-step instructions for setting up and maintaining user rights management in A+W Production. It begins with a high-level overview of the capability to control access to various A+W Production functions via Windows Local Group Policy. Organizations are reminded that configuration changes may need to be performed by their IT support to ensure correct and compliant implementation.

The document then outlines the prerequisites for enabling rights management, which include developing an authorization concept and installing the required policy templates. Administrators must obtain the A+W Software GmbH ADMX package and deploy its contents to the appropriate PolicyDefinitions directories on the server: placing the ADML file into C:\Windows\PolicyDefinitions\en-US and the ADMX file into C:\Windows\PolicyDefinitions. These files are available from the official A+W support channel.

Once the templates are in place, configuration is performed using the Local Group Policy Editor (gpedit.msc). After launching gpedit.msc, administrators should navigate to the A+W Software GmbH nodes under both Computer Configuration and User Configuration within Administrative Templates. Rights can be defined globally (computer-wide) or per user; for user-specific changes, the operator must be logged in as the target user when adjusting settings under the User Configuration branch.

Each policy within the A+W Software GmbH configuration can be set to Not Configured, Enabled, or Disabled. By combining these states appropriately, administrators can permit or restrict access to A+W Production features. For example, rights might be enabled for the Article Master while disabled for Capacity Planning, effectively tailoring access to operational needs and responsibilities.

To introduce rights management in a controlled manner, the guide suggests first disabling all rights globally and then granting access through user-level groups. Example groups include Administrators (full access), Power Users (no changes to Production Master Data but permission to change Item Master Data), and Normal Users (no changes to Production Master Data). To simplify deployment across the organization, administrators may create the user-related groups with a single test account, export the relevant registry paths after each group’s configuration, and use logon scripts to apply the required settings at user sign-in. This approach streamlines ongoing administration and makes it easier to move users between groups as roles change."
---

# A+W Production User Rights Management
## Overview
With A+W Production it is now possible to set up user rights management for the various functionalities within the A+W Production.
User rights are set up and managed through the local Windows Group Policy.
> Note: Note - The configuration of user management right may need to be implemented by the companies IT Support to ensure correct configuration.
## Enable Rights Management
To enable rights management, the following steps must be performed:
- Development of an authorization concept
- Installing user rights management
## Installation Files
Ensure that the file - A+W Software GmbH.admx.zip has been supplied as this contains the files needed for the configuration.
To install rights management, the following files must be installed on the appropriate server to the following folders:
These files can be requested via your local official A+W Support Channel.
- File A+W Software GmbH.adml into folder C:\Windows\PolicyDefinitions\en-US
- File A+W Software GmbH.admx into folder C:\Windows\PolicyDefinitions
## Configure via Local Group Policy Editor
If the files have been copied to the appropriate directories, rights management can be set up using the Local Group Policy Editor.
To start configuring the settings choose Start > Run or Windows Key + R and enter gpedit.msc.
## Group Policy Paths
After gpedit.msc is opened expand the two following keys.
- Local Computer Policy > Computer Configuration > Administrative Templates > A+W Software GmbH
- Local Computer Policy > User Configuration > Administrative Templates > A+W Software GmbH
## Rights Scope
Rights can be setup both globally and in relation to users. Configuration of users will require the operator to be logged in as the user before making changes for any specific changes wanted under the entry User Configuration.
## Policy Settings and Examples
Under each folder of the A+W Software GmbH configuration is a setting that can be changed from Not Configured, Enabled or Disabled.
This means we can prohibit a user from accessing the configuration of the A+W Production Master Data.
Example - We can Enable users rights to the Article Master or Disable it for Capacity Planning.
## Implementation Outline
An outline to introduce rights management to A+W Production could be the following.
### Recommended User Groups and Access Levels
- Globally disable all rights for all users.
- Distribute rights at the user level via groups group examples - Administrators, Power and Normal Users.
- Administrators - Full Access to A+W Production.
- Powers Users - Cannot change A+W Production Master Data however they can change the Item Master Data.
- Normal Users - Cannot change any A+W Production Master Data.
### Automation and Deployment
- To simplify the configuration, it is possible to create all three user-related groups with one user and export the registry path after each groups creation.
- Using a Logon Script, user rights can be reapplied for each user at logon. Using these logon scripts it also makes it easier to change a users group when required.
