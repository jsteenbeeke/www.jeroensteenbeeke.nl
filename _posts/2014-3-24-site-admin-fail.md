---
layout:    post
title:     "Site admin fail"
date:      2014-3-24 21:26:46 +0100
excerpt_separator: <!--more-->
permalink: /blog/2014/3/24/site-admin-fail
---

Today I wanted to write a large-ish post about how I obsess over sales numbers, but it seems the stars weren't aligned properly (or if you prefer a more scientific explanations: the Higgs Bosons were feeling heavier than usual). Where I normally have no issues logging into my own site, I could not, for the life of me, remember my password.

<!--more-->
Normally, this is solved pretty quickly by resetting my password into something easier to remember. Just hit &quot;Reset Password&quot;, enter e-mail, wait for the link, enter new password, problem solved.

Unfortunately my site felt otherwise - and instead of resetting my password as it should, it gave me a 403 error (for those of you unfamiliar with HTTP status codes, this means &quot;Forbidden&quot;). Not feeling up for a wrestling match with my host's server settings, I gave up and went on to do other stuff (such as [Dance Dance Revolution](http://en.wikipedia.org/wiki/Dance_Dance_Revolution), which is probably a good subject for another post).

Anyway, about fifteen minutes ago I decided to give it another try. I logged into the host's admin panel, ready to start fiddling with file permissions. All I needed was the file path that was failing. I tried the password reset link again, entered a new password, hit submit.

And it worked. No strange configuration voodoo needed, it just worked.

I'm still not sure why I got the 403 this afternoon, but at least I'm able to blog again. I think WordPress is trying to tell me I need to finish the replacement site.