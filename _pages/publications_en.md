---
title: Publications
permalink: /en/publications/
---

## Selected Publications

<ol class="paper-list">
{% assign publications = site.publications | sort: "year" | reverse %}
{% for publication in publications %}
  <li>
    {{ publication.paperauthors }}.
    "<a href="{{ publication.url | relative_url }}">{{ publication.title }}</a>."
    <em>{{ publication.venue }}</em>, {{ publication.year }}.
    {% assign publication_note = publication.note_en | default: publication.note %}
    {% if publication_note %}<span class="venue-tag">{{ publication_note }}</span>{% endif %}
  </li>
{% endfor %}
</ol>