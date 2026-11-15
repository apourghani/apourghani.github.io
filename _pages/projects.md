---
layout: page
title: Research
permalink: /projects/
nav: true
nav_order: 3
---

{% assign research_projects = site.projects | where: "category", "research" | sort: "importance" %}
<div class="projects">
  {% for project in research_projects %}
    {% include projects_horizontal.liquid %}
  {% endfor %}
</div>
