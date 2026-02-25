---
layout: subpage
permalink: /essays
category: Essays
---

{% for project in site.projects %}
{% if project.category == page.category %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}