---
layout: page
title: Archive
permalink: /archive/
---

  
{% for post in site.posts %}
<div class="list-group">
    <a href="{{ site.baseurl }}/{{ post.permalink }}" class="list-group-item" style="border: none;">
      <h4 class="list-group-item-heading">{{ post.title }}</h4>
      <p class="list-group-item-text">{{ post.content | strip_html | truncatewords:75}}</p>
    </a>
</div>
{% endfor %}