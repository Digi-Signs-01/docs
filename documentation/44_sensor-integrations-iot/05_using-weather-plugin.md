---
title: "Using Weather Plugin"
slug: using-weather-plugin
publish: false
date: 2025-05-03
update: 2025-05-03
description: Using Weather Plugin
categories:
  - start
---

Using Weather Plugin
====================

The Player Local Weather Info is a Player Plugin. Once configured and published to the Player, it will fetch weather info every hour and store the retrieved data into the Players' Custom Attributes.

CONTACT US TO ENABLE THIS FEATURE ON YOUR ACCOUNT.

Before continuing, make sure you have a Player version of 10.1.0 or higher installed on your device.

Overview Local Weather Info Player Plugin
-----------------------------------------

Attributes work as a local variable on each Player and can be configured in your general Settings > Custom Attributes.

Select a unique Attribute for each Local Weather Info Player Plugin or just click on create a new App Attribute in the dropdown menu of the Plugin. Current Weather Conditions must be associated with an Attribute in Text format and all Temperature related Conditions must be in a Numeric format.

Weather Conditions are case sensitive and will always be set in lower case to one of these values:

* clear-day
* clear-night
* cloudy
* fog
* hail
* partly-cloudy-day
* partly-cloudy-night
* rain
* sleet
* snow
* thunderstorm
* tornado
* wind

### Player Location

By default, the Player Local Weather Info Plugin will retrieve information based on the player location, but in case this is not available, it is important to set the Fallback location.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671267348/weather%20plugin%201.png)

### Temperature Scale

Select either Celsius or Fahrenheit so the temperature is presented in the desired scale.

### Creating Weather based playback rules

Once the Weather Plugin is correctly configured and published, it will retrieve the Weather info and store it on each player attribute. With this it is possible to create custom rules so content is only played when specific weather criteria are matched.

These rules can be added to a specific content item, a playlist item, or when publishing content to your screens.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671309587/weather%20plugin%202.png)

Using Weather Infos (First time users)
--------------------------------------

1. First let’s create a new **Player Plugin**. On your Content page, click New > Player Plugin > Player Plugins.
2. Select the plugin Player Local Weather Info.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671383195/weather%20plugin%203.png)
3. Enter a name and create a new player attribute for all attributes. First for Weather Condition, then for: Temperature, Minimum temperature, and Maximum temperature. Find the option “Create New Player Attribute” in the dropdown list and define a proper name for the attribute. Set the Location Fallback and the Celsius or Fahrenheit scale, then save the plugin.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671398617/weather%20plugin%204.png)
4. Publish the new Automation App to available players. It must appear in the “Automation Loop” area. When the plugin is saved, go to your Player. Look for the "Plugins" menu and Add a Plugin:  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671410961/weather%20plugin%205.png)![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671426271/1a93ef53-e2b6-4ef9-b3a6-aedabfe0aa43.png)
5. Now, we can apply restrictions to images/videos, campaigns, or playlists.

How to apply weather restrictions?
----------------------------------

Restrictions are a staple of the content programming. You can set restrictions:

* [When Publishing](https://onsign.atlassian.net/wiki/spaces/OTT/pages/32276643)
* [To items in a Playlist](https://onsign.atlassian.net/wiki/spaces/OTT/pages/32145476)
* On an item in a Campaign Timeline
* [As a general restriction on a piece of content](https://onsign.atlassian.net/wiki/spaces/OTT/pages/32145813)

When you want to send your audience a PSA reminding them to drink water on a hot day, publish this message to your player with a restriction to only play when the weather is sunny and the temperature is 30°C or higher.

1. Go to publish the message.
2. Select your Players.
3. As Playback Restrictions select “Play only when..”
4. Change the Mode from Visual Mode to Logic Mode.
5. Scroll down to the attributes and look for the weather attribute.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671523299/weather%20plugin%207.png)
6. Set the weather conditions to "is sunny" and confirm with "Done".  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671561384/weather%20plugin%208.png)
7. Add a second item for the temperature. Scroll down to the temperature attribute and set it to "is greater than or equal to 30". This means 30°C when you have set the attribute to the Celsius temperature scale.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671578556/weather%20plugin%209.png)
8. Your result should look like this:  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671590816/weather%20plugin%2010.png)
9. Finish by clicking on the orange Publish button at the bottom of the page.  
   Now your message to drink water will only play when the weather is sunny and the temperature is over 30°C.
