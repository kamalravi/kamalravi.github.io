---
layout: page
permalink: /publications/
title: publications
description:
years: [2025, 2024, 2023, 2022, 2021, 2018, 2014]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">
<font size="2">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}
