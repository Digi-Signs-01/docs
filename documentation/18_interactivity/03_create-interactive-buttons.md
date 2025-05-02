---
title: "Create Interactive Buttons"
slug: create-interactive-buttons
publish: false
date: 2025-05-03
update: 2025-05-03
description: Create Interactive Buttons
categories:
  - start
---

Create interactive buttons
==========================

Allow your audience to interact with your Campaign at the touch of a button.

Supported on the OnSign TV Player App for Android 4.2.0 or higher and Windows 9.1.1 or higher.

Before you create buttons, you have to establish where the button is going to be on your screen and what the button is supposed to do. To design the image with the button, you can use the [Composition Creator](/media/using-composition).

Let's walk through a very easy scenario where you just want to have one button on screen which will give out an aquarium image when clicking the button.

1. Go into your OnSign TV account and create a Composition with a blue background and an orange area where the button is going to be.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678676682/how-to-create-interactive-buttons_1.png)
2. Next, create a new Campaign. Name the Campaign and then create a new Custom Layout which matches the Composition you have designed. We have the background area (A) and the button zone (B). The more accurate you are with the position the better.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678699264/how-to-create-interactive-buttons_2.png)
3. Now, we add the Composition we previously created into the Timeline in area A. For area B, we use a transparent png image. In the Timeline, you will not add the image of the aquarium we want to display at the click of the button.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678712118/how-to-create-interactive-buttons_3.jpg)
4. "Save and Publish" the Campaign.
5. On the newly loaded page "Publish to These Players", click on Interactivity.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678740195/how-to-create-interactive-buttons_4.jpg)
6. This is the last step. You need to set the rules for the interactive button. Click on "Add Interaction" and fill out the fields as follows:  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731678755227/how-to-create-interactive-buttons_5.png)
   * **Name:** Touch region  
     This is just for yourself so that you know what is going to happen.
   * **What:** Touch region  
     We want the touch of the button to provoke the image change.
   * **Which one:** Region 2  
     This is our button.
   * **Action:** Replace  
     When the button is clicked a new image will display.
   * **Destination:** Region 1  
     The image will be displayed in the main screen area (A).
   * **When playing:** Any media  
     Since we only have one item in area B in the Timeline, any media is fine.
   * **With media:** our aquarium image
   * **Duration:** For as many seconds as you like
7. Click on the check mark and "Save". You are finished.

Once, you have mastered setting buttons, there are many other fun things you can do with interactivity.
