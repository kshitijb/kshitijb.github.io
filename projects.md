---
layout: page
title: Projects
permalink: /projects/
header_order: 4
---
<div>
  {% assign groups = site.projects | group_by: "category" %}
  <div class="project-list-container">
    {% for company in site.company-order %}
    {% assign current_company = groups | where: 'name', company | first%}
    <div class='project-category-container'>
      {% if current_company.name != 'Flipkart' %}
        <div class="project-container-heading">{{current_company.name}}</div>
      {% endif %}
      {% for project in current_company.items %}
      {% if project.draft != true %}
        <div class="project-container">
          <a href="{{project.url}}">{{project.title}}</a>
          <div>{{project.excerpt}}</div>
        </div>
      {% endif %}
      {% endfor %}
    </div>
    {% endfor %}
  </div>
</div>