---
layout: default
---

<div class="w3-container">
    <h1><b>{{ site.title }}</b></h1>
    {% assign sorted = site.pages | sort: 'eventDate' %}
 
  <!-- flashbacks -->
  <ul class="w3-ul w3-hoverable">
    {% for page in sorted %}
        {% if page.title and page.advertise and page.category == "flashback" %}
        <li class="w3-large">
            <a href="{{ page.url }}">{{ page.title }} {{ page.eventDate }}</a>
        </li>
        {% endif %}
    {% endfor %}
    
    <!-- essays -->
    {% for page in sorted %}
    	{{ page.category }}
        {% if page.title and page.advertise and page.category == "essay" %}
        <li class="w3-large">
            <a href="{{ page.url }}">{{ page.title }} {{ page.eventDate }}</a>
        </li>
        {% endif %}
    {% endfor %}
    
    <!-- MITOC -->
    {% for page in sorted %}
    	{{ page.category }} {{ page.title }}
        {% if page.title and page.advertise and page.category == "MITOC" %}
        <li class="w3-large">
            <a href="{{ page.url }}">{{ page.title }} {{ page.eventDate }}</a>
        </li>
        {% endif %}
    {% endfor %}
    
  </ul>

</div>
