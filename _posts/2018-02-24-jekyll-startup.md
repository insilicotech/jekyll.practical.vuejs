---
date: 2017-01-16
title: Jekyll Startup
categories:
  - Jekyll
description: Jekyll Startup
type: Document
---
## Quick Startup

### Installation

~~~ bash
# Install Jekyll and Bundler gems through RubyGems
~ $ gem install jekyll bundler

# Create a new Jekyll site at ./myblog
~ $ jekyll new myblog

# Change into your new directory
~ $ cd myblog

# Build the site on the preview server
~/myblog $ bundle exec jekyll serve

# Now browse to http://localhost:4000
~~~


### Basic Usage

The Jekyll gem makes a `jekyll` executable available to you in your Terminal window. You can use this command in a number of ways:

~~~ bash
$ jekyll build
# => The current folder will be generated into ./_site

$ jekyll build --destination <destination>
# => The current folder will be generated into <destination>

$ jekyll build --source <source> --destination <destination>
# => The <source> folder will be generated into <destination>

$ jekyll build --watch
# => The current folder will be generated into ./_site,
#    watched for changes, and regenerated automatically.
~~~

## Fundmental of Jekyll

### Core Concept

Jekyll is a simple, blog-aware, static site generator. It takes a template directory containing raw text files in various formats, runs it through a converter (like Markdown) and our Liquid renderer, and spits out a complete, ready-to-publish static website suitable for serving with your favorite web server.

Jekyll is, at its core, a text transformation engine. The concept behind the system is this: you give it text written in your favorite markup language, be that Markdown, Textile, or just plain HTML, and it churns that through a layout or a series of layout files. Throughout that process you can tweak how you want the site URLs to look, what data gets displayed in the layout, and more. This is all done through editing text files; the static web site is the final product.

### Directory structure

A basic Jekyll site usually looks something like this:

~~~ bash
.
├── _config.yml
├── _data
|   └── members.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.md
|   └── on-simplicity-in-technology.md
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.md
|   └── 2009-04-26-barcamp-boston-4-roundup.md
├── _sass
|   ├── _base.scss
|   └── _layout.scss
├── _site
├── .jekyll-metadata
└── index.html # can also be an 'index.md' with valid YAML Frontmatter
~~~

* XML sitemaps
* RSS/Atom feeds
* Social Media buttons (on article pages)

### Front matter

The front matter is where Jekyll starts to get really cool. Any file that contains a YAML front matter block will be processed by Jekyll as a special file. The front matter must be the first thing in the file and must take the form of valid YAML set between triple-dashed lines. Here is a basic example:

~~~ html
---
layout: post
title: Blogging Like a Hacker
---
~~~

Between these triple-dashed lines, you can set predefined variables (see below for a reference) or even create custom ones of your own. These variables will then be available to you to access using Liquid tags both further down in the file and also in any layouts or includes that the page or post in question relies on.

## Reference

### Books

* [Ed](http://themes.jekyllrc.org/ed/Ed)
* [Good Clean Read](http://themes.jekyllrc.org/good-clean-read/)
* [Poole](https://github.com/poole/poole)
* [Lanyon](https://github.com/poole/lanyon)
* [Lanyon Plus](http://themes.jekyllrc.org/lanyon-plus)

### MISC

* [Jekyll static comment](https://mademistakes.com/articles/jekyll-static-comments/)
* [First familiarize yourself with `HTML5 Bilerplate`](http://html5boilerplate.com/)
* [When this wasn't enough learn more from `HTML5 Doctor`](http://html5doctor.com/)

### Themes

* [Hydepress](https://hydepress.github.io/jekyll-themes)

### WebFeed

* RSS
* Atom
* [Stringer: A self-hosted, anti-social RSS reader](https://github.com/swanson/stringer)

### Bootstrap Themes

* [Inspinia](https://github.com/Chuibility/inspinia)
