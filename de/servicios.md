---
title: Dienstleistungen
layout: page
lang: de
permalink: /de/dienstleistungen
cta:
  text: Mehr erfahren
  link: /de/kontact
---

**TKN** ist Spezialist in **multimodalem Transport** von Containern, die sowohl *chemische Flüssigkeiten*, die unter die Kategorie der *Gefahrengüter fallen*, als auch *feste Ladungen als Massengut*, *Lebensmittel*, *Gase*,  *Isocyanate*, *Polysocianate* und  *Wasserstoffperoxid* enthalten.

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
