---
title: Education
layout: page
permalink: /education
category: education
---

{% for education in site.education %}
{% if education.category == page.category %}
{{ education.degree }}
{{ education.date }}
{{ education.location }}
{{ education.other }}
{% endif %}
{% endfor %}