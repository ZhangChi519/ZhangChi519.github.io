---
title: Publications
permalink: /en/publications/
---

## Selected Publications

{% for publication in site.publications reversed %}
{{ publication.bibtex }}
{: .notice--info }
{% endfor %}