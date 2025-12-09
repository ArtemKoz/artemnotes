---
layout: default
title: Home
---

<div style="max-width: 700px; margin: 0 auto;">

Latest Posts

<ul>
{% for post in site.posts limit:5 %}
  <li style="margin-bottom: 10px;">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> – {{ post.date | date: "%B %d, %Y" }}</small>
  </li>
{% endfor %}
</ul>

<p><a href="/posts/">See all posts →</a></p>

</div>



