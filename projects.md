---
layout: page
title: Projects
permalink: /projects/
header_order: 3
---
<div>
  {% for project in site.projects %}
  <div class="project-list-container">
    <a href="{{project.url}}">{{project.title}}</a>
    <div>{{project.excerpt}}</div>
    <div></div>
  </div>
  {% endfor %}
</div>

PSYCHOLOGY