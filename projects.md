---
title: Projects
layout: page
permalink: /projects
page_id: projects
---

{% for item in site.data.categories %}
    {% include project.md %}
{% endfor %}

