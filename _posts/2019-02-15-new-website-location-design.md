---
layout:    post
title:     "New website location and design"
date:      2019-2-15 11:35:00 +0100
excerpt_separator: <!--more-->
permalink: /blog/2019/2/15/new-website-location-design.html
---

This website has had several incarnations over the years. It originally started as a Wordpress site, but
after a rather dicey experience with malware I kind of lost faith in that approach. Back then my free time
was somewhat less constrained then it is now, so I decided to build my own CMS system from scratch.

This worked well enough, but considering the frameworks I used this meant that hosting was rather expensive
compared to what it had been (around $160 a year as opposed to the $15 I was paying for the Wordpress site), not
to mention it had to be kept up-to-date whenever security vulnerabilities were discovered.

It worked, but it wasn't cheap, both time-wise and money-wise, but I kept it around because there wasn't really
any alternative I considered good enough, and migrating all the content would be a pain.

About a year ago, I first started working with Jekyll, however, which is a tool that is primarily used
to generate static sites based on (for instance) Markdown files, and I was quite surprised by its
flexibility. Many of the custom stuff I had on my existing site could be modelled using custom includes, 
so it didn't take long to conclude that Jekyll would indeed be a good replacement for my custom software.

Except, of course, that all the content needed to be migrated, which was written in a format that isn't
supported by Jekyll, so I needed to write my own converter. This took a while to finish, but the result
is sitting in front of you.

I had originally planned to host this site on a cheap VPS (at $10 a year), until my co-worker Martijn Dashorst
pointed out that Github pages (which is free) also supports custom domains, and that you can have multiple
pages (I was already using the default one for a page I use to scare away IT recruiters). This took a few
days to properly configure (which meant this site was behaving rather wonkily), but right now everything
appears to be working fine. 
