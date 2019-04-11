---
title: Stories of the Ar'sho
navtext: Stories
description: Read the stories of the Ar'sho enclaves, seperatists of the Tau Empire. Backstories are published here, books are coming! Based in the Warhammer 40,000 universe.
permalink: /stories/index.html
---

<h1>Stories <span>of the</span> Ar'sho Enclave</h1>

These are the stories behind the Ar'sho Enclave. Learn the history of the characters and whet your appetite for the greatest tale ever told about the young Tau race.*  
<small>*author's personal opinion.</small>

A series of novel-length stories are in the works for this separatist Tau enclave. While they are under development, the backstories of various characters will be published and updated here from time to time. We will post for our social media followers when new stories appear here, so subscribe to your favorite work distraction below for regular updates! 

**None of this is canon** (*yet...*), so take it for what it is - fanfiction. 

Really.  
Magnificent.  
Fanfiction.

{% assign category = '' %}
{% for item in site.stories %}
  {% assign splitted = item.relative_path  | split: "/" %}
  {% if category != splitted[1] %}
    {% unless category contains ".md" %}
      {% assign category = splitted[1] %}
      {% unless category contains ".md" %}
<h2>{{category}}</h2>
      {% endunless %}
    {% endunless %}
  {% endif %}
<h4><a href="{{ item.url }}">{% if item.navtext %}{{item.navtext}}{% else %}{{item.title}}{% endif %}</a></h4>
<p>{{item.description}}</p>
{% endfor %}
