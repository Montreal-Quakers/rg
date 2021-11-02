---
title: "Photos from the Contemplative Walk: Regional Gathering 2021"
lang: en
author: Regional Gathering clerk
tag: [photos,gathering,2021]
type: system_grid
---
_And into the forest I go, to lose my mind and find my soul_

Thanks for another fabulous regional gathering. See the [resources](#resources) and [photos](#photos)!

### Resources
[The complex futures of blended meetings for worship by Rhiannon Grant](https://brigidfoxandbuddha.wordpress.com/2021/10/16/the-complex-futures-of-blended-meetings-for-worship/?fbclid=IwAR36A3GN2AGnYx0dP10mDdJmNTKY5qqfw_cBATzLBo0KQI3vlX3-ml5RlFo)

### Photos<span class="stanchor"><a name="photos"> </a></span>
<div class="gallery"><ul class="gallery__list">
{% for image in site.static_files %}
    {% assign folder = '/assets/images/RG2021_10/' %}
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
