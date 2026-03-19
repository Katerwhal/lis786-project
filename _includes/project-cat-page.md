{% for project in site.projects %}
{% if project.category == page.category %}
### [{{ project.title }}]({{ project.permalink | relative_url }})
{{ project.content }}
{% endif %}
{% endfor %}

