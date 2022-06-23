---
layout: page
permalink: /publications/
title: publications
description: publications reversed chronological order.
# years: [1956, 1950, 1935, 1905]
nav: true
nav_order: 2
---
Coming soon.
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
