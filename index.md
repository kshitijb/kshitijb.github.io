---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Home
header_order: 1
skill_tags: [Product Management, Project Management, Design Thinking, Product Strategy, Analytics, System Design, Technical Communication, Innovation, New Product Development, Business Process, User Experience, User Interface, User Research, User Testing, Fullstack Development]
---
<div class="cv-highlight cv-block" markdown="block">
  {% for highlight in site.data.cv_highlights %}
  - {{highlight}}
  {% endfor %}
</div>

{% for experience in site.data.cv_experiences %}
<div class="cv-experience cv-block">
  <div class="cv-heading caret">
    {% if experience.heading_link != "" %}
    <a href="{{experience.heading_link}}" target="_blank_">{{experience.heading}}</a>
    {% else %}
    <div>{{experience.heading}}</div>
    {% endif %}
  </div>
  <div>
    <span class="cv-role">{{experience.role}}</span>
     | <span class="cv-duration">{{experience.duration}}</span>
  </div>
  <div class="cv-summary">
    {{experience.summary}}
  </div>
  {% if experience.points.size > 0 %}
  <ul>
    {% for point in experience.points %}
    <li>{{point}}</li>
    {% endfor %}
  </ul>
  {% endif %}
</div>
{% endfor %}

{% for other in site.data.cv_others%}
<div class="cv-other cv-block">
  <div class="cv-heading">
  {{other.heading}}
  </div>
  <ul>
    {% for point in other.points%}
    <li>
      {% if point.url != "" %}
      <div class="caret"><a href="{{point.url}}" target="_blank_">{{point.name}}</a></div>
      {% else %}
      <div>{{point.name}}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endfor %}

<span class="cv-heading">**SKILLS**</span>
<div class="skill-container">
{% for skill in page.skill_tags %}
<div class="skill-tag">{{skill}}</div>
{% endfor %}
</div>
