---
layout: subpage
permalink: /digital-design
category: Web/Tool Design
---

{% for project in site.projects %}
{% if project.category == page.category %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}