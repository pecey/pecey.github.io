---
layout: page
permalink: /publications/
title: publications
paper_years: [2023]
workshop_years: [2024]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.paper_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


<h1 class="post-title"> workshops </h1>
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.workshop_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f workshop -q @*[year={{y}}]* %}
{% endfor %}

</div>
