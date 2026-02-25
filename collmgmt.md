---
layout: subpage
permalink: /collmgmt
category: Collection Management
---

{% for project in site.projects %}
{% if category=Collection Management %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}