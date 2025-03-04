---
layout: blog_card
title: Home
---

# Welcome to My Website

{% for post in site.posts %}
- **[{{ post.date-post.title }}]({{ post.url }})** - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}