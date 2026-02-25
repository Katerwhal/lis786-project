---
layout: subpage
permalink: /collmgmt
category: Collection Management
---

{% for project in site.projects %}
{% if category=page.category %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}