---
title: "Installing Raspberry Pi Player Software"
slug: installing-raspberry-pi-player-software
publish: false
date: 2025-05-03
update: 2025-05-03
description: Installing Raspberry Pi Player Software
categories:
  - start
---

Installing Raspberry Pi Player Software
=======================================

**BETA VERSION** – While we have already performed several tests, the current OnSign TV Raspberry Pi Player is still marked as Beta. Please report any issue you may find to [Support](https://onsign.tv/support-submit-a-ticket/).

Important notes before installing
---------------------------------

* We recommend using a screen output resolution of 1920x1080. Older boards may require lower resolution for smooth playback.
* We recommend using videos encoded up to FullHD on Pi4 and HD on Pi3.
* The OnSign TV  Player will automatically be updated whenever a new version is released.
* All Beta releases will be numbered 9.99.x The official release will be 10.xx.xx.
* Dual monitor output is not supported.

Supported OS
------------

* Raspberry Pi OS with desktop 32 bits (Recommended)
* Raspberry Pi OS with desktop 64 bits

Supported boards
----------------

* Raspberry Pi 3B - We recommend running it in 1280x720 to improve performance
* Raspberry Pi 4
* OrangePi

Steps for Installation
----------------------

1. Download and install the latest Raspberry Pi OS (we recommend using the 32bits version).
   1. You can find the latest OS on the Raspberry Pi [official site](https://www.raspberrypi.com/software/).
   2. Use the [Raspberry Pi Imager](https://www.raspberrypi.com/software/) or any other tool you may prefer to install the Raspberry Pi OS into a MicroSD Card.
2. Insert the MicroSD Card into your Raspberry Pi board, connect to a screen using an HDMI cable, connect a mouse and keyboard, and turn the board on. Now, just wait until the Board is fully booted.
3. Configure the Country, Language, and Timezone.
4. Create a username "pi". The OnSign TV  Player will NOT WORK if a different username is set. Just repeating, the configured username MUST BE "pi". Choose any convenient, strong password.
5. Configure the network.
6. Allow the board to download and install the latest updates. Let the board restart if requested and wait for it to finish the boot process.
7. Download the OnSign TV installer package by opening the web browser and entering the URL below which matches your Raspberry Pi OS:
   1. [Arm 32-Bits](https://onsign.tv/pi32)
   2. [Arm 64-Bits](https://onsign.tv/pi64)
8. Once the download is finished, install the OnSign TV package.
9. You can now start the OnSign TV  Player by going to "Sound & Video" in the Raspberry Pi menu.
