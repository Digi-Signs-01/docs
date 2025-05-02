---
title: "Installing Iadea Player Software"
slug: installing-iadea-player-software
publish: false
date: 2025-05-03
update: 2025-05-03
description: Installing Iadea Player Software
categories:
  - start
---

Installing iAdea Player Software
================================

Beforehand, use your PC to download the latest OnSign TV Player App and iAdea SPM package onto a USB stick. You can get the APKs from:

* <https://app.onsign.tv/download/player/latest/android/>
* [SPM 3.3.0 for XMP-8550](https://signagewidgets.net/update/a6112c143d30193e3d637966e4a0290ab6c5a539.apk?filename=spm-3.3.0-xmp8550.apk)
* [SPM 1.1.2 for XMP-7500](https://signagewidgets.net/update/45dcdd38313fd524b33e9affb10cdfd99d66c491.apk?filename=spm-1.1.2-xmp7500.apk)

Next, install the OnSign TV  Player App and SPM on your iAdea Player.

Get the iAdea instruction PDF here or follow the steps below.

1. Plug the USB stick into the iAdea device.
2. In the "Basic Settings", click "Advanced".
3. Click 3 times with the mouse on the bottom-right corner. This is a somewhat painful process because you need to perform the clicks fast. Click, click, click... The best way is to click several times until you get to the Android Screen!

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409354975/how-to-install-onsign-tv-on-iadea-players_1.png)

4. Click the Android App icon:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409422795/how-to-install-onsign-tv-on-iadea-players_2.jpg)

5. Open the APKInstaller and click "Install".
6. Select "USB Memory".
7. Follow the installation instructions to install both Apps.
8. When finished, you can click the Android Home Button to return to the initial setup screen.

Set the iAdea Player to Auto-Start the OnSign TV Software
---------------------------------------------------------

More information about iAdea Auto-Start is available [here](https://support.iadea.com/hc/en-us/articles/115004165506-How-to-launch-the-app-by-AppStart-and-exit-the-app-properly).

1. Starting from the "Basic Settings" screen again, click on "Advanced".

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409493914/how-to-install-onsign-tv-on-iadea-players_3.jpg)

2. Click on "Content" and then on "App Start".
3. Underneath the URL in the window on the right, click to unfold "Advanced".

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409511269/how-to-install-onsign-tv-on-iadea-players_4.png)

4. Use these parameters in the "Advanced" configurations:
   * Enter Package Name: **tv.onsign**
   * Enter Class Name: **tv.onsign.PlayActivity**

**From version 10 and up:**

* Enter Class Name: tv.onsign**.activities.play.PlayActivity instead**
* Enter Action: **android.intent.action.VIEW**

Configuring your Network
------------------------

1. Click on "Advanced".
2. Select the Network Option to configure your WiFi and/or Ethernet port.

Setting the Player Clock
------------------------

This is a very important step which the playback schedule relies on!

1. Click on “Advanced”
2. Go to “Scheduling”
3. Select "Time And Date" and set the correct time and date.

Setting scheduled Reboots
-------------------------

We recommend scheduling a daily reboot, so that the system is regularly refreshed.

1. Click on “Advanced”
2. Go to “Scheduling”
3. Select “Scheduled reboot”
4. Enable the reboot and set it to a time which will not disrupt your operation, let's say 4:00 AM.

**Once everything is set, restart the device. OnSign TV should start automatically!**
