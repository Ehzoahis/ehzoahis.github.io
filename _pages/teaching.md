---
layout: page
permalink: /teaching/
title: Teaching
description: My teaching experience.
years: [2023]
nav: false
horizontal: True
---
<div class="teaching">
  <!-- Display projects without categories -->
    {% assign sorted_teaching = site.teaching | sort: "years" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for teaching in sorted_teaching %}
          {% include projects_horizontal.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for project in sorted_projects %}
          {% include projects.html %}
        {% endfor %}
      </div>
    {% endif %}


</div>
