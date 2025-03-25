---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 1
---

You can also find my publications in <a href="https://scholar.google.com/citations?user=8VGz9BIAAAAJ&hl=en">my Google Scholar profile.</a>

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="pubyear">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}


</div>
