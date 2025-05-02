---
title: "Spm Dpc Installation"
slug: spm-dpc-installation
publish: false
date: 2025-05-03
update: 2025-05-03
description: Spm Dpc Installation
categories:
  - start
---

SPM DPC Installation
====================

From SPM version 3.2.0 onwards, there is a new SPM type which can be installed on any Android device. If there is a dedicated SPM for your device, a standard SPM still offers more privileges on your device's Android operating system. This new SPM type is useful in case there is no specific SPM for your device available.

This new SPM type is called DPC. It installs itself as a Device Administrator on your player and allows an important subset of the original SPM functionalities. The available functionalities depend on your Android version.

The table below illustrates the functionalities available with each Android version.

|  |  |
| --- | --- |
| **Functionality** | **Minimum Android Version** |
| Remote Software Update | Android 6.0 |
| Scheduled and Remote Reboot | Android 7.0 |
| Remote Clock and Date adjustments | Android 9.0 |
| Remote view | Not supported |

Even though the SPM DPC is more limited than the standard SPM, it is still highly recommended to install it if there is no other SPM type available for your device.

With the SPM DPC your device will allow remote software update and receive all the bug fixes and enhancements of new OnSign versions.

**Important:** Only OnSign TV player versions 10.3.7 or above are compatible with the SPM DPC.

Installation
------------

To install the SPM DPC, you need to perform a few more steps than a regular APK installation.

SPM DPC can only be installed after a factory reset of the device because this is an Android requirement for the installation of Device Administrator Apps.

You will also need a PC to connect to the device with an 'adb' software in order to enable the Device Administrator.

There are 6 steps in this process:

### 1- Factory reset device

This varies between Android versions, but you should find Reset options under the System menu in the Android Settings.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731418335553/ec568a47-70c1-4985-8565-8e8342ca945d.png)

Choose "Reset options" and perform an (Erase all data) Factory Reset.

**ATTENTION:** Factory Reset will erase all your device info.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731418429608/4fead0ba-88a9-4867-8c2a-d947e50f9eec%20(1).png)

After confirmation, the device will reset and reboot.

### 2- Initial Setup

After restarting the device, go through the initial device setup. Set up network and other parameters, but:

**By all means, SKIP Google sign-in!**

**DO NOT ENTER A GOOGLE ACCOUNT!**

This is very important. A Device Administrator needs to be configured before any account is created in the system.

### 3- Enable developer mode

* Go to device Settings.
* Click on "About".
* Then, click 7 times on the Build number section to activate developer mode.

Once the developer mode is activated:

* Go to Settings > System > Advanced and click on Developer Options.
* Under Developer Options enable USB debugging.

### 4- Install APK

Download the SPM DPC apk from <https://onsign.tv/spm/>

Connect your device using adb and install the downloaded apk:

```
# adb install -r spm-3.3.0-dpc.apk
Performing Streamed Install
Success
```

### 5- Enable device administrator

Once installed, activate the Device Administrator by running the command: `adb shell dpm set-device-owner module.platform.signage/.AdminReceiver`

The console should log:

```
Success: Device owner set to package
ComponentInfo{module.platform.signage/module.platform.signage.AdminReceiver}
Active admin set to component {module.platform.signage/module.platform.signage.AdminReceiver}
```

Pay attention to the return message, if done correctly it should say:  Success: Device owner set to package

![](https://docs.onsign.tv/resources/Storage/en/spm-dpc-installation/spm-dpc-installation-2024-07-04.png)

### 6- Install OnSign TV

Once the SPM DPC is installed, it's time to install the OnSign TV Player. The latest version of the OnSign TV APK is always available at: <https://app.onsign.tv/download/player/latest/android/>.

OnSign TV can be installed by:

* Downloading and installing it on the device;
* Downloading, copying it to a USB drive, and using the USB drive to install the APK; or
* Using the ADB command: `adb install`

Once the player is installed, start OnSign TV and ensure to give it all requested permissions.

Check that the SPM DPC was correctly installed
----------------------------------------------

To ensure everything is correct, you can check if the SPM was correctly installed by requesting a remote reboot on the player settings page and verifying the SPM version in the status page of the player information page.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731418714365/1fe958b9-8914-4076-a059-92ba252f5331.png)![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731418724895/d25520b9-d02d-4e3b-bb35-7bed43a8df09.png)
