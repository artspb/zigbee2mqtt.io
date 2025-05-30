---
title: "IMOU ZD1-EN control via MQTT"
description: "Integrate your IMOU ZD1-EN via Zigbee2MQTT with whatever smart home infrastructure you are using without the vendor's bridge or gateway."
addedAt: 2025-04-01T18:30:52
pageClass: device-page
---

<!-- !!!! -->
<!-- ATTENTION: This file is auto-generated through docgen! -->
<!-- You can only edit the "Notes"-Section between the two comment lines "Notes BEGIN" and "Notes END". -->
<!-- Do not use h1 or h2 heading within "## Notes"-Section. -->
<!-- !!!! -->

# IMOU ZD1-EN

|     |     |
|-----|-----|
| Model | ZD1-EN  |
| Vendor  | [IMOU](/supported-devices/#v=IMOU)  |
| Description | Door & window sensor |
| Exposes | alarm, tamper, battery_low, battery |
| Picture | ![IMOU ZD1-EN](https://www.zigbee2mqtt.io/images/devices/ZD1-EN.png) |


<!-- Notes BEGIN: You can edit here. Add "## Notes" headline if not already present. -->


<!-- Notes END: Do not edit below this line -->




## Exposes

### Alarm (binary)
Indicates whether the alarm is triggered.
Value can be found in the published state on the `alarm` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` alarm is ON, if `false` OFF.

### Tamper (binary)
Indicates whether the device is tampered.
Value can be found in the published state on the `tamper` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` tamper is ON, if `false` OFF.

### Battery low (binary)
Indicates whether the battery of the device is almost empty.
Value can be found in the published state on the `battery_low` property.
It's not possible to read (`/get`) or write (`/set`) this value.
If value equals `true` battery low is ON, if `false` OFF.

### Battery (numeric)
Remaining battery in %.
Value can be found in the published state on the `battery` property.
To read (`/get`) the value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/get` with payload `{"battery": ""}`.
It's not possible to write (`/set`) this value.
The minimal value is `0` and the maximum value is `100`.
The unit of this value is `%`.

