---
layout: page
title: 
tagline: 
---
#### The Goal of Life ####
	The goal of life is to make your heartbeat match the beat of the universe, to match your nature with Nature.  
	                                                                              --- Joseph Campbell  
#### Rules for Happiness ####
	Something to do; Someone to love; Something to hope for.  
																		                                       --- Immanuel Kant
{% include JB/setup %}
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
