---
layout: default
---

<div class="w3-container">
    <h1><b>{{ site.title }}</b></h1>
    {% assign sorted = site.pages | sort: 'eventDate' %}
 
  <ul class="w3-ul w3-hoverable">
    {% for page in sorted %}
        {% if page.title and page.advertise %}
        <li class="w3-large">
            <a href="{{ page.url }}">{{ page.title }} {{ page.eventDate }}</a>
        </li>
        {% endif %}
    {% endfor %}
  </ul>

</div>
