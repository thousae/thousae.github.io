---
layout: page
title: Research
permalink: /research/
page_class: research-page
---

<p class="research-intro">I study efficient AI systems for foundation models and embodied agents, focusing on inference, memory, and computation reuse.</p>

<section class="research-section" aria-labelledby="research-areas-title">
  <h2 id="research-areas-title">Research areas</h2>
  <ul class="research-area-list">
    {% for area in site.data.research %}
    <li>
      <h3>{{ area.name | escape }}</h3>
      <ul class="research-points">
        {% for point in area.points %}
        <li>{{ point | escape }}</li>
        {% endfor %}
      </ul>
    </li>
    {% endfor %}
  </ul>
</section>

<section class="research-section" aria-labelledby="projects-title">
  <h2 id="projects-title">Projects</h2>
  <ul class="research-project-list">
    {% for project in site.data.projects %}
    <li class="research-project" id="{{ project.id | escape }}">
      <p class="project-period">{{ project.period | escape }}</p>
      <div class="project-details">
        <h3>{{ project.title | escape }}</h3>
        <p class="project-role">{{ project.role | escape }}</p>
        <p class="project-organization">{{ project.organization | escape }}</p>
        <ul class="research-points">
          {% for point in project.points %}
          <li>{{ point | escape }}</li>
          {% endfor %}
        </ul>
        {% if project.code %}<p class="project-links"><a href="{{ project.code | escape }}" target="_blank" rel="noopener">Code</a></p>{% endif %}
      </div>
    </li>
    {% endfor %}
  </ul>
</section>

<section class="research-section research-publications" aria-labelledby="research-publications-title">
  <h2 id="research-publications-title">Publications</h2>
  <p>Full titles, author lists, venues, and paper links are available in the <a href="{{ '/publications/' | relative_url }}">publication list</a>.</p>
</section>
