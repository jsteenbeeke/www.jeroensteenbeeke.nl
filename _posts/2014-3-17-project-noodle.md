---
layout:    post
title:     "Project Noodle"
date:      2014-3-17 09:12:35 +0100
excerpt_separator: <!--more-->
permalink: /blog/2014/3/17/project-noodle.html
---

My blog got blacklisted by Google a little over a week ago, as a result of a malware infection. With each page requested, two pieces of Javascript were inserted that were doing &quot;bad stuff&quot; in the background - downloading malicious software. I managed to clean out the infection, removed the plugin that gave them the vulnerability, and I patched up a few holes in the process.

<!--more-->
As a result, the contact form is disabled for the time being. If you need to contact me, send me a message on [Twitter](http://twitter.com/JSteenbeeke), make sure you're following me and I'll DM you my e-mail address.

Anyway, this &quot;ordeal&quot; got me thinking about the state of my website. While I'm more or less satisfied by the layout and things I can do with it, it took quite a bit of configuration and mixing and matching plugins, some of which I am now finding out are of questionable quality security-wise. While a PHP-based site has the advantage of cheap hosting, it has the disadvantage of being [one of the most horrid programming languages in existence](http://me.veekun.com/blog/2012/04/09/php-a-fractal-of-bad-design/), and even decent programmers can easily make mistakes that leave your site vulnerable. There is simply too much potential for errors.

As a result of this, I intend to replace this site with something homegrown - an [Apache Wicket](http://wicket.apache.org/) based site I'm currently referring to as Project Noodle. There are many pros and cons to this decision.

**Cons**
* Time - Building a site like this isn't something you do in a few hours, and I'll be required to maintain it myself
* Cost - Apache Wicket is Java-based, which means I'll require specialized hosting
* Security - I'll be fully responsible for any security issues in the site. Fortunately, with my experience + the tools chosen, it's much harder to screw up security
* Migration - I'll need to get the content from this site to the new one somehow

**Pros**
* Control - I can build **exactly** what I want, instead of patching together a &quot;good enough&quot; solution with a dozen Wordpress plugins
* Twitter integration - Often when I post here, I get lots of response through Twitter, but rarely any responses through the actual comment system (aside from fellow writer Jeroen Vogel). If I build my own site, I can integrate Twitter more closely.
* SSL - Secure communication for the entire site
* Security - Many common vulnerabilities are already taken care of by the frameworks in question, which makes it much harder to shoot yourself in the foot
* Familiarity - I know a hell of a lot more about Java and related frameworks than I do about Wordpress.

As a result of this, my posting rate may be a bit lower than it has been the past few weeks, but it's for a good cause.