---
layout: default
---

<h3> Test that all birds have genus and species defined </h3>

{% assign birds = site.birdsofDB %}
<ul>
{% for bird in birds %}
  <li>
  {% if bird.title %}
    {{ bird.title }}
  {% endif %}

  {% unless bird.genus %}
    Missing genus
  {% endunless %}

  {% unless bird.species %}
    Missing species
  {% endunless %}

  {% comment %}
  {% unless bird.cat %}
    -> Missing category
  {% endunless %}
  
  {% unless bird.size %}
    Missing size
  {% endunless %} 
 
  {{ bird.title }} : {{ bird.genus }}->{{ bird.species }}
  {% endcomment %}
  </li>

{% endfor %}
</ul>

