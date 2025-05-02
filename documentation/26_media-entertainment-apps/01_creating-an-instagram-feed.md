---
title: "Creating An Instagram Feed"
slug: creating-an-instagram-feed
publish: false
date: 2025-05-03
update: 2025-05-03
description: Creating An Instagram Feed
categories:
  - start
---

Creating an Instagram feed
==========================

OnSign TV has several Apps to display Instagram content to choose from. Let's take the most simplest App called "Instagram". In this tutorial, we show you how to set it up.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657298524/create-instagram-feed_11.png)

1. First, you need to [integrate your Instagram account](/account-settings/connecting-social-media-accounts) with your OnSign TV account. Go to your account settings and look for the Integration Accounts on the menu. Click on "+ Add Account" and choose "Add Instagram Account".  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657377487/create-instagram-feed_12.png)
2. You will be send over to Instagram to grant OnSign TV access to your Instagram account. Click on the blue button to "Allow" it.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657391136/create-instagram-feed_13.png)
3. You will be sent back to OnSign TV telling you that your Instagram account was successfully added.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657403747/create-instagram-feed_14.png)
4. Now, you can create an App which allows you to show your Instagram content on your OnSign TV Players. As with every App, start by [creating a new App](/apps/creating-an-app) from your Content page. Click on the "New" button and select "App". In the App library look for the Instagram App.
5. Give the App a name. In the Instagram Account field you will see the name of your Instagram account. You can of course have several Instagram Accounts connected with your OnSign TV platform. In this case, select the applicable Instagram Account from the drop-down menu.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657442335/create-instagram-feed_15.png)
6. Configure the Instagram App further by selecting how many posts will be shown, if there is a transition between posts, the amount of time each post is shown on screen, as well as font, colors, backgrounds, and the language of labels.
7. Your Instagram feed is ready to be used.

Via Zapier (Deprecated)
-----------------------

In the way back past, Instagram had to be integrated via Zapier. For completeness, we leave this tutorial here, but it is no longer necessary to do it this way.

You need first to allow Zapier to access your Instagram account. If you don't have a Zapier account yet, [check out this tutorial and learn how to create it](/popular-apps-setup/creating-a-zapier-account). This will take less than two minutes by following these steps:

### Integrate accounts

1. On your [Zapier homepage](https://zapier.com/app/explore), click on your username on the top-right corner. Then, select “Connected Accounts” on the drop-down menu.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657530993/create-instagram-feed-for-onsign-tv_1.jpg)
2. Look for Instagram under “Connected Accounts” or just write it down on the text field. As you click on Instagram icon, a new dialog box will be displayed on your screen. Hit “Authorize” so Zapier can reach your account data.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657544370/create-instagram-feed-for-onsign-tv_2.jpg)
3. Your Instagram account will be listed on the Connected accounts page. To avoid confusion, we suggest you rename it in case you manage more Instagram accounts. Just click on the icon to the left of “Instagram Account 1#” and write a new name.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657556756/create-instagram-feed-for-onsign-tv_3.jpg)

### Create Instagram feed for OnSign TV

On Zapier, they call any computer automation a “zap”. So you can display your Instagram photos on OnSign TV, we are going to create a RSS feed which will collect all Instagram data. Check step by step below:

1. Click on “MAKE A ZAP!” at the top of the page.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657597150/create-instagram-feed-for-onsign-tv_4.jpg)
2. Select Instagram icon and then click “next”.
3. Choose from which source Zapier should collect photos: “New Liked Media” or “New Media Posted”. Use the first to show other users' posts the account has liked and the latter to show only content from the user. Hit “Save + Continue” at the bottom.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657616748/create-instagram-feed-for-onsign-tv_5.jpg)

Zapier requires at least one posted picture to be able to continue.

4. Choose the Instagram account you have just integrated on the previous step and then click “continue”.

5. In this step, Zapier requires you to test the zap by liking or posting a new photo on Instagram. You can just click “Fetch & Continue” or test it as required.

6. The following message should appear for you. Hit continue.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657676124/create-instagram-feed-for-onsign-tv_6.jpg)

7. Now, type “RSS” under “Choose an action app”. Select “RSS by Zapier” and click on “Save + Continue” on the loaded page.

8. The new page will display an form. Fill the fields as described below, then hit "Continue":

**URL:** Write “instagram-” and complement with whatever you want. Click on the button "Copy to clipboard" on the right. **Paste the URL somewhere because you will need it to** [**add the App on OnSign TV**](https://docs.onsign.tv/articles/docs/configure-zapier-instagram-rss-on-an-app).

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657726872/create-instagram-feed-for-onsign-tv_7.png)

**Max records:** 20

**Title:** Name it as you wish.

**Source:** Do not change the current text.

**Content:** copy and paste the following:

u={{user\_\_username}};ui={{user\_\_profile\_picture}};lc={{likes\_\_count}};cc={{comments\_\_count}};i={{images\_\_standard\_resolution\_\_url}};c={{caption\_\_text}}

As you paste the text above, you shoud see the following:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657775640/create-instagram-feed-for-onsign-tv_8.jpg)

**Pubdate:** Copy and paste the following.

{{created\_time}}

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657795252/create-instagram-feed-for-onsign-tv_9.jpg)

Zapier will display the feed URL. It will vary depending on your account and content. Just click on "Create & Continue".

10) Your zap will be tested. If it is successful, click on "Finish".

11) Last, but not least: don’t forget to turn your zap on! Also name it to find it on Zapier website easily.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731657814158/create-instagram-feed-for-onsign-tv_10.jpg)
