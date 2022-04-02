---
layout: page
permalink: /publications/
title: Publications
description: publication in 
peer-reviewed: [2021, 2007, 1950]
non-peer-reviewed: [1905]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Peer-reviewed</h2>
{%- for y in page.peer-reviewed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h2>Proposed Workshop</h2>
{%- for y in page.non-peer-reviewed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


</div>
