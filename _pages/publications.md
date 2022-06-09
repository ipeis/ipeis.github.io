---
layout: page
permalink: /publications/
title: publications
description: sorted list of publications
years: [2022, 2020, 2019, 2017, 2016]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
