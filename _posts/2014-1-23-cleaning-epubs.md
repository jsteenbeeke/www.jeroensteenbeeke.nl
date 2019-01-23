---
layout:    post
title:     "Cleaning up the EPUBs"
date:      2014-1-23 12:12:35 +0100
excerpt_separator: <!--more-->
permalink: /blog/2014/1/23/cleaning-epubs
---

Back when I started self-publishing my novels, I used two different channels to distribute my ebooks: Kindle Direct Publishing, and Smashwords. Each platform provided a different challenge with regard to distribution, mostly because of my choice of writing software (TeXMaker, a LaTeX editor). KDP requires a zipped HTML file (easiest format for me to convert to), and Smashwords required a Microsoft Word file. The former was easily automated, but the latter proved to be a nightmare. Each time I made a revision, I had to reformat from scratch.

<!--more-->
Naturally, as soon as I found an alternative, I left Smashwords, and went to Lulu, where I had already published my print editions.

Lulu offers a different challenge with regard to formatting. Instead of requiring Word documents, they require EPUB files. EPUB is a format that is remarkably easy to understand for a programmer such as me, and it's only a little more complex than the zipped HTML I used for Kindle.

But there are differences, stemming in part from the fact that there is a whole range of e-readers and software that can read EPUB files, all of which behave just a bit differently. As such, creating a good EPUB is more involved than creating a Kindle file.

I have managed to get it *mostly right* for my books, but the biggest disadvantage was that I didn't know of a good way to force a page break in EPUB files. Granted, page breaks should be used sparingly in ebooks, as each device works with different screen and font sizes, but certain parts of the book (such as the dedication) I want to intentionally display on a single page. In a Kindle HTML file, this is &lt;mbp:pagebreak /&gt;, a custom XML tag, but EPUBs have no equivalent tag. Some sites suggest using the CSS property page-break-before: always, but this does not seem to have an effect on the EPUB readers I have used to test. After some more Googling, I found the suggestion to split the EPUB into multiple internal HTML files - one for each section - where each new file will force a page break.

The good news is: this works. The bad news: it was quite a bit of work to get my custom converter to do this. The code for my converter got quite messy, so I spent some time cleaning it up. As I was testing, I noticed and fixed a number of other formatting problems (mostly related to centering text), cleaned up the inline CSS, the handling of labels, and the table of contents generation.

The result: I can now create much higher quality EPUB files. Soon (probably next week), I will re-upload all my existing EPUB editions (on Lulu and Kobo), which also means Barnes and Noble and iTunes editions will be updated.