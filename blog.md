---
layout: page
title: Posts
image: /assets/og-david.jpg
permalink: /blog/
---
Here you'll find any utterances I find necessary to make — be that externally imposed or internally motivated.
<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>