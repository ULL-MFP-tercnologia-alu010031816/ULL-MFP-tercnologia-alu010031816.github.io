---
layout: page
title: tareas
permalink: /tareas/
---

{%- for practica in site.tareas %}
  {%- if practica.visible %}
{{ practica.name | slice: 0, 2  }}.  <a href="{{site.baseurl}}{{ practica.url }}">Práctica {{ practica.name }}</a>
  {%- endif %}
{%- endfor %}

