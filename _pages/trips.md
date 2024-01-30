---
title: "SoftSec Lab - trips"
layout: textlay
excerpt: "SoftSec Lab -- trips"
sitemap: false
permalink: /trips/
---
### Trips


{% for trip in site.data.trips %}
#### {{ trip.name }}
    {% for detail in trip.details %}
* {{detail.writer}} - {{detail.title}} ({% for data in detail.contents %} <a href="{{data.href}}" target="_blank">{{data.type}}</a>{% endfor %} )
    {% endfor %}
{% endfor %}

