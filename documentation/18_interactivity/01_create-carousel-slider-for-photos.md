---
title: "Create Carousel Slider For Photos"
slug: create-carousel-slider-for-photos
publish: false
date: 2025-05-03
update: 2025-05-03
description: Create Carousel Slider For Photos
categories:
  - start
---

Create carousel slider for photos
=================================

Let the audience decide when it's time to switch the image, as opposed to a non-stop loop.

Supported on the OnSign TV  Player App for Android 4.2.0 or higher and Windows 9.1.1 or higher.

Assemble photos in an image carousel slider with the interactivity feature. Check out the result below:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678173470/create-carousel-slider-for-photos_1.gif)

In this tutorial, we are going to create a simple four photo carousel. Get the images used for the Campaign shown above from this [zip file](https://onsign.tv/media/caroussel-slider.zip "https://onsign.tv/media/caroussel-slider.zip"), or use your own images.

Besides creating a Campaign from scratch, we are going to use the interactivity feature. If you don’t know how to use Interactivity, we highly recommend you first take a look at the following tutorials to better understand the topic:

* [Create interactive Campaigns](/interactivity/create-interactive-campaigns "https://onsign.atlassian.net/wiki/spaces/OTT/pages/33488897")
* [Create interactive menus](/interactivity/create-interactive-menus "https://onsign.atlassian.net/wiki/spaces/OTT/pages/33423378")
* [Create expanded interactive menus](/interactivity/create-expanded-interactive-menus "https://onsign.atlassian.net/wiki/spaces/OTT/pages/33554444")

1. In your OnSign TV account, create a Campaign. Fill out the basic info, such as name and category.
2. A carousel slide consists of three basic elements: a central photo frame and two buttons to go back and forth on the pictures. Hence, click on “Add Custom Layout” in your Campaign and create a zone for each of those. We have also created a screen zone for the background image.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678263301/create-carousel-slider-for-photos_2.jpg)
3. Upload the images you are going to use in this specific Campaign to your OnSign TV account. In your Timeline, place the buttons in their respective screen zone and place the background image and a single photo of the carousel.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678324030/create-carousel-slider-for-photos_3.jpg)

Don’t place more than one photo in the carousel frame, or else it won't obey the commands of the buttons we will set later and instead play a non-stop loop.

4. Publish the Campaign to a Player. When you reach the “Published to these Players” page, select “Interactivity” from the menu on the left below the Campaign thumbnail.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678343299/create-carousel-slider-for-photos_4.jpg)

5. Now, we are going to add Interactivity to our carousel slider! Before setting any actions, decide on the carousel photo sequence. We have used the following sequence to the pictures available in the zip file: IAdea.png > J22.png > minix x5.png > minix x7.png > IAdea > J22 (...) etc.

With this sequence set, we need to set an action to both buttons around each photo. It is important that one action only happens to a specific photo, so we need to apply filters to each action.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678471623/create-carousel-slider-for-photos_5.png)

Let’s first set the action for the next button when the IAdea photo is exhibited in the Campaign. Fill out the fields as follows:

* **Name**: a name which indicates for you what is going to happen, here "image flip".
* **What**: Touch region.
* **Which one**: Region 4, which is the next button.
* **Action**: Replace.
* **Destination**: Region 2, which is the photo frame.

In the row below, we set a filter so it only changes to the next photo of the sequence (J22.png) when the specific photo is on screen. Thus, only when “IAdea.png” is shown, the next button will change it to “J22.png”.

* **When playing**: IAdea
* **With Media**: J22

6. Apply actions to all the following buttons with the right filters. This is going to be a little bit of effort, but it's worth it. Don't forget the back button!

7. Click on “Save changes” when you are done and test the Campaign on your Player!
