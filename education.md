---
title: Education
layout: page
permalink: /education
category: education
---

{% for education in site.education %}
{% if education.category == page.category %}
## {{ education.degree }}
### {{ education.location }}
{{ education.start-date | date: %B %Y }} - {{ education end.date | %B %Y }}
{{ education.other }}
{% endif %}
{% endfor %}