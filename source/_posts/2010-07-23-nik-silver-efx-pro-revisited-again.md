---
layout: post
title: Nik Silver EFX Pro Revisited Again
comments: true
categories:
- Articles
- Black and White
- General Photography
- Nik Silver EFX Pro
- photoshop
---
<a rel="lightbox" href="/wp-content/uploads/2010/07/1999_009_09_flatten_4x6.jpg"><img title="1999_009_09_flatten_4x6.jpg" src="/wp-content/uploads/2010/07/.thumbs/.1999_009_09_flatten_4x6.jpg" border="0" alt="1999_009_09_flatten_4x6.jpg" hspace="10" vspace="10" width="100" height="150" align="left" /></a>I have written about Nik's wonderful Silver EFX Pro on numerous occasions, including one of my very rare non-review reviews. In a word it is the only black and white simulation software I would bother with. It is really really good in a lot of ways. In my review I did complain about the film simulations not being quite right - sort of like over the top cartoon versions of the represented films - of course you can fine tune them to your liking. My main point was that if you are going to simulate a bunch of different classic B+W films why not do it "right" - I guess that is in the eye of the beholder.

My other complaint was that I really didn't like the way the grain simulation engine worked - from a perspective of the defaults that are built into each film simulation and far more importantly I really would like a better way to tell the software - or for the software to determine how much grain their should be. To summarize - there is no real "scale" to the grain. You absolutely need to treat the grain simulation entirely on two factors - one how many pixels your image actually has - and how big a print you are making. The other thing I didn't really declare as perfect was that the simulation didn't really work the way real grain does - I will say it is by far the closest thing out there.

That summarizes what I have written about Silver EFX Pro's grain simulation and film simulations - so why do I bring this up? Well... A reader that consumed all of that as well as my rants on how wonderful film is and why you need to treat it intelligently when you digitize it and scale it in a very very nice way told me that it would be freaking nice if I said something productive instead of just complaining. Okay - so I will show you and then let you know how I deal with some issues of grain simulation - I will take Silver EFX Pro first, rather than film since I am sure that is the more productive conversation.

Here is a 100% view of real Kodak TRI-X processed in D-76 by me:

<img title="1999_009_09_crop.jpg" src="/wp-content/uploads/2010/07/1999_009_09_crop.jpg" border="0" alt="1999_009_09_crop.jpg" hspace="10" vspace="10" width="438" height="438" />\

Here is an image captured on a DSLR 100% processed with Silver EFX Pro's TRI-X simulation:

<img title="06022008000089SFX_TX_crop.jpg" src="/wp-content/uploads/2010/07/06022008000089SFX_TX_crop.jpg" border="0" alt="06022008000089SFX_TX_crop.jpg" hspace="10" vspace="10" width="466" height="466" />

Now - when I say 100% that can mean a lot of things - in this case it means that I upres'ed the digital image to the same pixel dimensions as the film scan and then ran the Silver EFX Pro simulation - why did I do this? Because if I didn't it would not be a fair comparison. The relative grain to deal would be lower. In other words the grain would be proportionally BIGGER to the image detail because the Silver EFX Pro's complete dependency on the original image pixel dimensions (remember this is something that I criticized). You might say - no RB you are wrong - because that is not what the grain engine says it is doing... I say to you - No you are wrong think about the grain per pixel thing for a couple of more minutes and then get back to me. Better yet let me show you.

Here is the TRI-X simulation run on a full size (same size as 35mm film scanned at 4000 DPI or about 25 megapixels) and then resized to approximately 4x6 on your monitor.

<img title="06022008000089SFX_TX_flatten_4x6.jpg" src="/wp-content/uploads/2010/07/06022008000089SFX_TX_flatten_4x6.jpg" border="0" alt="06022008000089SFX_TX_flatten_4x6.jpg" hspace="10" vspace="10" width="600" height="402" />

Here is the image resized to 4x6 on your monitor and THEN the TRI-X simulation is run on that smaller image:

<img title="06022008000089SFX_TX_smart_4x6.jpg" src="/wp-content/uploads/2010/07/06022008000089SFX_TX_smart_4x6.jpg" border="0" alt="06022008000089SFX_TX_smart_4x6.jpg" hspace="10" vspace="10" width="600" height="402" />

Whoa... Wot? Okay it is exaggerated a little bit because the image I sent in was really small but it exaggerates the problem that I have been talking about. The image size you start with TOTALLY dictates what the grain simulation effects are.

Assuming you are following this so far let's evaluate the real TRI-X scan vs the simulation. Depending on how picky you are you can evaluate it one of two ways as visually presented. For arguments sake let's say you are not super picky and we'll say - "hey it's not too bad - in fact it is pretty close". Okay it is pretty good but that is ONLY because the digital capture is now the equivalent of 25 megapixels - if you are shooting at say a more reasonable 12-15 it is going to be far far exaggerated as compared to the detail size in the image. Hold that thought for a second and also consider that to a large degree that digital resizing works the opposite of optical resizing. There are some things that work the same but when it comes to grain downsizing the image for display actually exaggerates the grain. It does this in areas of the image where the grain has relatively high contrast because it keeps those high contrast pixels and throws out the low contrast pixels that are the same - this is because to render things you CANNOT get smaller then a pixel, even though the grain is only a pixel or two across at 40x magnification it stays the same size even as the image gets resized smaller.

So what does this translate into in the real world of displaying images? It boils down to this - There is no one size fits all setting that works on ANY ONE image let alone across all images of differing input sizes. There are dependencies that need to be taken into account and different simulation settings. They are:
<ol>
	<li>Input image pixel dimensions.</li>
	<li>Output image apparent magnification (you can use the word size but it is really size vs. what size you want to seem like you started with 35mm, MF, LF?)</li>
	<li>Output resolution/ppi/dpi</li>
</ol>
The bottom line is that you will need different settings for print vs screen at any given real image dimensions and those settings will vary tremendously based on the pixel dimensions of the original image you started with (4 mpix, 6mpix, 12mpix, 24mpix?)

If you were expecting a one shot recipe that you could stamp all over your images - sorry but that is impossible for me to deliver given the workings of the software at this point. I can give you some general guidance - compared to real life film. If you are working with 25 megapixel starting images the settings are almost right assuming you are comparing 35mm film. I would say they may be a little overboard  but it depends on real world processing factors that can only be speculated on. You be the judge based on the two images I showed you. They are way way too much for medium format and larger at similar pixel densities. So... If you are starting with less pixels and/or you are trying to simulate larger formats of film - you need LESS and smaller grain in the simulation.

I say all of that in the context of making prints where your real output resolution is at or above 300ppi. Images to be displayed at web sizes on the screen require far less grain for the given film sizes - the issue is that what settings are appropriate are highly image and resize method dependent.

Someday I wish Nik would provide parameters that are conceptually similar to what they have done with Sharpen Pro vs what they have with Silver EFX Pro at the moment. Maybe something like film format, output magnification, and output medium or ppi. The the software could render the appropriate grain simulation taking into account what you were after. You could spec something like 35mm, 8x (8x10), print (vs monitor). Nik would take over and render the appropriate grain simulation based on film type and give you an image that looked appropriate no matter what you input image size was.

Hope this was at all helpful to any fellow Silver EFX Pro fans/users.

RB

Ps - yet another reason I run Nik filters in PS on smart objects.