---
layout: default
title: Best of
permalink: /best-of/
---

# Best of (4★ and above)

<ul>
{% for post in site.posts %}
  {% if post.rating and post.rating >= 4 %}
    <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> - ★{{ post.rating }}</li>
  {% endif %}
{% endfor %}
</ul>
