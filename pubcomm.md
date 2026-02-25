---
layout: subpage
permalink: /pubcomm
category: Public Communication
---

{% for project in site.projects %}
{% if project.category == page.category %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}