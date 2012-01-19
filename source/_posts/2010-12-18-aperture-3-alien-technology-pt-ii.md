---
layout: post
title: Aperture 3 - Alien Technology Pt. II
comments: true
categories:
- Aperture 3
- Apple Aperture
- Articles
- SAN
---
{% img http://photo.rwboyer.com/wp-content/uploads/2010/12/kids-in-cray1.jpg %}All I can see is "color me surprised". <a href="http://photo.rwboyer.com/2010/12/15/aperture-3-and-alien-technology/">That little poll I put out after a long and winding diatribe</a> has received way way more response than I expected. What's more is that a whopping 70% of respondents actually want to read a long boring eBook about the nitty gritty of forking around with all the bits and pieces of putting together a home-grown alien technology™ storage area network. I am also surprised at the number of people that think they might want to buy a black-box that just works. I had no idea there were that many people that are outrunning the simple way of doing things.

Okay, I guess I will get crackin' on the eBook. As for the black-box I am building <a href="http://blog.lesterpickerphoto.com/">prototype #000000 for this guy</a>. For those of you that asked here are some of my high level thoughts on what I am going to do for the eBook and the black-box.

First off.... the eBook. In my minds eye this will not just be a recipe. It will be a list of considerations and decisions to be made when designing and acquiring the parts/software/etc. along with some rationale on why you might want to do what in each phase of the process. Of course it will also have a basic end-game type of recipe to actually build a SAN including the nitty gritty specifics that should work just fine if you happen to make the same exact example criteria decisions as I am making as you follow along with the eBook. How does that sound? Good? Maybe you guys/gals just want a recipe - that's simpler but not too too useful as time marches on. Yea right - gals. I would love to see the demographic skew on this eBook.

Now for the eBook and Black-box people, mostly the black-box people but also for eBook people that want to know what kind of minimal example I have rattling around in my head. Here is a simple list of "must haves" in my black-box prototype/s:
<ol>
	<li>Full local fault resiliency and transparent recovery from an HD failure.</li>
	<li>Better performance than a locally connected single spindle drive in it's most humble config.</li>
	<li>iSCSI target to look like a local drive to your Mac.</li>
	<li>Network drive attachment for flexibility.</li>
	<li>Instant snapshot capability of all managed storage. If you are not familiar with this think of it as the ability to put a stake in the ground at any time you want that you can go back to in an instant if anything logical goes wrong. Say an upgrade to an Aperture library and you want to go right back to where you were without copying/restoring/moving data etc.</li>
	<li>Instant snapshot based cloning and export as iSCSI targets with all underlying data shared/copy-on-write. Hey how does TWO Aperture libraries sound that take the same exact amount of storage as one does? Hmmm wouldn't this be great for testing/debug of failed upgrades while continuing to do real work?</li>
	<li>Promotion of clones to separate storage blocks.</li>
	<li>Option to connect at 10 Gig/bits for not too too much money now and way way less down the road. Yep you heard me - that is 10 times faster than your internal drive at a minimum - more like 20 or 30 times faster when you take the throughput of the whole thing in to account vs a single spindle internal SATA drive.</li>
	<li>Low startup cost - like &lt;$1000 for fully redundant 1Gig/s 4 Terabyte fully redundant with all capabilities.</li>
	<li>Low expansion costs - how about &lt;$3000 for 24 Terabytes all in? Yep we are still under the cost of DROBO's biggest best thing they've got with 3 times the storage (actually more than 3 times I am being nice here). Oh and you can do a couple of those expansions at declining costs and increasing bigness without changing a single thing. Almost unlimited expansion.</li>
	<li>Option to replicate data to a remote site/cloud</li>
	<li>Etc. etc. along with the ability to control EXACTLY the way it works for the more techno-geek out there.</li>
</ol>
Okay that is what is in my head. A simplified version of my home SAN with a little bit of simplified UI chucked in. No FC, no FC switch, gigabit connections and switch to start out. 10Gigabit point to point as a low cost option. Multi 10Gigabit Multipath if you want it (not cheap yet).

Please give me some feedback on if this is what you Aperture folk had in mind?

RB