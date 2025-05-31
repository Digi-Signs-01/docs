---
title: Installing On WebOS 4.0 To 6.0
slug: installing-on-webos-40-to-60
publish: true
date: 2025-05-03
update: 2025-05-03
description: Installing On Webos 40 To 60
categories:
  - start
---

Installing on webOS 4.0 to 6.0
==============================

Installing the Digisigns Software on your LG Smart Signage Platform webOS screens is really simple and easy!

This tutorial applies **to the following screen models**:

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Player OS** | **Video** | **HDMI-IN** | **Portrait Support** | **Models** |
| webOS Signage 4.0 | 4K / 1080P | Yes | Yes | BH5E, BH7E, BH7F, LAA015F, SH7E, SH7E,SM5E, SM5KE, SVH7F, SVH7PF, UH5E, UH5PE,UH5F, UM3E, VH7E, VM5E, WP400, XE4F |
| webOS Signage 4.1 | 4K / 1080P | Yes | Yes | UM3D, UM3DF, UH5F, UH7F, 22SM3G, UL3G, UM3F |
| webOS Signage 6.0 | 4K | Yes | Yes | SM5J, UL3J, UH5J, UH7J |

[Refer to this tutorial](/02_player-installation/19_lg-webos/02_installing-on-webos-20-to-32) for instructions on how to install on **LG webOS 2.0, 3.0**, and **3.2** instead.

Installation Process
--------------------

### Before you start:

1. Make sure to uninstall any other App or Signage Software which might be installed on the device.
2. Double check your device date and time. Incorrect settings may cause SSL validation to fail, blocking connection to our servers.
3. If your network is protected by a firewall, make sure it complies with our requirements. Be sure to check the hardware specific section at the end of the document.

1. Turn your LG TV on.
2. **Press the "Settings"** button on the remote control.
3. Select "SI Server Setting" from the menu.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731443419296/how-to-install-onsign-tv-on-lg-webos-4-0-to-6-0_1.png)

4. Select the "SI Server Setting" option again.
5. The LG Server Setting will appear on screen. Configure the settings as presented below:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731443434082/c0b44e8a-5f00-4e9e-bfab-c63fb6e68f82.png)

#### **LG Setup**

* Application Launch Mode: **Local**
* Fully Qualified Domain Name: **ON**
* URL: https://www.digisigns.in/lg.ipk (*Make sure to type all characters, including the last "/"*.)
* Application Type: **IPK\***
* (\*If this option is **not available**, it means you need to upgrade the TV's firmware. Upgrade the firmware and re-start the OnSign TV installation process.)
* Auto Set: **OFF** (Warning: Leaving this option enabled disables remote Player updates.)

6. Next to the **Local Application Upgrade** option, select **REMOTE** and confirm with **OK** on your remote control.
7. **Restart your device when the message confirming completion appears**.
