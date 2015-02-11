---
layout: post
title:  "Bulk-adding @3x assets to Xcode Asset Catalogs"
date:   2015-02-11 16:34:14
categories: using-gemba Xcode
---

If you’ve been holding out on making your apps ready for the iPhones 6 because of the hassle involved with re-exporting all assets and integrating them into Xcode, here’s some good news for you.

With Gemba, you simply **drop all your newly exported @3x assets** into the app, and they will automatically be added to the image set that contains their @1x/@2x counterparts. **Press “Deliver Changes”. Done.**

That’s all there is to it. Try it out now.

![Xcode asset catalog image set missing the @3x asset](https://gallery.mailchimp.com/5d34b5747a626d1665f586dd0/images/7f47102f-9df2-41c3-ae48-da0fd2112253.png)

# How it works

Gemba matches the asset names to find the correct image set, and it copies the new asset there.

Since Xcode manages a “Contents.json” file for describing an image set’s “slots”, Gemba updates it to link the @3x slot with the new asset.

The new assets, as well as their respective Contents.json files, are listed in Gemba for you to review. When you’re ready, simply press “Deliver Changes”. With the next build, all the new @3x assets will shine in all their glory on an iPhone 6.

# Limitations

Gemba is designed to work perfectly for the most common use cases, and this feature is no exception.

- While it’s no longer strictly required if you’re using asset catalogs, Gemba relies on you using the **traditional naming convention**: “icon[@3x][~ipad].png”
- Launch Image sets and advanced image set features are not supported: asset slicing, size classes, device-specific “568h” assets.

# Saved yourself hours of tedium?

Say you’ve just **integrated hundreds of assets in just two minutes**, instead of wasting an hour doing it manually. And now you’re enjoying a **well-deserved extended coffee break**. If you have a minute to spare, perhaps you could let me in on your joy and tweet at [@GembaApp](http://twitter.com/GembaApp)?
