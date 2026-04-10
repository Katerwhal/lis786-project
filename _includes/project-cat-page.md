{% for project in site.projects %}
{% if project.category == page.category %}
### [{{ project.title }}]({{ project.permalink | relative_url }}) ⮕
{{ project.description }}
{% endif %}
{% endfor %}

<a href="/lis786-project/projects">Back to Projects ⮌</a>