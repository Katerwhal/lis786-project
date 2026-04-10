---
title: Work
layout: page
permalink: /work
category: work
---
{% for item in site.data.skills %}
Skills:{{ skill | sort | join: ", " }}
Competencies:{{ competency | sort | join: ", " }}
{% endfor %}

{% include work.md %}
