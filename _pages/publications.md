---
layout: page
permalink: /publications/
title: publications
description:
years: [2022, 2021, 2019]
nav: true
nav_order: 2
---

For the complete list of papers, please see my [Google scholar](https://scholar.google.com/citations?user=Slhn1M4AAAAJ&hl=en).

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
