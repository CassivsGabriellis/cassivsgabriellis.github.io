---
layout: page
title: Categorias
---

{% for category in site.categories %}
  <details>
    <summary>{{ category[0] }}</summary>
    <ul class="category-list" data-category="{{ category[0] }}">
      {% for post in category[1] %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </details>
{% endfor %}
