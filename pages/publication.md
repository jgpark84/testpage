---
title: Publications
description: Publication list
background: /assets/theme/images/banne.jpg
permalink: /newpaper/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ paper.url }}">{{ paper.title }}</a>
    </li>
  {% endfor %}
</ul>
