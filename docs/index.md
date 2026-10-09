---
title: Home
---

{% for p in site.pages %}{% if p.url != page.url and p.path contains '.md' %}
- [{{ p.title | default: p.name }}]({{ p.url | relative_url }})
{% endif %}{% endfor %}
