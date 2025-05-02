---
title: "Firewall Settings"
slug: firewall-settings
publish: false
date: 2025-05-03
update: 2025-05-03
description: Firewall Settings
categories:
  - start
---

Firewall Settings
=================

Running your OnSign TV Players behind a firewall requires a few domains and ports to be configured for the Players to operate.

Please, make sure you build your firewall rules with the domains listed below and NOT an IP-based whitelisting. We would like to reinforce this recommendation as:

* Using domains will keep the service working in case an IP is changed.
* OnSign TV requires access to the Google Cloud Storage, which does not have a published list of IPs. Read more about [proxying Google Cloud Storage](https://cloud.google.com/storage/docs/troubleshooting#proxy-server).

Please note that all ports are **outbound** connections as OnSign TV player always initiate the connection to the servers.

OnSign TV Domains and Ports
---------------------------

### HTTPS traffic (port 443)

#### Domains:

* `*.onsign.tv`
* `*.signagewidgets.net`, `signagewidgets.net`
* `storage.googleapis.com`
* `CNAME.signagewidgets.net`

To add your server-specific URL (port 443), use the URL which is configured as your URL's CNAME. You can use [this tool](https://mxtoolbox.com/SuperTool.aspx?action=cname%3aapp.123-signage.com&run=toolpage) to find your CNAME setting if you don’t remember it.  
As an example, `app.123-signage.com` would add the rule: `app-r4zfwn.signagewidgets.net` (443)

#### Purpose:

OnSign TV uses HTTP requests over port 443 to retrieve media playback information, report statistics and events. A permanent WebSocket connection is also established for remote view and realtime data exchange.

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

<https://api.onsign.tv/test/>
