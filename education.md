---
title: Education
layout: page
permalink: /education
---

{% for education in site.education %}
{{ page.degree }}
{{ page.date }}
{{ page.location }}
{{ page.other }}
{% endfor %}