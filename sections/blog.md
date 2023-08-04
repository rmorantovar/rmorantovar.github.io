---
layout: default
title: Blog
---
<div style = "text-align: justify; max-width: 1000px; margin: 0 auto;">
<br>
<div class="figure" style="text-align: center;">
    <img src="../assets/images/camino.JPG" alt="fig1" style="display: inline-block;">
    <p class="image-caption">Póvoa de Varzim, Portugal. Camino portugués de la costa hacia Santiago de Compostela. 2020</p>
</div>

<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
  	{% if post.blog == "Blog" %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
    {% endif %}
  {% endfor %}
</ul>
