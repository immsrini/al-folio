---
layout: page
permalink: /publications/
title: publications
description: Some recent papers describing research motivations & directions
years: [2018, 2015, 2014]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
