---
type: index
layout: default
---

<div class="part-header">
  <h1><a href="part021.pdf">{{ page.description }} Volume 1 (pdf)</a></h1>
</div>

{% assign pages = site.pages | where:"volume","Volume 1" %}
{% for page in pages %}
  {% if page.edition == "current" %}
  <h2><a href="{{ page.url }}">{{ page.chapter }}</a></h2>
  {% endif %}
{% endfor %}

<div class="part-header">
  <h1><a href="part022.pdf">{{ page.description }} Volume 2 (pdf)</a></h1>
</div>

{% assign pages = site.pages | where:"volume","Volume 2" %}
{% for page in pages %}
  {% if page.edition == "current" %}
  <h2><a href="{{ page.url }}">{{ page.chapter }}</a></h2>
  {% endif %}
{% endfor %}

