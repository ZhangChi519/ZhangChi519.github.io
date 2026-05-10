---
title: News
permalink: /en/news/
---

## Latest News

<ul>
  {% for post in site.posts %}
    <li>
      <strong>{{ post.date | date: "%Y-%m-%d" }}</strong> — {{ post.content | truncate: 200 }}
    </li>
  {% endfor %}
</ul>