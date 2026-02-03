---
layout: default
title: Home
---

# {{ site.title }}
{{ site.description }}

## Latest
<ul>
{% for post in site.posts limit: 15 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
{% endfor %}
</ul>
