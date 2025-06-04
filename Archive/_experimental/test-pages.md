---
layout: default
---

<h3> Test for unpublished pages</h3>

<ul>
{% assign pages = site.pages %}
	{% for page in pages %}
		<li>{{ page.title }} {{ page.published }}
    {% unless page.published %}
      {{ UNPUBLISHED }} 
    {% endunless %}
    </li>
	{% endfor %}
</ul>
