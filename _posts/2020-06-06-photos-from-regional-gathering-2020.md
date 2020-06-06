---
lang: en
author: Regional Gathering clerk
tag: [photos,gathering]
---
A poem from Caroline, Goshen Friends Meeting June 17, 2018: 

Shadows of my childhood family align along this  
plain meetinghouse bench in Chester County,  
where I have come to worship. Once our row was  
anchored by my strong blue serge-suited Father.  
Now I sit immersed in today’s quiet, seeking Source.  

Long ago I would touch his round stone watch-fob,  
slide it in and out of its shallow stitched vest fold,  
fingering its shape. Was I finding my own place  
among parents, brother, sisters, gathered seekers?  
I felt his still body beside my restless small girl self.    

Where is my Self this Sunday in my seventy-fourth year?  
O Father-Mother Spirit, Abba, Amma, breathe through me.  
My Father’s gold watch chain spanned his chest,  
rose and fell with his breath, that timepiece enclosed  
In a deeper pocket. Was Spirit hidden or within our reach?  

We searched other faces and watched the wall clock,  
brass pendulum swinging, tick-tock tick-tock; then  
I counted thin gray stripes on Daddy’s trouser leg,  
and the firm elders on the solid facing benches.  
Today, I list my blessings, these stirred-up recollections.  

My Mother sat amongst her little ones, another support.  
Her loving arms curled round us; calm hand held mine;  
sometimes she whispered careful counsel. Each  
sibling squirmed yet slowly dropped into the silence  
undergirded every Sunday by familiar, faithful Friends.  

Their deep patient waiting enveloped every one of us.  
Panelled wooden walls framed our souls, and we rested  
in those circles of connection, of parents, other Quakers.  
Seated on stiff horsehair cushions, we all eased into  
some surprising Infinity - and found an hour passed.  

In this later century, watching my inward cycles, I beseech  
You, Spirit of the slow-ticking wall clock, expand my sense  
of Mystery, infuse our aging adult days with timelessness,  
transform my memories of older ones overseeing children,  
reaching into Truth, and let history slip into Presence.  

<div class="gallery"><ul class="gallery__list">
{% for image in site.static_files %}
    {% if image.path contains 'assets/images/RG2020' %}
{% assign word = image.basename.size | minus: 1 %}{% assign caption = image.basename | capitalize | truncate: word, "" %}
 <li><figure><img src="{{ image.path }}" alt="{{ image.basename }}">
<figcaption>{{ caption }}</figcaption></figure></li>
  {% endif %}
{% endfor %}
</ul></div>
