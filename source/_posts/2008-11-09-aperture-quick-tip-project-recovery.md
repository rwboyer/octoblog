---
layout: post
title: Aperture Quick Tip - Project Recovery
comments: true
categories:
- Aperture
- Aperture 2
- Aperture Project
- Apple
- Apple Aperture
- Articles
- folders
- Organization
- package contents
---
<a href="/wp-content/uploads/2008/Aperture_QT___Project_Recovery.jpg"><img title="Aperture_QT___Project_Recovery.jpg" src="/wp-content/uploads/2008/.thumbs/.Aperture_QT___Project_Recovery.jpg" border="0" alt="Aperture_QT___Project_Recovery.jpg" width="150" height="94" align="left" /></a>I really should title this tip something more like "Quick and Dirty Project Recovery When You Are In a Bind" or something like that. If you ever find yourself in the unenviable position of being on a tight deadline for a wedding, story, commercial client, whatever and you have a problem accessing your Aperture library you only have a few options that are supported by Apple. Option one - recover your entire library from a vault, time machine backup, or other backup if you have one (and you should). <!--more-->Option two - Try rebuilding your library using the well documented methods on Apple's web site. The problem with both of these is they can take a long time and you may still have some debugging or catch-up work to do after that process completes. So here is a quick work around to get you going that will also allow you to keep all of the work you do while using the work around situation when you get your main library back up and healthy.

In the finder go to the Aperture library in question. Right click on it and choose show package contents. This is a screen shot of what you will see in a new finder window that opens up.<a rel="lightbox" href="/wp-content/uploads/2008/Aperture_QT___Project_Recovery_Finder.jpg"><img title="Aperture_QT___Project_Recovery_Finder.jpg" src="/wp-content/uploads/2008/.thumbs/.Aperture_QT___Project_Recovery_Finder.jpg" border="0" alt="Aperture_QT___Project_Recovery_Finder.jpg" width="150" height="90" align="baseline" /></a> The folders that you see mirror the blue folders in your Aperture organization structure. Now you just navigate to the folder that contains that project that you desperately need right freaking now. Here is the important part - copy (option + drag) the project to your desktop or whatever folder you wish outside the library. Don't move it. After the project has been copied out of the Aperture library make a brand spanking new pristine library by holding down the option key while starting up Aperture. Choose create new library when presented with the choice. When Aperture finishes firing up with nothing in it go to File-&gt;Import-&gt;Projects... Navigate to the folder that you copied your important project to and import it. When it's complete it should be about where you left off. If you notice a little strangeness it is probably due to context issues of mixing images that exist in other projects- no big deal - the other reason is that some of the database stuff for that project is screwy - just close Aperture and rebuild the library on startup. It should be much faster than rebuilding your main library. For those that haven't done it hold Option-Command while starting Aperture to get the rebuild screen. I have only had to do this once about a year ago and don't make a habit of this but time was not on my side. When you get your main library back up an running you may want to use the supported project export/project import to move the project from your temporary library back to your main library if you did work on it.

Take heed that I have verified this to work in Aperture 1.5.X and 2.X but it is absolutely not a supported solution and could become completely invalid in a future release from Apple considering how much they want to abstract physical storage from the user of their products. If this doesn't work for you there is a good chance that you have a preference file issue, a corrupted/broken Aperture installation, or some hardware issues.

RB