---
layout: default
title: "Welcome to The Stress Factor"
---

# Welcome to "The Stress Factor"

Here, we'll post weekly solved problems to help you prepare for the Mechanical Engineering Machine Design PE exam.

# Problem of the Week
{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

{{ post.excerpt }}
{% endfor %}


