---
layout: post
title: Aperture - The Pesky Wrong Thumbnail Problem
comments: true
categories:
- Apple Aperture
- Articles
- broken thumbnails
- file management
- mismatched thumbnails
---
<a rel="lightbox" href="/wp-content/uploads/2010/01/ApertureScreen1.jpg"><img title="ApertureScreen1.jpg" src="/wp-content/uploads/2010/01/.thumbs/.ApertureScreen1.jpg" border="0" alt="ApertureScreen1.jpg" hspace="10" vspace="10" width="150" height="92" align="left" /></a>I have seen this issue and question on how to resolve it so much lately that I thought I would share a tidbit from my Aperture File Management eBook. If you have been using Aperture heavily for a while you have probably run into the problem where Aperture associates the wrong thumbnail image to a master image. I don't know the exact conditions that cause this to happen but I can tell you it is definitely some sort of concurrency bug in Aperture. Based on my non-clinical research and my own experience this issue rears it's ugly head when you are trying to do a whole lot at the same time within Aperture. Like running an import and moving files into/out of a project into another one, generating previews, etc.

When this problem happens logical courses of action rarely resolve it like "rebuild thumbnails". Sure try that first but most likely you already did or you wouldn't be searching the internet for an answer. I have personally done just about every bizarre gyration including diving into the Aperture library structure and database internals to figure out how to MAKE aperture fix this or at least find a way to fix it myself instead of starting from scratch.

By a wide margin the easiest way to make Aperture fix this problem while not getting rid of your images/edits/metadata/etc by starting over on the effected images is to create a new empty project. Copy the images in the project with the problem to the new empty project by selecting them and then option dragging them to the new one. Now just to be save do not do anything while the images are being copied. When it is all done check out your "new" project and if everything looks honky-dory then delete the old project hook, line, and sinker.

The reason this works is that the problem stems from sqlite database structures that are inside the project being corrupted in such a way that nothing you can do from within Aperture including "database repair" fixes them. Actually the database structures are fine - the data in them is wrong.  When you copy the images to a new project all of the data structures are rebuilt one by one from scratch in the new project.

RB

Ps. Hope this helps some poor lost souls out there.