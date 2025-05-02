---
title: "Google Sheets As Data Feed External Source"
slug: google-sheets-as-data-feed-external-source
publish: false
date: 2025-05-03
update: 2025-05-03
description: Google Sheets As Data Feed External Source
categories:
  - start
---

Google Sheets as Data Feed external source
==========================================

Sourcing data from Google Sheets works in the same way as every other external data source before. No Data Feed is created for its own sake. They should do something.

First look at the App you want to source with the Data Feed. What type of input does it require? You will find this in the Data Feed Requirement of every Data Feed enabled App.

In the example of the Menu Board - Basic App, it requires input in the form of three text fields – one for the Item Name, one for an Item Subtitle and one for the Currency, the latter two are optional – and of one number field.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731680729581/google-sheets-as-data-feed-external-source_1.png)

Your Google Sheet must have one text and one number field at a minimum. You need to have your Google Sheet ready and enabled as shareable to anyone with the link.

At first, your Google Sheet will come as “Restricted”. You need to change the share setting to “Anyone with the link”.

1. In your Google Sheet click on the green Share button on your top right.
2. The following pop-up has two sections:
   1. Share with people and groups
   2. Get link
   3. Select Get link.
3. You will see the Sheet as restricted. Click on the dropdown arrow to the right of “Restricted” and select “Anyone with the link”.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731680825889/google-sheets-as-data-feed-external-source_2.png)![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731680838413/google-sheets-as-data-feed-external-source_3.png)
4. Copy the link and finish by clicking on “Done”.

If you need help with setting your Google Sheet shareable, go to Google Support for further reference: <https://support.google.com/drive/answer/2494822>

1. Create a new Data Feed by clicking the orange New button at the top left and selecting Data Feed from the dropdown menu
2. Give the Data Feed a name and switch the checkbox from Manual Data Feed to Data Feed From Source.
3. Change the Import Data From selection to “Google Sheets”.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1741722349531/image.png)

4. Paste your previously copied Google Sheets URL in the designated text box.
5. A new window will open where you define the data field formats according to the App you want to use the Google Sheet in. The default for all fields is text. In our example of the Menu Board - Basic App we need one data field to be a number.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731680946436/google-sheets-as-data-feed-external-source_6.png)

6. Click on the dropdown menu of the format box and select “number” or the appropriate format for your Data Feed. In the case of number, you have the option in the top left to customize the Number format.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731680960804/google-sheets-as-data-feed-external-source_7.png)

7. Click on the orange Finish on the bottom right.
8. You return back to your Data Feed where the complete information from your Google Sheet is now added. Click on the orange Create button at the bottom right.
9. Another window opens where you can make changes if needed. Click on “Save” on the top right. Your Data Feed is now ready to be used in a Data Feed Enabled App.

OnSign TV Academy - Data Feed App
---------------------------------
