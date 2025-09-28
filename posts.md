---
layout: page
title: All posts
permalink: /posts/
---

> This page lists all posts on the site in reverse chronological order.

{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
{% if sorted_posts and sorted_posts.size > 0 %}
{% for post in sorted_posts %}

- [{{ post.title | escape }}]({{ post.url | relative_url }}) ({{ post.date | date: "%Y-%m-%d" }})

{% endfor %}
{% else %}
No posts yet.
{% endif %}
