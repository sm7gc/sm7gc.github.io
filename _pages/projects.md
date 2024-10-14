---
layout: page
title: projects
nav: projects
permalink: /projects/
description: some of the projects I have worked on
---

<!-- <div class="alert alert-danger" role="alert">
  This part of the site is still under construction.
</div> -->

<div id="projects" class="row mt-2 pt-3" style="overflow: visible !important;">
  {% assign sorted_projects = site.projects | sort: "importance" | reverse %}
  {% for project in sorted_projects %}
    <div class="project-card w-50">
      {% if project.redirect %}
        <a href="{{ project.redirect }}" target="_blank">
      {% else %}
        <a href="{{ project.url | prepend: site.baseurl }}">
      {% endif %}
        <div class="card">
          <img class="card-img-top" src="{{ project.img | prepend: site.baseurl }}" alt="project thumbnail">
          <div class="card-body">
            <h5 class="card-title">{{ project.title }}</h5>
            <p class="card-text">{{ project.description }}</p>
          </div>
        </div>
      </a>
    </div>
  {% endfor %}
</div>

<!-- {% for project in sorted_projects %}
  <div class="row m-0 p-0" style="border-top: 1px solid #ddd;">
    <div class="col-sm-11 p-0">
        <img src="{{ project.img | prepend: site.baseurl }}" alt="project thumbnail">
        {% if project.redirect %}
          <a href="{{ project.redirect }}" target="_blank">
        {% else %}
          <a href="{{ project.url | prepend: site.baseurl }}">
        {% endif %}
        <h5>{{ project.title }}</h5>
        </a>
        <p>{{ project.description }}</p>
    </div>
  </div>
{% endfor %} -->