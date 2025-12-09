---
layout: default
title: All Posts
permalink: /posts/
---

<div style="max-width: 700px; margin: 0 auto;">

# All Posts

<ul>
{% for post in site.posts %}
  <li style="margin-bottom: 10px;">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> – {{ post.date | date: "%B %d, %Y" }}</small>
  </li>
{% endfor %}
</ul>

</div>
