---
layout: page
permalink: /publications/
title: Publications
description: My recent publictions.
years: [2024，2023, 2022]
nav: True
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
