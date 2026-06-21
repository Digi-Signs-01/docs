---
title: Binding to the Digisigns Server
slug: binding-to-the-digisigns-server
publish: true
date: 2026-06-22
update: 2026-06-22
description: Bind a NovaStar Taurus player to the Digisigns VNNOX server using ViPlex Express.
categories:
  - start
---

# Binding to the Digisigns server

The Taurus connects to Digisigns through the VNNOX platform. Point the player at the
Digisigns server in **ViPlex Express** (Windows).

## Before you start

- The Taurus must have a working internet connection — see
  [Configuring networks](01_configuring-networks.md).
- Install **ViPlex Express** on a Windows PC on the same network as the player.
- Have the player's **admin** password ready (printed on the SSID label).

## Bind the player

1. Connect your PC to the Taurus (over the same network, or via the player's Wi-Fi AP),
   then open **ViPlex Express**.
2. Click **Refresh** to update the screen list. A **green** icon means the player is
   online and available to log in; a **red** icon means it is offline.
3. Click **Connect** next to the player, enter the **admin** password, and click **OK**.
4. Go to **Control → Server configuration** and select the player from the terminal list.
5. In the **Bind to VNNOX Standard/AD** section, enter the Digisigns server details
   exactly as below:

| Field | Value |
| --- | --- |
| Server Address | `https://api-in.vnnox.com` |
| Authentication User Name | `digisigns` |
| Authentication Password | *Provided by Digisigns Support* |

> [!note]
> For security, the authentication password is not published here. Email
> [support@digisigns.in](mailto:support@digisigns.in) to obtain the password for your
> account.

6. Click **Bind**.

The player registers with the Digisigns server within a minute. Next, add it to your
account — see [Pairing in the Digisigns dashboard](03_pairing-in-the-digisigns-dashboard.md).

> [!warning]
> Enter the server address and credentials exactly as shown, including `https://`. An
> incorrect value will stop the player from binding.
