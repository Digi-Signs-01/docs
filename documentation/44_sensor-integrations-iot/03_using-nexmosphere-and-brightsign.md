---
title: "Using Nexmosphere And Brightsign"
slug: using-nexmosphere-and-brightsign
publish: false
date: 2025-05-03
update: 2025-05-03
description: Using Nexmosphere And Brightsign
categories:
  - start
---

Using Nexmosphere and BrightSign
================================

In this tutorial we demonstrate how we can apply interactivity using Nexmosphere devices attached to a BrightSign device.

Watch this [demo video](https://youtube.com/shorts/MLh2Z7uzZfc "https://youtube.com/shorts/MLh2Z7uzZfc").

Requirements for this setup
---------------------------

* OnSign TV Player installed on a BrightSign computer ([tutorial](https://onsign.atlassian.net/wiki/spaces/OTT/pages/30277659 "https://onsign.atlassian.net/wiki/spaces/OTT/pages/30277659")).
* [Nexmosphere devices installed](https://nexmosphere.com/support-documentation/ "https://nexmosphere.com/support-documentation/") on a USB port of a BrightSign device.
* 1x Nexmosphere XN-185 controller ([manual](https://static1.squarespace.com/static/6554c6b08c8bde3649fca4ed/t/66bf604c9e5bf60c7f35a714/1723818069229/XN-185+Quick+Start+Guide.pdf "https://nexmosphere.com/document/XN-185%20Quick%20Start%20Guide.pdf")).
* 2x Push buttons with LED ([manual](https://static1.squarespace.com/static/6554c6b08c8bde3649fca4ed/t/66bcd0a43306306cdd14d329/1723650222461/Product+Manual+-+XT+Push+Button+interface.pdf "https://nexmosphere.com/document/Product%20Manual%20-%20XT%20Push%20Button%20interface.pdf")).
* 1x X-Wave LED Strip ([manual](https://static1.squarespace.com/static/6554c6b08c8bde3649fca4ed/t/66be20825db46a4575c0349f/1723736198930/Manual+-+Controlling+X-Wave+LEDs.pdf "https://nexmosphere.com/document/Manual%20-%20Controlling%20X-Wave%20LEDs.pdf")).
* 2x Nexmosphere XR-C10 (RFID antenna).
* 2x XR-DR1 RFID antenna driver.
* 1x RFID Tag.

Below are examplary images of the testbed built for this demo:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669678143/testbed-up.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669688284/testbed-down.jpg)

BrightSign - USB connection
---------------------------

When using an XN controller with USB connection such as the XN-185 or XN-135, an USB-A to Micro-USB cable should be used to connect the micro USB interface of the XN-185/XN-135 to the USB-A interface of the BrightSign Player. The

XN controller is powered via the USB port of the BrightSign Player in this case. Make sure the XN controller is connected to the USB port before powering up the BrightSign Player.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669706303/brightsign-xn185.jpg)

XN-185 Xperience controller
---------------------------

[The XN-185 Xperience controller manual](https://static1.squarespace.com/static/6554c6b08c8bde3649fca4ed/t/66bf604c9e5bf60c7f35a714/1723818069229/XN-185+Quick+Start+Guide.pdf "https://nexmosphere.com/document/XN-185%20Quick%20Start%20Guide.pdf").

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669728187/xn185-ports.jpg)

The XN-185 Xperience controller has 8 X-talk interfaces to which any combination of Elements can be connected. The API commands and operation will remain the same. When connecting multiple Elements which require a high amount of current (LEDs or push buttons with LED ring), calculate the total required current of the Elements and check if this is within the specification of the controller and its power supply source.

This is an interconnection scheme combining some Elements. Not all components of the scheme below were used in the demonstration in this tutorial.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669739755/xn185-combining-elements.jpg)

XN-Range
--------

The XN-180 and XN-185 both have 8 X-Talk interfaces, addressed 1 to 8. Since an address in an API command should always consist of 3 digits, the addresses are numbered 001, 002, and so on. The physical layout of the addresses on the XN-180 and XN-185 controller is indicated in the image on the right. The XN-135 has 3 X-Talk interfaces of which the 3rd is a MicroBay.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669766340/xn-range.jpg)

How to set up OnSign TV for this interactivity demonstration
------------------------------------------------------------

### 1) Activate the Serial Port in the Player Settings

Open the **Player Settings** and find the option Serial Port Settings (RS-232), select the option **USB Port** and set an **alias** to better locate the port in any App.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669795099/serial-port-1.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669805304/serial-port-2.jpg)

### 2) Create Automation Apps

Log into your OnSign TV [account](https://app.onsign.tv/content/ "https://app.onsign.tv/content/") and go to **Content > New > App**.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669831247/automation-app-1.jpg)

Locate the Nexmosphere Apps in the Automation & IoT category and configure the new Apps as shown further on.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669846500/automation-app-2.jpg)

Create two **LED Strip Apps**. The first one for the RED color as shown below, and then repeat the same step creating the second with Brightness = 0 (this one will turn the LED Strip off).

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669878348/led-strip-on-red.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669888699/led-strip-off.jpg)

Create four **XT Push Button** Apps, the first one will **turn on all** button LEDs as shown in the image below. Now create three more Apps: first to **blink all buttons fast**, the second to **blink only button 1 fast** and the third to **blink only button 2 fast**.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669923478/pb-on-all.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669933395/pb-target.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669942737/pb-actions.jpg)

Below are all the **Automation Apps** listed we created for this demo.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669966728/automation-apps-created.jpg)

### 3) Testing the Automation Apps

Now let’s test the Automation Apps created. Go to **Content in Player** in the Player menu and click the **Publish** button in the top-right corner. To test on-demand we need to Publish the Apps to the Player with the option for How to Play It “**Play On-Demand**”.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731669980987/play-on-demand.jpg)

After publishing the Automation App, click the **Play Icon** on the Content in Player page. In the window which opens, click the red **Play** button.

If no feedback is returned, check the settings for the **Nexmosphere Device Channel (**[**X-talk interface**](https://onsign.atlassian.net/wiki/spaces/OTT/pages/edit-v2/33423517?draftShareId=fbe8253a-f062-49ea-9c92-f6549a013139#XN-185-Xperience-controller "https://onsign.atlassian.net/wiki/spaces/OTT/pages/edit-v2/33423517?draftShareId=fbe8253a-f062-49ea-9c92-f6549a013139#XN-185-Xperience-controller")**)** and the Serial Port Alias in the **Automation App Settings** & **Player Settings**.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670037817/check-serial-port-1.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670056903/image.png)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670065719/automation-app-testing.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670084060/on-demand-play.jpg)

### 4) Create Campaigns with Automation Tracks

Now we will create the Campaigns to use in this demo. It will be necessary to activate the **Automation Track** so that we can add interactivity within the Campaigns. We will add the **Automation Apps** created before to this new track. Also, we will use demo images to display content on the screen after the Interactivity action.

Go to **Content > New > Campaign** and follow the settings below. Activate the Automation Track to display this additional track of the timeline. To this new track add the Automation App to **turn on all push button LEDs** and **turn off the LED Strip**. This Campaign will be shown until an interactivity action is triggered.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670111072/automation-track.jpg)

Now create two more Campaigns to be shown when a **Push Button is pressed**. Add the Automation App **Blink Fast Push Button LED 1** to the Automation Track of the first. Then create the second Campaign and add the Automation App **Blink Fast Push Button LED 2**.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670135233/automation-track-PB1.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670145127/automation-track-PB2.jpg)

Now create two Campaigns to be shown when we **pick up** and **put back** the object that has the RFID Tag. Add the Automation Apps **Turn the Led Stripe Red** and **Blink Fast All Push Buttons** to the first one. In the second Campaign add the Automation Apps **Turn Off the LED Stripe** and **Turn On All Push Button LEDs**.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670175256/automation-track-pickup.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670187244/automation-track-putback.jpg)

