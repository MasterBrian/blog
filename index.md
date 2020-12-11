---
layout: default
title: "Scotch & Thoughts"
---

## Welcome

<ul>
  {% for post in site.posts limit 1 %}
    <li>
      <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.date | date: "%m/%d/%Y" }} : {{ post.title }}</a>
      {{ post.excerpt }}
      <a href="{{ BASE_PATH }}{{ post.url }}">Read More... </a>
    </li>
  {% endfor %}
</ul>

<ul>
  {% for post in site.posts limit 1 %}
    <li>
      <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.date | date: "%m/%d/%Y" }} : {{ post.title }}</a>
      {{ post.content }}
      <a href="{{ BASE_PATH }}{{ post.url }}">Read More... </a>
    </li>
  {% endfor %}
</ul>
