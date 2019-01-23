---
layout:    post
title:     "Implementing Social Media Logins"
date:      2014-9-19 08:00:00 +0100
excerpt_separator: <!--more-->
permalink: /blog/2014/9/19/implementing-social-media-logins
---

This new site (currently) has three different ways to log in:

* Twitter
* Facebook
* Google+


Originally, the site only supported Twitter, but when I gave the first few people a demo they suggested supporting other social media sites as well. My experiences with the various login methods have been mixed.

<!--more-->
https://twitter.com/JSteenbeeke/status/512553542155255809

Twitter was the easiest. I've written half a dozen or so log in using Twitter procedures for various personal projects, so this was mostly copy/paste and using the Twitter4J API.

https://twitter.com/JSteenbeeke/status/512553760779173888

I am not aware of any Facebook libraries for Java that have the same level of maturity as Twitter4J, though considering the fact that I had a working implementation in another project, I didn't look very hard. It was mostly copy/paste with a few minor tweaks to get the info I needed.

https://twitter.com/JSteenbeeke/status/512554464390422528

Boy. Google+ was **really hard** to get to work. Google has comprehensive library support for its various APIs, so you'd think this would be pretty easy. The login flow resembles the one used by Facebook and Twitter (they're essentially all OAuth implementations). But working with the API is the equivalent of opening the puzzlebox that summons the [Cenobites](http://en.wikipedia.org/wiki/Cenobite_%28Hellraiser%29), or mud-wrestling with a [Xenomorph](http://en.wikipedia.org/wiki/Alien_%28creature_in_Alien_franchise%29).

Fortunately, I had an example to work with: a login using Youtube thingy I had written for a pet project. It's slightly less complicated than Google+, but gave me enough info to finish it without eating too much of my free time.

And there you have it! Three different ways to log in. Any others you think I should add? Github perhaps? Maybe Wordpress.com (not sure if that's even possible)?