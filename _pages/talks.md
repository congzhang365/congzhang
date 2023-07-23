---
layout: page
permalink: /talks/
title: talks
description: A list of my talks
years: [2023, 2022, 2021, 2020, 2019, 2018, 2015, 2014]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

<h1>invited talks</h1>
  {% bibliography -f invited %}


<h1>conference presentations</h1>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f presentations -q @*[year={{y}}]* %}
{% endfor %}

</div>
