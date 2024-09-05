---
title: Publications
description: Publication list
background: /assets/theme/images/banne.jpg
permalink: /publication/
---

<ul>
  {% for post in site.paper %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
