---
layout: post
title: Aperture 3 And Alien Technology
comments: true
categories:
- Aperture 3
- Apple Aperture
- Articles
- disk management
- SAN
- storage
---
{% img http://photo.rwboyer.com/wp-content/uploads/2010/12/P1000845.jpg %}I have received about seven hundred and 2 thousand e-mails and one-on-one requests for help with Aperture 3. A lot of them have a two common themes. The first one is -" help my Aperture 3 has fallen and it can't get up". The second is - "How comes you never have no Aperture 3 problems?".

With respect to the first theme - of course I will try to help you out if I can. Time goes to one-on-one people on a first come first serve basis. I do have a life - sort of. With respect to the second questions I never really answer that, instead I focus on the way that other people actually operate their own little data-center instead and offer what I consider appropriate suggestions based on a lot of factors.

Today I am going to offer a tiny little bit of the way I operate my little data-center and why I don't have no Aperture issues. I am also going to ask readers to answer a very simple question at the end before I go off the deep-end with this kind of stuff.

First off I do have "Aperture issues". Probably not a lot - like most people. The real reason I am not going berserk with any of my application software is because I really don't give a hoot when it goes wonky. The reason is simple. No matter what happens, no matter how it happens, no matter if it is the software's fault or self inflicted. Under any set of circumstances I can get right back to where I was in less than 5 seconds. That is not hyperbole - it is a conservative estimate, assuming I am drunk and can't see strait when I initiate the plan B switch. Under better circumstances it takes me about 2 seconds.

Here is the part were the obvious happens - everyone wants to know how and what I do to achieve that. I am not being stingy because I never talk about my underlying technical infrastructure, I am being responsible. I honestly believe answering that question and writing about what I use and how in bit's and pieces of techno-babble and alphabet soup will cause more people disaster than not.

The truth is that most people have no need for anything remotely similar to what I do. The truth is not many people that do have the attention span or time to waste in ever managing to implement what I do at home. If you are an Aperture 3 user that is on a trajectory that is the same as the "Apple plan" you are golden - no complicated stuff required. That plan is roughly equivalent to all your stuff fits in a current iMac and the amount you add will easily be overwhelmed with the annual capacity increases that we all see in capacity and speed. It this is you - stick to the way Apple wants you to do things and just get decent gear every year. Timemachine has you covered.

If your data storage needs have already outpaced the "Apple normal people plan" you need to do something different. A bunch of people have gone the Drobo route. Some have gone the ga-gillion different libraries on a ga-gillion external hard-drives. This route sucks and I would never go there myself. From my point of view the Drobo expensive and doesn't actually do much for the price of entry. I guess it is okay for a very narrow group of people but the reality is the Drobo route is lacking functionality and is still a dead-end hard-stop step function that is EXACTLY like the lots-0-external non-managed drive solution. If you are outpacing single device technology so much so that you NEED a Drobo you need something way different than what you do today. Your life is now complicated.

The answer? Hmmm, there is only one in my hard-headed way of thinking, it's a SAN. Any storage area network that is halfway reasonable can do just about anything you ever dreamed of in terms of managing your storage in ways that will seem like "alien technology" Really it will - I swear. I have been doing SAN stuff since the mid-90's back when the only game in town was IBM ESCON clusters. Nothing ever ever goes awry in a way that the end consumers of the application and data ever actually notice. How about zero down-time and outages from an end-user point of view? It's like magic. I swear, you really don't want to know how it works, you just want to bask in the glory of a never ending, never down, do-anything with reckless abandon with no worries alien technology and have the confidence that you can be back to where you were with the press of a button - no waiting - NOW.

So what's the rub? Hmmm. Do you have a full-time big data center guy that deals with this crap for you? No well there's the rub. Even the most consumer oriented SAN from say Studio Network Solutions will be daunting to any non-IT type regular people out there. Added on to that obstacle is the cost of entry. You haven't really experienced sticker shock until you start pricing this kind of thing out from a traditional SAN vendor like EMC2 or even Studio Network Solutions. Apple used to have there own but it's pretty much gone by the wayside as I am sure their typical consumer target market don't really "get it". IT-guys already have their preferred recipe and there ain't no forking way they are going to mix Apple stuff with their storage network.

That brings us to my point - what do I do? I build my own SAN with all of the capability I want for less than the cost of a Drobo. Really. I also do other crap to my own Macs that I would never ever advise anyone to do that isn't already doing it. Here is why you have read this so far. You have a need and maybe I can help. I can and I will. Last week I agreed to build a black-box solution for an Aperture buddy of mine that gives him the capability I have with NO changes to his macs. Sort of plug and play. For the cost of a big Drobo with never ending capacity, instant recovery, cloud replication, and... performance that will DESTROY ANY SINGLE drive solution. Like 320 MBs write throughput.

I have a couple choices on how I might go forward with the couple of you out there that might also appreciate this kind of thing. One - piecemeal posts on how to roll-your-own. Bad idea - just enough info to spend a bunch of money and be really dangerous. A full scale eBook with every single thing laid out. Hmmm.... Maybe but still not for the feint of heart. Lastly make the "black box" solution available pre integrated with Apple and Aperture and provide support to Aperture users. Well not just me - but some other people as well.

I really really would love to hear what your interests are on this subject before I waste a lot of time on any of these approaches to this topic. If you have come this far please take a couple of seonds to think about this and answer this poll. As usual feel free to question or comment.

[poll id="22"]

RB