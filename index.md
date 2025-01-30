---
layout: default
title: "Blog para Robótica de Baldo"
---

# 📌 Últimos Posts

<ul>
  {% for post in paginator.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%d %b %Y" }}
    </li>
  {% endfor %}
</ul>

{% if paginator.previous_page %}
[⬅️ Anterior]({{ paginator.previous_page_path }})
{% endif %}
{% if paginator.next_page %}
[➡️ Siguiente]({{ paginator.next_page_path }})
{% endif %}
