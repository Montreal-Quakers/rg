---
layout: default
title: <i class="far fa-newspaper"></i> &nbsp; Regional Gathering
hovertitle: The Latest Updates
lang: en
trans: index
permalink: /index.html
---
### Regional Gathering 2020 will be happening via videoconference!
Here is the [program](/rg2020_program.html) and the [registration form](/rg2020_registration.html).

All the latest news about the [St. Lawrence Regional Quaker Gathering](/rg.html):

<ul>
{% assign posty=site.posts | where:"lang","en" %}
  {% for post in posty %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} -- posted {{ post.date | date: "%B %-d, %Y" }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
