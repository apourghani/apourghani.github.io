---
layout: page
title: projects
permalink: /projects/
description: Research papers
nav: true
nav_order: 3
---

{% assign research_projects = site.projects | where: "category", "research" | sort: "importance" %}
<div class="projects">
  {% for project in research_projects %}
    {% include projects_horizontal.liquid %}
  {% endfor %}
</div>
