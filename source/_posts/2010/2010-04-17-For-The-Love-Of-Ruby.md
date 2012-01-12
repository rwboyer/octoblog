---
layout: post
title: For The Love Of Ruby
comments: true
---

## 17 Apr 2010 - Along Way From Home

Well, I am sick and tired of WordPress. Really I am sick of the whole mess that is PHP land. A long long time ago in a galaxy far far away, I was a software developer for about 18 years - accidently. You see I went to school for Physics and Math and chucked in a CompSci major for the fun of it then accidently spent 18 years screwing around with computer crap. Then I sort of semi-retired and did the commercial photography thing - then I got sick of it when it felt just like.

Anyway here we are. Every time I mess around with my site I have to fix somebody's crappy PHP code. The issue is some of the stuff I want to get done with it leaves me... dreading looking at the mess of fork-lift reuse and horrendously bad crap that is WordPress plug-in's, themes, etc, etc. I really wouldn't mind if it was even remotely elegant, clever, cool... pretty but it is not. When I came across this stuff in my professional life I "refactored" it - a nice way of saying ditch it and start over. The problem is that I really do not want to write software any more - if I did I would. The pay is fantastic. Now I enjoy fooling around with a few things here and there for pure recreation. When doing that I will only use the tools I actually love to use. I can write C in my sleep and as long as any code that touches mine is fantastically good I don't mind that. Forget C++, not because it is bad - it is just the majority of the frameworks blow and again it is a hopeless mess done mostly by people that have not a clue. Cutting to the chase the two things I am willing to mess with at this point are Obj-C (just for the cool Cocoa frameworks so I can mess with new Apple stuff and my real love - Ruby.

Not that Ruby is a holy grail or anything - it is just the community is sooooo.. much different. It seems that language, and all of the frameworks, and conventions, and tools were brought into existence by software developers - real ones. Where PHP and the world around it seems to be the creation of VB knuckle heads and a few McDonalds fry cooks that hacked around in a Wordpress theme for a couple of weeks to get it to work. So... I think I might abandon Wordpress, the entire reason I use it is that I didn't want any "computer work" while publishing my little blog. Trying to navigate that WordPress plug-in mess to find things that actually work and work the way I want them to is a nightmare. If I am going to have to screw with this stuff for more than 10 minutes then I may as well just do it myself - or at least the parts that I want to. 

Here is my rediculously quick and dirty "conversion" of the old site with virtually no work. Behind the scenes there is a lot going on here, I just didn't feel like dealling with the CSS for the other stuff yet. The really cool part is I actually wrote a custom WordPress converter in IRB that took 5 minutes with DataMapper and then grabbed a copy of the source of [Jekyll](http://github.com/mojombo/jekyll) and coverted it to use HAML AND SASS so I wouldn't have to blow my brains out closing HTML tags. Heck I use HAML/SASS to create any HTML or CSS that I have to do vs getting some sort of repetitive motion injuries from all the </screw you> nonsence. 

The other really nice thing is that I can either host it statcally as I am doing over on [GitHub](http://rwboyer.github.com/) or I can do it dynamically. The best part is for all the parts that need to be dynamic - as in server side code - I can just write them as lightweight web services with RACK/Sinatra. 
Yes I think I am done with the whole PHP/Wordpress shitty ass mess.

RB
