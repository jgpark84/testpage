---
layout: base
title: publication
description: Current GWOTY members
permalink: /publication/
---

<article class="article-page" style="margin-bottom: 40px;">
  <div class="page-content" style="max-width: 800px; margin: 0 auto; padding: 20px;">
    {% if page.img %}
    <div class="page-cover-image" style="text-align: center;">
      <figure>
        <img class="page-image" src="{{ "/assets/img/" | prepend: site.baseurl | append: page.img }}" alt="{{page.title}}" style="width: 100%; height: auto; display: block;">
        {% if page.fig-caption %}
          <figcaption style="font-size: 0.9em; color: #666; text-align: center;">{{page.fig-caption}}</figcaption>
        {% endif %}
      </figure>
    </div> <!-- End Page Cover Image -->
    {% endif %}
    <div class="wrap-content" style="padding: 20px;">
      <header class="header-page" style="margin-bottom: 20px;">
        <h1 class="page-title" style="font-size: 2em; font-weight: bold;">{{page.title}}</h1>
        <div class="page-date" style="font-size: 0.8em; color: #888;"><span>{{page.date | date: '%Y, %b %d'}}&nbsp;&nbsp;&nbsp;&nbsp;</span></div>
      </header>
      <div style="font-size: 1em; line-height: 1.6;">
        {{content | markdownify}}
      </div>
      <div class="page-footer" style="margin-top: 40px;">
        <div class="page-share" style="margin-bottom: 20px;">
          <a href="https://twitter.com/intent/tweet?text={{ page.title }}&url={{ site.url }}{{ page.url }}" title="Share on Twitter" rel="nofollow" target="_blank" style="margin-right: 10px;">Twitter</a>
          <a href="https://facebook.com/sharer.php?u={{ site.url }}{{ page.url }}" title="Share on Facebook" rel="nofollow" target="_blank" style="margin-right: 10px;">Facebook</a>
          <a href="https://plus.google.com/share?url={{ site.url }}{{ page.url }}" title="Share on Google+" rel="nofollow" target="_blank" style="margin-right: 10px;">Google+</a>
        </div>
        <div class="page-tag" style="font-size: 0.8em; color: #555;">
          {% for tag in page.tags %}
            <a href="{{site.baseurl}}/tags#{{tag}}" class="tag" style="margin-right: 5px;">&#35; {{ tag }}</a>
          {% endfor %}
        </div>
      </div>
      {% include disqus.html %}
    </div> <!-- End Wrap Content -->
  </div> <!-- End Page Content -->
</article> <!-- End Article Page -->
