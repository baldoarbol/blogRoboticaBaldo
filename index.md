---
layout: default
title: "Blog para Robótica de Baldo"
---

# 📖 Últimos Posts 📖

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%d %b %Y" }}
    </li>
  {% endfor %}
</ul>
