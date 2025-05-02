---
title: "Setup Nexmosphere Sensors"
slug: setup-nexmosphere-sensors
publish: false
date: 2025-05-03
update: 2025-05-03
description: Setup Nexmosphere Sensors
categories:
  - start
---

Setup Nexmosphere Sensors
=========================

The Nexmosphere sensors are supported by the following OnSign TV players:

* OnSign TV Android Player
* OnSign TV Windows Player
* [OnSign TV BrightSign Player](/sensor-integrations-iot/using-nexmosphere-and-brightsign)

Connecting the Nexmosphere controller to the Player Hardware
------------------------------------------------------------

The first step to get things working is to connect and ensure the Nexmosphere hub correctly connected and communicating with the Player hardware. This process is slightly different depending on the Player Hardware operating system:

1 - Have your Nexmosphere devices ready and connected to the Nexmosphere Controller (Ex: XN-185)

2 - Connect the Nexmosphere controller USB to the Android Player Hardware

Android
-------

* A popup will open on Android with a prompt. Make sure to select "Always open OnSign TV when USB-Serial Controller is connected. This is very important so Android can remember this after the device is rebooted.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669169362/12ff611e-42b1-46ba-8d8b-586aefeb018b.png)

Note: While the vast majority of players will work well, some Android devices may not be able to connect to Nexmosphere devices. This happens when the Android firmware don't have support to USB-over-serial connections.

Windows
-------

* Go to the Windows Device manager and look for "Prolific USB-to-Serial Comm Port".
* In the example below, COM3 has been assigned.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669216643/3b410636-3ee5-47e5-b99f-7cfcc040c3e0.png)

Setup the Player Serial Port at OnSign TV Platform
--------------------------------------------------

After getting the Nexmosphere controller connected and identified by the player hardware, it's time to configure the Player serial port at the OnSign TV Platform.

1 - Go to the OnSign TV Player menu, and select the specific player to be configured

2 - Click on Settings

3- Scroll down on player settings to *"Serial Port Settings (RS-232)"*

4 - Click on the button "*+ Add Port*"

5-  Set Port type to "Nexmosphere"

6 - Select the Port from the drop down menu

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669263243/e1afa1f2-3c5e-4c0a-b7c7-0fbfef69fb7d.png)

Important Note: If your player is an Android device:

* Android may list internal Serial ports, make sure to select an option that has the "usb" string on the path
* Remove the last number of the serial path. In the example above, /dev/bus/usb/002/002  should be changed to /dev/bus/usb/002 . This is required as Android may change the last number of the serial port path in specific circumstances.

7 -Configure an Alias - This is the port name. Use a simple to remember name, as this will need to be entered on Apps and other OnSign settings whenever connecting to this port. By default OnSign will set the alias to Nexmosphere.

8 - Save the settings to store the new Serial Port configuration.

Configure Interactions using OnSign TV Interactivity API
--------------------------------------------------------

Once the player serial port is correctly configured, all content received from the serial port is parsed by the OnSign TV API and can be used to create an interactivity trigger.

Let's say we are implementing a **lift-and-learn scenario**, so we expect to receive the strings:

* XR[PU001] - when tag 1 is lifted
* XR[PB001] - when tag 1 is put back

Here are the steps to implement the scenario above:

1. Click either on Campaign Interactivity, or Player Interactivity
2. Give the Interactivity a Name
3. Select the Option called Local API
4. Enter the string pattern that when received through the serial port should trigger this interactivity.

IMPORTANT: The matching pattern is entered as a regular expression, therefore [special characters must be escaped](https://riptutorial.com/regex/example/15848/what-characters-need-to-be-escaped-). To escape a character  just add the "/" before the character. Here are the characters that must be escaped:

* Brackets: []
* Parentheses: ()
* Curly braces: {}
* Operators: \*, +, ?, |
* Anchors: ^, $
* Others: ., \

In order to use a literal ^ at the start or a literal $ at the end of a regex, the character must be escaped.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669408936/Interactivity-Nexmosphere-RegEx.png)
