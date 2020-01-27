---
layout: blog
title: Jekyll Theme - Blog Page - Massively
description: Every great website starts with a great homepage. The homepage tells your viewers what your site is all about and gives your viewers a place to come back to.
sitemap:
    priority: 1.0
    lastmod: 2017-11-02
    changefreq: weekly
---

<ul class="post-list">
  {% assign posts=site.posts | where:"lang", page.lang | sort: 'date' | reverse %}
  {% for post in posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <a class="heading-page" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

        <div class="excerpt">{{ post.content | strip_html | truncatewords:10 }}</div>
    </li>
  {% endfor %}
</ul>
