---
title: Education
layout: page
permalink: /education
category: education
---

{% for education in site.education %}
{% if education.category == page.category %}
{{ education.degree }}
{{ education.start-date - education.end-date | date: %B %Y }}
{{ education.location }}
{{ education.other }}
{% endif %}
{% endfor %}