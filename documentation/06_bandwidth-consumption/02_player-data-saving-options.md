---
title: "Player Data Saving Options"
slug: player-data-saving-options
publish: false
date: 2025-05-03
update: 2025-05-03
description: Player Data Saving Options
categories:
  - start
---

Player Data Saving Options
==========================

OnSign TV offers three options to configure on each Player to reduce the bandwidth usage:

Option 1 - Download Schedule
----------------------------

This will define what time of the day the Player is allowed to download new Content. This feature is very helpful to avoid the Players from competing for bandwidth at an office during the day.

The [Download Schedule](/player-download-settings/content-download-schedule) will also block the updates of:

* RSS,
* MRSS,
* Apps based on fetch\_text.

[Download Schedule](/player-download-settings/content-download-schedule) will NOT block the updates of:

* Calendar,
* Currency,
* Weather,
* YouTube,
* Website Link,
* Famous Quotes,
* Content Channels,
* X (previously Twitter) (no longer supported),
* Upcoming Movies,
* Birthday Announcements.

Option 2 - Content Update Interval
----------------------------------

The [Content Update Interval](/player-download-settings/content-update-interval) will define how often your Player will check for updates. By default, the Player is set to "Realtime", meaning the Player will immediately synchronize when there is a Content update.

The [Content Update Interval](/player-download-settings/content-update-interval) can range from Realtime all the way up to 48 hours. Checking for updates less often will reduce the amount of data consumed by your Player.

### IMPORTANT NOTE:

* Remote view is only available for Players which are configured to Realtime.
* Players which are not configured to "Realtime" will be shown as offline. This happens as the Players are truly not talking to the server in-between the set update interval. If you keep watching, it is possible to see the Player connecting and synchronizing the Content each time the update interval is up next.

Option 3 - Enable Internet Data Saving Mode
-------------------------------------------

This is by far the most efficient method to reduce the amount of data transferred. Once enabled, the Player will stop sending statistics and playback events to the server. As a side effect, no playback reports and no resource usage statistics will be available for this Player.
