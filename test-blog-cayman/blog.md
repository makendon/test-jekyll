---
title: Blog
layout: default
permalink: /blog/
---
<h1>Latest Posts</h1>

<ul>
<ul style="list-style: none;">
  {% for post in site.posts %}
    <li>
    {{ post.date | date_to_string }}
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
      <br>
    </li>
  {% endfor %}
</ul>