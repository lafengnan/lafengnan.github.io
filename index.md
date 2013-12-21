---
layout: page
---
{% include JB/setup %}


<ul class="artical-list">
  {% for post in site.posts %}
    <li>
	   <span>{{ post.date | date_to_string }}</span> &raquo; <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
	   <div class="title-desc">{{ post.content}}</div>
	   </li>
  {% endfor %}
</ul>
