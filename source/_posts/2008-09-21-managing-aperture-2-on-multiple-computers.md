---
layout: post
title: Managing Aperture 2 on Multiple Computers
comments: true
categories:
- Aperture 2
- Apple Aperture
- Articles
- work-flow
- Workflow
---
<a href="/wp-content/uploads/FromIweb/ghostships_book.jpg"><img title="ghostships_book.jpg" src="/wp-content/uploads/FromIweb/.thumbs/.ghostships_book.jpg" border="0" alt="ghostships_book.jpg" hspace="10" vspace="10" width="150" height="94" align="left" /></a>In the effort to keep this overview an actual over view I will discuss two basic approaches. Of course there are endless variations, and permutations, and combinations of each of these so feel free to mix and match until you find the right way for your workflow. The first approach being based on the concept that each Aperture library is separate and distinct. One on the â€œmainâ€ computer back at home base, the other being a portable library on your laptop computer. The second approach is based on the concept of a replicated library that is pretty much the same library on both machines.<!--more-->

The Separate and Distinct Aperture Library Approach:

Using the first approach is based on using the file-&gt;export-&gt;project and the converse file-&gt;import-&gt;project functions within Aperture 2. As an example letâ€™s say that you capture most of your images while you are away traveling. At the end of each day you would import your images into Aperture either into an existing project or a new project, whatever is appropriate. Now you can sort them, keyword the images, do all of your metadata work, your rating, and even get to some adjustments while you are on the road. Great! When you get back to home base and your main computer/Aperture library all you do is use file-&gt;export-&gt;project on your laptop, get the projectname.app file over to your main machine in whatever way you choose, and then use file-&gt;import-&gt;project on your main computer. Viola - you now have all of your images, metadata, adjustments, albums, light tables, etc. that were on your laptop there in your main Aperture library. In fact you now have it on both your laptop computer and your main computer. Get rid of it on the laptop if you want, unless of course you want to continue to work on in while you are on the go. If that is the case just continue working on it on your laptop and do the export/import thing again. The rub is every time you import on your main computer you will get another copy of the project. No big deal just delete the old one lock, stock, and barrel. The only caveat here is that every time you work on a project and want to continue working on it on a different computer you have to export the latest greatest, import it on the other computer, and then delete the older version from that computer (if it exists there). As long as your projects are a reasonable size this is extremely fast on modern hardware and gigabit network connections.

That was easy enough, letâ€™s throw in a couple of variations. Letâ€™s say you used a managed library on your laptop and referenced masters on your main computer (this is actually the scenario that I use personally). Easy. When you import the project into your main computer/Aperture library you will end up with managed masters for that project (it wonâ€™t change your other projects, a common misconception with Aperture is that a library is either a â€œmanaged masterâ€ library or a â€œreferenced masterâ€ library - Not true - you can mix an match all you like). All you need to do after you import the project with managed masters is to select all of the images in the imported project and use file-&gt;relocate masters to to put the master images where they belong on your main machine for whatever your file management scheme is. If you would like to take a project on the road with you that happens to be stored on your main Aperture library so that you can say.... do some long overdue keywording while you are on the plane but your main library uses referenced masters just use the "consolidate masters" option in the file-&gt;export-&gt;project dialog. This will put all of the referenced masters into the exported project, it will not turn the referenced masters into managed masters in your main library. When you get home just do the same thing you usually do. Export the project from your laptop, import it into your main library, and use the relocate masters to put the masters where they belong. Just a note - when you do this you will end up with duplicate copies of your project and a second set of referenced masters. Although there are ways to get around this and use the same masters that were already sitting on your file system in the same place I highly recommend from a workflow simplicity sake that you just delete the old project and old set of referenced masters.

The Replicated Aperture Library Approach:

Approach number two is for photographers that like to take their entire library with them on the road. Well thatâ€™s simple when using a â€œmanaged mastersâ€ Aperture library. Just copy the library from your main computer to your laptop. Move the old one out of the way and Bobâ€™s your uncle you are done. When you are sure that it worked go ahead and blast the old one. When you get home with all your new images and projects just copy the library from your laptop to your main computer using the same approach.

Now for reality, if you have a whole lot of images and shoot raw the whole Aperture library probably wonâ€™t fit on your laptop. No problem just use referenced masters on your main computer. When you want to take your library with you just copy it to your laptop. If you are generating previews everything will still work fine except for adjustments and a few other things where you actually need to have the masters on-line to work with them. Letâ€™s take a look at a fairly common scenario - a main library with referenced masters that you take with you by copying it (leaving the actual masters at home). While you are away you shoot a bunch of images and add some projects. If you are using managed masters for the new projects, when you get back to home base just copy the whole Aperture library from your laptop to your main computer and then select all of the images in the new projects and use file-&gt;relocate masters to put them where they belong in your file management scheme. (A real nice trick for keeping track of this while you are way is to put all of the new projects in a blue folder, when you get home just click on the blue folder itself. All of the images in all of the new projects will show up in the browser and you can relocate them in one fell swoop)

If you would like to work on an existing project (as in add new images, and do adjustments) while you are on the road just remember to select all of the images in that project and use file-&gt;consolidate masters on your main computer before you copy the main Aperture library to your laptop. When you get back and copy the library from your laptop to your main computer you can again just select all of the images in those projects and use file-&gt;relocate masters to make them referenced again. I cannot stress enough that although there are ways to use the old set of masters it is much simpler and safer to just duplicate them and get rid of the old set until you get used to dealing with the whole multiple machine workflow.

As I mentioned at the start of this article there are tons of variations on both of these themes. The main features to really get familiar with for coming up with a recipe to suit your particular Aperture 2 workflow needs are:
<ul>
	<li> Relocate masters</li>
</ul>
<ul>
	<li> Consolidate masters</li>
</ul>
<ul>
	<li> Delete previews</li>
</ul>
<ul>
	<li> Update previews</li>
</ul>
<ul>
	<li> Manage referenced files and of course...</li>
</ul>
<ul>
	<li> Import project and export project</li>
</ul>
Down the road maybe Iâ€™ll put a PDF together on managing huge libraries and some more complicated (but more efficient) ways of dealing with master images. For now if you have any specific questions about either of these approaches feel free to comment or <a href="mailto:rwboyer@mac.com">email</a> me.