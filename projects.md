---
layout: single
title: "My Projects"
permalink: /projects/
author_profile: true
classes: wide
---

Projects relating to tech, psychology, or whatever, that sparked my curiosity.

---

{% for project in site.projects %}
<div class="project-card">
  {% if project.header.image_path %}
    <a href="{{ project.url | relative_url }}">
      
      {% comment %}<!-- This is the new, smart logic -->{% endcomment %}
      {% if project.header.image_path contains "://" %}
        <img src="{{ project.header.image_path }}" alt="{{ project.header.alt }}">
      {% else %}
        <img src="{{ project.header.image_path | relative_url }}" alt="{{ project.header.alt }}">
      {% endif %}

    </a>
  {% endif %}
  <div class="project-content">
    <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
    <p>{{ project.excerpt }}</p>
    <a href="{{ project.url | relative_url }}" class="btn btn--info">Read More...</a>
  </div>
</div>
<hr>
{% endfor %}
