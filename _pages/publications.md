---
layout: page
permalink: /publications/
title: publications
publication_years: [2023,2025]
workshop_years: [2025]
nav: true
---
<!-- _pages/publications.md -->

<div class="publications">

{%- for y in page.publication_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<h1 class="post-title">workshops</h1>
<div class="publications">

{%- for y in page.workshop_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshop -q @*[year={{y}}]* %}
{% endfor %}

</div>