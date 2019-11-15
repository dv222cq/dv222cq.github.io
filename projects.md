---
layout: page
title: Projects
image: /assets/og-david.jpg
permalink: /projects/
---
Appears to be nothing here at this point.
<ul>
  {% for author in site.authors %}
    <li>
      <h2><a href="{{ author.url }}">{{ author.name }}</a></h2>
      <h3>{{ author.position }}</h3>
      <p>{{ author.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>