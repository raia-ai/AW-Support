---
description: "A+W Configuration: MQTT Broker"
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
