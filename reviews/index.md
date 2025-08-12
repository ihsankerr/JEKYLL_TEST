---
layout: default
title: Reviews
permalink: /reviews/
---

# All Reviews

<ul>
{% for post in site.posts %}
  <li class="review-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.rating %} - <span class="stars">★{{ post.rating }}</span>{% endif %}
    <p>{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>
