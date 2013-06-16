---
layout: post
title: "Stereotypical First Post"
date: 2013-06-14 22:30
comments: true
categories: meta octopress markdown projects github emacs
---

I've been meaning to create this site for a while, that is I've been looking in to the most enjoyable way for me to create simple websites. I first heard of static site generators while reading the excellent retropectives by [Don Melton](http://donmelton.com/), who created [Magneto](https://github.com/donmelton/magneto) for his own blog.

For the uninformed, a static site generator is a way of writing your website with a collection of Markdown pages. I really liked the idea, though Magneto didn't fit my needs. Let alone its lack of support, it is a very stripped down, verbose solution. So I searched around and tried some other solutions:

* [Docpad](http://docpad.org/)
* [Wintersmith](http://wintersmith.io/)
* [Nanoc](http://nanoc.ws/)
* [Middleman](http://middlemanapp.com/)

I liked some ideas from all of these, but none of them really fit together the way I wanted them to. Docpad is very flexible, but requires a lot of scafolding and was a pain to simply throw together. Wintersmith was simple, but it has some odd conventions. Magneto took a lot of cues from Nanoc, most noteably the build script. At first I liked the idea of this much control, but the control turns in on itself when trying to set up a flexible website. Middleman was nice because of its dry conventions, but it goes too overboard with this without explaining itself.

Finally I've settled on using Jekyll, or more specifically [Octopress](http://octopress.org/). Octopress is a set of extensions for Jekyll to make creating blogs easier. Like Middleman, it follows a set of conventions in it's file structure. Unlike Middleman, it has been popularized through Github Pages it is obvious in what it is doing. Setting up Octopress is as easy as downloading/cloning a git repository and ensuring Jekyll is installed. It's configuration is a breeze, and the default theme sets up the website in the way I want. It also includes a Rakefile, to easily create new posts/pages and preview your site. So far the only complaint I have is themes are not aware of their own files, and will pollute your source directory when you install a new one.

There are a couple nice things traditional blogging software provides that a static site generator does not, most notably: comments and site search. To get around these I'm using [disqus](http://disqus.com/) and Google's simple search. Octopress provides built in ways to take advantage of these in its default theme, as well as many other community themes.

The next step for me with this site is to create a theme, along with some custom asides, showing off more of what I am doing around the Internet.

Allong with the [source code to this website](https://github.com/oppenlander/oppenlanderco), you can find [my .emacs.d](https://github.com/oppenlander/.emacs.d) on Github. To write this site, I'm mostly using Emacs with it's excellent markdown, paired web, and ruby modes.
