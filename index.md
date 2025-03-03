---
layout: default
title: Home
---

# Welcome to My Blog

Here's what I've been writing about:

{% raw %}
{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
{{ post.date | date: "%B %d, %Y" }}

{{ post.excerpt }}

---
{% endfor %}
{% endraw %} 