---
layout: default
title: En español
---
<div style = "text-align: justify; max-width: 1000px; margin: 0 auto;">
<br>
<center>
<figure>
<img src= "../assets/images/nevado.jpg" width="500px" height="auto">
<figcaption>Nevado Poleka Kasué, Parque de los nevados, Colombia. 2023
</figcaption>
</figure>
</center>

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
