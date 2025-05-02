---
title: "Programatic Ads With Place Exchange"
slug: programatic-ads-with-place-exchange
publish: false
date: 2025-05-03
update: 2025-05-03
description: Programatic Ads With Place Exchange
categories:
  - start
---

Programatic Ads with Place Exchange
===================================

Place Exchange OnSign Integration
---------------------------------

IMPORTANT: Programmatic Ads is a separate service not included in the standard OnSign license. Please contact our team if you are interested in subscribing to it.

**Requirements:**

* An active **OnSign TV Account**
* An active **PlaceExchange Account**
* You should have a **PlaceExchange Organization ID** given by PlaceExchange
* You will need a **PlaceExchange Ad Unit Name**  for each Player screen
* **Player requirements:**
  + **Windows, Android, or Linux** player -  Running OnSign TV App version 10.3.0 or higher
  + **Samsung SSSP6** - Running OnSign TV App 10.3.5 or above and Firmware 2430.3 or above
  + **LG webOS 6** - Running OnSign TV App 10.3.5 or above and Firmware 03.68.33/1.6.8 or above

IMPORTANT: The Programmatic integration **will not** work in case the OnSign TV App is outdated, or in case the SoC firmware is not matching the requirements.

The OnSign TV Account must be enabled for the following features which are not enabled by default:

* Custom Attributes
* App Events
* Player Plugin
* PlaceExchange App

Step 1 - Configuring Custom Player Attributes
---------------------------------------------

**Custom Player Attributes** work as local Player variables which Apps can access during playback time.

Once a Custom Player Attribute is created from the settings menu, it will be possible to enter a Custom Attribute for each Player.

Custom Player Attributes are configured on each Player in **Settings > Custom Attributes**

To use the Place Exchange App, these two Custom Attributes must be configured:

* **PlaceExchange Organization ID** - Type Text
* **PlaceExchange Ad Unit Name** - Type Text

Custom Attributes are case-sensitive and must be entered in the exact spelling.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731663498632/programatic-ads-with-place-exchange-2024-06-17.png)

Now that the Custom Player Attributes are created, the PlaceExchange Organization ID and Screen ID need to be configured in the settings of every Player.

1. Click on the Player Menu
2. Select a specific Player
3. Click on Settings
4. Enter the PlaceExchange Organization ID and Screen ID

Step 2 - Set up the PlaceExchange App
-------------------------------------

Configuring the Place Exchange App follows the same process as any other OnSign TV content application.

Click on the Content menu and navigate to the folder where the Place Exchange App should be stored.

Click the New button > App > Then type "Place Exchange" into the search box and select the Place Exchange App.

1 - Configure the App name (like any other OnSign TV App).

2 - **Select a fallback media**. This will be shown when there is no Creative available from PlaceExchange or when there is not enough time to retrieve the creative from the PlaceExchange platform.

The Debug mode can be activated to provide additional information. This is a handy way to ensure all is working as expected or to debug what is wrong in case the App is not correctly presenting the Creatives.

Common errors are:

* Using a **PlaceExchange Organization ID** or an **Ad Unit Name** won't allow the App to obtain the Creatives from the PlaceExchange server.
* In case the media is too large and the complete media download was not fully executed on time to be presented. Don't worry, as the media will be downloaded in the background and should be gracefully presented in the next cycle.

Here is an App published with the Debug mode enabled.

Note that as the retrieved media is 20 seconds long, the playback of this media will be exactly 20 seconds, even if the published duration of the container is larger.

### Step 3 - Programmatic Plugin to each player

In addition to a dedicated app for each SSP platform, the OnSign team has developed a Programmatic Ad plugin. This plugin provides a return channel to each programmatic SSP, confirming the playback of each programmatic ad.

Handling programmatic ad confirmation through the plugin offers a significant advantage: it ensures that the event is not dependent on the ad's display time. This architecture enhances reliability and can withstand temporary network issues, allowing the plugin to confirm ad playback up to 10 minutes after it occurs.

The Programmatic Plugin is generic, supporting all OnSign TV integrated programmatic platforms. Only one instance needs to be added per player.

Therefore, for any player presenting Programmatic Ads, a Programmatic Plugin must be configured and installed.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731663585115/programatic-ads-with-place-exchange-2024-06-17-4.png)

Step 4 - Create a Wrapper Campaign
----------------------------------

The PlaceExchange App has a variable length behavior. This allows the playback of Creatives with different lengths coming from PlaceExchange. To take advantage of this feature, the PlaceExchange App should be placed in a container which is at least as long as the largest Creative to be presented.

For example, if the Creative has a maximum length of 15 seconds, the App should be placed either in a Campaign which lasts at least 15 seconds or within a Playlist, and then the Playlist item should be set as 15 seconds.

Still, due to its variable behavior, if the received Creative is only 10 seconds long, the item will be only played for 10 seconds and skip to the next item.

Step 5 - Programmatic App Playback Report
-----------------------------------------

OnSign TV can provide two different reports for the PlaceExchange App:

* **Content Playback Report** - This will count the times the PlaceExchange App has been presented.
* App Events - This will provide detailed information for every media played by the PlaceExchange App. This is a great way to cross-reference the number of presented ads, comparing it to the PlaceExchange Platform reports.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731663638434/programatic-ads-with-place-exchange-2024-06-17-1.png)

**Investigating Errors**

If the PlaceExchange App is not behaving as expected, the most likely issues are:

* **No network** - If there is no network, the app can't check if there is a designated ad to be presented.
* **Wrong or missing credentials** - If anyhow the OrgID or Screen ID is missing, the app will not be able to query for available ads.
