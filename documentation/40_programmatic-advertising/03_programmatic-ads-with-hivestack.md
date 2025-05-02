---
title: "Programmatic Ads With Hivestack"
slug: programmatic-ads-with-hivestack
publish: false
date: 2025-05-03
update: 2025-05-03
description: Programmatic Ads With Hivestack
categories:
  - start
---

Programmatic Ads with Hivestack
===============================

Hivestack OnSign TV Integration
-------------------------------

Programmatic platforms are a strong trend and a great way to increase DOOH advertisement sales.

Hivestack is a full-featured, world-wide Programmatic Advertising Platform offering easy access to the largest DSPs in the market, such as Yahoo OmniChannel and Google DV360.

This tutorial describes how to integrate OnSign TV Screens with Hivestack.

**Requirements:**

* An active **OnSign TV Account**
* An active **Hivestack Account**
* You should have a **Hivestack API Key**given by Hivestack for making ad requests
* You will need a **Hivestack Screen ID** for each Player screen
* ****Player requirements:****

We recommend using players version 10.5.0 or later for Programmatic Ads to leverage OnSign’s advanced programmatic ad caching.

**IMPORTANT** - Programmatic integration ****will not work**** in case the OnSign TV App is outdated, or in case the SoC firmware is not matching the requirements.

The OnSign TV Account must be enabled for the following features which are not enabled by default:

* Custom Attributes
* App Events
* Hivestack App

Step 1 - Configuring Custom Player Attributes
---------------------------------------------

****Custom** **Player** **Attributes**** work as local Player variables which Apps can access during playback time.

Once a Custom Player Attribute is created from the settings menu, it will be possible to enter a Custom Attribute for each Player.

Custom Player Attributes are configured on each Player in ****Settings > Custom Attributes****

To use the Hivestack App, these two Custom Attributes must be configured:

* Hivestack API Key - Type Text
* Hivestack Screen ID - Type Text

Custom Attributes are case-sensitive and must be entered in the exact spelling.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662406629/programmatic-ads-with-hivestack_1.jpg)

Now that the Custom Player Attributes are created, the Hivestack API Key and Screen ID need to be configured in the settings of every Player.

1. Click on the Player Menu
2. Select a specific Player
3. Click on Settings
4. Enter the Hivestack API Key and Hivestack Screen ID

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662440680/programmatic-ads-with-hivestack_2.jpg)

Step 2 - Set up the Hivestack App
---------------------------------

Configuring the Hivestack App follows the same process as any other OnSign TV content application.

Click on the Content menu and navigate to the folder where the Hivestack App should be stored.

Click the New button > App > Then type "Hivestack" into the search box and select the Hivestack App.

1 - Configure the App name (like any other OnSign TV App).

2 - Select the **Hivestack Environment** the App should connect. This is either Staging, in case you are still validating the solution, or Production, in case your environment is set and ready for showing Ads to your audience.

3 - **Select a fallback image**. This will be shown when there is no Creative available from Hivestack or when there is not enough time to retrieve the Creative from the Hivestack platform.

The Debug mode can be activated to provide additional information. This is a handy way to ensure all is working as expected or to debug what is wrong in case the App is not correctly presenting the Creatives.

Common errors are:

* Using a wrong API Key or an invalid Screen ID won't allow the App to obtain the Creatives from the Hivestack server.
* The media is too large and the complete media download was not fully executed on time to be presented. Don't worry, as the media will be downloaded in the background and should be gracefully presented in the next cycle.

Here is an App published with the Debug mode enabled.

Note that as the retrieved media is 20 seconds long, the playback of this media will be exactly 20 seconds, even if the published duration of the container is larger.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662496273/programmatic-ads-with-hivestack_3.jpg)

Step 3 - Create a Wrapper Campaign
----------------------------------

The Hivestack App has a variable length behavior. This allows the playback of Creatives with different lengths coming from Hivestack. To take advantage of this feature, the Hivestack App should be placed in a container which is at least as long as the largest Creative to be presented.

For example, if the Creative has a maximum length of 15 seconds, the App should be placed either in a Campaign which lasts at least 15 seconds or within a Playlist, and then the Playlist item should be set as 15 seconds.

Still, due to its variable behavior, if the received Creative is only 10 seconds long, the item will be only played for 10 seconds and skip to the next item.

Step 4 - Hivestack App Playback Report
--------------------------------------

OnSign TV can provide two different reports for the Hivestack App:

* **Content Playback Report** - This will count the times the Hivestack App has been presented.
* **App Events** - This will provide detailed information for every media played by the Hivestack app. This is a great way to cross-reference the number of presented ads, comparing it to the Hivestack Platform reports.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731662547985/programmatic-ads-with-hivestack_4.jpg)

**Firewall requirements**
-------------------------

In addition to the [OnSign firewall settings](/network-settings/firewall-settings), please ensure the following domains can be accessed from each player that needs to present Hivestack programmatic Ads:

* apps.hivestack.com (To send ad request and play confirmation calls)
* dgg3rnz8nudgw.cloudfront.net (To download the creative files)
* cdn-apps.hivestack.com (To download the creative files)

**Investigating Errors**
------------------------

If the Hivestack app is not behaving as expected, the most likely issues are:

* **No network** – If there is no network, the app can't check if there is a designated ad to be presented.
* **Wrong or missing credentials** – If anyhow the OrgID or Screen ID is missing, the app will not be able to query for available ads.

**Testing your Hivestack Credentials**
--------------------------------------

Testing your Hivestack credentials is quite simple, just open one of the two URLs below, replacing the [ScreenID] and [Org\_ID] with your credentials.

### **Staging** – If your credentials working only on staging and testing environment

```
https://uat.hivestack.com/nirvana/api/v1/units/schedulevast/[SCREEN_ID]?apikey=[API_KEY]
```

### **Production** – If your credentials are already available on production environment

```
https://apps.hivestack.com/nirvana/api/v1/units/schedulevast/[SCREEN_ID]?apikey=[API_KEY]
```
