---
title: "Using The Cafeteria App"
slug: using-the-cafeteria-app
publish: false
date: 2025-05-03
update: 2025-05-03
description: Using The Cafeteria App
categories:
  - start
---

Using the Cafeteria App
=======================

The Cafeteria App is part of the Menu Boards & Tables App category. As the name suggests it is useful for daily changing cafeteria menus. This is just one possible application. Use this App every time you want to list something which changes by the day and time of day.

Examples: A health clinic with specialized doctors, a university with the consultation hours of the professors, a conference with various workshops, a gym with diverse classes, and many more.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731681826790/how-to-use-the-cafeteria-app_1.png)

The maximum tables on one page will be three. If you have more tables on a day, they will be shown on the next page. If you have only 1 or 2 tables on a given day, only 1 or 2 columns will be shown for that day.

Example with 2 tables on Monday:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731681840759/how-to-use-the-cafeteria-app_2.png)

This App gets its contents from a [Data Feed](/data-feeds/creating-a-new-data-feed). The App tells us the required information:

* a number column for the **Day Of The Week**.
* a text column for the parent category which is the table header, here named **Meal Name**. Think of it like Breakfast, Lunch, Dinner.
* a text column for the individual entries, here named **Menu**. Think Müsli and Pancakes.
* and an optional text column for the time of day **Schedule**. It will show as a second line in the table header.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731681892045/how-to-use-the-cafeteria-app_3.png)

Create a Data Feed with the content of the App
----------------------------------------------

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731681918209/how-to-use-the-cafeteria-app_4.png)

This can be a manual Data Feed on the OnSign TV platform or an outside source like CVS, Google Sheets, and so on. We create a Manual Data Feed.

1. Column: Day Of The Week

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731681990204/how-to-use-the-cafeteria-app_5.png)

The day of the week is a number field. 1.00 represents Sunday, 2.00 Monday, 3.00 Tuesday and so on.

2. Column: Meal Name

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731682005820/how-to-use-the-cafeteria-app_6.png)

The meal name is the table header and is a text field.

3. Column: Schedule  
   The schedule is a line under the table header to give additional information on the column. It is also a text field and the only optional field.

1. Column: Menu  
   The Menu contains all table data under the table header. Separate each entry by a comma.
2. Populating the Data Feed  
   To reflect four times per day, you need four rows with the number 2.00 as the Day of the Week for Monday.

To fill out your app completely, you need as many rows as you have

days of the week  X  times per day

In this case 4 X 7 = 28 rows.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731682036716/how-to-use-the-cafeteria-app_7.png)

The App will work just the same with less rows. If you don’t have any service on Saturday (Day of the Week = 7.00) or Sunday (Day of the Week = 1.00), these days will be skipped.

Create the Cafeteria App and connect it to the Data Feed
--------------------------------------------------------

1. Select New > App > Menu Boards & Tables > Cafeteria App.
2. Name the App and connect the Cafeteria Data Feed.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731682096903/how-to-use-the-cafeteria-app_8.png)

3. Confirm if the columns are assigned correctly.
4. Personalize the duration on each page, font, colors, background, labels, language, as well as if only the present day should be shown or the App should rotate through all available days.
5. Your Cafeteria App is now ready to be published

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731682110430/how-to-use-the-cafeteria-app_9.png)

Check out how to set up the Cafeteria App in action
---------------------------------------------------
