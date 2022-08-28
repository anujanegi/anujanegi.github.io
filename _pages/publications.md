---
layout: page
permalink: /publications/
title: publications
description: See the updated list on <a href='https://scholar.google.com/citations?user=Cu7zyVkAAAAJ&hl'>scholar</a>!
years: [2022, 2020, 2018]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
