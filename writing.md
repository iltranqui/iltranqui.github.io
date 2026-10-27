---
layout: page
title: Writing
permalink: /writing/
alt: /it/writing/
includelink: true
---

<p class="writing-page-intro">Notes, reflections, and ideas on engineering, machine learning, and life.</p>

<ul class="writing-list">
  {% assign en_posts = site.posts | where: "lang", "en" %}
  {% for post in en_posts %}
  <li>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    <span>{{ post.excerpt | strip_html | truncate: 180 }}</span>
  </li>
  {% endfor %}
</ul>
