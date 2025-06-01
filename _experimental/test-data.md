---
layout: default
---

{% comment %}
List unspecified birds diagnostic
{% endcomment %}
{% for bird in site.birdsofDB %}
  {{ bird.title }}
  {% unless bird.genus %}
    <h3>Missing genus from "{{ bird.title }}"</h3>
  {% endunless %}   
{% endfor %}


