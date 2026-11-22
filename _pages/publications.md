---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<p class="page__lede" markdown="0">
  Papers on coherent accelerator integration, RISC-V silicon, and large-scale RTL simulation.
  The full, up-to-date list is on
  <a href="{{ site.author.googlescholar }}">Google Scholar</a>.
</p>

{% assign pubs_by_year = site.publications | sort: "date" | reverse | group_by_exp: "p", "p.date | date: '%Y'" %}
{% for year in pubs_by_year %}
<h2 class="pub-year">{{ year.name }}</h2>
<ul class="pub-list" markdown="0">
  {% for post in year.items %}
  <li class="pub{% if post.role %} pub--lead{% endif %}">
    <p class="pub__title"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></p>
    <p class="pub__meta">
      {% if post.role %}<span class="pub-badge">{{ post.role }}</span>{% endif %}
      <span class="pub__venue">{{ post.venue }}</span>
      {% if post.paperurl %} · <a href="{{ post.paperurl }}">Paper <i class="fas fa-external-link-alt" aria-hidden="true"></i></a>{% endif %}
    </p>
    {% if post.excerpt %}<p class="pub__desc">{{ post.excerpt | strip_html | strip }}</p>{% endif %}
  </li>
  {% endfor %}
</ul>
{% endfor %}
