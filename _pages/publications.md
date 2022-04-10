---
layout: page
permalink: /publications/
title: Publications
sort: 2
description: 
peer-reviewed: [2021]
non-peer-reviewed: [2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Peer-reviewed</h2>
{%- for y in page.peer-reviewed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h2>Workshop, Position Papers & Other</h2>
{%- for y in page.non-peer-reviewed %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshop -q @*[year={{y}}]* %}
{% endfor %}


</div>
