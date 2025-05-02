---
title: "Create Expanded Interactive Menus"
slug: create-expanded-interactive-menus
publish: false
date: 2025-05-03
update: 2025-05-03
description: Create Expanded Interactive Menus
categories:
  - start
---

Create expanded interactive menus
=================================

Supported on the OnSign TV  Player App for Android 4.2.0 or higher and Windows 9.1.1 or higher.

You can create at most ten different screen zones in a Campaign Layout. Anything else would look too cluttered. Hence, you are not able to create a single menu with more than ten buttons at a time. If you have more options you want to share with your audience, you will need to create a second menu by changing the background zone image. See an example below:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677779641/create-expanded-interactive-menus_1.gif)

Learn how to create two menus in the instructions below.

We have used an Interactive Campaign which we showed you in the [previous interactive tutorial](/interactivity/create-interactive-menus). We recommend you follow that tutorial first. If you have already done so, [download the second set of image files which are used in the expanded interactive Campaign](https://docs.onsign.tv/resources/Storage/en/create-expanded-interactive-menus/Expanded-menu-tutorial-files.zip) and follow the instructions below to create a second menu.

1. For an expanded menu, create a menu image with a next icon at the bottom (see image below). Replace the menu image in your Timeline with this new menu image.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677857507/create-expanded-interactive-menus_2.png)
2. Add a screen division for the next button. In the Timeline, drag again a transparent PNG image to this Timeline like you did for the other three buttons of the Campaign in the previous tutorial.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677871794/create-expanded-interactive-menus_3.jpg)
3. Create a second menu image. It should have different buttons and a back icon at the bottom (see example below). For now, only upload this image to your OnSign TV platform – do not place it into the Timeline.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677885017/create-expanded-interactive-menus_4.png)
4. "Save" the Campaign.
5. On the newly loaded page, click “Interactivity” on the sidebar menu.
6. Click the "Add Interaction" button. From now onwards, we will set all remaining interactions to our buttons.  
   Our first goal is to trigger the second menu when the “next” icon is clicked. Fill out the settings as shown below:  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677915240/create-expanded-interactive-menus_5.png)
   * **Which one:** Region 6 (next button).
   * **Action:** Replace.
   * **Destination:** Region 2, as we want the menu to change.
   * **When playing:** Because the next button belongs to menu 1, set the action to be carried out only when “menu 1” is playing.
   * **With media:** Select “menu 2” and confirm with the checkmark icon.

The next button will now lead to the second menu. Now, we need to add filters to all actions which are already set for the menu 1 buttons. Set "menu 1 (with button)" for the "When playing" field. This will avoid that any content from menu 2 is shown when we click a button from menu 1.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677968915/create-expanded-interactive-menus_6.png)

Then, we need to set up all actions for the second menu. Instead of choosing "menu 1" for "When playing", we have to select "menu 2". Choose the files your option buttons should trigger in the “with media” field.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677981620/create-expanded-interactive-menus_7.png)

At last, configure the "back" button on the bottom for changing the menu back again.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731677999447/create-expanded-interactive-menus_8.png)

**Tip:** When you replace media items on a screen zone, set long display durations to allow the user to navigate freely through the content. If you keep a shorter time duration, it may happen that the user is interrupted while reading the text.

7. Hit “Save” when you are done. Wait for the Player to synchronize the modifications and check out the outcome on screen!
