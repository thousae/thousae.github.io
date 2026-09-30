---
layout: page
title: Research
permalink: /research/
---

My work brings together **robot foundation models, embodied AI, and efficient AI systems**. Continuous observations create repeated computation, growing memory, and latency constraints. I study how models and agents can reuse prior computation while staying consistent with a changing physical world.

## Research areas

{% for area in site.data.research %}
### {{ area.name }}

{{ area.description }}
{% endfor %}

## Projects

{% for project in site.data.projects %}
<article class="research-project" id="{{ project.id }}">
  <div class="project-heading"><h3>{{ project.title }}</h3><p class="project-status">{{ project.status }}</p></div>
  <p><strong>{{ project.question }}</strong></p>
  <p>{{ project.description }}</p>
  <p class="project-keywords">{{ project.keywords }}</p>
  {% if project.paper %}<p><a href="{{ project.paper }}" target="_blank" rel="noopener">Paper</a></p>{% endif %}
</article>
{% endfor %}

## Publications

See the [publication list]({{ '/publications/' | relative_url }}) for full titles, author lists, venues, and paper links.
