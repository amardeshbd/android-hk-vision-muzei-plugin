[![Android CI](https://github.com/amardeshbd/android-hk-vision-muzei-plugin/workflows/Android%20CI/badge.svg?branch=master)](https://github.com/amardeshbd/android-hk-vision-muzei-plugin/actions) [![CodeFactor](https://www.codefactor.io/repository/github/amardeshbd/android-hk-vision-muzei-plugin/badge)](https://www.codefactor.io/repository/github/amardeshbd/android-hk-vision-muzei-plugin) [![Muzei.co](https://img.shields.io/badge/muzei.co-API%203.4%2B-blue)](http://api.muzei.co/)

# HK Vision - Muzei Plugin
Muzei wallpaper source plugin for [vision.hossainkhan.com](https://vision.hossainkhan.com/) site.

## Background
I wrote a quick article behind creating this plugin. [Read more about it at Medium.com](https://medium.com/@hossainkhan/hackathon-creating-the-simplest-muzei-wallpaper-plugin-for-android-9d080dbb4bf)

## How to use
Install [Muzei app](https://play.google.com/store/apps/details?id=net.nurik.roman.muzei) from Google Play.
[![Muzei-on-Google-Play](https://user-images.githubusercontent.com/99822/81494196-decc1600-9274-11ea-9296-f167952e5fc1.png)](https://play.google.com/store/apps/details?id=net.nurik.roman.muzei)

Next, install [Vision Muzei Plugin app](https://play.google.com/store/apps/details?id=com.hossainkhan.vision) from Google Play.

Once installed, go back to **Muzei** app, then the source should show up. Choose the wallpaper you like for your phone. Enjoy.

> _NOTE: By default, the walpaper changes **every 3 hours**, you may want to change it to you liking. For example every day :-)_

[![android-muzei-plugin-demo-large-small](https://user-images.githubusercontent.com/99822/81618324-19d56300-93b5-11ea-8367-62376439a99c.png)](https://play.google.com/store/apps/details?id=com.hossainkhan.vision)

## Dev Note
To build and install locally, use following command:

```
adb uninstall com.hossainkhan.vision && \
./gradlew clean assembleDebug && \
adb install app/build/outputs/apk/debug/app-debug.apk 
```

### New Release
```
./gradlew bundleRelease
```
> Make sure you have `keystore.properties` available in the project.

# References
* https://muzei.co/
* https://api.muzei.co/
* https://github.com/romannurik/muzei/releases/tag/api3.4.0-alpha3
* https://medium.com/muzei/muzei-3-0-and-the-new-api-4fd3d6133db6
* https://medium.com/muzei/announcing-muzei-live-wallpaper-3-0-d167dd5795a4
