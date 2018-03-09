---
layout: page
title: Advanced
permalink: /advanced/
---

This page is intended for those students who really are looking for a
challenge, and really are tired of working on little projects. Listed below is
a collection of activities which should help expand your horizons and really
understand the world of Computer Science.

### Tutorials
<ul class="post-list">
  {% for tutorial in site.tutorials %}
    {% if tutorial.difficulty == 'advanced' %}
      <li>
        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
          {% if tutorial.estimate %} <span class="post-meta">Estimated Time: {{ tutorial.estimate }}</span> {% endif %}
          <h3>
            <a class="post-link" href="{{ tutorial.url | relative_url }}">
              {{ tutorial.title | escape }}
            </a>
          </h3>

          {{ tutorial.excerpt }}
      </li>
    {% endif %}
  {% endfor %}
</ul>

