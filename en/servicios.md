---
title: Services
layout: page
lang: en
permalink: /en/services
cta:
  text: Learn more
  link: /en/contact
---

**TKN** specialises in the **multimodal transport** of *liquid chemical* containers, including *dangerous goods*, *solid bulk product* containers, *food products*, *gases*, *isocyanates and polyisocyanates*, and *hydrogen peroxides*.

<!-- Abbreviations -->
*[TKN]: Transkontenord

<div class="row">
{% assign servicios = site.servicios | where: "lang", page.lang | sort: "orden" %}
{{ servicios }}
{% for servicio in servicios %}
{% include servicio.html %}
{% endfor %}
</div>

<div class="jumbotron clearfix">
  <p class="text-center"><a class="btn btn-default btn-lg" href="{{ page.cta.link }}" role="button">{{ page.cta.text }}</a></p>
</div>
