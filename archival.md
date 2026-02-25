---
layout: subpage
permalink: /archival
category: Archival Work
---

{% for project in site.projects %}
{% if project.category == page.category %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}