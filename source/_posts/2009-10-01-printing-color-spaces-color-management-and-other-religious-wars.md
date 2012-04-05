---
layout: post
title: Printing, Color Spaces, Color Management and Other Religious Wars
comments: true
categories:
- Adobe
- Aperture
- Apple
- Apple Aperture
- Articles
- blurb
- book
- cmyk
- color management
- General Photography
- InDesign
- photoshop
- printing
- rgb
---
<a rel="lightbox" href="/wp-content/uploads/2009/10/IDPDFblurb.jpg"><img title="IDPDFblurb.jpg" src="/wp-content/uploads/2009/10/.thumbs/.IDPDFblurb.jpg" border="0" alt="IDPDFblurb.jpg" hspace="10" vspace="10" width="150" height="134" align="left" /></a>Been doing a lot of correspondence lately with some poor souls that are lost in the evil wilderness between color management hocus-pocus, the bizarre alternate reality that is Aperture printing behavior, and Blurb.com. I hope that I didn't come off sounding dismissive of good color management practices or someone that thinks sRGB is the end all be all. I am not and have been dealing with end to end color management since the dark ages when it was "hard".

Most of the time color management should be easy nowadays as I explain in <a href="http://photo.rwboyer.com/2008/04/16/color-management-and-other-stupid-internet-tricks/">this rant from a while ago</a>.Â Let me try to set a couple of things strait and convey some useful info as well. I will start out by saying that Aperture printing is hopelessly broken in a lot of cases. I say this because a lot of readers are Aperture users. I personally think that it is shameful that Apple's "pro" image application is so prone to producing really bad prints through no fault of the users. The big issue here is that quite a substantial number of Aperture users follow what are perfectly reasonable color management paths then go to make a print from Aperture and it is horrible. After trying 72 different random settings with no real improvement except in the rare case that 42 wrongs add up to make a right, they turn to the web for answers.

On the quest for answers they pickup all kinds of voodoo mixed in with fantastically detailed and idiotically low level technical information (mostly related to CMYK 4 color processes) from the probably brilliant but obtuse likes of Heinrick Heimlichk over on the apple board and such. They end up with a hopelessly confused color paranoia at then end of it when the real answer is A - Aperture printing is broken and B - there is not a lot of practical "how to" information out there.

In cases where Aperture is producing a print that is obviously wrong and you are sure you did everything right (I will spare you the details they are all over the place on choosing the correct paper/printer profile) here is what I have done with limited success to "fix" it.

1) Trash the Aperture printing preferences.

2) Go download the absolutely latest driver for your printer from the manufacturer (this matters a lot)

3) Reinstall the printer driver.

4) Try it again making sure all of the settings in Aperture print dialog and the OS dialog match and make sense.

If this doesn't work you are probably out of luck printing from Aperture and using "good" color management practices until either Apple or the printer manufacturer releases updates that happen to fix your issue - these are rarely labeled with "fixes Aperture print issue" tags. Trust me on this a driver from Canon that was released in early 2009 did produced really bad results with Aperture (only Aperture) and the same exact driver released in June worked fine with no mention of anything remotely related as changes or fixes.

Okay, moving on to dealing with color management, profiles, etc no matter what your preferred software is. There are a couple of practical tips that I want to address here some of which are technically not "correct" and if you are someone that has been dealing with color management and conversion for years in the commercial world I am sure you will argue the special cases with me - please don't. If you are a photographer that wants to get good prints and are having some issues or just want to make them a little better - this may be for you.

There are two different cases of profile conversions that you need to concern yourself with. The first one is converting an image file from one color space/profile to another in order to meet some other outside parties specifications and ensure that you are doing the conversion that you want and NOT using the other parties default conversion settings. This is important, really important if you care about color and controlling how your images look. I cannot stress enough how important this is even if the third party is "color managed". Here is why - Let's say you have an image that is in Adobe RGB color space and you "soft proof" it on your calibrated screen. Fantastic and things will most like likely turn out okay if you send your images and it's profile to this outside provider/partner/whatever that will ultimately be converted into the color space for whatever the intent is (printing, projection, web, etc). This is probably what 99% of the world does and is generally okay but it is not at all okay if you really want to control and understand the results. Here is why - the proof and conversion settings maybe wildly different even if the profiles are exactly the same and that difference can be anything from about the same to catastrophically different. The two main conversion settings that are likely to vary are the "black point compensation" and the "rendering intent". If you do not think these matter a lot switch them back and forth/on and off while looking at a soft proof - still not convinced - make two prints with opposite settings.

