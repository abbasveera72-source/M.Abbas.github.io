---
layout: page
title: Blog
permalink: /blog/
---

## Recent Posts
Click on a title below to read the full article.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date_to_string }}
    </li>
  {% endfor %}
</ul>
