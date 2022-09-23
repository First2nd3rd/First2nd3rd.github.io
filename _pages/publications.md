---
layout: page
permalink: /publications/
title: Publications
sort: 2
description: 
full-papers: [2022]
short-papers: [2022]
others: [2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Full Paper</h2>
{%- for y in page.full-papers %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h2>Demo & Poster </h2>
{%- for y in page.short-papers %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f short -q @*[year={{y}}]* %}
{% endfor %}

<h2>Workshop, Position Papers & Other</h2>
{%- for y in page.others %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshop -q @*[year={{y}}]* %}
{% endfor %}


</div>
