{% for project in site.projects %}
{% if project.media.size > 0 %}
### [{{ project.title }} ({{ project.category }})]({{ project.permalink | relative_url ⮕ }}) 

{% if project.description.size > 0 %}
  {{ project.description }}
  <br>
  {% endif %}

{% if project.skills.size > 0 %}
  **Skill{% if project.skills.size >1 %}s{% endif %}:**
  {{ project.skills | sort | join: ", " }}
  <br>
  {% endif %}

{% if project.competencies.size > 0 %}
  **Competenc{% if project.competencies.size == 1 %}y{% endif %}{% if project.competencies.size > 1 %}ies{% endif %}:**
  {{ project.competencies | sort | join: ", " }}
  <br>
  {% endif %}

{% endif %}

***

{% endfor %}

<a href="/lis786-project/projects">Back to Project Categories ⮌</a>