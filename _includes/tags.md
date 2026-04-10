{% if page.tags.size > 0 %}
  Tag{% if page.tags.size > 1 %}s{% endif %}:
  {{ page.tags | sort | join: ", " }}
{% endif %}
{% if page.skills.size > 0 %}
Skill{% if page.skills.size >1 %}s{% endif %}:
{{ page.skills | sort | join: ", " }}
{% endif %}
{% if page.competencies.size > 0 %}
Competenc{% if page.competencies.size == 1 %}y{% endif %}{% if page.competencies.size > 1 %}ies{% endif %}:
{{ page.competencies | sort | join: ", " }}
{% endif %}
    