---
title: Installing the Samsung Tizen App
slug: installing-the-samsung-tizen-app
publish: true
date: 2025-05-03
update: 2026-06-21
description: Step-by-step guide to installing the Digisigns player on Samsung SSSP / Tizen commercial signage displays.
categories:
  - start
  - Samsung
  - digital signage
  - tizen
  - SSSP
---

Installing Samsung SSSP Tizen Digisigns App
===========================================

Digisigns is compatible with Samsung Tizen and Samsung Signage Platform (SSSP) screens.
This tutorial covers preparing the display, installing the Digisigns player via the URL
Launcher, and pairing the screen to your account.

Digisigns runs on Samsung's **professional signage** screens only and **cannot be
installed on regular Samsung Smart TVs**.

## Supported Samsung models

| Platform | Video | HDMI-IN | Portrait Support | Tizen | Models |
| --- | --- | --- | --- | --- | --- |
| **SSSP4** | 4K/1080P/720P | Yes | Yes | 2.4 | PHF, PMF, PMH, PHF-P, PMF-BC, OHF, OMH |
| **SSSP5** | 4K/1080P/720P | Yes | Yes | 3.0 | DBJ, QHH, QMH |
| **SSSP6** | 4K/1080P/720P | Yes | Yes | 4.0 | QBN, QBR, QEN, QHR, QMN, QMR, OMN, OHN-D, OHN-S, OMN-D, VMR-U, QBR-N, QBR-T, OMA, OHA-S, OHB, OMB, OMN-DS |
| **SSSP7** | 8K/4K/1080P/720P | Yes | Yes | 5.0 | QPR, QER, OMR |
| **Tizen 6.5** | 8K/4K/1080P/720P | Yes | Yes | 6.5 | QBB, QMB, QHB |
| **Tizen 7.0** | 8K/4K/1080P/720P | Yes | Yes | 7.0 | QMC, QBC, QHC |

## Before you start

1. **Remove any other signage app** already installed on the device.
2. **Check the device date and time.** Incorrect settings cause SSL validation to fail,
   blocking the connection to our servers.
3. **Firewall:** make sure your network complies with our
   [firewall requirements](/27_network-settings/01_firewall-settings).

!!! info "Application hosting URL"
    Type this URL exactly, including `https://`:

    **https://digisigns.in/s**

## Prepare your Samsung display

Complete the display's first-time setup before installing Digisigns. Skipping these
steps is the most common cause of a failed install.

1. Power on the display and run the setup wizard — choose your **language**, then connect
   to the network (Ethernet LAN recommended).
2. Set the **correct date, time, and time zone** — essential for SSL.
3. Choose the standard signage / **LFD** mode when prompted (not the consumer setup).

![Samsung first-time setup — language selection](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-01-language.jpg)

!!! note
    If the display was previously configured for another CMS,
    [reset it](/02_player-installation/43_samsung-sssp-and-tizen/01_how-to-reset-sssp)
    before continuing so no residual configuration interferes.

## Install via URL Launcher

The exact menu wording depends on your platform version.

### On SSSP 6 (Tizen 4)

1. Press the **Home** button on the remote and select **URL Launcher**.

![Home menu — URL Launcher](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-02-home-url-launcher.jpg)

2. Select **Install Web App**.

![URL Launcher Settings — Install Web App](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-03-install-web-app.jpg)

3. Enter **https://digisigns.in/s** and confirm.

![Enter the Digisigns URL](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-04-enter-url.jpg)

4. The Digisigns player installs and starts automatically.

![Installation complete](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-05-install-complete.jpg)

### On SSSP 10 (Tizen 6.5) and Tizen 7.0

1. Press **Home**, open **Settings → System → Play Via**, and select **Custom App**.
2. Go to **Home → App Management → Install Custom App**.

![Custom App on the Home menu](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-06-custom-app.jpg)

3. Enter **https://digisigns.in/s** and confirm.

![Enter the Digisigns URL](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-07-enter-url-customapp.jpg)

4. When installation completes, launch the new app from the Home menu to start the player.

!!! tip "Portrait displays"
    Use the same URL — `https://digisigns.in/s` — for both orientations; there is no
    separate portrait build. For a portrait installation, rotate the panel in the
    display's settings — see
    [Rotating the screen](/02_player-installation/43_samsung-sssp-and-tizen/04_rotating-the-screen-portrait).

!!! note "Don't see URL Launcher?"
    If pressing **Home** loads **MagicINFO** instead of the URL Launcher / Custom App
    option, the panel is set to boot MagicINFO. See
    [Switch to Digisigns from Samsung MagicINFO](/02_player-installation/43_samsung-sssp-and-tizen/05_switch-to-digisigns-from-samsung-magic-info)
    to change Play Via, then return here.

![Play Via — switch from MagicINFO](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-08-play-via.jpg)

## Get the registration code and pair

After the player launches, a **9-digit registration code** appears in the centre of the
screen.

1. Log in to your Digisigns account and go to the **Screens** section.
2. Click **+ Add Screen** and choose the **Tizen Player** option.
3. Enter the **9-digit** code and click **Save**.

The screen registers within a minute and the assigned content begins playing. If the
code does not appear, confirm the display has internet access and the correct date/time,
then relaunch the Digisigns app from the Home menu.

## Recommended settings for signage

For reliable 24/7 operation, apply these after installation:

- **Auto Power Off / No-Signal Power Off:** turn **off** so the display stays on.
- **Daily restart:** schedule a daily reboot to keep the player fresh.
- **Standby / eco timers:** disable any sleep or screensaver timers that interrupt playback.

![Power and energy settings](https://digiboardimages.s3.ap-south-1.amazonaws.com/docs/samsung-tizen/samsung-09-power-settings.jpg)

## Uninstall

To remove the player, press **Home**, open the app list (**App Management** on Tizen 6.5
/ 7.0), select the Digisigns app, choose **Delete**, and power-cycle the display.
Reinstall by repeating the steps above.

## FAQ

**The installation link isn't working — I get "Unable to download".**
The Tizen app cannot be downloaded in a normal browser; the URL must be used from within
the Tizen URL Launcher itself. Try adding a trailing slash (`/`) to the URL — Tizen
inconsistently requires this. If you already have one, try removing it. If it still
fails, check the display's date and time.

**"Unable to connect to the server. Please try again later."**
This almost always means the display's date and time are wrong. Set them correctly (and
enable automatic time) so the device can install/update apps.

---

Need help? Email **support@digisigns.in**.
