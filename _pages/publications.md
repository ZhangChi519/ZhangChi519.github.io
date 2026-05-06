---
title: 发表论文
permalink: /publications/
---

## 代表性论文

{% for publication in site.publications reversed %}
{{ publication.bibtex }}
{: .notice--info }
{% endfor %}
