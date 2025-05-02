---
title: "Playing On Demand Content"
slug: playing-on-demand-content
publish: false
date: 2025-05-03
update: 2025-05-03
description: Playing On Demand Content
categories:
  - start
---

Playing on-demand Content
=========================

"**On-demand Content**" is a great way to trigger a specific piece of Content on one or multiple Players only when the need for it arises!

This feature is ideal for displaying emergency messages, impromptu sales, and any type of live content you would like to pop up on your screens!

**Follow these steps to publish an on demand Content.**

1. On the Content page of your OnSign TV account, right-click on the Content you wish to set a trigger to, and select “**Publish**” from the pop-up menu.
2. Select where the content will be published, either **Players our Player Groups**
3. Scroll down to the "**How to Play It**" header and expand the drop-down menu.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692485562/play-content-on-demand_1.png)
4. Select “**Play On-Demand**”  
   In addition to triggering an on-demand, OnSign TV allows to setup a redirect URL to be loaded by the browser that makes the on-demand content request. A great use case for this is to [create a QR Code with the on-demand link](https://onsign.atlassian.net/wiki/spaces/OTT/pages/edit-v2/32145835?draftShareId=b5c1e5f9-7662-43e9-980f-59f072a8aafb#Triggering-with-content-using-the-on-demand-link "https://onsign.atlassian.net/wiki/spaces/OTT/pages/edit-v2/32145835?draftShareId=b5c1e5f9-7662-43e9-980f-59f072a8aafb#Triggering-with-content-using-the-on-demand-link"), so once the code is scanned the browser will get redirected to the configured Redirect to URL.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692516964/play-content-on-demand_2.png)
5. Once published, your on-demand Content will show in each Player or Player Group published content.

Triggering an on-demand Content from Player Content
---------------------------------------------------

With these few steps you trigger Content on a Player from your account.

1. Click on the **Players** tab on the left-hand side.
2. Select the Player where the Content has been published to.
3. Select “**Content in Players**” from the sidebar menu.
4. Find the on-demand Content within Triggered Content and click on the play icon on the right-side.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692557718/play-content-on-demand_4.png)  
   **Note**: Triggering on-demand Content on Player Groups follows a similar process: select the target Player Group where the Content has been published. Click on "Content in Group". All other steps are the same.
5. A pop-up window will ask how many times in a row you want the Content to be displayed on the Player before resuming the normal playback loop. If you want it to be displayed infinitely, write “0”. Then you have to actively stop the playback like you see below.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692579385/play-content-on-demand_5.png)

Triggering with content using the on-demand link
------------------------------------------------

When an on-demand content is published, a special link is created that can be used to trigger it.

To obtain the on-demand link, just click on the "Chain icon" within the Triggered Content as shown below.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692603928/play-content-on-demand_4%20(1).png)

This will open another pop-up, so you can copy or change the on-demand URL:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692615367/playing-on-demand-content-2024-03-14.png)

The on-demand URL accepts two parameters:

**Queue** - This will only play the on-demand content after the current content being played is finished. Here is an example of how to use the queue action:

* [https://app.onsign.tv/play/DJXzrLqMuQ9N8YDgnWeS](https://app.onsign.tv/play/DJXzrLqMuQ9N8YDgnWeS "https://app.onsign.tv/play/DJXzrLqMuQ9N8YDgnWeS")**?action=queue**

**Repeat** - This will set how many times the on-demand content should be repeated. If repeat is =0, then the on-demand content will be repeated for ever, or until a "Stop On-demand" is sent. Syntax example below:

* [https://app.onsign.tv/play/DJXzrLqMuQ9N8YDgnWeS](https://app.onsign.tv/play/DJXzrLqMuQ9N8YDgnWeS "https://app.onsign.tv/play/DJXzrLqMuQ9N8YDgnWeS")**?repeat=0**

Stop on-demand Playback
-----------------------

When ever you want to pause the Content playback, press the blue “**Stop On Demand Playback**” button in the Triggered Content header.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731692647082/play-content-on-demand_4%20(2).png)

OnSign TV Academy - Content Publishing and Playback Rules
---------------------------------------------------------

OnSign TV Academy - On-demand Content Playback
----------------------------------------------
