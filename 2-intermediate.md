---
layout: page
title: Intermediate
permalink: /intermediate/
---

This page is intended for those students who have completed the "Beginners"
page, and already know what they are doing. Listed below is a collection of
activities to help you build your skills- the best way to learn code is by
coding!

### Tutorials
<ul class="post-list">
  {% for tutorial in site.tutorials %}
    {% if tutorial.difficulty == 'intermediate' %}
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

