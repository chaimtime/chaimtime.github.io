---
title: "Moving to Github Pages"
layout: post
date: 2022-07-20 08:52
image: /assets/images/markdown.jpg
headerImage: false
tag:
- github
- FAQ
category: blog
author: Chaim
description: All the trials and tribulations from moving from a VPS to Github pages
---



For 6 years, I've used Digital Ocean to host my website. Literally, a website that has my picuture, and a bunch of social links. Yes, I had some blog entries, but I realized that I don't blog consistantly. What I do want to showcase is how I solved problems. 

# The Problem
I'm creating many different websites for very simple purposes. My current website is a very simple landing page. I'm done blogging for a living, however, I'm finding out that these problems will occur over and over. If I spend a few minutes documenting them, with sources, hopefully, I'll minimize redoing work. 

Since I'm not updating daily, I need a way to update, but I contstantly don't want to look up rsync commands and build commands. 

### Properties
I have 5 different static websites that need hosting. None of these websites need any source of real power to host. <br>
Chaimtime.com - my personal landing site
Chaimtime Tutoring - a tutoring website to send people to. 
Chaimtime Resume - my current resume
My wife's website - a future website for my wife's law practice
My dad's website - Another landing page for my dad's business

As you can see, nothing special, but 5 sites starts moving you into a higher tier of cost. Digital Ocean now how a 3 free deploy application tier, but 5 is more than 3. I don't want to change what I'm doing for a few dollars a month, however, I started looking for alternatives. 

### GitHub Pages
GitHub started hosting these static sites mainly because they are tiny. A whole website is a few hundred KBs. They are hosting and deploying websites for free. 

My first issue started with how do you host multiple projects. I figured out you can do Chaimtime.com/project. For me that is perfect. However, chaimtime.com/wifeswebsite is not appopriate. I was ready to start multiple accounts to figure this out.

I was ready to use my 3 digital ocean deployments to do my site, my wife's site, and my dad's site. 

However, this site, is exactly what I needed:  [How to set up MULTIPLE GitHub Pages websites with custom domains](https://deanattali.com/blog/multiple-github-pages-domains/)

The above site is way better than the github tutorial. The github tutorial is way too complicated for what most people needed. Essentially, you name your root repo githubname.github.io. Then set your custom domain to that repo. Seriously the above website solves many problems.

### Enforce HTTPS
My next problem is getting a TLS certificate. ~~I found out that you must have the www.domainname.com, instead of just domainname.com. I didn't look for a solution for a bit, but it was driving me crazy for days.~~ I had lots of problems. I thought I had it working, but it would just fail.

I finally contacted github, and it was DNS. Literally typed the the DNS resolver wrong. 

### Root Structure
With my template, I followed the above link. I don't mind that my projects are chaimtime.com/repo. That is fine. I really wanted subdomains, but it wasn't a dealbreaker, especially, that free is the right price. 

### Workflow
I'm currently using VScode to edit my site, then committing to github. I'm so happy that as soon as build with Jekyll, then commit, the website gets updated fairly instantly. No rysnc. I'll finally be able to keep copyright up to date. 
