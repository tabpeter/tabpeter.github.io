---
layout: page
permalink: /publications/
title: publications
description: Publications listed here, includes both peer-reviewed articles and pre-prints
years: [2019, 2020, 2021, 2022, 2023, 2024, 2025]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
