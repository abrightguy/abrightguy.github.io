---
layout: default
---
{% assign pages = site.pages | sort:"partfile" %}
{% for page in pages %}
  {% if page.edition == "current" and page.type == "index" %}
  <h1><a href="{{ page.url }}">{{ page.description }}</a></h1>
  {% endif %}
{% endfor %}