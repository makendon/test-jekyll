---
layout: default
title: Blog
permalink: /blog/
---
<h1>Latest Posts</h1>

<ul>
<ul style="list-style: none;">
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }} - {{ post.date | date_to_string }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>