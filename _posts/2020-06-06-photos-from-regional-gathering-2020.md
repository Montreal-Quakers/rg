---
lang: en
author: Regional Gathering clerk
tag: [photos,gathering]
type: system_grid
---
Three poems, from [Caroline](#caroline), [Rosemarie](#rosemarie), and [Bert](#bert) and then the [photos](#photos).

A poem from Caroline<span class="stanchor"><a name="caroline"> </a></span>, Goshen Friends Meeting June 17, 2018: 

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

A poem from Rosemarie<span class="stanchor"><a name="rosemarie"></a></span>:

#### Pandemic

What if you thought of it  
as the Jews consider the Sabbath—  
the most sacred of times?  
Cease from travel.  
Cease from buying and selling.  
Give up, just for now,  
on trying to make the world  
different than it is.  
Sing. Pray. Touch only those  
to whom you commit your life.  
Center down.  

And when your body has become still,  
reach out with your heart.   
Know that we are connected   
in ways that are terrifying and beautiful.   
(You could hardly deny it now.)   
Know that our lives   
are in one another’s hands.   
(Surely, that has come clear.)   
Do not reach out your hands.   
Reach out your heart.   
Reach out your words.   
Reach out all the tendrils   
of compassion that move, invisibly,   
where we cannot touch.   

Promise this world your love--   
for better or for worse,   
in sickness and in health,   
so long as we all shall live.   

--Lynn Ungar 3/11/20

Bert's poem<span class="stanchor"><a name="bert"></a></span>, by John O’Donohue from his book _To Bless the Space Between Us_

This is the time to be slow,  
Lie low to the wall  
Until the bitter weather passes.  

Try, as best you can, not to let  
The wire brush of doubt  
Scrape from your heart  
All sense of yourself  
And your hesitant light.  

If you remain generous,  
Time will come good;  
And you will find your feet  
Again on fresh pastures of promise,  
Where the air will be kind  
And blushed with beginning.  

### Photos<span class="stanchor"><a name="photos"> </a></span>
<div class="gallery"><ul class="gallery__list">
{% for image in site.static_files %}
    {% if image.path contains 'assets/images/RG2020' %}
{% unless image.extname == ".webp" %}{% assign ext = image.extname | remove: "." %}
{% assign word = image.basename.size | minus: 1 %}{% assign caption = image.basename | capitalize | truncate: word, "" %}
 <li>
   <figure>
     <picture>
       <source srcset="/assets/images/RG2020/{{ image.basename }}.webp" type="image/webp"> 
       <source srcset="{{ image.path }}" type="image/{{ ext }}">
       <img src="/assets/images/RG2020/{{ image.basename }}.webp" alt="{{ image.basename }}">
     </picture>
     <figcaption>{{ caption }}</figcaption>
   </figure>
</li>
  {% endunless %}
  {% endif %}
{% endfor %}
</ul></div>
