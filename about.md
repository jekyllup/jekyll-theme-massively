---
layout: page
title: About
permalink: /about/
ref: about
lang: en
sitemap:
    priority: 0.7
    lastmod: 2017-11-02
    changefreq: weekly
---

We, the Computer Science Student Association (CSSA) of the University of Ottawa, provide by this Constitution an organization dedicated to the pursuit of obtaining and managing resources for all members of the undergraduate Computer Science community at the University of Ottawa. We are also dedicated to providing social programming, academic services and employment resource opportunities to all our members. We are dedicated to fostering a sense of community among students, professors and members of the computer science department through these events and services.

View our constitution in English [here.]({{ site.url }}/2017-2018-cssa-constitution.pdf) We are working on the French translation for our constitution.

## The Team 2018-2019

<ul>
{% for member in site.data.executives %}
    <li>{{ member.position.[page.lang] }}: {{ member.name.[page.lang] }} </li>
    <ul>
        <li><a href="mailto:{{ member.contact.[page.lang] }}">{{ member.contact.[page.lang] }}</a></li>
    </ul>
{% endfor %}
</ul>

## The office
Our office is located at <b>SITE 4076</b>, feel free to stop by.
