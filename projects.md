---
title: Projects
layout: page
permalink: /projects
page_id: projects
---
{% assign sorted_categories = site.data.categories | sort_natural: "category" %}

{% for item in site.data.categories %}
    {% include linked-heading.md %}
{% endfor %}

## <a href="/lis786-project/all-projects">All Projects ⮕</a>