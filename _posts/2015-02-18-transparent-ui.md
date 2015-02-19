---
layout: post
title:  "Too Simple to Be Good"
date:   2015-02-18 15:30:00
categories: creating-gemba
---

From the start, one of Gemba’s design goals was to make it **simple for designers** to push assets to a Git repository. Gemba actively shields users from its internal workings, so that you can deliver assets with a minimal UI. However, I learned from beta testers and usage metrics that Gemba’s **simplicity made it harder for new users** to get started.

### The Post Office and Leaps of Faith

<div style="float:right; width:184px; margin-left:2em; margin-bottom:1em; text-align:center">
	<img src="/img/posts/2015-02-letter-box.jpg" width="184" height="253" alt="Victorian letter box" style="clear:both" />
	<p style="margin-bottom:0.3em">
		Victorian letter box.
	</p>
	<cite style="display:block; line-height:1.1em; font-size:0.7rem;">
		Adapted from <a href="http://www.geograph.org.uk/photo/2323800">Sarah Smith</a>, licensed under <a href="http://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA 2.0</a>
	</cite>
</div>

Using Gemba is as simple as dropping assets into a window and pressing the Deliver button. Dead simple – and perfect, once you have learned to use and trust Gemba.

Indeed, it’s exactly how the Post Office works: you put your stuff into an envelope, then drop it in a mailbox. The Post Office takes care of delivering it to the correct address.

But **Gemba is not the Post Office.**

Gemba has _not_ been around for centuries, gaining **trust** by proving its effectiveness over and over again. Moreover, people have a reassuring **mental model** of how the Post Office gets the envelope to the recipient.

In contrast, Gemba expected new users to take this **huge leap of faith** that it will actually do what you expect with your assets and the repository. What I hadn’t realized: Hiding all complexity under the surface made it hard for users (1) to understand what was going on, and (2) to trust that Gemba will work as expected.

### Exposing the Seams

In a [wonderfully thoughtful essay](http://www.elasticspace.com/2013/03/no-to-no-ui), Timo Arnall explores the virtues of “seamful” interfaces that don’t hide but expose how its parts work together. Quoting Dieter Rams’ famous dictum that **well-designed products are understandable**, he advocates transparent[^1]. user interfaces that explain the way they work through “legible microinteractions”.

So while simplicity is still the goal, I have started to **carefully expose more** of what is happening under the hood through contextual feedback. Gemba now tells you where dropped assets are put; it keeps you informed what it’s currently doing; and the upcoming version will be more transparent with how [.gemba configuration files](http://www.gemba.io/onboard/sample.gemba) are handled. Crucially, listing the dropped assets alongside all existing assets makes the app less of a black box.

### tl;dr

Simplicity and transparency are a trade-off, and I have learned that simple is not automatically better.

I’d love to hear your thoughts at [@GembaApp](http://twitter.com/GembaApp)!

[^1]: Confusingly, there are two opposing meanings to the word “transparency” in our industry. Generally, transparency denotes a “see-through” quality, as in a watch that reveals its inner mechanics behind the revolving hands. In computing, though, transparent is often used to mean “invisible”, e.g. Dropbox transparently syncs files between devices. I use the word in its traditional sense.