Even if your settings are the same things can still go wrong because "black point compensation" is not a standard it is an algorithm that may vary from color conversion engine to color conversion engine. Same thing with the rendering intent "perceptual" - not a standard. The bottom line is if you care you will do the conversion yourself so no conversion happens on the other side.

The second and very closely related color space conversions that you will be doing are the conversion to make a print on your own printer in the print settings dialog. Here is a clue - use the same settings to print that you used to soft proof on your screen. In Aperture this is an issue because you can choose the profile but you cannot choose the rendering intent or black point compensation. Same deal with printing in Aperture except you get to choose black point compensation this time. Another reason Aperture printing is hopelessly broken and unacceptable at this state of the game. For those of you wondering - as far as I know the rendering intent in Aperture is "relative colormetric" - not a bad thing actually.

So what settings should you use for converting files and/or printing - the good news is that they are usually relative colormetric and black point compensation turned on. The better news is in 99.9% of all cases these are the "best" settings for photographs in both printing and file conversion situations. The only other setting that you may want to use for photographs is "perceptual", the reason you may want to use this is if significant areas - especially if they are adjacent to each other - are out of the target color gamut. In other words the color space that you are converting to cannot reproduce the colors in your image. How do you know if they are out of gamut - you need software that shows you like Photoshop. As far as I can tell Aperture has no way of showing you what colors are out of gamut in a target colorspace. Not good.

I guess that brings us to why I recommended Aperture users just sending sRGB to blurb.com - Well to make it easy. Most of your images - if they are like my images will not have a significant gamut issues in the conversion from Adobe 1998 to sRGB and you can actually see what that conversion will look like without anything special just by looking at them on your computer vs. sending them a wider gamut profile like Adobe RGB and having no idea what the conversion at blub will look like. Reason two is there is no way to do the conversion to the HP Indigo CMYK profile from within Aperture. Sure you can look at it using Apertures fixed soft proof settings - by all means do that but you cannot do the conversion within Aperture. Three blurb.com has tons of experience and satisfied customers that send them sRGB and the conversion settings they use are about as good as you are going to get, there is no reason to send them wider gamut RGB files as all of them go sRGB first (they say so) - you just don't get to see them first.

For those of you wishing a finer degree of control over the output the recipe is Photoshop to view gamut warnings, Photoshop to soft proof the conversions and parameters, Photoshop for the conversions and parameters. Then InDesign for the layout. Sure you can do all the Photoshop conversions but why the hell would you want to import CMYK PSD's back into Aperture trust me it will import them but Aperture wreaks havoc on them when you try to export them with the source profile. I don't even want to try to figure out what the hell isgoing on here it would be an intellectual exercise that leads nowhere with a bunch of model and space conversion going on just to use the Aperture book tool pretty much canceling out all of that fine degree of control you were after in the first place. <a rel="lightbox" href="/wp-content/uploads/2009/10/ApCMYK.jpg"><img title="ApCMYK.jpg" src="/wp-content/uploads/2009/10/.thumbs/.ApCMYK.jpg" border="0" alt="ApCMYK.jpg" hspace="10" vspace="10" width="95" height="150" align="right" /></a>The attached image is what happens to a when you try to export a TIFF from aperture using a CMYK PSD and a CMYK profile - I cannot even begin to explain what the hell Aperture is doing nor why they would allow you to import it in the first place considering ALL CMYK COLOR MODELS ARE DEVICE DEPENDENT. The funny thing is that it does work to export to an RGB color profile - how useless is that for managing your color very precisely at the source?

I hope that this helps some of you out with both Blurb.com, deciding on a tool set to use for your book project, and Aperture printing. One final word of advise if you are choosing InDesign for your blurb.com layout tool and are processing your final images in Photoshop and using the CMYK profile blurb.com provides: The default color settings in InDesign will not work - you much change them to use attached CMYK profiles versus retain CMYK numbers.

RB