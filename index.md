---
layout: page
title: Lankar
tagline: simple is best 
---
{% include JB/setup %}
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
![lengerfulluse](assets/img/plan-9-artwork.png) 
