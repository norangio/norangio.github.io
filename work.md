---
layout: single
title: Work & Writing
permalink: /work/
nav_order: 3
---

## Writing & exploratory analysis

{% for post in site.posts limit: 5 %}
### [{{ post.title }}]({{ post.url }})

<p class="page__meta">{{ post.date | date: "%b %-d, %Y" }}</p>

{{ post.excerpt | strip_html | truncate: 220 }}

{% endfor %}