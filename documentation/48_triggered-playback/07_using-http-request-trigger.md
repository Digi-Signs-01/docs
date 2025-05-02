---
title: "Using Http Request Trigger"
slug: using-http-request-trigger
publish: false
date: 2025-05-03
update: 2025-05-03
description: Using Http Request Trigger
categories:
  - start
---

Using HTTP Request Trigger
==========================

When you publish an on-demand Content to Android and Windows, but also other  Players, it is possible to trigger the Content by clicking the “Play" icon on the Content in Player page in your OnSign TV account, or through an **HTTP request**.

Do you not know yet what an on-demand Content is? Check out the tutorial on [playing on-demand Content](/triggered-playback/playing-on-demand-content).

In this tutorial, we explain how to obtain the Content on-demand URL and how to trigger it on screen to desired parameters:

1. Open the Player or Player Group in which you have published the on-demand Content.
2. Go to the "Content in Player" menu option.
3. In the "Triggered Content" section, the published Content will be marked as "Play On Demand". Click on the "Share" button, indicated by a chain icon, and click "Copy URL" to get a Playback URL.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731693251067/http-request-trigger-1.jpg)

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731693260626/http-request-trigger-2.jpg)

### Automating the playback

The Playback URL can be used to automate playback of the Content on that specific Player, through a regular GET HTTP request:

```
https://app.onsign.tv/play/VL3GR4qlL7ZcdHLOF4O0
```

4. When doing so, there are some parameters to be used to control the playback behavior:

|  |  |
| --- | --- |
| **Parameter** | **Behavior** |
| **repeat** | A number from 0 to 999 to specify for how long the Campaign should be played. The special value 0 indicates it's repeated indefintely. |
| **action** | Controls the On Demand Queue. Read more below. |
| **Any other** | Any other parameter added to the Playback URL gets forwarded to the Player and is available through Javascript on signage.playbackInfo() |

**Example:**

Requesting the URL below will cause the Player to play a Content item indefinitely (repeat=0) and having the info parameter available for the Content.

```
$ curl 'https://app.onsign.tv/play/VL3GR4qlL7ZcdHLOF4O0?repeat=0&info=1234'
```

### Using the on-demand Queue

By default, playback of the Content starts as soon as the Playback URL is accessed, interrupting whatever is currently playing, be it either scheduled or other on-demand Content.

The OnSign TV Player version 7.0.3 or greater for Android devices adds new ways of playing Content on-demand, through the action parameter.

|  |  |
| --- | --- |
| Action | Result |
| play | Interrupts the currently playing Campaign and starts playing the new content. Any existing queued content is discarded. **This is the default if action is not specified otherwise.** |
| queue | Queues the new content to be played as soon as the currently playing Campaign is over. If there is other content in queue, they will be played first. |
| playqueue | Queues the new content. If the currently playing Campaign is from a scheduled loop (meaning **not played on demand**), this interrupts it and starts playing the queue. |

Those three actions allow for a myriad of interactions.

**Examples:**

Assume a Player has the Campaigns "A", "B", and "C" published on-demand, while having two Campaigns playing through the scheduled loop: "X", "Y".

**Trigger three Campaigns on-demand in a sequence**

If the Player is playing "X" and you call:

```
https://app.onsign.tv/play/token_A?action=playqueue
```

```
https://app.onsign.tv/play/token_B?action=playqueue
```

```
https://app.onsign.tv/play/token_C?action=playqueue
```

The Player would immediately interrupt Campaign "X" and start playing Campaign "A", followed by Campaigns "B" and "C".

**Trigger another Campaign on-demand and discard queue**

Now assume that Campaign "B" is playing and you call:

```
https://app.onsign.tv/play/token_A
```

The Player would immediately start playing Campaign "A", followed by Campaign "X" which was previously interrupted. After that, it resumes the loop, playing "Y", "X", "Y", and so on.

Please mind that Campaign "C" would not play in this scenario, because the queue is dropped when action=play.
