---
layout: page
permalink: /publications/
title: Publications
description: Publications which I have authored or co-authored.
years: [2025, 2024, 2023, 2022]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
