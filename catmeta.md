---
layout: subpage
permalink: /catmeta
category: Cataloging/Metadata
---

{% for project in site.projects %}
{% if project.category == page.category %}
### {{ project.title }}
{{ project.content }}
{% endif %}
{% endfor %}