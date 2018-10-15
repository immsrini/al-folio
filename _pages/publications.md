---
layout: page
permalink: /publications/
title: publications
description: Some recent papers describing research motivations & directions
years: [2018, 2015, 2014]
---

 <a href="https://scholar.google.com/citations?user=MahZ6toAAAAJ"> Google Scholar |</a> <a href="https://dblp.uni-trier.de/pers/hy/s/Srinivasan:Mukundhan"> DBLP </a>

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
