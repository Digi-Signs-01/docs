---
title: " View File Specifications"
slug: view-file-specifications
publish: false
date: 2025-05-03
update: 2025-05-03
description:  View File Specifications
categories:
  - start
---

View File Specifications
========================

Files, in particular videos, come in a lot of different shapes and forms. Even though a file type may be supported by the OnSign TV platform, it may not have the specifications your hardware can deal with.

A very easy example of that is a MOV video file. MOV is a file format created by Apple Inc. This is the file format you will get when recording a video on your iPhone, your iPad, or on a MacBook. However, naturally your Android media player which your OnSign TV application runs on will not easily support this file type. In this case it is better to convert a MOV video to MP4.

Yet, this is just of several specifications to watch out for when you want to run a smooth digital signage operation. The majority of playback errors or black screens during playback come from unsuitable video specifications.

On the OnSign TV platform, you can easily view the specifications of any file you have uploaded to your account.

1. Look for the file in your Content.
2. Uncollapse the right-side panel.   
   *(The right-side panel also gives you a reference to how much more storage space you have on your account.)*
3. Click on the file.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731583984216/8b9bafab-b762-4db5-8e6b-bbeba9a4b5c0.png)

Here, you will see specifications such as: Type, ID, Size, Duration, Dimensions, last Modification, Bit rate, Video codec, and Frame rate. Sometimes, not all specifications are provided by the file.

We want to highlight a few specifications which can be a source for issues:

* **Dimensions:** Videos come in all shapes and sizes, but for your video decoder it is best to use a file which has the same dimensions as the output. Otherwise, the device has to work extra hard to scale the video to the output. For videos which will be shown in fullscreen, you can check your player information for the detected screen resolution.
* **Bit rate:** Below 5 Mbps (Megabits per second) is best.
* **Video codec:** This is where there is the most variety in specs. H.264 has proven to be the most widely accepted codec. Much more than H.263 or H.265 for example. AV1 is only supported from Android 10 onwards. Another aspect to look at is the codec profile which often comes in High, Main, or Baseline. High is too high for many decoders. Choose Baseline or at maximum Main.
* **Frame rate:** Around 25-30 fps (frames per second) is best. 60 fps is not supported by many devices.

If your video file falls out of the recommended ranges, you can reencode it. [Handbrake](/media/optimizing-videos-with-handbrake) is a web tool which we use.

The right-hand side panel has another useful information for you. At the very bottom it shows you how much storage space you still have available for new uploads.
