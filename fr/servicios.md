---
title: Services
layout: page
lang: fr
permalink: /fr/services
cta:
  text: Plus d'informations
  link: /fr/contact
---

**TKN** est spécialisé dans le **transport intermodal** de conteneurs de produits *chimiques liquides*, y *compris ceux classés ADR*, de conteneurs de *produits solides en vrac*, de *produits alimentaires*, de *gaz*, *d’isocyanates  et polyisocyanates et de *peroxydes d’hydrogène*.

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
