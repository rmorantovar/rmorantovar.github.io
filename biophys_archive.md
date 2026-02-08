---
layout: default
title: Biophysics Archive
permalink: /biophys_archive/
order: 3
---

# Paper Summaries

{% assign sorted = site.biophys_archive | sort_natural: "year" %}

<ul>
  {% for p in sorted %}
    <li>
      <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      {% if p.authors %} — {{ p.authors }}{% endif %},
      {% if p.journal %} {{ p.journal }}{% endif %},
      {% if p.year %} {{ p.year }}{% endif %}
    </li>
  {% endfor %}
</ul>
