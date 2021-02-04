---
layout: page
permalink: /publications/
title: Publications
<!-- description: Publications in reversed chronological order. -->
years: [2021, 2020, 2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
