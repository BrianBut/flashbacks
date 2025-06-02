---
layout: default
---

<div class="w3-container">
    <h1><b>pagesTest</b></h1>
    
    <!-- Find any page without a title -->
    <ul class="w3-ul w3-hoverable">
    {% for page in site.pages %}
    <li class="w3-large">
    	<a href="{{ page.url }}">{{ page.url }}</a>
    	{% unless page.title %}
    	   <h2>Missing page.title</h2>
    	{% endunless %}	
    	{% unless page.eventDate %}
    	   <h2>Missing page.eventDate</h2>
    	{% endunless %}	
    	{% unless page.category %}
    	   <h2>Missing page.category</h2>
    	{% endunless %}	
    	{% unless page.published %}
    	   <h2>Missing page.published</h2>
    	{% endunless %}	
    </li>
    {% else %}
    <h2>No Pages</h3>
    {% endfor %}
    </ul>
    
</div>
