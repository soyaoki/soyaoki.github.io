---
layout: default
title: Home
---

# Home Page

## Recent Posts

{% for post in paginator.posts %}
  - [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
