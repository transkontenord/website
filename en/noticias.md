---
title: News
layout: page
lang: en
permalink: /en/news
---

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) {{ post.date | date: "%d-%b-%Y" }}
{% endfor %}
