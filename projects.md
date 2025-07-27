---
layout: single
title: "My Projects"
permalink: /projects/
author_profile: true
classes: wide
---

Projects relating to tech, psychology, or whatever, that sparked my curiosity.

<hr>

{% for project in site.projects %}

<div class="project-card-single-column">
  {% if project.header.image_path %}
    <a href="{{ project.url | relative_url }}">
      {% if project.header.image_path contains "://" %}
        <img src="{{ project.header.image_path }}" alt="{{ project.header.alt }}" style="display: block; margin-left: auto; margin-right: auto; max-width: 600px; width: auto;">
      {% else %}
        <img src="{{ project.header.image_path | relative_url }}" alt="{{ project.header.alt }}" style="display: block; margin-left: auto; margin-right: auto; max-width: 600px; width: auto;">
      {% endif %}
    </a>
  {% endif %}

  <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
  
  <p>{{ project.excerpt }}</p>
  
  <a href="{{ project.url | relative_url }}" class="btn btn--info">Read More...</a>

</div>
<hr>
{% endfor %}
