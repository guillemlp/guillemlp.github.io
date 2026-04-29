---
permalink: /research/
title: "Research"
excerpt: "Selected research projects"
author_profile: true
layout: archive
published: false   # under review; not built into the live site yet
---

<p class="page__lede" markdown="0">
  My research sits at the intersection of <strong>computer architecture</strong>,
  <strong>simulation infrastructure</strong>, and <strong>hyperscale data movement</strong>.
  Most of it is open-source. Each project below has its own page with the problem statement,
  approach, key results, paper, and code.
</p>

<ul class="cards" markdown="0">
{% assign sorted = site.research | sort: "order" %}
{% for project in sorted %}
  <li class="card">
    {% if project.tag %}<span class="card__tag">{{ project.tag }}</span>{% endif %}
    <h3 class="card__title"><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    {% if project.tagline %}<p class="card__desc">{{ project.tagline }}</p>{% endif %}
    <p class="card__meta">
      {% if project.role %}{{ project.role }}{% endif %}
      {% if project.role and project.collaborators_short %} · {% endif %}
      {% if project.collaborators_short %}{{ project.collaborators_short }}{% endif %}
    </p>
  </li>
{% endfor %}
</ul>
