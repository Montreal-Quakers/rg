---
layout: default
title: <i class="far fa-newspaper"></i> &nbsp; Regional Gathering
hovertitle: The Latest Updates
lang: en
trans: index
permalink: /index.html
---
### The latest news

<ul>
{% assign posty=site.posts | where:"lang","en" %}
  {% for post in posty %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} -- posted {{ post.date | date: "%B %-d, %Y" }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
