---
title: "Enabling Kiosk Mode"
slug: enabling-kiosk-mode
publish: false
date: 2025-05-03
update: 2025-05-03
description: Enabling Kiosk Mode
categories:
  - start
---

Enabling Kiosk Mode
===================

Kiosk Mode is a feature available from Android 5 and up which locks the device to only run OnSign TV. This is a security feature particularly useful for touch devices. It prevents users to access any other Android feature or setting.

**Once the Kiosk mode is configured, the device will:**

* Not allow users to leave the OnSign TV  Player App
* Block users from accessing the setup menu by performing a swipe on the top of the screen
* Not show the Android navigation bar

For maintenance, it is possible to set a password, so only authorized personal can exit the OnSign TV  Player App. This is explained at the end of this tutorial.

**Samsung Devices:**

For **Samsung devices, OnSign TV offers a different kiosk mode setup** with several advantages over the method described in this tutorial. Click [here](/android/samsung-kiosk-manager-skm) to learn more.

**To configure your device to kiosk mode, you need:**

* A device running Android 5 or higher
* The OnSign TV Android Player App 5.1.6 or higher
* To have ADB installed. (ADB is a command-line tool which lets you communicate with an Android device.) Learn [how to install ADB](/android/installing-adb).
* Have your device set to run OnSign TV as Device Owner App.

Please note, once OnSign TV is configured as "Device Owner", the only way to remove it is by **performing a "Device Factory Reset"**.

**There are three steps required to configure your Android device to Kiosk Mode**

1. Factory reset
2. Install the OnSign TV Player App
3. Run the adb dpm command

1) Factory reset
----------------

1. A factory reset returns the device to an empty default state. In "Android Settings", click on the "Backup & reset" option.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731407945211/enabling-kiosk-mode_1.jpg)

2. Select "Factory data reset" and wait for the process to finish. Your device will reboot when ready.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731407959502/enabling-kiosk-mode_2.jpg)

3. Once the device reboots, you will need to re-enable the Developer Mode as described in the ADB tutorial.

2) Install the OnSign TV Player App
-----------------------------------

When the Developer Mode is enabled, it is time to use the ADB to install OnSign TV and activate it as a Device Owner.

1. Download the latest OnSign TV version from the [website](https://onsign.tv/downloads/).
2. Connect your device to your computer using a USB cable.
3. Open the Command Prompt and install OnSign TV by typing the following command:  
   `adb install OnSignTV-N.N.N.apk`

OnSignTV-N.N.N.apk is the name of the file you downloaded. The N.N.N is a placeholder for the OnSign TV version.

3) Run the adb dpm command
--------------------------

1. Once the apk is successfully installed, activate Device Owner by running the following command:  
   `adb shell dpm set-device-owner tv.onsign/.command.target.platform.dpc.command.SignageAdminReceiver`

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731408193225/enabling-kiosk-mode_3.jpg)

2. From this point on, OnSign TV is active as the Device Owner and cannot be removed.
3. Associate the Player with your account by entering the code displayed on your screen:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731408325533/enabling-kiosk-mode_5.jpg)

4. During association, you will be presented with an optional extra password field (Lock Password). This password is used for to exit the OnSign TV Player App when running in Kiosk Mode.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731408341945/enabling-kiosk-mode_6.jpg)

How to Exit Kiosk Mode
----------------------

1. On the app on your device, click on the bottom-left corner 7 times to exit.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731408457932/enabling-kiosk-mode_7.jpg)

2. If you chose to add a password in the Player setup, an input box will request it.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731408474101/enabling-kiosk-mode_8.jpg)

If you did not set a password, the OnSign TV Player Software will just exit without asking for a password.
