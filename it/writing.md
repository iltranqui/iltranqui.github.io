---
layout: page
title: Scritti
permalink: /it/writing/
alt: /writing/
includelink: true
---

<p class="writing-page-intro">Note, riflessioni e idee su ingegneria, machine learning e vita.</p>

<ul class="writing-list">
  {% assign it_posts = site.posts | where: "lang", "it" %}
  {% for post in it_posts %}
  <li>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%-d %b %Y" }}</time>
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    <span>{{ post.excerpt | strip_html | truncate: 180 }}</span>
  </li>
  {% endfor %}
</ul>
