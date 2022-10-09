---
layout: page
permalink: /publications/
title: publications
description: Selected publications. For the full list please check <a href='https://scholar.google.pt/citations?user=z7oCodwAAAAJ&hl=en'>Google Scholar</a>.
years: [2018, 2017, 2015, 2014, 2013, 2012]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
