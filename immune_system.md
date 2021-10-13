---
layout: default_IS
title: Immune System
---
<h1>Quantitative Immunology for Physicist</h1>

<center>
{% include youtube.html id='lXfEK8G8CUI' %}
</center>

<ul>
  {% for post in site.posts reversed%}
  	{% if post.blog == "IS" %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
    {% endif %}
  {% endfor %}
</ul>
