---
title: "Local Web Api"
slug: local-web-api
publish: false
date: 2025-05-03
update: 2025-05-03
description: Local Web Api
categories:
  - start
---

Local Web API
=============

Local Web API is a simple way to integrate outside devices and trigger Content on the Player through a local network HTTP call.

The Local Web API is supported by OnSign TV on Android, Windows, Linux, Mac, and BrightSign Players.

Important: To use the Local Web API this option must be enabled in the Player settings.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731693674646/local-web-api-1.jpg)

Local Web API for Android Player 9.8.5

|  |  |  |
| --- | --- | --- |
| **Endpoint** | **Method** | **Meaning** |
| [http://127.0.0.1:5544/trigger/{pattern}](http://127.0.0.1:5544/trigger/%7Bpattern%7D "http://127.0.0.1:5544/trigger/{pattern}") | POST | Triggers the play of a campaign or a Playlist which is configured with an interactivity containing the pattern {pattern}. |
| [http://127.0.0.1:5544/campaign/current/stop](http://127.0.0.1:5544/campaign/current/stop "http://127.0.0.1:5544/campaign/current/stop") | POST | Stops the current content playing, skipping to the next one in the loop. |
| [http://127.0.0.1:5544/attribute/{name}/{value}](http://127.0.0.1:5544/attribute/%7Bname%7D/%7Bvalue%7D "http://127.0.0.1:5544/attribute/{name}/{value}") | PUT | Sets the attribute {name} with the value {value}. |
| [http://127.0.0.1:5544/attribute/{name}](http://127.0.0.1:5544/attribute/%7Bname%7D "http://127.0.0.1:5544/attribute/{name}") | GET | Retrieves the attribute named {name} as JSON, in the format {"name": "attr\_name", "value": "attr\_value"}. If no value is set for this attribute or attribute doesn't exist, returns {"name": "attr\_name", "value": null}. |
| [http://127.0.0.1:5544/attributes](http://127.0.0.1:5544/attributes "http://127.0.0.1:5544/attributes") | GET | Retrieves list of all attributes currently set as JSON, in the format {"attributes": [{"name": "attr\_name", "value": "attr\_value"}]}. If no value is set for an attribute, it is not listed. |

Local Web API for Windows/Mac/Linux Player 9.3.9:
-------------------------------------------------

|  |  |  |
| --- | --- | --- |
| **Endpoint** | **Method** | **Meaning** |
| [http://127.0.0.1:5544/trigger/{pattern}](http://127.0.0.1:5544/trigger/%7Bpattern%7D "http://127.0.0.1:5544/trigger/{pattern}") | GET, POST | Triggers the play of a campaign or a Playlist which is configured with an interactivity containing the pattern {pattern}. |
| [http://127.0.0.1:5544/campaign/current/stop](http://127.0.0.1:5544/campaign/current/stop "http://127.0.0.1:5544/campaign/current/stop") | GET, POST | Stops the current content playing, skipping to the next one in the loop. |
| [http://127.0.0.1:5544/playback/status](http://127.0.0.1:5544/playback/status "http://127.0.0.1:5544/playback/status") | GET, POST | Retrieve the playback status as JSON, in the format {"visible": true, "playing": true}. |
| [http://127.0.0.1:5544/playback/show](http://127.0.0.1:5544/playback/show "http://127.0.0.1:5544/playback/show") | GET, POST | Shows the Player window. If window is already visible, nothing happens. |
| [http://127.0.0.1:5544/playback/hide](http://127.0.0.1:5544/playback/hide "http://127.0.0.1:5544/playback/hide") | GET, POST | Hides the Player window. Playback still happens in the background. |
| [http://127.0.0.1:5544/playback/start](http://127.0.0.1:5544/playback/start "http://127.0.0.1:5544/playback/start") | GET, POST | Starts playing content. If content is already playing, nothing happens. |
| [http://127.0.0.1:5544/playback/stop](http://127.0.0.1:5544/playback/stop "http://127.0.0.1:5544/playback/stop") | GET, POST | Stops playing content. Displays a black screen until playback is resumed. |

OnSign TV Academy - Keyboard and Local Network Interacticity
------------------------------------------------------------
