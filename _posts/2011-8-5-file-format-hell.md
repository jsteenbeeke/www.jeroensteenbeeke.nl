---
layout:    post
title:     "File format hell"
date:      2011-8-5 08:28:44 +0100
excerpt_separator: <!--more-->
permalink: /blog/2011/8/5/file-format-hell
---

As� I am nearing the completion of Revenant Rising, all sorts of practical problems arise. My book's cover isn't finished yet, I still need to do a black and white version of the [world map](https://www.jeroensteenbeeke.nl/revenant-rising-map/), and once all those are complete, I need to get the manuscript in the proper format and sent to the various distributors. The manuscript is currently written using [LaTeX](http://en.wikipedia.org/wiki/LaTeX), which is an excellent format to work in if you're using a version control system that's used to text-based formats, and it makes generating PDFs that can be directly turned into print books a breeze. Butwhat is suitable for print books may not be suitable for e-books.

<!--more-->
## Kindle Direct Publishing (Amazon)


### Kindle Direct Publishing (Amazon)


To get a book to the Kindle, you need to pick one of the [following formats](https://kdp.amazon.com/self-publishing/help/ref=hp_kdp_formats_navbox?topicId=A2V645S25NG1WN):
* Microsoft Word .DOC
* ePub
* Plain text
* Mobipocket
* Zipped HTML
* PDF

Now, this is quite an extensive list, and at least 3 of those are fairly easy to convert to using LaTeX as a base. However, PDF is essentially a format that describes pages, not structured text, so it's less than optimal as a basis for e-books. Plain text is also easy using LaTeX (using the detex program), but kills any formatting and doesn't allow you to include images. The last candidate, zipped HTML, is not that hard either, were it not that Kindle Direct Publishing is a bit quirky in how it interrprets the HTML, and requires you to put in specialized tags to achieve certain goals. Using existing LaTeX to HTML converters is probably not going to work.

## Smashwords


### Smashwords


[Smashwords](http://www.smashwords.com) only supports 1 format: Microsoft .DOC. Whatever their reasons are for choosing such an inane format are beyond me, but it does provide a bit of a challenge. There is no easy way to convert LaTeX to .DOC without several steps inbetween, or without manually having to redo all the formatting.

## Createspace


### Createspace


[Createspace](http://www.createspace.com) is a publishing on demand service, and makes print books. Createspace is probably the easiest company to submit my book to, as I can send my already-formatted PDF files directly to them.

## **How� do I proceed?**


### **How� do I proceed?**


Turning my LaTeX file into format supported by Kindle or Smashwords is going to be a challenge, but not an extremely difficult one. As a computer scientist I am confident I can create a tool that can convert my LaTeX source into a proper .DOC file for submission.

Or does anyone have an easier solution?

PS. I know I didn't mention Barnes and Noble and their Pubit program in this post. Ask me again when they decide to support non-US authors.