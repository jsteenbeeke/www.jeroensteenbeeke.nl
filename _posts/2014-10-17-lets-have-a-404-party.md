---
layout:    post
title:     "Let's have a 404 party"
date:      2014-10-17 12:00:00 +0100
excerpt_separator: <!--more-->
permalink: /blog/2014/10/17/lets-have-a-404-party
---

One of the more recent additions to this new site is the detection and handling of 404 (file not found) errors. This is done primarily to give me insight in malfunctioning parts of the website, but it also helps search engines and such.

One side effect, which my old site has as well, is that it exposes a lot of invalid requests that are sent to my site, namely that of [vulnerability scanners](http://en.wikipedia.org/wiki/Vulnerability_scanner). As of writing this, the URL to this new site is not yet public knowledge. I have only shared it on Facebook in a non-public post, and it has had only a limited number of visitors. My guess is that the vulnerability scanners in question just target IPs at random, and happened to find my box. 

<!--more-->
They didn't do any harm, of course, and their scanning did expose a few issues with regard to usability (for instance: how do you quickly create redirects for 86 invalid URLs?) that helped me improve the site.