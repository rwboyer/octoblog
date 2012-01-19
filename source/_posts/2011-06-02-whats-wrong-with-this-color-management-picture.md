---
layout: post
title: What's Wrong With This Color Management Picture? 
comments: true
categories:
- Apple
- Articles
- color management
- General Photography
- iMac
---
Okay so I could just use words to express what is going on here but I will let this speak for itself.

{% img http://photo.rwboyer.com/wp-content/uploads/2011/06/P1010837-WTF.jpg %}

Now time for some words...

No matter what you are using to view the photo above you can see that something is amiss. You see no matter if your color managed or not, no matter if your monitor is "calibrated" or not. No matter how "off" my camera's white balance or color is you should see the relative difference between the monitor on the left and the monitor on the right. The only two exceptions are if you are actually blind or your viewing hardware has some sort of strange rendering issue from left to right that actually corrects the issue here.

Now you might be saying "That's why you calibrate monitors". Hmmmm. This is AFTER "calibration" . If you have been at this a while you may also say "Well your calibration software merely builds a profile of what the monitor does so that the color management engine can do the best it can do with the two different devices". Ah ha.... you are correct but MY software and calibration device have a matching mode that is SUPPOSED to at least get the neutral in gamut colors to match. You might also say "Well that's what you get when you have two different devices that are displaying an image with out of gamut colors from an image with a larger space"  yep you're right.

All of these things might be the reason but I can assure you that it is not any of those things in this case. In this case this image is well with in the native color spaces of both devices, they have been calibrated, profiles created more than once, and "matched" from a white point etc,  perspective by the hardware and software I have that is SUPPOSED to make these as good as it gets. Understand that I do not typically work like this. I don't remember the last time that I did not use the EXACT same monitors in multi-monitor setups.

I rigged this up with an old 24" LED Cinema I had laying around and my new 27" iMac to try to help a reader out that is having the same exact issue. I don't have answers yet so I am not going to name names. I do commit to do my best to get to the bottom of this and understand what is going on with this situation. If this is as good as it gets we all might want to same a few bucks on the calibration devices and software because the profiles that get built are so close to the Apple supplied profiles it's not funny. Not only that but I can tell you that the days of "drifting" are long gone. I have not built a new profile for a monitor that has had any real difference in a long time.

If this is the case and the multi-hundred dollar measuring devices/software cannot get you to a matching neutral gray any better than this then why bother? Seriously. This is not real different than it looks doing absolutely nothing.

As I said - I am on the case and will keep you updated as to my investigations. I did go through a lot of trouble to reproduce this while eliminating all of the things I know that cause this to happen when viewing the same image on different devices. This is not intuitive and not what photographers need or want when they buy a color management solution.

RB