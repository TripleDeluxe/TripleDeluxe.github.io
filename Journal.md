---
layout: default
title: Journal de bord
permalink: /Journal/
---
<h1>Journal de bord</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{post.dateString}} : {{ post.title }}</a>
    </li>
  {% endfor %}
</ul>