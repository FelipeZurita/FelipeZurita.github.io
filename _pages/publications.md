---
layout: page
permalink: /publications/
title: publications
description: Publications I've worked on.
years: [2021,2017,2015,2011,2010,2005,2004]
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
