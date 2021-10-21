---
layout: default_IS
title: Immune System
---


<h1>Quantitative Immunology for Physicist</h1>

The course gives an introduction to modern immunology for physicists, with an emphasis on statistical and evolutionary questions. It is arranged as a weekly discussion group on selected topics in quantitative immunology. For each topic, common reading should first introduce each student to the basics of the topic. Then, more advanced topics that are relevant to the chapter are provided and discussed. In the discussion session, we will then go together over the central message of the paper, possible problems and difficulties, and the relevance for our broader understanding of quantitative immunology. The course is centred around reading and self-study: students are expected to have read the selected paper(s) before each discussion. Students are expected to take an active part in the discussion and to have read the selected paper(s) before. Moreover, for each week a new chair is assigned to lead the discussion for a topic discussed the following week. This includes a short summary of the paper, and possible discussion questions.

<ul>
  {% for post in site.posts reversed%}
  	{% if post.blog == "IS" %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <!--{{ post.excerpt }}-->
    </li>
    {% endif %}
  {% endfor %}

  <li><h2>General References</h2>
<ul>
<li> <a href="https://www.sciencedirect.com/science/article/pii/S0370157320300090">Quantitative immunology for physicists, G. Altan-Bonnet, et.al. (2020) </a>
  <li> <a href= "https://www.theatlantic.com/science/archive/2021/10/waning-immunity-not-all-bad/620436/" > The Good Part About ‘Waning’ Immunity. <em>The Atlantic</em>
  </a></li>
  </li>
</ul>
</li>
</ul>
&nbsp;

