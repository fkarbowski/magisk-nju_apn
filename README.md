# Magisk Module – Custom APN List for MMS (Android 15)

## Overview
This Magisk module replaces the system file **`/system/etc/apns-conf.xml`**, which contains the APN (Access Point Name) configuration list for MMS services on **Android 15** (`Ulefone` version).  
It is designed to ensure proper MMS functionality on **NJU Mobile (Orange)** by injecting a verified APN configuration.

---

## Features
- Replaces the default APN configuration file (`/system/etc/apns-conf.xml`)
- Adds a working **MMS APN for NJU Mobile (Orange)**  
- Preserves system integrity via Magisk overlay (no direct system modification)
- Verified and tested on **Ulefone Armor 28 Ultra** running Android 15
- Compatible with AOSP-based and custom ROMs

---

## NJU Mobile (Orange) – Correct MMS APN Configuration

```xml
<apn carrier="Orange MMS"
     mcc="260"
     mnc="03"
     apn="mms"
     user="mms"
     password="mms"
     mmsc="http://mms.orange.pl"
     mmsproxy="192.168.6.104"
     mmsport="8080"
     type="mms"
     network_type_bitmask="1|2|3|4|5|6|7|8|9|10|11|12|13|14|15|16|17|18|19|20"
     user_editable="true"
/>
```

---

## Installation
- Download the module ZIP from the Releases page.
- Open the Magisk app on your device.
- Go to Modules → Install from storage.
- Select the downloaded ZIP file.
- Reboot your device.
