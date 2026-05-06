---
title: 最新动态
permalink: /news/
---

## 最新动态

<ul>
  {% for post in site.posts %}
    <li>
      <strong>{{ post.date | date: "%Y-%m-%d" }}</strong> — {{ post.content | truncate: 200 }}
    </li>
  {% endfor %}
</ul>
