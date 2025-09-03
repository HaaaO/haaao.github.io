---
layout: page
title: Research Projects
permalink: projects/
---

Research publications on human-centered AI, robotics and Machine Learning,

<div class="project-spacer-small"></div>

<div class="l-page project-grid">
    {% for project in site.categories.papers %}
    {% include project.html project=project %}
    {% endfor %}
</div>

<div class="project-spacer"></div>
