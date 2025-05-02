---
title: "Installing Using Bsncloud Preferred Method"
slug: installing-using-bsncloud-preferred-method
publish: false
date: 2025-05-03
update: 2025-05-03
description: Installing Using Bsncloud Preferred Method
categories:
  - start
---

Installing using BSN.cloud (preferred method)
=============================================

BSN.cloud is a free service provided by BrightSign to help with deployment and remote Player management. This is the preferred installation method for BrightSign Players.

Using the BSN.cloud in combination with OnSign TV you can:
----------------------------------------------------------

* Install the OnSign TV  Player App on BrightSign devices remotely.
* Remotely update the BrightSign Player Firmware.
* Get remote Player screenshots. You can even see the OnSign TV paring code before getting the Player connected to OnSign TV.
* Remotely reboot the Player.
* Remotely factory reset the Player while maintaining the OnSign TV  Player installed.
* Remotely format the SD card.
* Remotely test and change network settings.
* Get additional debugging logs, including the option to browse SD Card files.

Before moving forward, make sure:
---------------------------------

* The Player network is configured and connected to the internet either through ethernet or Wifi.
* The BrightSign Player is running firmware which is 8.0.119 or newer.
* If you have both of the above set, the Player will display the BSN.cloud activation code directly after booting.
* In case you don’t get the activation code, you can try a factory reset before starting the process.

Step by step Installation
-------------------------

1. Login to BSN.cloud

The BSN.cloud can be accessed with the URL: <https://bsn.cloud>. On the first access to the page, it will show you a screen like this.

* Check the box “Don’t show this again”, so next time you will go directly to the login page.
* Click on “Continue in browser” at the bottom of the page.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1742839985475/brightsign-installing-onsign-tv-using-bsn.cloud_1.png)

Now, you will be prompted with the BSN.cloud login page. Create a user in case you don’t have one yet, and log into your account.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1742840002170/brightsign-installing-onsign-tv-using-bsn.cloud_2.png)

2. Create a Player Setup Profile

Before connecting a Player to your BSN.cloud, you should first create a “**Default Player Setup Profile**”. These settings will be used by all your Players deployed on BSN.cloud.

To do this, connect to your BSN.cloud account and go to Admin > “**Device Settings**“.

Now, configure the three parameters below:

* Package name: **Default Setup** (See the note below to configure this item.).
* Device name: **Default Setting**.
* Partner Application: OnSign TV.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1742840064869/brightsign-installing-onsign-tv-using-bsn.cloud_3.png)

It is VERY important to name the package “Default Setup”, so all new devices will be created using these settings. Otherwise, you will later have to go to your provided devices and apply the OnSign TV device setup profile to your connected BSN.cloud Players.

3. Connecting the Player to BSN.cloud

The final step is actually connecting the BrightSign Player to BSN.cloud.

Go to:

1. Admin > “**Device Activation**”.
2. **Read the code** which is presented on your Player screen.
3. **Enter the activation** code and submit.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1742840130412/brightsign-installing-onsign-tv-using-bsn.cloud_4.jpg)

4. Once you press the submit button, the Player will start to download and install the OnSign TV software. Just wait until the Player finishes the process. No need to worry when the device will go through several reboots and the whole process takes a couple of minutes.

If you can’t see the activation code on your screen, please make sure:

* You are running firmware 8.0.119 or newer.
* Make sure your Player is connected to the internet.
* Consider formatting the SD card to ensure nothing is running on the Player and factory reset the device.

Now, the BrightSign Player is connected to the BSN.cloud and should have OnSign TV installed and ready to go!

Requirements:
-------------

* Make sure you have an empty SD Card as storage device connected to your Player. It must be formatted with FAT32 or ExFAT.
  + **If the storage device is not empty, the installation process will not work!**
* Make sure the Player's ethernet cable is connected, so that the Player can obtain an IP address.
* You will need a computer connected to the same network as the Player to remotely access the BrightSign Player web interface.
* **This tutorial is valid for BrightSign 8.0.119 and up**. Devices with BrightSign firmware 7.+ which had the OnSign TV version 3 installed will still work with the installation done as described in this tutorial, but from OnSign TV version 10 onwards, you need the BrightSign firmware 8 and up.
