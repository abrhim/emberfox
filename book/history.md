---
title: History of the Web
type: Background
next: http
prev: intro
...

If you've read this far, hopefully you're convinced that browsers are
interesting and important to study. Now we'll dig a bit into the web itself,
where it came from, and how the web and browsers have evolved to date. This
history is by no means exhaustive.[^sgml] Instead, you should view it as a brief
view into a much larger---and quite interesting in its own right---subject.

[^sgml]: For example, nothing much about
[SGML](https://en.wikipedia.org/wiki/Standard_Generalized_Markup_Language) or
other predecessors to HTML. (Except in this footnote!)

The Memex concept
=================

The earliest exploration of how computers might revolutionize information is a
1945 essay entitled [As We May
Think](https://en.wikipedia.org/wiki/As_We_May_Think). This essay envisioned a
machine called a [Memex](https://en.wikipedia.org/wiki/Memex). The Memex was an
imagined machine that helps (think: User Agent) an individual human to see and
explore all the information in the world. It was described in terms of microfilm
screen technology of the time, but its purpose and concept has some clear
similarities to the web as we know it today, even if the user interface and
technology details differ.

The web is at its core organized around the Memex-like goal of _representing and
displaying information_, and how to provide a way for humans to effectively
learn and explore that information. The collective knowledge and wisdom of the
species long ago exceeded the capacity of a single mind, organization, library,
country, culture, group or language. However, while we as humans cannot possibly
know even a tiny fraction of what is possible to know, we can use technology to
learn more efficiently than before, and most importantly, to quickly access
information we need to learn or remember. Computers, and the Internet, allow us
to _process and store_ as much information as we want. The _web_, on the other
hand, plays the role of _organizing and finding_ that information and knowledge
to make it useful.[^google-mission]

[^google-mission]: The search engine Google’s [mission](https://about.google/)
statement to “organize the world’s information and make it universally
accessible and useful” is almost exactly the same as this. This is not a
coincidence - the search engine concept is inherently connected to the web.

Documents and hyperlinks
========================

The concept of interlinked documents began to appear in about
[1964-65](https://en.wikipedia.org/wiki/Hyperlink), when the term “link”
appeared (though connected to text rather than pages).[^literary-criticism]
Researchers then began to advocate for building a network of computers to
realize the concept. Independently, the first hyperlink system appeared (though
apparently not using that word[^hyperlink-first]) for navigating within a single
document; it was later generalized to linking between multiple documents. This
work also formed one of the key parts of the [mother of all
demos](https://en.wikipedia.org/wiki/The_Mother_of_All_Demos), the most famous
technology demonstration in the history of computing.

[^hyperlink-first]: The word "hyperlink" may have first appeared in 1987, in
connection with the HyperCard system on the Macintosh.)

[^literary-criticism]: These concepts are also the computer-based evolution of
the long tradition of citation in academics and literary criticism.

There is of course a very direct connection between this research and the
document+URL+hyperlink setup of the web, which built this idea and applied it
in practice.

The web emerges
===============

In 1983 the [HyperTIES](http://www.cs.umd.edu/hcil/hyperties/) system was
developed around highlighted hyperlinks. This was used to develop the world’s
first electronically published academic journal, the 1988 issue of the
[Communications of the ACM](https://cacm.acm.org/). Tim Berners-Lee cites this
1988 event as the source of the link concept in his World Wide Web
concept,[^world-wide-web-terminology] in which he proposed to join the link
concept with the availability of the Internet, thus realizing many of the
original goals of all the work from previous decades.[^realize-web-decades]

[^world-wide-web-terminology]: Nowadays the World Wide Web is called just “the
web”, or “the web ecosystem”---ecosystem being another way to capture the same
concept as “World Wide”). The original wording lives on in the "www" in many
website domain names.

[^realize-web-decades]: The web itself is, therefore, an example of the
realization of previous ambitions and dreams, just as today we strive to realize
the vision laid out by the web. (No, it's not done yet!)

In 1989-1990, the first browser (named “WorldWideWeb”) and web server (named
“httpd”, for “HTTP Daemon” according to UNIX naming conventions) were born,
again written in their first version by Berners-Lee. Interestingly, that
browser’s capabilities were in some ways inferior to the browser you will
implement in this book,[^no-css] and in some ways go beyond the capabilities
available even in modern browsers.[^more-less-powerful] On December 20, 1990 the
[first web page](http://info.cern.ch/hypertext/WWW/TheProject.html) was created.
The browser we will implement in this book is easily able to render this web
page, even today.[^original-aesthetics] In 1991, Berners-Lee advertised his
browser and the concept on the [alt.hypertext Usenet
group](https://www.w3.org/People/Berners-Lee/1991/08/art-6484.txt).

[^no-css]: No CSS!

[^more-less-powerful]: For example, it included the concept of an index page
meant for searching within a site (vestiges of which exist today in the
“index.html” convention when a URL path ends in /”), and had a WYSIWYG web page
editor (the “contenteditable” HTML attribute and “html()” method on DOM elements
have similar semantic behavior, but built-in file saving is gone). Today, the
index is replaced with a search engine, and web page editors as a concept are
somewhat obsolete due to the highly dynamic nature of today’s web page
rendering.

[^original-aesthetics]: Also, as you can see clearly, that web page has not been
updated in the meantime, and retains its original aesthetics!

Berners-Lee has also written a [Brief History of the
Web](https://www.w3.org/DesignIssues/TimBook-old/History.html) that  highlights
a number of other interesting factors leading to the establishment of the web as
we know it. One key factor was its decentralized nature, which he describes as
arising from the culture of CERN, where he worked. The decentralized nature of
the web is a key feature that distinguishes it from many systems that came
before or after, and his explanation of it is worth quoting here (highlight is
mine):

> There was clearly a need for something like Enquire [ed: a predecessor
> software system] but accessible to everyone. I wanted it to scale so that if
> two people started to use it independently, and later started to work
> together, *they could start linking together their information without
> making any other changes*. This was the concept of the web.

This quote captures one of the key value propositions of the web. The web was
successful for several reasons, but I believe it’s primarily the following
three:

*   It provides a very low-friction way to publish information and applications.
There is no gatekeeper to doing anything, and it’s easy for novices to make a
simple web page and publish it.

*   Once bootstrapped, it builds quickly upon itself via [network
effects](https://en.wikipedia.org/wiki/Network_effect) made possible by
compatibility between sites and the power of the hyperlink to reinforce this
compatibility. Hyperlinks drive traffic between sites, but also into the web
_from the outside_, via email, social networking, and search engines.

*   It is outside the control of any one entity - and kept that way via
standards organizations - and therefore not subject to problems of monopoly
control or manipulation.

History of browsers
===================

I'll now give a brief overview of the evolution of browser implementations. The
first _widely distributed_ browser may have been
[ViolaWWW](https://en.wikipedia.org/wiki/ViolaWWW); this browser also pioneered
multiple interesting features such as applets and images. This browser was in
turn the inspiration for [NCSA
Mosaic](https://en.wikipedia.org/wiki/Mosaic_(web_browser)), which launched in
1993. One of the two original authors of Mosaic went on to co-found
[Netscape](https://en.wikipedia.org/wiki/Netscape_Navigator), the first
_commercial browser_,[^commercial-browser] which launched in 1994. The era of
the [”first browser
war”](https://en.wikipedia.org/wiki/Browser_wars#First_Browser_War_(1995%E2%80%932001))
ensued, in a competition between Netscape and Internet Explorer. In addition,
there were other browsers with smaller market shares; one notable example is
[Opera](https://en.wikipedia.org/wiki/Opera_(web_browser)). The
[WebKit](https://en.wikipedia.org/wiki/WebKit) project began in 1999
([Safari](https://en.wikipedia.org/wiki/Safari_(web_browser)) and
[Chromium](https://www.chromium.org/)-based browsers, such as Chrome and newer
versions of [Edge](https://en.wikipedia.org/wiki/Microsoft_Edge), descend from
this codebase). Likewise, the
[Gecko](https://en.wikipedia.org/wiki/Gecko_(software)) rendering engine was
originally developed by Netscape starting in 1997; the
[Firefox](https://en.wikipedia.org/wiki/Firefox) browser is descended from this
codebase.  During the first browser war period, nearly all of the core features
you will implement in your browser that goes along with this book were added,
including CSS, DOM, and JavaScript.

 The "second browser war", which according to Wikipedia was
[2004-2017](https://en.wikipedia.org/wiki/Browser_wars#Second_Browser_War_(2004%E2%80%932017)),
was between a variety of browsers - Internet Explorer, Firefox, Safari and
Chrome in particular. Chrome split off its rendering engine subsystem into its
own code base called
[Blink](https://en.wikipedia.org/wiki/Blink_(browser_engine)) in 2013.

[^commercial-browser]: By commercial I mean built by a for-profit entity.
Netscape's early versions were also not free software---you had to buy them from
a store.

Web standards
=============

In parallel with these developments was another, equally important, one---the
standardization of web APIs. In October 1994, the [World Wide Web
Consortium](https://www.w3.org/Consortium/facts) (W3C) was founded in order to
provide oversight and standards for web features. After this point, browsers
would often introduce new HTML elements or APIs, and competing browsers would
copy them. Those elements and APIs were subsequently agreed upon and documented
in W3C specifications. (These days, an initial discussion,  design and
specification precedes any new feature.) Later on, the HTML specification ended
up moving to a different standards body called the
[WHATWG](https://whatwg.org/), but [CSS](https://drafts.csswg.org/) and other
features are still standardized at the W3C. JavaScript is standardized at
[TC39](https://tc39.es/) (“Technical Committee 39” at
[ECMA](https://www.ecma-international.org/memento/history.htm), yet another
standards body). [HTTP](https://tools.ietf.org/html/rfc2616) is standardized by
the [IETF](https://www.ietf.org/about/).

In the first years of the web, it was not so clear that browsers would remain
standard and that one browser might not end up “winning” and becoming another
proprietary software platform. There are multiple reasons this didn’t happen,
among them the egalitarian ethos of the computing community and the presence and
strength of the W3C.  Equally important was the networked nature of the web, and
therefore the desire of web developers to make sure their pages worked correctly
in most or all of the browsers (otherwise they would lose customers), leading
them to avoid any proprietary extensions.

Despite fears that this might happen, there never really was a point where any
browser openly attempted to break away from the standard. Instead, intense
competition for market share was channeled into very fast innovation and an
ever-expanding set of APIs and capabilities for the web, which we nowadays refer
to as _the web platform,_ not just the “World Wide Web”. This recognizes the
fact that the web is no longer a document viewing mechanism, but has evolved
into a fully realized computing platform and ecosystem.[^web-os]

[^web-os]: There have even been operating systems built around the web! Examples
include [webOS](https://en.wikipedia.org/wiki/WebOS), which powered some Palm
smartphones, [Firefox OS](https://en.wikipedia.org/wiki/Firefox_OS) (that today
lives on in [KaiOS](https://en.wikipedia.org/wiki/KaiOS)-based phones), and
[ChromeOS](https://en.wikipedia.org/wiki/Chrome_OS), which is a desktop
operating system. All of these OSes are based on using the Web as the UI layer
for all applications, with some JavaScript-exposed APIs on top for system
integration.

Given these outcomes---multiple competing browsers and well-developed
standards---in retrospect it is clearly not so relevant to know which browser
“won” or “lost” each of the browser “wars”. In both cases _the web won_ and was
preserved and enhanced for the future.

Open source
===========

Another important and interesting outcome of the _second_ browser war was that
all mainstream browsers today (of which there are *many* more than
three[^examples-of-browsers-today]) are based on _three open-source web
rendering / JavaScript engines_: Chromium, Gecko and WebKit.[^javascript-repo]
Since Chromium and WebKit have a common ancestral codebase, while Gecko is an
open-source descendant of Netscape, all three date back to the 1990s---almost to
the beginning of the web.
[^examples-of-browsers-today]: Examples of Chromium-based browsers include
Chrome, Edge, Opera (which switched to Chromium from the
[Presto](https://en.wikipedia.org/wiki/Presto_(browser_engine)) engine in 2013),
Samsung Internet, Yandex Browser, and UC Browser. In addition, there are many
"embedded" browsers, based on one or another of the three engines, for a wide
variety of automobiles, phones, TVs and other electronic devices.

[^javascript-repo]: The JavaScript engines are actually in different
repositories (as are various other sub-components that we won’t get into here),
and can and do exist outside of browsers as JavaScript virtual machines. One
important such application is the use of
[v8](https://en.wikipedia.org/wiki/V8_(JavaScript_engine)) to power
[node.js](https://en.wikipedia.org/wiki/Node.js). However, each of the three
rendering engines does have its own JavaScript implementation, so conflating the
two is reasonable.

That this occurred is not an accident, and in fact tells us something quite
interesting about the most cost-effective way to implement a rendering engine
based on a commodity set of platform APIs. For example, it's common for a wide
variety of independent developers (ones not paid by the company nominally
controlling the browser) to contribute code and features. There are even
companies and individuals that specialize in implementing these features!