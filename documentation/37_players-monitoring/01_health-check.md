---
title: 'Health Check'
slug: health-check
publish: false
date: 2025-05-03
update: 2025-05-03
description: Health Check
categories:
  - start
---

# Health Check

Health Check is a powerful and convenient tool for finding and fixing issues across your network.

### The Health Check will inform you about:

- **Advice to install the Digisigns SPM** - Players where the Digisigns SPM should be installed for enabling advanced features: like [remote view](07_remote-view.md), [remote control](05_remote-control-android-players.md), [scheduled reboot](06_remote-reboot.md), and [remote upgrade](../35_player-update/04_remote-player-update.md).
- **Expired Content** - Content which is published with an [expired restriction](../09_basics-publishing/08_publish-content-with-restrictions.md). This Content won't be shown any more, but is still using valuable storage space on the Player. The Health Check will only highlight Content which is expired for more than 48h.
- **Invalid Apps**
  - Due to an invalid parameter.
  - Due to either invalid or empty feeds.
  - Due to missing [integration Accounts](../01_account-settings/01_connecting-social-media-accounts.md).

Different from a static reports, the Health Check will run a new scan every time it gets loaded.

## Accessing the Health Check

1. Click on **Health Check**.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1741805679946/image.png)

## Filtering Results

Use the search bar to enter the name of a specific item you would like to check or use the filtering icon to only list a specific asset type.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731689122253/health-check-2.jpg)

## Health Check Icons

Each Health Check item is marked with an icon indicating how severe the issue is:

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731689139970/health-check_3.png)

## Example Health Check Issues

### SPM - Installation Advised

The Health Check scan found that the “Lobby Player” can take advantage of advanced features by installing the [Digisigns SPM](https://onsign.tv/spm/).

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731689186310/health-check_4.png)

Suggested actions:

- Click on the "Download SPM" button.
- Save the downloaded content on a USB Drive.
- Install the SPM on your Android Player.

**IMPORTANT** - The SPM APK is custom built for each Android Distribution. The "Download SPM" button will provide the right SPM version for the specific Player listed. Android will block the SPM installation if the SPM version is not the correct one for the target Player.

### Content Published with an Expired Restriction

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731689238996/health-check_5.png)

The Campaign “Flight Info” is published to the Player “Hall”, but will not be shown any more due to an expired restriction.

Suggested actions:

- **Option 1** - [Unpublish the Campaign](../09_basics-publishing/11_unpublishing-content.md) by clicking the "Unpublish Campaign" button.
- **Option 2** - [Edit the Campaign restrictions](../09_basics-publishing/01_adding-restrictions-to-content.md) by clicking on the arrow on the right side of the "Unpublish Campaign" button.

### RSS App Containing an Empty Feed

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731689295423/health-check_6.png)

The App called “News APP - RSS” is not going to work because the RSS feed is empty.

Suggested actions:

- **Option 1** – Click on the App thumbnail and edit the App by [changing the App feed](../39_popular-apps-setup/10_using-rss-feeds.md).
- **Option 2** – Before deleting the App, [check its usage](../25_media/12_tracking-content-usage.md) or edit it by clicking on the arrow on the right side of the "Delete App" button.

### Digisigns Academy - Dashboard and Health Check
