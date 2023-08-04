---
layout: default
title: En español
---

<h1>Últimas entradas</h1>

<ul>
  {% for post in site.posts %}
  	{% if post.blog == "En_espaniol" %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <!-- {{ post.excerpt }} -->
    </li>
    {% endif %}
  {% endfor %}
</ul>
