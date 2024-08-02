---
title: "SoftSec Lab - Publications"
layout: gridlay
excerpt: "SoftSec Lab: Publications."
sitemap: true  # Ensure this is set to true to be included in the sitemap
permalink: /publications/
---

<!-- Meta tags for SEO -->
<meta name="description" content="Explore the extensive research publications from SoftSec Lab at SKKU.">
<meta name="robots" content="index, follow">
<meta name="keywords" content="SoftSec Lab, SKKU, Software Security, Publications, Research">

## Publications

<!-- Include CSS for the publication list -->
<link rel="stylesheet" type="text/css" href="/css/publications.css" media="screen,projection">

<ul class="list-group">
  {% for publi in site.data.publist %}
  {% assign hasUrl = publi.link.url != null %}
  <li class="list-group-item list-group-item-action flex-column align-items-start" {% if hasUrl %}onclick="window.open('{{ publi.link.url }}', '_blank');" style="cursor: pointer;"{% endif %}>
    <div class="d-flex w-100 justify-content-between">
      <h5 class="mb-1">{{ publi.title }}{% if hasUrl %}<img src="/images/link.png" alt="External link" class="d-inline-block align-top" style="float:right">{% endif %}</h5>
    </div>
    <p class="mb-1">{{ publi.link.display }}</p>
    <small class="text-muted">{{ publi.authors }}</small>
  </li>
  {% endfor %}
</ul>

<!-- Hidden div for SEO -->
<div style="display: none">
  {% for publi in site.data.publist %}
  <p>{{ publi.link.title }} - {{ publi.authors }}</p>
  {% endfor %}
</div>
