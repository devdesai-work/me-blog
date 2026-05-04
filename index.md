---
layout: default
title: Home
---
# Hi, I am Devendra.

I made this blog to write my thoughts down. Someone told me this helps organize them..... I dont know.. but lets give it a shot. 

If you stumble across this page by accident, you gotta go touch grass man, but also before that I have got some interesting stuff so check it out.

You can reach me at neeldesai63@gmail.com

[Read all posts →]({{ '/posts/' | relative_url }})

## Recent posts

{% assign recent_posts = site.posts | slice: 0, 5 %}
{% if recent_posts.size > 0 %}
<ul class="post-list">
{% for post in recent_posts %}
  <li>
    <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.excerpt %}
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 120 }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
No posts yet. Add markdown files in `/_posts`.
{% endif %}
