---
title: It Started With a Bang!
date: 2019-01-21 01:06:33
categories: 
- [blog, hfoss]
tags:
- open-source
- class
- hexo
---

# It Started With a BANG #

At least, I wish creating a personal website was as cinematic and bombastic as a Michael Bay-directed Transformers film. Alas, as with most projects, it takes a little bit of research to know what we're getting into. Let's take a look at how this site was made, shall we?

<!-- more -->

## First Flight ##

### IRC ###

I decided to use [HexChat](https://hexchat.github.io/), and registered my nick: effendiian.

### Email ###

I signed up for the [floss-seminar discussion](https://lists.rit.edu/mailman/listinfo.mmcgi/floss-seminar) mailing list!

## Getting Started ##

Finally I was ready to work on my blog. After I put on my Spotify playlist of, "[Iconic, Inspirational, and Intriguing](https://open.spotify.com/user/1271966423/playlist/6MlIJGplHSLlgmQgb0BKpw?si=khc3sdT-Sce904oMTdbeKQ)" orcheastral music, it was time to get to work. Before I could choose a framework to get started with, I needed to *know* what it was that I wanted to create.

### Priority Features ###

The term [*blog*](https://en.wiktionary.org/wiki/blog) is the shortened form of *weblog*, a term coined by Jorn Barger in the early days of the internet. It's a space for authors to journal thoughts and share them publicly. As such, there are a series of features expected of modern blog format websites.

- **Publish posts**. It's important that the time it takes to write and publish entries is quick, painless, and easy. The simpler the process is, the better.
- **Use an RSS feed**. This is necessary for my own personal needs; RSS/ATOM feeds are incredibly useful for aggregators and I would like to incorporate that with my solution.
- **Open source**. A big part of my work is going to emphasize open source technologies. It's only fitting that the blog itself is built with open source tools as well.
- **Free hosting**. Less of a user feature and more of a development limitation, the website needs to be hosted for free. The budget is nil. Zilch. Nada. Free.

### Secondary Features ###

These additional features are great for quality of life and I kept them in mind while searching for the tools that I would use in order to make the blog.

- **Multimedia support**. Not all my work involves code. Graphic design, artwork, and animations that I create should be able to reside on the website.
- **Customizable Theme**. I like to have control over my website's layout. This way, I can iterate the design across several periods of development, instead of implementing everything all at once.
- **Comment System**. Allowing people to comment on my articles would not be a bad idea.

## What Type of Website ##

I'll be hosting my website on GitHub using [**GitHub Pages**](https://help.github.com/articles/using-a-static-site-generator-other-than-jekyll/) - but I won't be using [Jekyll](https://jekyllrb.com/). Instead, I'll be using the static-site generator Hexo, for these reasons:

- **Easy GitHub Pages publishing**. While Jekyll does have GitHub pages support and integration, the differences needed in order to host Hexo's generated sites are minimal.
- **Extensibility with NodeJS**. The NodeJS integration delivers the rich package ecosystem on npm (and yarn) to Hexo developers.
- **Speedy**. Node is speedy; as a result, Hexo generates its static files in a matter of seconds. This is one advantage to using Hexo over Jekyll:
- **Unopinionated Asset Handling**. Unlike Jekyll, Hexo doesn't come with an asset pipeline for pre-processing assests by default. Instead, you're encouraged to roll what works for your setup using Node utilities.
- **Template How You Want To**. Hexo contains support for several types of templating engines, including [Swig](https://github.com/paularmstrong/swig) (by default), [EJS](https://github.com/hexojs/hexo-renderer-ejs), [Haml](https://github.com/hexojs/hexo-renderer-haml), and [Jade](https://github.com/hexojs/hexo-renderer-jade)/[Pug](https://github.com/maxknee/hexo-render-pug). Although good, Jekyll is limited to the Liquid templating engine.
- **Local CMS**. Both Hexo and Jekyll have this option that isn't true for all static-site generators; access to a local development CMS through [Hexo Admin](https://github.com/jaredly/hexo-admin) and [Jekyll Admin](https://github.com/jekyll/jekyll-admin), respectively.

## The JAMStack ##

By using Hexo to create content and hosting my static content on GitHub Pages, we end up with a website that's been built on what's known as the [JAMStack](https://jamstack.org/).

> **J**avaScript
> **A**PIs
> **M**arkup

JAM is sticky and it holds the pieces all together. There are benefits (as listed on [their site](https://jamstack.org/best-practices/)) that come with using this stack.

## Working With Hexo ##

Hexo's extensibility offers a lot of power if you're willing to put in the extra work to set things up. By default, Hexo projects are initialized with a standard set of plugins and is installed with the default theme, [Landscape](https://github.com/hexojs/hexo-theme-landscape).

### Plugins ###

I used these additional plugins while setting up the site:

- [Hexagon](https://github.com/adamsiwiec/hexagon) - Package manager for installing Hexo plugins and themes.
- [Archive Generator](https://github.com/hexojs/hexo-generator-archive) - Generates a blog post archive.
- [Feed Generator](https://github.com/hexojs/hexo-generator-feed) - Generates feed for ATOM or RSS2 aggregators.
- [Search Generator](https://www.npmjs.com/package/hexo-generator-search) - Generates a search index with configuration options available.
- [Git Deployer](https://github.com/hexojs/hexo-deployer-git) - Allows Hexo to deploy to a git repository.

### Themes ###

I used this theme for my website:

- [Cactus (Dark)](https://github.com/probberechts/hexo-theme-cactus).

This should give a good overview of how this website was created. All that's left is to put up some posts on the website itself!

## Tools ##

I used the following open source tools during the creation of this website.

### [Joplin](https://joplin.cozic.net/) ###

Joplin is a free, open source note taking and to-do application, which can handle a large number of notes organised into notebooks. The notes are searchable, can be copied, tagged and modified either from the applications directly or from your own text editor. The notes are in Markdown format. This was useful for drafting blog posts and keeping track of all the resources I needed to use.

### [Draw.io](https://github.com/jgraph/drawio/blob/master/LICENSE) ###

Useful for putting up wireframes when designing website layouts.

### [Hexo .gitignore](https://gist.github.com/spacemonkey/0a9a69004c11f82fc894) ###

Used this .gitignore file as the base of my own.

### [Real Favicon Generator](https://realfavicongenerator.net/) ###

Used to create the favicon for the browser and for other application platforms (iOS, Android, etc.).

### [Game-Icons](https://game-icons.net/) ###

Ever growing collection of free game icons. PNG and SVG file formats available.