---
layout: post
title: Color Spaces And Aperture 3
comments: true
categories:
- Aperture 3
- Apple Aperture
- Articles
- color management
- color space
- General Photography
---
I have received a ton of questions regarding Aperture 3 color spaces over the last week or so. Been busy so I haven't posted a whole lot - sorry. Anyway... I am going to try to answer a gaggle of questions, throwing some Apple specific tidbits, and hopefully give you a healthy dose of confidence regarding color in one fell swoop of Super Simple Stuff™.

First off - when processing RAW files Aperture uses what Apple refers to as a "internal super special wide gamut color space" for all image adjustments, manipulations, etc. They do not tell you what color space it is but from my experience it is perfectly fine to handle the native gamut of whatever RAW files I have ever thrown at it based on comparisons to testing in other software using ProPhoto color space. Bottom line - don't worry about it. The only time a specific color space comes into play is when you export the image to a JPG or TIFF file and of course when you shoot it to an external editing program or plug-in. For those of you that need to make absolutely sure you are not "losing" color information on that export just setup up your export presets etc. to use something like ProPhoto. In reality Adobe RBG if usually bigger than required anyway.

Okay so for all of you that have no idea what I am talking about, I am going to give you a tool that may help you visualize why some people go nuts with this stuff. It is a visual tool that comes free with all Apple computers and is pretty amazing. I continue to forget that a lot of you are not long time Apple folk like me. The magic tool is called  "ColorSync Utility". Just use spotlight to open it. Here is what it looks like.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs1.jpg %}

Now here is how to use it. First let's look at our monitors space, just find the profile your display is  using at the left. If you calibrated your display use that profile instead of the generic one. You can drag the mouse around over the 3D graph to see all the sides of it.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs2.jpg %}

Next lets have some fun by comparing a simple little profile we all know and love like sRGB to our monitor. In the upper left of the 3D graph click the arrow and choose "hold for comparison". Then find sRGB on the left and click on it  like so.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs3.jpg %}

Hmmmm. look at the overlay. I thought sRGB was "narrow". Well it is my monitor can show more oranges, yellows, and greens than sRGB but less blues and purples. So what does this tell me? It tells me that my monitor cannot show all the colors even in sRGB. Let's compare it to Adobe RGB by clicking on that. Remember - the display is the one that is "held for comparison". Holy crap - my monitor doesn't show anything. Well it's a little better in the orange and yellow but man you gotta be kidding me.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs4.jpg %}

Next lets take a look at Adobe RGB vs. let's say the blurb.com printing profile.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs5.jpg %}

Man - the printing gamut of those Indigo printers is REALLY SMALL, except for that turquoise area there. Maybe we should compare sRGB to the Indigo.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs6.jpg %}

Holy crap the indigo still can do that turquoise stuff better than either profile but sRGB is still way way way more color info everywhere else. Amazing. One last comparison, maybe our monitor to the Indigo.

{% img http://photo.rwboyer.com/wp-content/uploads/2010/10/cs7.jpg %}

So... What does all this tell you. Well for one it tells you that adobe RGB is way bigger than my screen in representing color. sRGB is pretty close - weaker in some areas and bigger in others.  But more importantly my screen, sRGB, and Adobe RGB all have way more color info capability than can possibly be represented on Blurb.com Indigo printers, EXCEPT for the blue/green/turquoise area in which none of those three represent that well. Do I care? Sure I do if I actually have an image that has a lot of information and subtile tone differentiation in that hue/color area. Remember that the graph is representative NOT the actual colors - your monitor cannot even show them. In practice this kind of stuff is good to know but this should give you a good feel for understanding why I tell non-color-professionals to send files to printers in sRGB.

If you can't see why let me lay it out. YOU CAN SEE sRGB for the most part, it is wider in most areas than a lot of commercial printers with some exceptions, and you don't have to guess. Now that you can see how to know what is going on and what might happen with image color profile conversions in the output process and WHAT YOU CANNOT SEE with your own eyes on your own monitor this should give you a guide on when to worry about it and what you may want to do.

Trust me there is no magic bullet here yet. You actually have to KNOW THINGS. Just using the widest gamut possible is not a great idea. Especially if you don't have a lot of experience at guessing results. It can actually be detrimental to you seeing issues with your own eyes on your monitor. Soft proofing using Aperture 3 or PS can give you a good idea for all the colors except where the printer is stronger in color representation than your monitor. You should know this to know what you are looking at. Where the blues and the greens are concerned in this case you have to think about the image that you are looking at to make an appropriate profile decision as well as what to do about areas that are not represented well.

I hope this actually helps you folks out with making progress on your digital color work. If it confused the crap out of you even more let me know, either way.

RB