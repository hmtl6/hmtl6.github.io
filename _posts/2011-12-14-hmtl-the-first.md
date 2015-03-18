---
layout: post
title:  HMTL the first
location: Britannia Pub, Southwark
speakers:
 - Rich - CSS modular/component systems
 - Davy - jQuery UI and widgets
 - Pete - Some silly fun projects
 - Scott - Ebla (ebook reader)
 - Ian - JS pub/sub
---

## Rich - CSS modular/component systems

[Smacss](http://smacss.com/) - Read it, use it...

It's like the best bits from OOCSS combined with how we've been doing it for yonks - then all neatly wrapped up in easy-to-read short book.

Read the [24ways article on CSS modular/component system](http://24ways.org/2011/front-end-style-guides)

The link just gives examples of "pattern primers", "component libraries" and "toolkits".  It makes sense to develop one of these first for each project before attempting to build "pages" as it maps neatly onto the smacss way of thinking.  A step by step process for building a toolkit can be found at the bottom of the standards doc.

[Flexible grid, flexible images, media queries](http://www.abookapart.com/products/responsive-web-design)
This book is all you need and it's sooo short.  The only thing he gets wrong through the whole thing (but corrects in the last chapter) is he designs for desktop first rather than mobile first.  Mobile first makes sense as 'a lack of mediaquery support should be seen as your first mediaquery i.e. old phones don't support media queries there for it makes to make default the mobile version'.  It also makes sense as a developer and feels very natural - you feel like your building it up and adhering to progressive enhancement principles.

I use [this technique](http://jonikorpi.com/leaving-old-IE-behind/) for IE6 and polyfill with [respond.js](https://github.com/scottjehl/Respond) for IE7-8.  Although I'm thinking of getting rid of respond and dishing up the narrow-viewport version to all IEs below 9.

Read [Richie's standards and conventions doc on github](http://jeddy3.github.com/coding-standards-front-end/)

[Code is available](https://github.com/jeddy3/coding-standards-front-end) (we use this as the starting point for new projects)

You can fork, if you like, [the upstream](https://github.com/specialmoves/coding-standards-front-end) (from specialmoves)

"Device-agnostic" is the big take-away here

Start with 320 & 960 designs - interpolate the middle ground breakpoints. That's the bare minimum.  But it's best to refer to them as the "narrow" and "wide" designs.  Ideally, there shouldn't be mention of dimensions (320, 960 etc) or devices (mobile, desktop, tablet or tv) as your endeavouring for device-agnostic (which implies viewport-size-agnostic i.e. any size between 100 and 10000 should work equally well as the next size)

Web kit transitions on breakpoint - just normal CSS3 transitions work dandy e.g.

{% highlight css %}
-webkit-transition: all 0.2s ease;
-moz-transition: all 0.2s ease;
-ms-transition: all 0.2s ease;
-o-transition: all 0.2s ease;
transition: all 0.2s ease;
{% endhighlight %}

The "all" keyword means that things like padding and position are also transitioned.

[Good online resource](http://csswizardry.com/2011/12/measuring-and-sizing-uis-2011-style/)

- [http://sidekickschool.org/](http://sidekickschool.org/ )
- [http://sidekickstudios.net/](http://sidekickstudios.net/)

None of the code is compressed so feel free take a gander.


## Davy - jQuery UI and widgets

Using a very small (poorly documented) part of the jQuery UI lib

[jQuery UI docs](http://docs.jquery.com/UI_Developer_Guide) - Everyone take time to laugh at the pitiful jQuery UI developer documentation.

[This](http://wiki.jqueryui.com/w/page/12138135/Widget%20factory) is the official documentation about the Widget Factory.


## Pete - Some silly fun projects

### Ghetto blaster

 - [Write-up](http://petegoodman.com/labs/ghetto-blaster-php-js-soundboard/)
 - [Github](https://github.com/thegingerbloke/ghetto-blaster)

### Wrrds

 - [Write-up](http://petegoodman.com/labs/wrrds/)
 - [Github](https://github.com/thegingerbloke/wrrds)

### And a few more

 - [http://petegoodman.com/labs/](http://petegoodman.com/labs/)
 - [https://github.com/thegingerbloke](https://github.com/thegingerbloke)


## Scott - Ebla (ebook reader)

Showcasing our ebook reader

 - [https://github.com/monospaced/paperback](https://github.com/monospaced/paperback)


## Ian - JS pub/sub

Different approaches to abstracting your JS

- [http://aron.github.com/async-events-talk/slides.pdf](http://aron.github.com/async-events-talk/slides.pdf)
- [https://github.com/aron/async-events-talk](https://github.com/aron/async-events-talk)

Also worth reading about backbone

 - [http://documentcloud.github.com/backbone/](http://documentcloud.github.com/backbone/)


## Misc

Someone made reference to "single vs. multiple page websites" - do these patterns lend themselves to single-page websites? Replicating
the business logic in the client.

 - [http://michaux.ca/articles/mvc-architecture-for-javascript-applications](http://michaux.ca/articles/mvc-architecture-for-javascript-applications)
 - [http://addyosmani.com/writing-modular-js/](http://addyosmani.com/writing-modular-js/)
 - [http://weblog.bocoup.com/organizing-your-backbone-js-application-with-modules](http://weblog.bocoup.com/organizing-your-backbone-js-application-with-modules)
 - [http://backbonetutorials.com/](http://backbonetutorials.com/)

We discussed [creating webpages hosted on github](http://pages.github.com/) using a gh-pages branch

