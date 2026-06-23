---
layout: page
title: research projects
permalink: /projects/
description: this is a list of my ongoing research projects
---

{% assign sorted_projects = site.projects | sort: "importance" %}
<div class="projects-grid">
  {% for project in sorted_projects %}
    <div class="project-card">
      {% if project.img %}
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.img | relative_url }}" alt="{{ project.title }}">
        </a>
      {% endif %}
      <div class="card-body">
        <h3 class="card-title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
        <p class="card-text">{{ project.description }}</p>
      </div>
    </div>
  {% endfor %}
</div>
