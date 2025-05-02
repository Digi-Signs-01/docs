---
title: "Quividi Integration"
slug: quividi-integration
publish: false
date: 2025-05-03
update: 2025-05-03
description: Quividi Integration
categories:
  - start
---

Quividi Integration
===================

In this tutorial we will demonstrate how to configure the OnSign TV to work with Quividi VidiReports.

Requirements for this demonstration
-----------------------------------

* OnSign TV Player version 10.3.x or installed on a media player
* VidiReports properly configured and running on a Windows PC.
* The IP address of the VidiReports PC

1- Configure Quividi plugin
---------------------------

In order to obtain audience metrics information from VidiReports and populate APC data, OnSign TV uses a plugin that exchanges information with VidiReports.

In your "Content" page, start by clicking on the "New" button and choosing “Plugin”

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670751262/91272927-7608-4dc4-8428-adb348a878fa.png)

From the "Third Party" pane, chose "Quividi Audience Tracking"

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670765530/Quividi-OnSign%20App.png)

Start by giving it a name that uniquely identifies this plugin instance.

In order to configure the plugin you need to set the name of the player attributes that will be set with the audience data. These attributes can be used later on to trigger content or impose restrictions based on the attribute value.

The plugin asks you to connect 6 attributes. You can connect them to an existing attribute or choose to create a new one.

* Total Audience
* Watching Audience
* Audience Male Percentage
* Audience Female Percentage
* Audience Age 0-19 Percentage
* Audience Age 20-29 Percentage
* Audience Age 30-39 Percentage
* Audience Age 40-49 Percentage
* Audience Age 50+ Percentage

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670807240/9eedfb60-840c-4a37-8d89-870133d8da35.png)

The next step is to configure the Quividi Device IP address and ports.

If you did not change the default ports on the Quividi device, there will be no need to change these values.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670831220/517f3d45-0daa-43cc-b203-567686d2a7df.png)

Once the plugin is properly configured, click on the Save button.

2- Install the Quividi plugin on the player
-------------------------------------------

Once the plugin is created, you need to add it to your player. Please note that this plugin can be added on more than one player. In this case all the players that have this plugin, will try to get audience information from the configured VidiReports device.

In order to install the plugin, on the player page chose the Plugins tab and click on "Add Plugin"

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670859732/095de2b4-869c-4551-8846-2f927aedb88a.png)

Search for the plugin instance in your content area and add it to the player.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670874092/46316a3c-193d-4274-a318-7c11380cdd95.png)

3- Test the plugin
------------------

Publish your signage content to the player as usual.

Once you have some content playing we are ready to test the plugin.

If the plugin is properly configured and VidiReports is running, you will see in the "Player Status" page the following event:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670905123/f40df7b3-85ae-4f4c-804a-0702b896aa41.png)

If you receive an error event like shown below, please double check the IP address, network access and if VidiReports is running on the device:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670919799/dc4c9c1a-1443-4300-8290-7f2af2b54b7c.png)

If the plugin is properly configured, it will start retrieving information from VidiRepors and storing in the player attributes. This can be checked in the player settings pane, where all attributes are shown:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670938808/c2588209-0b67-4e1c-adcf-45e35f72e117.png)

**Important:** Please note that attributes are changed on the player in real time and can be used to change the content being played. On the server side this is updated every 5 minutes, so the values shown on the settings page will not necessarily reflect the current state of the player.

The plugin will also automatically report content playback information to VidiReports in order to allow APC dashboards.

4- Install the Quividi Audience Overlay App (Optional)
------------------------------------------------------

If you want to display audience information in real time on your media player, you can publish the Quividi Audience App.

This app retrieves information from the attributes set by the Quividi plugin and displays it on the player.

This app can be found in the "Third Party" section of our app selection dialog.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670990509/a1725bb5-92db-451b-80c3-55e246800736.png)

In order to configure it, give it a name and connect it to the same attributes you configured in the plugin app:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671012442/6be7cab7-6249-4c71-aa3a-46cb66a71fd2.png)

Once configured, publish it to the player.

Note that this app is designed to be used as an overlay on top of other content. Using it in a campaign with overlapping regions will give you best results.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671057499/9a80b52f-8e3b-401d-9f4a-d2dc08746695.png)

Once published it will show audience changes in real time.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671068343/18ff800e-6244-4d2e-ab35-b4883389ad53.png)

5- Add restrictions based on audience data (Optional)
-----------------------------------------------------

Once the player attributes are being set with real time audience data from the Quividi plugin, you can use it to customize the playback of your content in many different ways.

You can add content playback restrictions based on the specific value of an attribute, like shown below:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671098405/9834fa90-b22e-42bb-9609-54d1a5620d44.png)

Alternatively, you can also trigger content when an attribute value reaches a specific threshold.

In the example below, the content will be triggered, interrupting the current content, when "Watching Audience" becomes greater than 2.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731671112784/221607b5-2bf5-43f0-ac50-e95e63c24421.png)
