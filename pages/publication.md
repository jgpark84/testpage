---
layout: paperarc
title: Pulications
description: Publication list
permalink: /publication/
---

<ul>
  {% for post in site.paper %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
