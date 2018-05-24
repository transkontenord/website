---
title: Informations
layout: page
lang: fr
permalink: /fr/informations
---

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) {{ post.date | date: "%d-%b-%Y" }}
{% endfor %}
