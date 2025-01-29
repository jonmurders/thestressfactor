---
layout: default
title: "Welcome to The Stress Factor"
---

# Welcome to "The Stress Factor"

Here, we'll post weekly solved problems to help you prepare for the Mechanical Engineering Machine Design PE exam.

# Problem of the Week
{% for post in site.posts %}
    {% if post.categories contains "questions" %}
        {% assign latest_question = post %}
        {% break %}
    {% endif %}
{% endfor %}

{% if latest_question %}
    ## [{{ latest_question.title }}]({{ latest_question.url }})
    {{ latest_question.excerpt }}
{% else %}
    No questions available at the moment.
{% endif %}
