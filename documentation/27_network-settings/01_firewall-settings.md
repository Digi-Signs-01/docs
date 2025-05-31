---
title: Firewall Settings
slug: firewall-settings
publish: true
date: 2025-05-03
update: 2025-05-03
description: Firewall Settings
categories:
  - start
  - firewall
  - network setting
  - whitelisting
---

Firewall Settings
=================

Running your Digisigns App behind a firewall requires a few domains and ports to be configured for the App to operate.

Please, make sure you build your firewall rules with the domains listed below and NOT an IP-based whitelisting. We would like to reinforce this recommendation as:

* Using domains will keep the service working in case an IP is changed.
* Digisigns requires access to the AWS S3 Storage, which does not have a published list of IPs. 

Please note that all ports are **outbound** connections as Digisigns App always initiate the connection to the servers.

Digisigns Domains and Ports
---------------------------

### HTTPS traffic (port 443)

#### Domains:

* `*.digisigns.in
* `*.amazonaws.com`
* `*.cloudfront.net`

#### Purpose:

Digisigns uses HTTP requests over port 443 to retrieve media playback information, report statistics and events. A permanent WebSocket connection is also established for remote view and realtime data exchange.

### HTTP traffic (port 80)

#### Domains:

* `ocsp.sectigo.com`
* `ocsp.comodoca.com`

#### Purpose:

Required by Samsung, LG and BrightSign players for Online Certificate Status Protocol - OCSP.

### NTP traffic (port 123)

#### Domains:

* `*.ntp.org`

#### Purpose:

Used for automatic network date and time adjustments.

Hardware Specific Whitelisting
------------------------------

Depending on your hardware manufacturer it is required to whitelist additional domains as follows:

### Samsung SSSP and Tizen Screens

* `*.samsungcloudsolution.com`

### LG webOS

* `lgtvonline.lge.com`

### BrightSign

* `*.brightsignnetwork.com`

Feature Specific Whitelisting
-----------------------------

If you are using specific third-party services it is required to whitelist additional domains as follows:

### Hivestack

* `apps.hivestack.com` (ad request and play confirmation calls)
* `*.cloudfront.net` (creative files download)
* `cdn-apps.hivestack.com` (creative files download)

Testing your Firewall
---------------------

The best way to test your firewall is to use the actual Player – or connect a computer to the same Player network – then open this URL in a browser:

<https://api.digisigns.in/test/>
