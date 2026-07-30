---
title: 发表论文
permalink: /publications/
---

## 代表性论文

<ol class="paper-list">
{% assign publications = site.publications | sort: "year" | reverse %}
{% for publication in publications %}
  <li>
    {{ publication.paperauthors }}.
    "<a href="{{ publication.url | relative_url }}">{{ publication.title }}</a>."
    <em>{{ publication.venue }}</em>, {{ publication.year }}.
    {% if publication.note %}<span class="venue-tag">{{ publication.note }}</span>{% endif %}
  </li>
{% endfor %}
</ol>
