---
layout: page
title: Малюнки
permalink: /drawings/
---

{% assign posts = site.tags.drawings %}

{% if posts %}
  {% for post in posts %}
    <div class="post">
      <h1 class="post-title">
        <a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
      </h1>

      <span class="post-date">{{ post.date | date: "%d.%m.%Y" }}</span>

      {{ post.excerpt }}
    </div>
  {% endfor %}
{% else %}
  <p>Поки що тут немає дописів.</p>
{% endif %}