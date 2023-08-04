---
layout: default
title: Statistical Physics
---
<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
  	{% if post.blog == "SP" %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
    {% endif %}
  {% endfor %}
</ul>
