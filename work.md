---
title: Work
layout: page
permalink: /work
category: work
skills: [ Oral and written communication, User centered design, Inclusive teaching and learning strategies, Research support, Mentoring and teamwork, Leadership ]
competencies: [ LIS standards and ethics, Universal Design for Learning principles, ACRL Information Literacy frameworks, Metadata and archival description, Web design (HTML CSS PowerApps), Google and Microsoft office suites, Past Perfect ]
---


Materials worked with: {% for material in site.data.skills.materials %}
{{ material | join: ", " }}
{% endfor %}

{% include work.md %}