---
layout: post
title:  "Using Placeholders in lean app development"
date:   2019-02-10 11:20:00
categories: creating-gemba
author:	yang

---
Historically, software was built in strictly separated phases, from conception through analysis to implementation. We have since learned how painfully ineffective and wasteful this [waterfall model](This is obviously a cultural problem) is, and have turned to Agile and Lean practices. Indeed, most teams of developers today organize their work using Scrum or [Kanban](https://en.wikipedia.org/wiki/Kanban_%28development%29).

## Bullshit – waterfall is prevalent

Look at the **product team as a whole**:

1. UX designers conceive a feature,
2. UI designers create pretty mockups and assets,
3. translators localize microcopy,
4. and _only then_ does everything get passed to developers, who proceed to implement it.

Without realizing it, many product teams are still adhering to the strict logic of passing “final” work down the waterfall!

I have seen developers refuse to start implementing a feature before all localized strings and assets are “final-final”. A simple helper app is not going to fix this cultural problem.

## A more parallelized workflow

<a href="https://itunes.apple.com/us/app/placeholders-create-stand/id1042257116?mt=12&at=1000lbLJ&ct=gembablog"><img src="{{ "/img/Placeholders-icon-with-name-100.png" | prepend: site.base_url }}" alt="Placeholders • Stand-in assets for Xcode and Android projects" style="float: right; margin: 0 1em 0.5em 0" /></a>

But what [Placeholders](https://itunes.apple.com/us/app/placeholders-create-stand/id1042257116?mt=12&at=1000lbLJ&ct=gembablog), my new little $1.99 Mac app, *can* do is to make it _easier_ to work more collaboratively and let developers start implementing a screen without all assets being ready.

![Placeholders screenshot, showing an iOS example asset]({{ site.base_url }}/img/screenshots/Placeholders-iOS.png)

Placeholders allows for a more parallelized workflow:

1. Ava wants to start coding a feature, but the assets for it haven’t been created.
2. She uses Placeholders to **create stand-in assets** that she uses to **prepare her layouts**.
3. When Bob, her designer, finds time to craft the actual assets, he **simply replaces the placeholders with the pretty assets**. _(You know, there’s this nifty Mac app called **[Gemba](http://gemba.io)** that makes it super-easy for designers like Bob to update the images all by themselves, without needing to ask and wait on Ava to integrate them.)_
4. In the meantime, Ava finished building the feature’s functionality. Now that Bob has integrated the final images, they can ship the feature. *Hooray!*

## Made for iOS & Android projects

Placeholders was created with iOS and Android product teams in mind, so it creates all the right image variants and puts them in the right places:

- For **Xcode projects**, it adds an Asset Catalog imageset with `@1x`/`@2x`/`@3x` resolutions.
- For **Android projects**, it creates placeholder images for all your densities (ldpi, mdpi, hdpi, xhdpi, xxhdpi, xxxhdpi) and puts them in the respective `res/drawable-{density}` folder.

## Running lean by working collaboratively

By putting walls (i.e. phases with deliverables) between different parts of the product creation, we are wasting a tremendous amount of resources. Instead, let us **work together more tightly** in everything that we do, let us be **open to exploration** and iteration, and let us **ship features and improvements faster** to learn from actual user behavior.

It is my hope that Placeholders may be a humble contribution to this change.

*[Placeholders](https://itunes.apple.com/us/app/placeholders-create-stand/id1042257116?mt=12&at=1000lbLJ&ct=gembablog) is available on the Mac App Store.*