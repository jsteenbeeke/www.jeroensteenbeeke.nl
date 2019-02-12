---
layout:    post
title:     "Feature Creep"
date:      2014-7-7 12:16:42 +0100
excerpt_separator: <!--more-->
permalink: /blog/2014/7/7/feature-creep.html
---

I mentioned a while ago that I'm working on[ a new website](https://www.jeroensteenbeeke.nl/project-noodle/), which will replace this one sometime in the future. Part of building this website involves converting all (or at least most) existing blog posts to a new format, complete with auto-migration of old style URLs to new style URLs. As a result of this, I'm rather hesitant to post new material on the current site. Each new post means more data to convert, and trickier URL management. This is the main reason this blog has been so silent lately.

<!--more-->
I intend to post more often once the new site goes live, but I've hit a little snag in that regard: I keep figuring out cool new features to add to it. The basic setup was simple:
* Twitter login
* Book pages
* Blog posts
* Dynamic pages

But then I realized the mailing list management site also runs on PHP, so I started incorporating that into the new site as well. Then I figured I might as well do the sending of actual e-mails from the website interface as well, saving me the trouble of logging in twice. Then I figured I could use [Mandrill](http://mandrill.com/) to send the e-mails instead of using my host's SMTP server, so I started making an implementation of their API in Java. And then, yesterday, I figured I could incorporate the distribution of alpha and beta reading copies (with automatic watermarks) through the site as well.

In short: the new website project might have a slight case of [Feature Creep](http://en.wikipedia.org/wiki/Feature_creep).