---
layout: single
title: "My Projects"
permalink: /projects/
author_profile: true
classes: wide
---

Here are some of the projects I've been developing as I explore the intersection of data, technology, and psychology.

---

{% for project in site.projects %}
  ## {{ project.title }}

  {{ project.excerpt }}

  <a href="{{ project.url | relative_url }}" class="btn btn--info">Read More...</a>
  <hr>
{% endfor %}
