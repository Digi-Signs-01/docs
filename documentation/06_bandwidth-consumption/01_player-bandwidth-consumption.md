---
title: "Player Bandwidth Consumption"
slug: player-bandwidth-consumption
publish: false
date: 2025-05-03
update: 2025-05-03
description: Player Bandwidth Consumption
categories:
  - start
---

Player Bandwidth Consumption
============================

By default, the OnSign TV Players are designed to always be connected, so whenever there is any content update, all connected Players will immediately synchronize and download the updated content.

The Player bandwidth consumption depends on five factors:

* **Player Control Channel** - This is the data sent back and forth to the server, so the Player can check for Content updates and also report its basic status.
* **Player Statistics** - This is the data sent to the server containing Player resource usage such as CPU, memory, disk usage, among others, and Content playback report.
* **Player Media Download** - This is a direct result of all media downloaded to the Player.
* **Live Content** - This category includes web pages and streaming content (like YouTube).
* **Dynamic Data of Apps** - Apps will require the download of dynamic content to be shown on screens e.g.: weather info, currency info, etc.

To illustrate practical examples, here are three different scenarios with the average expected data consumption:

**Case 1.** A Player configured to:

* Present one Content every 15 seconds (it doesn’t matter if it is the same Content or different Content)
* Content Update Interval configured to Realtime
* Internet Data Saving Mode Disabled (this means the Player will report every Content playback)

This Player will consume about 150 Mb/month.

**Case 2.** The scenario as above, but with Content presented every 10 seconds will increase the total bandwidth consumption.

**Case 3.** If you publish a media of 100 Mb size.

* The Player will download 100 Mb + some additional data for the control channel.
