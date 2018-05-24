---
title: Neuigkeiten
layout: page
lang: de
permalink: /de/neuigkeiten
---

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) {{ post.date | date: "%d-%b-%Y" }}
{% endfor %}
