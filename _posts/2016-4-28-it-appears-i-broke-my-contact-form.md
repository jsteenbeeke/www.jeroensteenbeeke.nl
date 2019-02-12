---
layout:    post
title:     "It appears I broke my contact form"
date:      2016-4-28 22:00:00 +0100
excerpt_separator: <!--more-->
permalink: /blog/2016/4/28/it-appears-i-broke-my-contact-form.html
---

A few months ago MailChimp and Mandrill decided it would be a good idea to extort Mandrill's customers by merging Mandrill back into the parent company, and requiring Mandrill customers to get a paid MailChimp account.

I'm not sure about the exact math, but it comes down to a fourfold increase in cost, and the elimination of the free tier, which I used.

<!--more-->
Now, this didn't appear to be that big of a problem. I thought I only used Mandrill for my Jenkins server (and previously for my mailing list, which is now managed, ironically, by MailChimp), and I had that migrated to MailGun in no time.

Feeling confident that I no longer used Mandrill, I deleted my account. And then, just ten minutes ago, I found out that this site also uses Mandrill, for the Contact Form.

Granted, I didn't get much mail through the contact form to begin with (three mails since launch?), but I hate having part of my site being non-functional. It should be relatively easy to fix though.