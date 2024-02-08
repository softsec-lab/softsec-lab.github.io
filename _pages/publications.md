---
title: "SoftSec Lab - Publications"
layout: gridlay
excerpt: "SoftSec Lab: Publications."
sitemap: false
permalink: /publications/
---


## Publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br />
  {% if publi.link.url == null %}{{ publi.link.display }}
  {% else %}<a href="{{ publi.link.url }}" target="_blank">{{ publi.link.display }}</a>
  {% endif %}

{% endfor %}
