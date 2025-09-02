---
layout: page
title: Projects
permalink: projects/
---

Things I do, including research, academic course projects, and miscellaneous interests.

<div class="project-spacer-small"></div>

## Research

Research publications for fans of natural language processing, computational social science, and machine learning.

<div class="project-spacer-small"></div>

<div class="l-page project-grid">
    {% for project in site.categories.papers %}
    {% include project.html project=project %}
    {% endfor %}
</div>

<div class="project-spacer"></div>
