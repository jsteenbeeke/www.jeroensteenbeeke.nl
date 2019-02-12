---
layout:    post
title:     "Do not track"
date:      2016-5-29 13:00:00 +0100
excerpt_separator: <!--more-->
permalink: /blog/2016/5/29/do-not-track.html
---

Last week I found something interesting in my 404 log. For those of you unfamiliar with the term, each time someone tries to access a page that does not exist, that person receives the Not Found error, which according to the HTTP protocol is error code 404. Each time this happens, my site records it, and asks me what I want to do about it. Do I want to keep throwing this error (i.e. the page really doesn't exist and never has), to give a more useful error (like 410, which means that the page used to be there but has been removed and will not return) or to redirect to another page (in case the URL changed, which happened when I switched from Wordpress to this custom site).

<!--more-->
Most 404 errors are either caused by vulnerability scanners, that are looking for outdated versions of common software packages or plugins (such as Wordpress), so they can install malware on my site. These quickly get changed to error code 418 whenever I encounter them. The next batch of my 404 errors are caused by Baidu and Yandex, which for some reason don't understand that a URL prefixed with a / should be resolved relative to the site root, and not the current folder. The remainder is caused by 1 IP address in (I believe) Germany who keeps trying to access **/blog/year/month/day/title** as **/year/month/day/title**, which was the old pattern used by Wordpress but is no longer valid, and keeps trying to do tricks such as **/folder/./some/relative/path**.

But last week I got an interesting hit in my 404 log:

**/We-hope-you-dont-mind-us-selling-your-data-since-you-are-helping-google-to-do-just-that-with-spyware-UA-35058905-2-hosted-on-your-site**

Apparently someone doesn't like the fact that this site uses Google Analytics to see what people are up to when they visit this site. I installed this to get a better idea of where my site needed improving and where my traffic was coming from. It's used by millions of websites, which is why some people are concerned about how much information Google is gathering through all sites using this. Similar concerns exist for the Facebook Like button which is also on this site.

I understand those concerns, which is why this site honors [Do Not Track](https://en.wikipedia.org/wiki/Do_Not_Track) headers. Don't want my site to report your behavior back to Google? Enabling Do Not Track disables both Google Analytics and the social buttons (Twitter, Facebook, Google+), so nothing gets sent to their servers (though some of my blog posts include tweets that necessitate the inclusion of some of Twitter's Javascript).

So am I tracking you? Am I enabling Google to track you? Facebook? Twitter? Only with your consent.