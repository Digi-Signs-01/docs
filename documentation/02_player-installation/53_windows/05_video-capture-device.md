---
title: "Video Capture Device"
slug: video-capture-device
publish: false
date: 2025-05-03
update: 2025-05-03
description: Video Capture Device
categories:
  - start
---

Video Capture Device
====================

This tutorial explains how to connect video capture devices to the OnSign TV  Windows  Player.

**Requirements:**

* OnSign TV  Windows  Player version 10 or higher.
* Using a VLC compatible video device.
* While installing VLC is not mandatory, it is nice to have for testing the capture device under VLC.
* Having successfully installed your video device card using the device manufacturer software and drivers.

VLC is one of the most popular media Players, offering both a graphical interface and a full command line for playback.

Although installing VLC on the Player is not necessary, we recommend it to test the correct operation of the capture device and to facilitate getting the configuration parameters.

**Compatible Capture Devices**

Any device compatible with VLC 3.0 can be used such as:

* Capture to capture HDMI
* WebCam or Camera
* TV Tuner Card

Step-by-step configuration:
---------------------------

1. Ensure that all necessary drivers for your capture card are correctly installed.
2. To check if the drivers are correct, the capture device must be working correctly when using the software provided by the device manufacturer.
3. Download and install [VLC](https://www.videolan.org/).
4. With the capture device installed and connected, open VLC and select:
   * Media > Open Capture Device
5. As **Capture mode** select "DirectShow" for video capture cards and WebCams; or **TV - Digital** for TV tuner card.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731419757453/windows-video-capture-device_1.jpg)

6. Select the **Video device name** from the menu:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731419792583/windows-video-capture-device_2.jpg)

7. Click **Show more options** to see the parameters used for the selected device.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731419811163/windows-video-capture-device_3.jpg)

8. Copy the content shown in **MRL** to the **Playback Media Resource Locator** field in the OnSign TV VLC App.
9. Copy the parameters shown in **Edit Options** to the **Playback Arguments** of the VLC App.

### IMPORTANT

Remove the colon symbol ":" before each parameter.

Use quotes to define parameters that contain spaces as characters:

Example:   
Parameters in VLC :dshow-vdev=HD Webcam C525 live-caching=300   
Change parameters to dshow-vdev= "HD Webcam C525" live-caching=300

Take a look [here](https://wiki.videolan.org/Documentation:Streaming_HowTo/Command_Line_Examples/) to know more about VLC parameter options.

Other command examples:
-----------------------

### Built-in webcam

This will usually be the default DirectShow device.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731419971307/windows-video-capture-device_4.jpg)![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731419983589/windows-video-capture-device_5.png)

### HDMI-in

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731420008399/windows-video-capture-device_6.jpg)![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731420017573/windows-video-capture-device_7.png)

### TV Tuner

Use the tuner card manufacturer's software to find the frequency of each channel.

The channel width depends on the location and the specific Digital TV Standard used. In this example, we set the channel width to 6 MHz (or 6000 Hz).

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731420046565/windows-video-capture-device_8.jpg)![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731420056926/windows-video-capture-device_9.png)
