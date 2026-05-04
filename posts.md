---
layout: default
title: Posts
permalink: /posts/
---
# Posts

{% if site.posts.size > 0 %}
<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.excerpt %}
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
No posts found. Add files to `/_posts` using this naming format:

`YYYY-MM-DD-your-title.md`
{% endif %}
