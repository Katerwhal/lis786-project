{% assign sorted_projects = site.projects | sort_natural: "title" %}

{% for project in site.projects %}
### [{{ project.title }}]({{ project.permalink | relative_url }}) ({{ project.category }}) ⮕

{% if project.tags.size > 0 %}
  Tag{% if project.tags.size > 1 %}s{% endif %}:
  {{ project.tags | sort | join: ", " }}
{% endif %}

{% if project.skills.size > 0 %}
  Skill{% if project.skills.size >1 %}s{% endif %}:
  {{ project.skills | sort | join: ", " }}
  {% endif %}

{% if project.competencies.size > 0 %}
  Competenc{% if project.competencies.size == 1 %}y{% endif %}{% if project.competencies.size > 1 %}ies{% endif %}:
  {{ project.competencies | sort | join: ", " }}
  {% endif %}
{% if project.description.size > 0 %}
  Description: {{ project.description }}
  {% endif %}

***

{% endfor %}

<a href="/lis786-project/projects">Back to Project Categories ⮌</a>