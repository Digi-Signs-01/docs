---
title: "Multi Screen Synchronized Playback"
slug: multi-screen-synchronized-playback
publish: false
date: 2025-05-03
update: 2025-05-03
description: Multi Screen Synchronized Playback
categories:
  - start
---

Multi-screen Synchronized Playback
==================================

OnSign TV allows you to define a Master Player to synchronize Content playback on multiple screens.

Requirements

To ensure efficient synchronization, all Players must be connected to a wired high speed network.

While it is possible with this feature to mix hardware, we recommend to stay within one hardware type as much as possible. The more mixed the hardware, the less they will be in perfect sync.

### Supported on

* [Android](https://onsign.tv/android-overview/)
* [Windows](https://onsign.tv/windows-overview/)
* [LG webOS](https://onsign.tv/lg-overview/)
* [Samsung Smart Signage Platform (SSSP)](https://onsign.tv/samsung-overview/)
* [BrightSign](https://onsign.tv/brightsign-overview/)
* [Chrome OS](https://onsign.tv/chrome-overview/)

How to create multi-screen synchronized playback
------------------------------------------------

1. Create a [Player Group](/player-groups/how-to-create-player-groups).
2. Go to the option "Synchronized Playback" and enable it by checking the box.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731672151001/multi-screen-synchronized-playback_1.png)

3. A new field appears where you can select a Player to act as the "Lead Player".

The "Lead Player" will trigger a Loop restart on all other Players forcing the Loops to start in-sync.

* The content on the Players can be identical. In this case, all Players will be in perfect sync presenting the content.
* The content io the Players can be different. Each screen will show different content, but in-sync from the content loop start.
