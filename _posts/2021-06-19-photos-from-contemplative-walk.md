---
title: "Photos from the Contemplative Walk: Regional Gathering 2021"
lang: en
author: Regional Gathering Admin
tag: [photos,gathering,2021]
type: system_grid
---
The readings from today's gathering will be posted here. During the gathering, a resource sheet was kept for [information and speakers relating to water and rivers](https://docs.google.com/document/d/1cwJ-to0Oj8m_MNR1fJoQzig-jb78U0LOjVOXZUbsmLk/edit#){: rel="noopener" target="_blank"}. Below that, the [photos](#photos)!

### Photos<span class="stanchor"><a name="photos"> </a></span>
<div class="gallery"><ul class="gallery__list">
{% for image in site.static_files %}
    {% assign folder = '/assets/images/RG2021/' %}
    {% if image.path contains folder  %}
{% unless image.extname == ".webp" %}{% assign ext = image.extname | remove: "." %}
{% assign word = image.basename.size | minus: 1 %}{% assign basecaption = image.basename | truncate: word, "" | split: " " %}
  {% capture caption %}{% for word in basecaption %}{{ word | capitalize }} {% endfor %}{% endcapture %}
 <li>
   <figure>
     <picture>
       <source srcset="{{ folder }}{{ image.basename }}.webp" type="image/webp"> 
       <source srcset="{{ folder }}{{ image.basename }}.{{ ext }}" type="image/{{ ext }}">
       <img src="{{ folder }}{{ image.basename }}.webp" alt="{{ image.basename }}">
     </picture>
     <figcaption>{{ caption }}</figcaption>
   </figure>
</li>
  {% endunless %}
  {% endif %}
{% endfor %}
</ul></div>
