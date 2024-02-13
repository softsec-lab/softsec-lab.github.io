---
title: "SoftSec Lab - Publications"
layout: gridlay
excerpt: "SoftSec Lab: Publications."
sitemap: false
permalink: /publications/
---


## Publications
<ul class="list-group">
{% for publi in site.data.publist %}
{% assign hasUrl = publi.link.url != null %}

  <a href="{% if hasUrl %}{{ publi.link.url }}{% else %}javascript:void(0);{% endif %}" class="list-group-item list-group-item-action flex-column align-items-start" {% if hasUrl %} target="_blank"{% endif %}>
    <div class="d-flex w-100 justify-content-between">
      <h5 class="mb-1">{{ publi.title }}{% if hasUrl %}<img src="/images/link.png" alt="Description" class="d-inline-block align-top" style = "float:right">{% endif %}</h5>
    </div>
    <p class="mb-1">{{ publi.link.display }}</p>
    <small class="text-muted">{{ publi.authors }}</small>
  </a>
{% endfor %}
</ul>
  