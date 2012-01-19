---
layout: post
title: Photoshop Lesson - Masks and Selections
comments: true
categories:
- adjustment layer
- Articles
- General Photography
- mask
- photoshop
- photoshop techniques
- selection
---
Had a conversation with a reader the other day who asked me why I am so down on Photoshop. Hmmm... I'm not. I am down on the what passes for a photo today. I am down on Time magazine covers that look downright horrible, like the glamourized Glen Beck. I am down on what I will call image abuse perpetrated via Photoshop. I don't write a lot about PS because I think that there are way too many sites about how to screw your perfectly good images up with idiotic photoshop techniques. I also think there are enough really fantastic sites that try to do a good job explaining what a wonderful piece of technology that is PS CS y through z. Enough of the explanation.

Tell you what - as things pop up in my mind that I think may be useful and are not covered 17,000 other places in both competent and incompetent ways I will try and post an article. I will start with a subject that has been covered quite possibly more than any other subject but... I'll do it in a way that I personally have not seen anyone do a really good job on a very powerful and useful set of techniques that are available in almost any recent version of PS. Yep, Masks and Selections. For a lot of people this is extremely painful so let me show you a really great way to deal with masks and selections of specific tonal ranges - this is fantastically useful and uses two of the most underutilized, under-promoted photoshop tools in history. Gradient Maps and Image Calculations. I am not going to show you what to use this for because the range of usefulness is infinite and to tell you the truth I really do not think the typical here is a crappy starting point and a WOW ending point is really that useful.

Follow along if you want, start with any image with any set of adjustment layers that you would like.

At the very top of all the layers add a new gradient map adjustment layer. Â Like so:

<a href="/wp-content/uploads/2009/09/ps1.jpg" target="_blank"><img style="margin: 10px;" title="ps1.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps1.jpg" border="0" alt="ps1.jpg" hspace="10" vspace="10" width="150" height="94" /></a>

The default gradient will be something simple like foreground to background, not terribly useful. This really comes into it's own when you add your own color "stops" at the bottom. We'll add two more just by clicking somewhere at the bottom of the gradient bar.

<a rel="lightbox" href="/wp-content/uploads/2009/09/ps3.jpg"><img title="ps3.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps3.jpg" border="0" alt="ps3.jpg" hspace="10" vspace="10" width="142" height="150" /></a>

Still not real useful but that will change in a second, what we are going to do now is change the color of each of these color stops by double clicking on the little squares at the bottom of each of them. We are dealing with selections and masks so we will be using black and white (000000 and ffffff).

<a rel="lightbox" href="/wp-content/uploads/2009/09/ps4.jpg"><img title="ps4.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps4.jpg" border="0" alt="ps4.jpg" hspace="10" vspace="10" width="143" height="150" /></a>

As you can see I changed the color stops on the ends to white and the color stops in the middle to black. You can do it the other way around if you want - I just prefer seeing what I am ultimately going to be "selecting" in black and gray and what I am not goinging to be selecting as white. This is exactly opposite of the way selections and masks actually work but no worries flip-flopping selections and masks it built in at every stage of the game in Photoshop as you will see. If you prefer not to flip flop just make your end points black and your middle ones white. No big deal. You may start to see where I am going with this. What I am going to do now is drag the middle sliders around to "select" Â the mid-tones or what I want to be mid-tones.

<a onclick="ps_imagemanager_popup(this.href,'ps5.jpg','1920','1200');return false" href="/wp-content/uploads/2009/09/ps5.jpg" target="_blank" onfocus="this.blur()"><img style="margin: 10px;" title="ps5.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps5.jpg" border="0" alt="ps5.jpg" hspace="10" vspace="10" width="150" height="94" /></a>

The next step is to play with the end point color stops and/or those little diamonds in the middle of the gradients to make things that you do not want selected absolutely white and to control how much of the selection is "feathered" into other tones. That is the grey part.

<a onclick="ps_imagemanager_popup(this.href,'ps6.jpg','1920','1200');return false" href="/wp-content/uploads/2009/09/ps6.jpg" target="_blank" onfocus="this.blur()"><img style="margin: 10px;" title="ps6.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps6.jpg" border="0" alt="ps6.jpg" hspace="10" vspace="10" width="150" height="94" /></a>

