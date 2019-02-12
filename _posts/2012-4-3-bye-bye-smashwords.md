---
layout:    post
title:     "Bye bye Smashwords"
date:      2012-4-3 12:30:42 +0100
excerpt_separator: <!--more-->
permalink: /blog/2012/4/3/bye-bye-smashwords.html
---

Regular readers of this blog know I do not use Microsoft Word. In fact, I tend to stay away from Windows software entirely when it comes to writing (even if I still consider it an adequate gaming platform). I realize I am a bit of an odd duck in this regard, but I'm a Software Engineer, and I like using my time efficiently.

<!--more-->
As such, I never was a fan of Smashwords, for the simple reason that it requires your manuscript to be submitted as a .doc file. As I've explained waaaay back in the post about [writing tools](https://www.jeroensteenbeeke.nl/my-writing-tools/), I use LaTeX for my manuscripts. For those who are unaware, [LaTeX](http://en.wikipedia.org/wiki/LaTeX) is a document markup language that works really well for typesetting books. It is mainly used in academia, but it works really well in auto-generated formatting for the print editions of my books. In addition to this, LaTeX files are really easy to convert to other formats, and I already have a converter that translates a LaTeX file in a zipped HTML file for Kindle Direct Publishing.

So once I finish a book, the process for creating a Kindle e-book is relatively simple:
* Package the LaTeX files and images (5 seconds of work)
* Feed it to the converter (30 seconds of work)
* Upload and go through KDP wizard

Print versions are even easier:
* Run PDFLaTeX on document file
* Go through Wizard at Lulu
* Upload, finish wizard

And then we have Smashwords:
1. Run detex on document file
1. Copy/paste into Microsoft Word or OpenOffice
1. Fiddle around with the settings for an hour to make sure it conforms to the style guide
1. Manually reapply all style settings (~1-2 hours)
1. Upload to Smashwords
1. Get rejected, repeat from step 3 until it's accepted (~1-2 hours)
1. File available

As you can see, using Smashwords is somewhat less pleasant. Where I can publish other books and e-books in a matter of minutes, Smashwords takes hours. This would be acceptable if it only happens once for each book, but I have a tendency to release revisions if people complain about typos (which happens despite editing). As you can understand, having to go through the same multi-hour routine is unacceptable to a guy who is used to automating tasks.

So naturally, I went looking for a better way. The main advantage of Smashwords is availability in a multitude of ebook stores, most importantly Barnes  Noble and the iBookStore. But Smashwords aren't the only aggregator for these ebook stores, so I figured I might as well try another.

To my surprise, Lulu, who does the print versions of my books, is an aggregator for BN and Apple as well. Contrary to Smashwords, Lulu requires you to submit your e-books in the international ebook standard: [EPUB](http://en.wikipedia.org/wiki/EPUB), which is a really machine-friendly format. It only took me two evenings of work to modify my LaTeX-to-Kindle converter into a LaTeX-to-EPUB converter. This significantly simplifies my e-book deployment for BN and Apple:
* Go through first part of Lulu wizard to get ISBN
* Package the LaTeX files and images (5 seconds of work)
* Feed package and ISBN to the converter (30 seconds of work)
* Upload and finish Lulu wizard

So when my KDP Select period runs out, I will not be republishing my Smashwords offering, but instead stick to Lulu.