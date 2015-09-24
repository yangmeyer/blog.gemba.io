---
layout: post
author: yang
title:  "What’s new in Beta 3"
date:   2015-06-23 15:30:00
categories: creating-gemba
---

With this latest Beta version, Gemba makes it easier for you to get started, is more transparent about what it does under the hood, and significantly improves performance.
 
## More than “just” Git
Ever since someone described it that way on [ProductHunt](http://www.producthunt.com/tech/gemba), I’ve positioned Gemba as “drag-n-drop Git for designers”. This was nice and catchy, but it belies the fact that Gemba streamlines your team’s asset pipeline in more than one way:

- Gemba **checks assets for mismatched dimensions** and other common problems before they get delivered/integrated. (Mistakes happen to the best of us :-))
- Gemba allows **batch-updating assets in Xcode asset catalogs**. No need to drag-and-drop them one by one into Xcode.
- And yes, once you’re ready to deliver/integrate your changes, Gemba handles the **Git** stuff, too.

This is reflected in the app’s new Welcome screen. I am also changing Gemba’s tagline to “Streamlined asset pipeline for designer–developer teams.” – Let me know what you think ([Tweet @GembaApp](https://twitter.com/GembaApp)).

## Sample repo on GitHub

When you launch the app as a new user, you can now sign in to your GitHub account and create a sample repository. The sample repository teaches you how to deliver your first asset.

![Onboarding with GitHub account](/img/posts/2015-06-onboarding-github.png)

This means you can now play around with Gemba without using a “real” repository and without setting up a playground repository yourself. Give it a try!

(If the Welcome window doesn’t appear, you can show it from the Window menu.)

## Under the hood

Most users shouldn’t care how an app works internally, as long as it does its job well. But for some, it is vital to understand what is going on. Often, this is a developer who wants to check out whether Gemba fits into her team’s workflow, how it works under the hood, and what exactly it does with the Git repository.

And Gemba really hasn’t helped the developer much to form a (positive) opinion. The app was designed to be super-easy to use for designers, and in this pursuit hid all its inner workings from the user. For designers, Gemba effectively is a black box into which they drop assets and _trust_ Gemba that it does the right thing with them. Unfortunately, this is the opposite of what developers evaluating the app need.

As a first step towards more-transparency-if-you-need-it (without complicating the core use of just dropping in and delivering assets), Gemba now makes it easy to show a repository in other Git clients, so you can watch what Gemba is doing as it does its “magic”:

![Show repository in other Git clients](/img/posts/2015-06-show-in-menu.png)

Also, Gemba now re-confirms with you before pushing anything to the remote repository, so you can feel safe about trying out Gemba:

![Dialog to reconfirm push](/img/posts/2015-06-push-reconfirm-dialog.png)

## 1.000 assets? No problem.

Some projects contain hundreds or even thousands of assets. I’m happy to report significant improvements in overall performance. Scrolling lists of 1.000+ assets and switching between repositories are now much, much smoother. _(Update July 1, 2015: One beta tester reported that Gemba worked well with his repository of 5.910 (!) assets.)_

Enough talking, now give a spin:

[Download Gemba (Beta 3)](http://gemba.io/download.html)

Thanks for reading. Hope you enjoy the new Beta. If you have any question, comment, concern – just [tweet @GembaApp](https://twitter.com/GembaApp).
