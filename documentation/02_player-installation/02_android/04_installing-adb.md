---
title: "Installing Adb"
slug: installing-adb
publish: false
date: 2025-05-03
update: 2025-05-03
description: Installing Adb
categories:
  - start
---

Installing ADB
==============

In order to install the Android Debug Bridge (ADB) and connect your device to a computer, you need to perform two steps:

1. Install ADB on your PC.
2. Enable Developer Mode.

ADB is an Android project tool available for free on the Android SDK. We suggest a stripped-down version like the ["15 seconds ADB installer"](https://forum.xda-developers.com/t/official-tool-windows-adb-fastboot-and-drivers-15-seconds-adb-installer-v1-4-3.2588979/) to avoid downloading the very large sized full SDK.

Installing ADB
--------------

1. Once you have downloaded the application, double-click it to start the installation process. If you have never installed the ADB on your PC, answer ‘Y’ to all questions.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406120254/installing-and-using-adb_1.jpg)

2. After the installation, run the ADB command in the command line to check the installation.
3. Start the Command Prompt application and type "ADB" finishing with the enter key. You should see the ADB help text as shown below:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406155292/installing-and-using-adb_2.jpg)

With the ADB installed, it is time to enable Developer Mode on your Android device and connect it to the PC.

Enabling Developer Mode
-----------------------

1. In your Android device, go to Settings and click on the “About tablet/phone/device” option.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406251920/installing-and-using-adb_3.jpg)

2. Scroll down to see the Build number entry and click on it seven times. As you click, you will see messages stating that you are about to become a developer.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406267973/installing-and-using-adb_4.jpg)

3. When you are in Developer Mode, hit "back" and click on the newly appearing “Developer options” option.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406298383/installing-and-using-adb_5.jpg)

4. Scroll down to the Debugging section and enable the "USB debugging" option.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406312362/installing-and-using-adb_6.jpg)

5. A confirmation dialog box will pop-up. Confirm with “OK”.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406340734/installing-and-using-adb_7.jpg)

6. Connect your device to the PC with a USB cable. You will be prompted with an authorization dialog box. Check *“Always allow from this computer”* and confirm with “OK”.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406364215/installing-and-using-adb_8.jpg)

7. At this point, your device is ready to use the ADB. Open the Windows Command Prompt and type "adb devices". The connected device should be listed.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731406396039/installing-and-using-adb_9.jpg)
