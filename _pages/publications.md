---
layout: page
permalink: /publications/
title: publications
description: Publications I've worked on.
years: [1999,2000,2005,2021,2022]
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
