---
layout: page
title: SH Dev Blog
description: s 
---
{% include JB/setup %}


The blog is the mainly to organize the knowledge about my favorite topics. Tec things like programming and hardware, mathematics or cooking. 

###Here are the latest posts:

<ul class="posts">
  {% for post in site.posts limit:5 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



