---
layout: post
title: Flash Player Issues On OS X?
comments: true
categories:
- Articles
- Final Cut Pro X
- flash
- General Photography
- Nikon D7000
- OS X
- Video
- vimeo
- youtube
---
As you might have noticed, I have been doing a lot of work with Final Cut Pro X and talking about video. In the past I have not give the time of day to video on my blog. Why all of a sudden all the FCP X and video posts? Well really two reasons. First I actually rather present still photos that are part of some project or story as a video when presenting it on the web or even to a group of people. Second I have some projects coming up where I will need to do quite a bit of this type of work. Third - Some of those projects will actually require me to make actual video footage. I have a bit of experience doing this way way back on both film and video cams as well as a bit of experience with non-linear editing. These requirements were actually a big part of my Nikon D7000 purchase decision. More about the DSLR video decision and why I choose the D7000 soon.

How does this relate to Flash Player? Ummm... tangentially. One way or another if you produce video for web consumption you it will probably touch Flash Player sooner or later. I hate Flash and cannot wait for it to die a horrible death. Until then unless you want to set up your own streaming infrastructure - you are stuck with your video being played via flash. In messing around with YouTube and Vimeo (both using flash players for the vast majority of people in the universe unless the consumer jumps through hoops NOT to have it use flash) I realized that the current version of Flash was dropping frames like crazy on some test videos - actually all videos played in flash. My machine is a way overconfigured iMac core i7 sandy bridge that takes a lot of effort to make it even break a sweat. So why with nothing going on is Flash dropping 10-20% of the frames in any video? Answer = Flash sucks.

If you happen to be experiencing dropped frames in Flash for no apparent reason here is the recipe that seemed to solve the issue for me on OS X...
<ol>
	<li>Un-install Flash using the Adobe uninstaller.</li>
	<li>Reset all of the caches, history in Safari.</li>
	<li>Repair permissions using Disk Utility on your boot drive.</li>
	<li>Re-install the latest version of the Flash Player.</li>
</ol>
Early on in OS X 10.6 there were some rumblings that Safari had to be running in 32-bit mode for Flash not to drop frames but in my case today with the latest update to 10.6 this does not seem to be a factor and 64-bit runs fine for me now. Even if you don't make video and just watch them - this may help you out if you are seeing dropped frames in YouTube, Vimeo, Hulu, etc...

RB
<ol>
	<li>Repair disk permissions on your boot drive.</li>
</ol>