### 5) Set Interactivity on the Player

Go to the Player Menu and select **Interactivity**. Then click the **Add Interaction** button on the top-right. We will set four interactions. Two for the buttons pressed and two more when we pick up or put back the RFID Tag.

The Local API will receive an API serial command from the XN-185 controller. These commands can be checked in the XN-185 quick start guide ([manual XN-185](https://nexmosphere.com/document/XN-185%20Quick%20Start%20Guide.pdf "https://nexmosphere.com/document/XN-185%20Quick%20Start%20Guide.pdf")).

Fill in the destination field with the Campaigns created for each related action.

In order to guarantee the correct listening of the API serial commands received in the Local API, pay close attention to the use of **backslashes before the square brackets** in the “**Which one**” field.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670217510/escuta-porta-serial.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670228521/interactive-content.jpg)

Now it's time to test the whole configuration made so far and test the interactivity in practice!

Alternative Demo Setup
----------------------

### 1) Create the Automation App “Serial Port Write Data”

Go to **Content > New > App > Automation & IoT,** and select **Serial Port Write Data.**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670281368/automation-app-serialportwritedata.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670302222/serial%20port%20write%20data.jpg)

X-Wave Leds Commands: [link](https://nexmosphere.com/document/Manual%20-%20Controlling%20X-Wave%20LEDs.pdf "https://nexmosphere.com/document/Manual%20-%20Controlling%20X-Wave%20LEDs.pdf")

For this demo, we have created three "Serial Port Write Data" Apps.

1. **WAVE-BLUE** with Data to Write: `X006B[4996240130000009]`
2. **waveLedPB1** with Data to Write: `X006B[4996240120000009]`
3. **waveLedPB2** with Data to Write: `X006B[4996240110000009]`

### 2) Group "Automation Apps" using “Automation Group”

You should use "**Automation Group**" when you need to group more than one Automation App to be executed at once (in parallel) or one after another (sequential) at a specific time frame of your timeline.

Go to **Content > New > App > Automation & IoT,** and select **Automation Group.**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670345703/automation-app-automationgroup.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670355725/edit-ag.jpg)

For this demo we have created five "**Automation Group**" Apps:

1. AutoGroup PB OFF  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670390085/AG-Putback.jpg)
2. AutoGroup PB1  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670402534/AG-PB-1.jpg)
3. AutoGroup PB2  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670433152/AG-PB-2.jpg)
4. AutoGroup Pickup  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670447250/AG-Pickup.jpg)
5. AutoGroup Putback

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670474180/AG-PB-OFF.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670482907/ag-alternative-demo.jpg)

### 3) Setting up Campaigns with Automation Groups

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670504415/campaigns.jpg)

In this alternative demo, we keep using the same Campaigns created for the first demo, but with a different setup as shown below:

* **campaign-pickup**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670531898/campaign-pickup2.jpg)

* **campaign-putback**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670545541/campaign-putback2.jpg)

* **campaign-pressed-button-1**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670573711/campaign-pressed-button1-2.jpg)

* **campaign-pressed-button-2**

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731670588541/campaign-pressed-button2-2.jpg)

The **"Spacer App"** was used to apply a delay to execute the next Automation App in the timeline.

The settings of "**Interactivity in the Player**" was not modified for this alternative demo.

Now it's time to test your alternative demo and compare it with our video demo!
