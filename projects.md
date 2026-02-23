---
title: Projects
layout: page
permalink: /projects
page_id: projects
---

{% for item in site.data.navigation %}
    {% include project.md
        category="Collection Management"
        description="Maintenance, weeding, and discovery." %}
{% endfor %}

{% for item in site.data.navigation %}
    {% include project.md
        category="Cataloging/Metadata"
        description="how I handle data in XML and application profiles." %}
{% endfor %}
    
{% for item in site.data.navigation %}
    {% include project.md
        category="Archival Work"
        description="Projects I've done in archival settings." %}
{% endfor %}

{% for item in site.data.navigation %}
    {% include project.md
        category="Essays"
        description="Longform, scholarly writing in the field of Information Science." %}
{% endfor %}

{% for item in site.data.navigation %}
    {% include project.md
        category="Public Communication"
        description="Presentations and lessons designed for the general public and information professionals." %}
{% endfor %}

{% for item in site.data.navigation %}
    {% include project.md
        category="Web Design"
        description="Web design projects using HTML, CSS, and JS." %}
{% endfor %}