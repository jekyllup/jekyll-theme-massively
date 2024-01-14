---
layout: post
title:  "This is the second post"
date:   2017-11-31
excerpt: "This post is about some random stuff"
image: "/images/pic02.jpg"
---

## How to Use This Theme
Just go ahead and read up on [how to install Jekyll](https://jekyllrb.com/). It's not too hard I promise!

Download this repository [here](https://github.com/iwiedenm/jekyll-theme-massively) and save it to any folder you want.

Open a terminal window or a command line and ```cd``` to that location.

Then enter: ```bundle exec jekyll serve```. You can now access your new Jekyll site from [http://127.0.0.1:4000/](http://127.0.0.1:4000/). Have fun exploring your new site!

## Features
### Auto-Generating Sitemap
The sitemap is auto generated! Just simply change the front matter of each site. It looks like so...
```
sitemap:
    priority: 0.7
    lastmod: 2017-11-02
    changefreq: weekly
```
### Formspring integration
The contact form below each page on the footer actually collects information! Just change your email address in the ```_config.yml``` file!