Okay now we have an image where all of the stuff I want to deal with, manipulate, lighten, darken, change contrast with - whatever is black and feathered in to all the stuff that I do not what to screw with. Now comes the cool part - let's turn it into an alpha channel using the widely not used image calculations (how is that for a sort of double negative oxy-non-moron), it's under the image menu - look for it. In the source 1 box we will choose the current document, the layer will be merged, and the channel will be grey. These should all be this way by default but if they are not make sure they are. In my case since I am screwy I will also check the invert box, if you choose your gradient opposite of mine you do not need to do this. In the source two the defaults should be fine - for this example they do nothing - source document is current document, layer is the gradient map layer, and channel is the layer mask - since the layer mask is revealing all kind it makes no difference. Now choose a normal blending mode, opacity 100%, and make sure the mask is not checked. Last but not least Â in the result channel choose new channel.

<a rel="lightbox" href="/wp-content/uploads/2009/09/ps7.jpg"><img title="ps7.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps7.jpg" border="0" alt="ps7.jpg" hspace="10" vspace="10" width="150" height="111" /></a>

Okay - now un-eyeball the gradient map layer so you can see the image again - you can leave it there, just don't view it. Let's say I want to bump up the brightness and contrast of all the crap that we targeted with the gradient map. If you take a look at your channels palette you will see we have a new alpha channel called "alpha-1". Let's use it. From the selection menu choose load selection and choose "alpha-1" from the channel drop down. After than add a new curves adjustment layer.

<a rel="lightbox" href="/wp-content/uploads/2009/09/ps8.jpg"><img title="ps8.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps8.jpg" border="0" alt="ps8.jpg" hspace="10" vspace="10" width="150" height="83" /></a>

What just happened was that since we loaded a selection prior to adding the adjustment layer, we automatically got a layer mask. You could always add it later but I will leave that as an exercise for the reader. Now you can jack around with the curves all you want and will just be affecting the mid-tone selection that we just did. Of course you can use that mask/selection for ANY layer or any photoshop action you would like - are you starting to see the POWER of this technique?

<a rel="lightbox" href="/wp-content/uploads/2009/09/ps9.jpg"><img title="ps9.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps9.jpg" border="0" alt="ps9.jpg" hspace="10" vspace="10" width="78" height="150" /></a>

Another example - this time a quick one vs. a walk-through. Let's say I want clouds in my image instead of a blank august grey-white sky. Okay I will just do what I did above but this time I am going for just the sky pixels. I then use the brush tools to get rid of stray highlights picked up, load an image of clouds, and use my second alpha channel just created as a mask for the clouds.

<a onclick="ps_imagemanager_popup(this.href,'ps10.jpg','1920','1200');return false" href="/wp-content/uploads/2009/09/ps10.jpg" target="_blank" onfocus="this.blur()"><img class="alignnone" style="margin: 10px;" title="ps10.jpg" src="/wp-content/uploads/2009/09/.thumbs/.ps10.jpg" border="0" alt="ps10.jpg" hspace="10" vspace="10" width="150" height="94" align="left" /></a>

Now this is terrible as I would not use these clouds with that image, nor would I consider this image finished, The point is with gradient map and image calculations you can make really complicated tonal based selections and fine tune them using ANY of the other photoshop tools. Yes this works on color images as well. This is by far the one of the most flexible and quick methods dealing with selecting parts of an image based on its tone (as in lightness or darkness) than any thing else out there. I have seen so many really really complicated ways of doing this that offer no benefit whatsoever. Of course there are quicker and easier tools to deal with various tonal issues globally but when you need to be able to mask/select any parts of an image for any other manipulation based on tone - this is the way.

If you followed or understood any of these meanderings you are well on your way to becoming dangerous with Photoshop considering what else you can do with Image calculations and not necessarily white and black gradient maps. For that matter some of you may see a whole new world just guessing what else you can use image calculations for based on the blending mode options and targets other than alpha channels.

If any of you find this type of info useful let me know and Â I will continue to shovel it forth.

RB