---
layout: page
permalink: /teaching/
title: Teaching
description: My recent teaching.
years: [2023]
nav: False
---

{% for y in page.years %}

  <h2 class="year">{{y}}</h2>

  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
