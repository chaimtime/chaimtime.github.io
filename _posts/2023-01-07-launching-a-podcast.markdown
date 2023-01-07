---
title: "Launching A Podcast"
layout: post
date: 2023-01-07 08:52
image: /assets/images/markdown.jpg
headerImage: false
tag:
- gitlab
- FAQ
category: blog
author: Chaim
description: Explaining how we relaunched a new podcast
---

Since 2011, I have podcasted in different iterations. It first started with my two friends talking technology. Later, I asked Tom if he was willing to do a security show with me. 275 episodes later we had to shut it down. 

We didn't want to stop, but we had to move off our current platform into something new. 

# The Problem
I lost control of the main email account to do lots of account management. We used Wordpress, which is great for podcasting. In fact, it may be too much. Either way, our email address either got locked, or de-activated. I couldn't do any management. While it wasn't a problem, it wasn't helpful for anything other than posting episodes. 

We couldn't change our logo, nor access any stats. At some point FTP broke, and I had to use the Wordpress uploader. Our feed was set wrong. There were no stats. Also there were a ton of ads. 

Our logo wasn't 3000 x 3000. We couldn't modify it, so we weren't featured in iTunes anymore.

Essentially we weren't in control. 

# Decision Time
My friend owned the domain and the hosting. He unfortunately wouldn't let us buy it from him. I don't know why, but there is no ill will. We were getting years of free hosting and registration, so call it a wash. 

Do we continue using it with the above restrictions or start over. 

## We decided to start over. 

Tom got a new job, and moved across the country. He wouldn't be able to podcast for a while, so we figured, build everything from the ground up. 

## We wanted to make sure we were partners, and no one had unilateral control of any assests that were needed. 

As I tell people. You are my friend, until you are my enemy. I didn't want what happened before to happen again. We would share all costs moving foward. 


# Steps
We needed a name, and logo. We liked our old name, so we wanted to keep the same time based show idea. Turns out, Short Explanations wasn't a podcast name, and the .com was available. Yes, we were suprised. 

We had a disagreement on the website. Being the one who updates everything, I was scared of something that I wouldn't be able to manage and update. While I like open source, updating needs to be simple. It needs a step by step that anyone can do. Wordpress was that. The freemium podcast sites are that. When you use the words compile and git, things get extra confusing that I can't do on my ipad or on the road. 

Tom assured me Hugo and static sites would be easy. I wasn't sure, but he said he would build it, so I was good with that. I made static sites over the summer, so I was good with them. I got nervous about using gitlab and hugo because I'm not a git expert, nor have any familiararity with Hugo.

Email - we chose fastmail. We could have used a free service, but whatever

Hosting - Podcasts are oddly expensive. There is no resources other than file storage. We decided on Digital Ocean and their CDN. Again, I would have gone with a hosting company, but I have experience with Digital Ocean, and a CDN is fine. 

Overlays - To have a professional production we needed overlays. 

Intro / Outro - Still haven't done this yet, but I don't know if I will.

Other shows -  We want to have separate shows. If we want to grow, we want a different RSS feed per show.

# Issues
Logo needs to be 3000x3000. This is a monster file. I'm hoping apple doesn't change sizes, but that is always an issue. Also, we want to create a network. We wanted a common logo, but something that can be used as a branding logo. 

I tasked someone on Fivrr to do it. I didn't know what I wanted, but we were happy. I will say that Fivrr asks for a tip on top of the cost. The person sets their cost, why are we tipping?

Hugo was great to work with (according to Tom). It just took Tom to make the website. We both do have jobs, and we do this for free. 

The RSS feed is still giving us headaches. I think I figured it out, but each podcast aggregator has some different requirements. Artist needs to be called Author. Email for some reason is required. Image because of its size breaks things down. 

# Old Subscribers

We accumulated 1000 subscribers at our peak. Remember we had no insight other than feedburner that broke, we did different hacks to try and get visiblity. PodTrac did something, but who knows. While we don't track our users, we do want to know how many people are listening.

 To start over means most likely losing all our subscribers. I'm hoping to cross post on the old show for the next month, as well as putting an 301 redirect on it. Hopefully this will work, and we can keep some. 

# After The First Episode

 Turns out our redirect was for a small number of sites. The main rss feed was feedburner, which I do not have access to. We did lose our subscriber base. I'm not concerned, for we knew this was a possibility.

 The workflow was different. It wasn't harder, but different. I do like it because anyone of us can do it. Everything is documented, and available. 

 So far we are three episodes in. No data is out yet, but I'm waiting for a few more than doing an advertising push.



