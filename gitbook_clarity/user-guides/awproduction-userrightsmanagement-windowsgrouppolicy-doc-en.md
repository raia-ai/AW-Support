---
description: "AW_Production_-_User_Rights_Management"
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
