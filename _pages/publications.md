---
layout: page
permalink: /publications/
title: Publications
description: >
    Conference and journal publications in reverse chronological order. An up-to-date list is also available on Google Scholar
years: [2023, 2022, 2021, 2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>