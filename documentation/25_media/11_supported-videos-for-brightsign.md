---
title: "Supported Videos For Brightsign"
slug: supported-videos-for-brightsign
publish: false
date: 2025-05-03
update: 2025-05-03
description: Supported Videos For Brightsign
categories:
  - start
---

Supported videos for BrightSign
===============================

The info below was copied from the [BrightSign webpage](https://docs.brightsign.biz/space/DOC/2396356609/Supported+Video+Formats+and+Codecs).

In the following we describe the requirements for video to play successfully on **BrightSign Players**. Bitrate information for older Players is available on [this page](https://brightsign.atlassian.net/wiki/spaces/DOC/pages/370673630/Optimizing+Video+Quality#Bitrates).

For format and encoding modification we recommend to take a look in [this tutorial](/media/optimizing-videos-with-handbrake).

XD5, HD5, LS5
-------------

* 4K Video Codecs: H.265/HEVC, H.264/AVC (max 30p), VP9
* 1080p Video Codecs: H.265/HEVC, H.264/AVC, VP9, MPEG 4 part 2, MPEG1 video, MPEG2 video
* Containers: .MP4, .MOV, .MKV, .WEBM, .TS, .MPG, .MPEG, .PS, .M2P, .MPV, .AVI, .HEVC, .H264, .AV1, .VP9, and .MJPG
* Resolution: Video sources larger than 1920x1080 resolution must be in HEVC (H.265), AVC (H.264), or VP9 format. AVC/H.264 is limited to 30p at 3840x2160.
* HDR: HDR10 (Single Video Zone only, No Graphics)
* Color Space: RGB color space, YUV420
* Bit Depth: 8 and 10 bit
* Profile: Main and Main10
* Level: 5.1 and below

XCxx55 (4K resolution and below)
--------------------------------

* 4K Video Codecs: H.265/HEVC, H.264/AVC, AV1, VP9, MPEG 4 part 2, MPEG1 video, MPEG2 video, or MJPEG video
* Containers: .MP4, .MOV, .MKV, .WEBM, .TS, .MPG, .MPEG, .PS, .M2P, .MPV, .AVI, .HEVC, .H264, .AV1, .VP9, and .MJPG
* Resolution: Video sources larger than 3840x2160 resolution must be in HEVC (H.265) or VP9 format. All video sources other than HEVC and VP9 are limited to 3840x2160.
* HDR: XCxx55 Players support HDR10 and HLG
* Color Space: RGB color space, YUV420
* Bit Depth: 8 and 10 bit
* Profile: Main and Main10
* Level: 6.1 and below
* Bitrate: The bitrate selected by your software should be supported by the codec, given the constraint that the level can’t be over 6.1. Wikipedia has more information about bitrates at different profiles and levels (for example, H264 ([Advanced Video Coding](https://en.wikipedia.org/wiki/Advanced_Video_Coding)), H265 ([High Efficiency Video Coding](https://en.wikipedia.org/wiki/High_Efficiency_Video_Coding)), and [VP9](https://en.wikipedia.org/wiki/VP9)).

XCxx55 (8K resolution)
----------------------

* 8K Video Codecs: H.265/HEVC, VP9
* Containers: .MP4, .MOV, .MKV, .WEBM, .TS, .MPG, .MPEG, .PS, .M2P, .MPV, .AVI, .HEVC, .H264, .AV1, .VP9, and .MJPG
* Resolution: The maximum supported resolution is 7680x4320x60p. Video sources larger than 3840x2160 resolution must be in HEVC (H.265) or VP9 format. Neither AV1 nor AVC (H.264) will work at 8K video resolution.
* HDR: XCxx55 Players support HDR10 and HLG
* Color Space: RGB color space, YUV420
* Bit Depth: 8 and 10 bit (Note that there is a difference between the XC4055 and the XC2055: The XC4055 can do 8Kp60 at 10 bit and the XC2055 can do 8Kp60 at 8 bit or 8Kp30 at 10 bit)
* Profile: Main and Main10
* Level: 6.1 and below
* Bitrate: The bitrate selected by your software should be supported by the codec, given the constraint that the level can’t be over 6.1. Wikipedia has more information about bitrates at different profiles and levels (for example, H265 ([High Efficiency Video Coding](https://en.wikipedia.org/wiki/High_Efficiency_Video_Coding)) and [VP9](https://en.wikipedia.org/wiki/VP9)).

XTx44, XDx34, HDx24
-------------------

### 4K Video

* Video Codec: H.264, H.265, or VP9
* Resolution: The maximum supported resolution is 4096x2160x60p.
* Color Depth: 4K video can be encoded at 4:2:0 subsampling with 8 bits (Main Profile) or 10 bits (Main 10 Profile) of depth.
* HDR and Dolby Vision: XTx44 Players support both HDR10 and Dolby Vision.
* Display Hardware: The maximum supported framerate and color depth are also affected by your display hardware. See this section of the [4K Video Encoding](http://docs.brightsign.biz/display/DOC/4K+Video+Quality+Overview#id-4KVideoQualityOverview-BestPracticesforEncoding) tech note for more details.

Note: BrightSign Players support both H.265 version 1 profiles: Main and Main 10. However, we do not support the recently ratified version 2 profiles.

* Container Format: The following container formats are supported: .ts, .mov, .mp4, .mkv, .webm.

Note: XTx44/XDx34 models currently support .webm video with the Opus audio codec (not Vorbis), while HDx24 models support .webm with the Vorbis audio codec (not Opus).

* Bitrate: The XTx44 and XDx34 models support a constant bit rate (CBR) between 70 and 80 Mbps. These values apply to both the primary and secondary video decoders.
* Merge Mode: If you use B-frames as references in H.265 “merge mode”, the size of the references list should be limited to two or less.
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall, as well as videos of large file size and/or duration.

Note: 4K video must be played from a Class 10 SD card.

### HD Video

* Supported Codecs: H.265, H.264, VP9, MPEG-2
* Resolution: The maximum supported resolution is 1920x1080. Note that some supported VESA video modes have limitations, as outlined in [this FAQ](https://docs.brightsign.biz/space/DOC/2138505217/Player+Troubleshooting+FAQ#Why-is-my-1280x800x60p-video-dropping-frames%3F).
* Supported Extensions/Containers: .ts, .mpg, .vob, .mov, .mp4, .m2ts

Note: .mov files with compressed "atoms" (i.e. metadata) are currently not supported.

* Additionally Supported Extensions: Players also support .webm video with Vorbis audio (the Opus audio codec is not supported).
* Specs for H.265 Extensions/Containers: Support for Main and Main 10 profiles up to level 5.1
* Specs for H.264 Extensions/Containers: Support for Main and High profiles up to level 4.2
* Maximum Recommended Video Bit Rate: 25Mbps
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall, as well as videos of large file size and/or duration.

XTx43, XDx33, 4Kx42
-------------------

### 4K Video

* Video Codec: 4K video must be encoded as an H.265 (HEVC) file.
* Resolution: The maximum supported resolution is 3840x2160x60p.
* Color Depth: 4K video can be encoded at 4:2:0 subsampling with 8 bits (Main Profile) or 10 bits (Main 10 Profile) of depth.
* HDR and Dolby Vision: XTx43 Players support HDR10
* Display Hardware: The maximum supported framerate and color depth are also affected by your display hardware. See this section of the [4K Video Encoding](http://docs.brightsign.biz/display/DOC/4K+Video+Quality+Overview#id-4KVideoQualityOverview-BestPracticesforEncoding) tech note for more details.

Note: BrightSign Players support both H.265 version 1 profiles: Main and Main 10. However, we do not support the recently ratified version 2 profiles.

* Container Format: The following container formats are supported: .ts, .mov, .mp4, .mkv, .webm.

Note: These Players support .webm video with Vorbis audio only. The Opus audio codec is not supported.

* Bitrate: We recommend a CBR between 30 and 40 Mbps. These values apply to both the primary and secondary video decoders.
* Merge Mode: If you use B-frames as references in H.265 “merge mode”, the size of the references list should be limited to two or less.
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall, as well as videos of large file size and/or duration.

Note: 4K video must be played from a Class 10 SD card.

### HD and SD video

* Supported Codecs: H.265, H.264, VP8, MPEG-2, MPEG-1
* Resolution: The maximum supported resolution is 1920x1080. Note that some supported VESA video modes have limitations, as outlined in [this FAQ](https://docs.brightsign.biz/space/DOC/2138505217/Player+Troubleshooting+FAQ#Why-is-my-1280x800x60p-video-dropping-frames%3F).
* Supported Extensions/Containers: .ts, .mpg, .vob, .mov, .mp4, .m2ts

Note: .mov files with compressed "atoms" (i.e. metadata) are currently not supported.

* Additionally Supported Extensions: BrightSign Players support .wmv files that are exported from PowerPoint (i.e. video-only .wmv without .wma audio). Players also support .webm video with Vorbis audio (the Opus audio codec is not supported).
* Specs for H.265 Extensions/Containers: Support for Main and Main 10 profiles up to level 5.1
* Specs for H.264 Extensions/Containers: Support for Main and High profiles up to level 4.2
* Specs for MPEG-1 Extensions/Containers: System streams only (elementary streams are not supported)
* Maximum Recommended Video Bit Rate: 25Mbps
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall, as well as videos of large file size and/or duration.

### LS424

* Supported Codecs: H.265, H.264, MPEG-2
* Resolution: The maximum supported resolution is 1920x1080. Note that some supported VESA video modes have limitations, as outlined in [this FAQ](https://docs.brightsign.biz/space/DOC/2138505217/Player+Troubleshooting+FAQ#Why-is-my-1280x800x60p-video-dropping-frames%3F).
* Supported Extensions/Containers: .ts, .mpg, .vob, .mov, .mp4, .m2ts

Note: .mov files with compressed "atoms" (i.e. metadata) are currently not supported.

* Additionally Supported Extensions: Players also support .webm video with Vorbis audio (the Opus audio codec is not supported).
* Specs for H.265 Extensions/Containers: Support for Main and Main 10 profiles up to level 5.1
* Specs for H.264 Extensions/Containers: Support for Main and High profiles up to level 4.2
* Maximum Recommended Video Bit Rate: 25Mbps
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall, as well as videos of large file size and/or duration.

HDx23, LS423
------------

* Supported Codecs: H.265, H.264, VP8, MPEG-2, MPEG-1
* Resolution: The maximum supported resolution is 1920x1080. Note that some supported VESA video modes have limitations, as outlined in [this FAQ](https://docs.brightsign.biz/space/DOC/2138505217/Player+Troubleshooting+FAQ#Why-is-my-1280x800x60p-video-dropping-frames%3F).
* Supported Extensions/Containers: .ts, .mpg, .vob, .mov, .mp4, .m2ts

Note: .mov files with compressed "atoms" (i.e. metadata) are currently not supported.

* Additionally Supported Extensions: BrightSign Players support .wmv files that are exported from PowerPoint (i.e. video-only .wmv without .wma audio). Players also support .webm video with Vorbis audio (the Opus audio codec is not supported).
* Specs for H.265 Extensions/Containers: Support for Main and Main 10 profiles up to level 5.1
* Specs for H.264 Extensions/Containers: Support for Main and High profiles up to level 4.2
* Specs for MPEG-1 Extensions/Containers: System streams only (elementary streams are not supported)
* Maximum Recommended Video Bit Rate: 25Mbps
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall, as well as videos of large file size and/or duration.

XDx32, XDx30, HDx22, HDx20, LSx22, HDx10
----------------------------------------

* Supported Codecs: H.264, MPEG-2, MPEG-1
* Resolution: The maximum supported resolution is 1920x1080. Note that some supported VESA video modes have limitations, as outlined in [this FAQ](https://docs.brightsign.biz/space/DOC/2138505217/Player+Troubleshooting+FAQ#Why-is-my-1280x800x60p-video-dropping-frames%3F).
* Supported Extensions/Containers: .ts, .mpg, .vob, .mov, .mp4, .m2ts

Note: .mov files with compressed "atoms" (i.e. metadata) are currently not supported.

* Additionally Supported Extensions: .wmv files that are exported from PowerPoint (i.e. video-only .wmv without .wma audio).
* Specs for H.264 Extensions/Containers: Support for Main and High Profiles up to level 4.2
* Specs for MPEG-1 Extensions/Containers: System streams only (elementary streams are not supported)
* Maximum Recommended Video Bit Rate: 25Mbps
* Audio Support: AAC audio (CBR/VBR) up to 288Kbps
* Fast Start: Enabling fast start (-movflags +faststart) is recommended, especially for videos used in synchronized playback and BrightWall (not applicable to HDx10 models), as well as videos of large file size and/or duration.

HD600
-----

* MPEG-1 or MPEG-2 Standard video files
* Supported extensions .MPG and .VOB
* Must be a Program Stream (System Stream for MPEG-1)
* Must contain an audio layer at a 48Khz sample rate, even if it's just silence.
* Maximum bit rate supported is 9Mbps
* Maximum video resolution supported is 720x480

HD2000
------

* MPEG-1 or MPEG-2 HD or Standard video files
* Supported extensions .MPG and .VOB
* Must be a Program Stream (System Stream for MPEG-1)
* Maximum bit rate supported is 25Mbps
* Maximum video resolution supported is 1920x1080i (interlaced)
