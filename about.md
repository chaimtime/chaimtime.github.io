---
title: About
layout: page
---

![Profile Image]({% if site.external-image %}{{ site.picture }}{% else %}{{ site.url }}/{{ site.picture }}{% endif %})
# About Me


My name is Chaim Cohen [Pronunciation: Silent C, rhymes with Time], hence the name Chaimtime.

Chaim is a computer science high school teacher in New Jersey. In his free time, he hosts [Short Explanations], a security podcast, teaching people that salted hashes are not breakfast. At home he teaches his son emoji as a second language, and 11 comes after 10.

# The Site

This is version 7 of Chaimtime. I started this site in 2002, to have a presence on the Internet. I thought I would blog; I still do.

Version 1: Hosted at Rutgers. Used Dreamweaver
<br>
Version 2: With the help of a friend, I created my own mySQL database for blogging. I really wanted to paginate
<br>
Version 3: Moved to Drupal
<br>
Version 4: Moved to Wordpress
<br>
Version 4.5: Moved hosts
<br>
Version 5: Significantly edited Wordpress themes
<br>
Version 6: Moved to Jekyll and Digital Ocean


Version 7 is a combination of a few things. First, it has been a few years, since anything was done. If you went to the site, you saw a copyright of 2020, if not earlier. I'm not blogging, so focus a theme on what I need it for.

### Learning about Github Pages
Who knew that website technologies would change. I went to Jekyll for speed and simplicity. I got half of that equation. Simplicity was achieved after I learned to SSH into [DigitalOcean] and rsync for each update. I would update the site on Github, then connect to my server, then rsync. That didn't even explain how to setup the whole thing. 

Now, I can use Github pages. Literally github will give me some space to host a really small site, and host it for free. Yes please. 

### Figuring out what I need
I don't blog. I admit it. However, I want a spot on the internet, for some stuff. Two things are really important to me right now. First is a new tutoring venture I'm trying out. Second is a spot for my resume. Both of those are again hosted with Github pages. There will hopefully be a blog post on how I got all of this working. 

What really started this was the fact I couldn't get a TLS certificate on my current hosting plan. If you believe the conspiracy theory, since they sold
TLS certs, they wouldn't integrate with [Let's Encrypt]. I also was being charged way too much by my old host. I really just wanted a landing page, with the
ability to blog every once in a while. Here were my requirements.

- Speed - Being able to write and publish a post fast
- Security - I'm tired of trying to secure wordpress
- Load Times- Black text on a white background shouldn't take that long to load
- Learning - I want to learn how all of this works.
	
I don't know why [Jekyll] jumped out at me. I was about to modify my old wordpress site, and call it a day. I guess I saw how fast it loaded, and figured
I could do this as well.


I heavily edited [NiceBlog] theme. Jekyll does not have a ton of themes to choose from. They were either too plain, or too blog heavy. 

I really like the idea of sharing individual pages. A lot of sites are moving away from having people click around. I want each post to be stand-alone. Yes, you can browse, but really the content
is contained in one page, then that is all the user should see.

# Hosting
Github pages is free, and I can have multiple projects. I'm sold. Now I save a few dollars per month, I can use on something else. I still love [DigitalOcean], and I'll be hosting my podcast there, however, 20 hits a day on a personal blog is worth looking elsewhere. 

~My requirement for hosting was that I needed to host multiple sites. I run other sites for family members, and they needed a place. Total, all of my websites maybe gets 20 hits a day. The problem is that hosting multiple websites puts you in the "expensive" tier of hosting plans. I really wished I could host the site on my home server. My friend Tom mentioned [DigitalOcean]. For $5 month, I got everything I needed, plus fantastic tutorials and learning experiences.~

# Favicon
The favicon was created by a student of mine, Tracy Fong. Every day after AP testing, she would draw that picture and color in
the shirt that I was wearing.

# Contact
On the top right of each page, you can choose how to contact me. I am pretty good about responding. 

# Privacy
Since I am interested in security and privacy, I take these things seriously. I was upset by how long Wordpress took to load. I took me forever to realize it was the sharing buttons. I didn't realize that they loaded so many scripts. What would be a simple page took 15 seconds to load.

There should not be any cookies. There is no reason to have them.



[Jekyll]: <https://jekyllrb.com>
[Let's Encrypt]: <https://letsencrypt.org>
[Nice Blog]: <http://jekyllthemes.org/themes/nice-blog/>
[DigitalOcean]: <https://m.do.co/c/d213df149b40>
[ShortExplanations]:<https://shortexplanations.com>
 
