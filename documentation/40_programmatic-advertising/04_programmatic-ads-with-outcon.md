---
title: "Programmatic Ads With Outcon"
slug: programmatic-ads-with-outcon
publish: false
date: 2025-05-03
update: 2025-05-03
description: Programmatic Ads With Outcon
categories:
  - start
---

Programmatic Ads with Outcon
============================

Outcon OnSign TV Integration
----------------------------

**Requirements:**

* An active **OnSign TV Account**
* An active **Outcon Account**
* You should have a **Outcon Publisher ID** given by Outcon
* You will need a **Outcon Screen ID** for each Player screen
* **Player requirements:**
  + **Windows, Android, or Linux** player -  Running OnSign TV App version 10.3.0 or higher
  + **Samsung SSSP6** - Running OnSign TV App 10.3.5 or above and Firmware 2430.3 or above
  + **LG webOS 6** - Running OnSign TV App 10.3.5 or above and Firmware 03.68.33/1.6.8 or above

**IMPORTANT** - The Programmatic integration **will not work** in case the OnSign TV App is outdated, or in case the SoC firmware is not matching the requirements.

The OnSign TV Account must be enabled for the following features which are not enabled by default:

* Custom Attributes
* App Events
* Outcon App

Step 1 - Configuring Custom Player Attributes
---------------------------------------------

**Custom Player Attributes** work as local Player variables which Apps can access during playback time.

Once a Custom Player Attribute is created from the settings menu, it will be possible to enter a Custom Attribute for each Player.

Custom Player Attributes are configured on each Player in **Settings > Custom Attributes**

To use the Outcon App, these two Custom Attributes must be configured:

* Outcon Publisher ID - Type Text
* Outcon Screen ID - Type Text

Custom Attributes are case-sensitive and must be entered in the exact spelling.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662873906/outcon-app.png)

Now that the Custom Player Attributes are created, the Outcon Publisher ID and Screen ID need to be configured in the settings of every Player.

The Outcon Screen ID must be unique for each configured screen or player. When configuring IDs in Player settings, remember to generate a new ID in Outcon for the new screen/player.

1. Click on the **Player Menu**
2. Select a **specific Player**
3. Click on **Settings**
4. Enter the **Outcon Screen ID**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662950135/outcon-id.png)

Step 2 - Set up the Outcon App
------------------------------

Configuring the Outcon App follows the same process as any other OnSign TV content application.

Click on the Content menu and navigate to the folder where the Outcon App should be stored.

Click the New button > App > Then type "Outcon" into the search box and select the Outcon App.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662984949/config.png)

1 - Configure the App name (like any other OnSign TV App).

2 - Check the checkbox "**Demo Mode Enabled**" to connect the app to the **Staging Environment**. This is useful in case you are still validating the solution, or uncheck the option to set as **Production**, in case your environment is set and ready for showing Ads to your audience.

3 - **Select a fallback image**. This will be shown when there is no Creative available from Outcon or when there is not enough time to retrieve the Creative from the Outcon platform.

The "**Debug mode**" can be activated to provide additional information. This is a handy way to ensure all is working as expected or to debug what is wrong in case the App is not correctly presenting the Creatives.

Common errors are:

* Using a invalid Publisher ID or Screen ID won't allow the App to obtain the Creatives from the Outcon server.
* The media is too large and the complete media download was not fully executed on time to be presented. Don't worry, as the media will be downloaded in the background and should be gracefully presented in the next cycle.

Here is an App published with the Debug mode enabled.

Note that as the retrieved media is 20 seconds long, the playback of this media will be exactly 20 seconds, even if the published duration of the container is larger.

Step 3 - Create a Wrapper Campaign
----------------------------------

The Outcon App has a variable length behavior. This allows the playback of Creatives with different lengths coming from Outcon. To take advantage of this feature, the Outcon App should be placed in a container which is at least as long as the largest Creative to be presented.

For example, if the Creative has a maximum length of 15 seconds, the App should be placed either in a Campaign which lasts at least 15 seconds or within a Playlist, and then the Playlist item should be set as 15 seconds.

Still, due to its variable behavior, if the received Creative is only 10 seconds long, the item will be only played for 10 seconds and skip to the next item.

Step 4 - Outcon App Playback Report
-----------------------------------

OnSign TV can provide two different reports for the Outcon App:

* **Content Playback Report** - This will count the times the Outcon App has been presented.
* **App Events** - This will provide detailed information for every media played by the Outcon app. This is a great way to cross-reference the number of presented ads, comparing it to the Outcon Platform reports.

Step 5 - Testing your Credentials
---------------------------------

Outcon requires two credentials to correctly retrieve ads:

* **Outcon Publisher ID** - Unique number to identify the advertising network
* **Outcon Screen ID** - Unique string to identify the specific screen

To ensure your  credentials are correct, you can enter this URL replacing the elements in BOLD with your credentials:

```
https://api.outcondigital.com/ad/get?internalId=[SCREEN_ID]&publisher=[PUBLISHER_ID]
```
