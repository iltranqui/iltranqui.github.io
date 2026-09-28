---
layout: page
title: Writing
permalink: /writing/
includelink: true
---

<p class="writing-page-intro">Notes, reflections, and ideas on engineering, machine learning, and life.</p>

<ul class="writing-list">
  {% for post in site.posts %}
  <li>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    <span>{{ post.excerpt | strip_html | truncate: 180 }}</span>
  </li>
  {% endfor %}
</ul>
