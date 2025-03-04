---
layout: default
title: Home
---

# Welcome to My Website

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})** - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}