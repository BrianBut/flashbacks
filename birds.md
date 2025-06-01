---
layout: default
---

<a class="w3-button w3-light-green" href="/habitats.html">Habitats</a>
{% assign items_grouped = site.birdsofdb | group_by: 'genus' %}

<div class="w3-container">
  <ul class="w3-ul w3-hoverable">

    {% for group in items_grouped  %}
      <b class="w3-large">{{ group.name }}</b>
      {% assign items = group.items | sort: 'name' %}

      {% for item in items  %}
        <a href="{{ item.url }}"><li class="w3-medium">{{ item.title }}<small> ({{ item.genus }} {{ item.species }})</small></li></a>
      {% endfor %}
    {% endfor %}

  </ul>
</div>
