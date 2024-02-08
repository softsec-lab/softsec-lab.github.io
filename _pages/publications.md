---
title: "SoftSec Lab - Publications"
layout: gridlay
excerpt: "SoftSec Lab: Publications."
sitemap: false
permalink: /publications/
---


## Publications

{% for publi in site.data.publist %}
{% assign hasUrl = publi.link.url != null %}
  {% if hasUrl %}<a href="{{ publi.link.url }}" target="_blank">{% endif %}{{ publi.title }}{% if hasUrl %}</a>{% endif %}<br />
  <em>{{ publi.authors }} </em><br />{{ publi.link.display }}

{% endfor %}
