---
layout: default
title: Home
---

## Welcome

This is a small Jekyll-powered review site. Below are the latest reviews:

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.rating %} - ★{{ post.rating }}{% endif %}
    <p>{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>
