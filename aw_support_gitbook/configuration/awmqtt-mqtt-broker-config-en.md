---
title: "A+W Configuration: MQTT Broker"
source: "EN-CONFIG-AW_MQTT_Broker.pdf"
tags: ["A+W", "MQTT", "Broker", "Configuration", "Mosquitto", "Software for Glass", "Authentication", "Port Configuration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A brief guide on configuring the A+W MQTT Broker, which is based on the Eclipse Mosquitto Broker. It covers post-installation adjustments such as changing the default port and managing user authentication."
long_description: "This document provides configuration instructions for the A+W MQTT Broker, a component used for MQTT communication within the A+W software ecosystem. The broker is based on the Eclipse Mosquitto Broker. The guide details post-installation procedures for system administrators. Key topics include locating and understanding the main configuration file (`mosquitto.conf`), changing the default communication port from 1883 to a custom port, and managing user authentication. It explains how to add new users to the password file (`passwd`) using the `mosquitto_passwd.exe` utility, including commands to add a single user or to replace the entire user list. This document is intended for users who have successfully installed the broker and need to customize its settings for their specific environment."
---

# A+W Configuration: MQTT Broker

---
## Change History

| Date | Author | Remarks | Version |
| :--- | :--- | :--- | :--- |
| 2021-05-21 | JNI | Original version | 1.0 |

## 1. General

The MQTT Broker is used for the MQTT communication. This document describes how you can adjust settings on the broker after successful installation.

## 2. Configuration

### 2.1. Configuration file

When you start the Mosquitto Broker, a configuration file is imported, which makes various settings. It is found in the directory `C:\Program Files\A+W\Mosquitto\mosquitto.conf`. After the installation, a default configuration file is delivered by Setup Launcher. For other adjustments, the Manufacturer's page of the Eclipse Mosquitto Broker has to be called up.

### 2.2. Configuration use cases

#### 2.2.1. Adjust port

In order to change the default port from 1883, you have to add the following entry in the `mosquitto.conf`:

```
listener port <desiredport>
```

#### 2.2.2. Adding users for authentication

All users who are permitted for authentication can be found in the file `C:\Program Files\A+W\Mosquitto\passwd`. To add a new user here, the help program `mosquitto_passwd.exe` in the same folder is used. A new user is added with the following command:

```
Mosquitto_passwd.exe -b passwd <User> <Password>
```

With the `-c` option, all existing users are removed and the specified one is the only one added:

```
Mosquitto_passwd.exe -c passwd <User> <Password>
```
