---
layout: page
permalink: /publications/
title: Publications
sort: 2
description: 
full-papers: [2025,2024, 2023]
short-papers: [2023, 2022, 2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Paper</h2>
{%- for y in page.full-papers %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h2>Demo & Poster & Workshop </h2>
{%- for y in page.short-papers %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f short -q @*[year={{y}}]* %}
{% endfor %}


</div>
