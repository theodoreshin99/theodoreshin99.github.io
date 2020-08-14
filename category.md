---
layout: page
title: category
permalink: category
---

{% if site.posts.size == 0 %}
  No post found
{% endif %}
<div>
  {% for eachCategory in site.categories %}
    <ul class="categories">
      {% for categoryName in eachCategory[0] %}
        {% if categoryName != null %}
          <li>
            <span><a href="/categories/{{ categoryName }}">
              CategoryName
              </a></span>
            <span class="count">{{ eachCategory[1].size }}</span>
            
            </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endfor %}
    </div>
         
