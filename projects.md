---
layout: page
title: Projects
permalink: /projects/
header_order: 3
---
<div>
  {% assign groups = site.projects | group_by: "category" %}
  <div class="project-list-container">
    {% for group in groups %}
      <div class='project-category-container'>
        <div class="project-container-heading">{{group.name}}</div>
        {% for project in group.items %}
          <div class="project-container">
            <a href="{{project.url}}">{{project.title}}</a>
            <div>{{project.excerpt}}</div>
          </div>
        {% endfor %}
      </div>
    {% endfor %}
  </div>
</div>

PSYCHOLOGY