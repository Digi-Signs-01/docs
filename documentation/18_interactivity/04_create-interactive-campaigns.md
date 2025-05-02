---
title: "Create Interactive Campaigns"
slug: create-interactive-campaigns
publish: false
date: 2025-05-03
update: 2025-05-03
description: Create Interactive Campaigns
categories:
  - start
---

Create interactive Campaigns
============================

Let your customers fully engage with the screens by creating interactive Campaigns.

Supported on OnSign TV Player App for Android 4.2.0+ and Windows App 9.1.1+

This feature turns screen areas clickable, revealing further content or leading to another Campaign. By adding interactivity, clients are able to explore the Campaign’s content as they want, in the order they want too.

There are several use cases for interactivity on Campaigns. In a restaurant, for instance, a promotional ad banner can lead to further details, like price, conditions, applicable dates, and so forth, on the main screen.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731676908235/create-interactive-campaigns_1.gif)

To learn how to apply interactivity, try making the Campaign shown above by repeating the following steps. Afterwards, you will be able to implement it with your own Campaign idea. [Download all required files](https://docs.onsign.tv/resources/Storage/en/create-interactive-campaigns/Interactive-campaign-Restaurant.zip) and let's go!

1. Create a new Campaign in your OnSign TV account. Select a two-zone preset layout.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731676966533/create-interactive-campaigns_2.jpg)
2. Place three images on the larger area 1. Drag two bar apps and the "Promotion banner" to the bottom area 2.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731676979125/create-interactive-campaigns_3.jpg)
3. Afterwards, just upload the image you want to show when the patron clicks on the screen. In this tutorial's case, it is the "more info promotion" image. Do **not** place it into the Campaign just yet.
4. Click “Save".
5. On the loaded page, select “Interactivity” from the sidebar menu.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677025778/create-interactive-campaigns_4.jpg)
6. Click the “Add interaction” button on the top-right. A panel with all interaction settings will be displayed. Check out each field's function:  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677038739/create-interactive-campaigns_5.png)
   * **Name:** If you want to allow several interactions, naming them makes it easier to know which setting does what.
   * **What:** Define what the audience has to do in order to reveal the Content. It can be either touching the screen, pressing a key, an API command, or simply a previous Content timing out.
   * **Which one:** Specify which region of the Screen Layout the person needs to click to trigger the action. If you choose to trigger the Campaign by pressing a key, define which key will do it.
   * **Action:** Define what is going to happen when the person interacts with the screen. You can either **play** another Campaign or **replace** a screen zone with another media item. In both cases, you need to choose a destination.   
     *Important: In case you choose to play another Campaign, there is no need to publish it to the Player as it will be downloaded automatically.*
   * **Destination:** For "Replace", set where on screen the file will be shown after the user touches the screen ("Region 2", for instance). For the Action "Play", choose which Content will play next.
   * **When playing:** This field works as a filter for the Action. If you keep “any media”, any time you click the defined screen area, the Action will be carried out (a Campaign will play back or a file will appear on the area you set as Destination). Change this field if you want the action to be performed only when a specific media is playing.
   * **With media:** This field is only active for the "Replace" Action. Select the file which should appear in the Destination you set after the interaction. You can choose [any media format](/media/supported-file-types).
7. For this tutorial's purpose, fill out the settings as shown below:  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677178714/create-interactive-campaigns_6.png)
   * Name: Promotion
   * What: Touch region
   * Which one: Region 2
   * Action: Replace
   * Destination: Region 1
   * When playing: Promotion banner.png
   * With media: More info promotion.png
   * Duration: 30s
8. Click on the check mark to the left and then hit “Save”.
9. Click on “Publish” on the menu on the left. Publish the Campaign to a Player and test the interactivity.

Besides for a Campaign, interactivity can also be set to an entire Player.

OnSign TV Academy - Touch Screen Interactivity
----------------------------------------------
