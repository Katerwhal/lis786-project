{% for project in site.projects %}
### [{{ project.title }}]({{ project.permalink | relative_url }}) ⮕
{% include tags.md %}
{% endfor %}

<a href="/lis786-project/projects">Back to Projects ⮌</a>