---
layout: base
title: publication
description: Current GWOTY members
permalink: /publication/
---

<ul>
  {% for post in site.paper %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p><strong>Date:</strong> {{ post.date | date: "%Y-%m-%d" }}</p>
      <p><strong>Description:</strong> {{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
