---
title: Servicios
layout: page
lang: es
permalink: /es/servicios
cta:
  text: Saber más
  link: /es/contacto
banner: /assets/uploads/images/originales/DSC_4796_1-2-ret.jpg
---

**TKN** es especialista en el **transporte multimodal** de  contenedores *químicos líquidos* incluidas *mercancías peligrosas*, contenedores de *productos sólidos a granel*, *productos alimentarios*, *gases*, *isocianatos y polisocianatos* y *peróxidos  de hidrógeno*.
{:.intro}

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
