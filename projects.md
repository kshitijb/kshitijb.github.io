---
layout: page
title: Projects
permalink: /projects/
header_order: 4
category_order: 
---
<div>
  {% assign groups = site.projects | group_by: "category" %}
  <div class="project-list-container">
    {% for company in site.company-order %}
    {% assign current_company = groups | where: 'name', company | first%}
    <div class='project-category-container'>
      <div class="project-container-heading">{{current_company.name}}</div>
      {% for project in current_company.items %}
        <div class="project-container">
          <a href="{{project.url}}">{{project.title}}</a>
          <div>{{project.excerpt}}</div>
        </div>
      {% endfor %}
    </div>
    {% endfor %}
  </div>
</div>