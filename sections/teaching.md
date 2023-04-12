---
layout: default
title: Teaching
---

<html>
  <head>
    <meta charset="utf-8">
    <title>{{ page.title }}</title>
  </head>

<body>

<nav>
  {% for item in site.data.teaching %}
    <a href="{{ item.link }}" {% if page.url == item.link %} class="current"{% endif %} > <h1>{{ item.name }}</h1></a> &nbsp; &nbsp;
  {% endfor %}
</nav>

  </body>
</html>