---
title: "SoftSec Lab - Publications"
layout: gridlay
excerpt: "SoftSec Lab: Publications."
sitemap: false
permalink: /publications/
---

<style>
.pub-list li {
  margin-bottom: 13px;
  line-height: 1.3;
}
</style>
## Publications

{% assign publications_by_year = site.data.publist | group_by: "year" | sort: "name" | reverse %}
{% assign before_group = nil %}

{% for year_group in publications_by_year %}
{% if year_group.name == "Before 2021" %}
{% assign before_group = year_group %}
{% else %}

### {{ year_group.name }}

<ul class="pub-list">
{% for publi in year_group.items %}
<li>
<strong>
{% if publi.link.url %}
<a href="{{ publi.link.url }}" target="_blank">{{ publi.title }}</a>
{% else %}
{{ publi.title }}
{% endif %}
</strong><br />
<em>{{ publi.authors }}</em> —
<em>{{ publi.link.display }}</em>
</li>
{% endfor %}
</ul>

{% endif %}
{% endfor %}

{% if before_group %}
### {{ before_group.name }}

<ul class="pub-list">
{% for publi in before_group.items %}
<li>
<strong>
{% if publi.link.url %}
<a href="{{ publi.link.url }}" target="_blank">{{ publi.title }}</a>
{% else %}
{{ publi.title }}
{% endif %}
</strong><br />
<em>{{ publi.authors }}</em> —
<em>{{ publi.link.display }}</em>
</li>
{% endfor %}
</ul>
{% endif %}
