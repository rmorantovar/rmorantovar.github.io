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

<br>
<br>
<nav>
  <div style = "text-align: justify; max-width: 1000px; margin: 0 auto;">

  {% for item in site.data.teaching %}
    <a href="{{ item.link }}" {% if page.url == item.link %} class="current"{% endif %} > <h1>{{ item.name }}</h1></a> &nbsp;
  {% endfor %}
</div>
</nav>

  </body>
</html>