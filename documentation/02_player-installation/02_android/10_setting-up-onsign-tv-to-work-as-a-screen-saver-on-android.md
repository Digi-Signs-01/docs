---
title: "Setting Up Onsign Tv To Work As A Screen Saver On Android"
slug: setting-up-onsign-tv-to-work-as-a-screen-saver-on-android
publish: false
date: 2025-05-03
update: 2025-05-03
description: Setting Up Onsign Tv To Work As A Screen Saver On Android
categories:
  - start
---

Setting up OnSign TV to work as a Screen Saver on Android
=========================================================

While not widely known, a significant number of Android devices allow setting up a screen saver. As a result, it is also possible to set up OnSign TV to work as a screen saver.

Once configured, the screen saver will appear on Android whenever the device becomes inactive (without touches) for a certain period of time.

When OnSign displays content as a screen saver, a single tap will close the Player app, and resume back to the Android interface.

### Important Notes

* The screen saver will only work when the Android device is connected to a charger! In other words, the screen saver does NOT work if the device is working on battery.
* Not all Android devices offer screen saver settings.
* To prevent OnSign TV from being activated at boot, we recommend disabling the "Automatically start the application when the device starts"(more details on this below).
* The screen saver mode is compatible with [SPM](/android/signage-platform-module-spm) (Signage Platform Manager) modules for generic Android devices and [SKM](/android/samsung-kiosk-manager-skm) (Samsung Kiosk Manager). In all cases, it is always recommended to have these modules installed to enable advanced remote device management.
* The OnSign TV screen saver does not implement any user restrictions. We emphasize this, as the user will have full Android access. Unless other restrictions are enforced on the device, the user can install and uninstall apps, or even disconnect the OnSign TV Player from the account.

Step-by-Step Set up:
--------------------

This step-by-step guide was created for Samsung devices, but the process is quite similar for other Android devices.

1. Download the SignageDream application - <https://downloads.onsign.tv/SignageDream-1.1.0.apk>.
2. Install the SignageDream application, and if prompted, grant permission to the browser in use to run the application.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731408922379/samsung-internet-settings.jpg)![](https://docs.onsign.tv/resources/Storage/en/setup-onsign-tv-to-work-as-a-screensaver-on-android/samsung-internet.jpg)![](https://docs.onsign.tv/resources/Storage/en/setup-onsign-tv-to-work-as-a-screensaver-on-android/signage-install.jpg)![](https://docs.onsign.tv/resources/Storage/en/setup-onsign-tv-to-work-as-a-screensaver-on-android/signage-done.jpg)

3. Install the [OnSign TV Player App](https://app.onsign.tv/download/player/latest/android/) and [associate this Player](/basic-player-operations/connecting-a-player) with your OnSign TV account.
4. To prevent the Player from being activated at boot, go to the Player's settings and disable the option: "Automatically start app when device is booting up".

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409023252/autostart.jpg)

5. After associating the Player with your OnSign TV account, add some Content to the Player to test the display testing.
6. On your Android device, access the notifications menu by dragging your finger from the top of the screen to the center. Look for the "Settings" icon, represented by a gear, and tap it to access the device settings.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409054979/configuracoes.jpg)

7. Scroll down to the "Display" section of the menu and click on it. Then, access the "Screen saver" option.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409093873/screen-saver-config.jpg)

8. Choose the Signage Dream app to be displayed as the screen saver. Click on "Preview" to preview the OnSign TV screen saver.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731409110569/screen-saver-config2.jpg)

There you go! Now, you just need to make sure your device is connected to a charger and wait for the screen saver to start.
