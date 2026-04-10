{% if page.tags.size > 0 %}
  <b>Tag{% if page.tags.size > 1 %}s{% endif %}:</b>
  {{ page.tags | sort | join: ", " }}
  <br>
{% endif %}  

{% if page.skills.size > 0 %}
<b>Skill{% if page.skills.size >1 %}s{% endif %}:</b>
{{ page.skills | sort | join: ", " }}
<br>
{% endif %}  

{% if page.competencies.size > 0 %}
<b>Competenc{% if page.competencies.size == 1 %}y{% endif %}{% if page.competencies.size > 1 %}ies{% endif %}:</b>
{{ page.competencies | sort | join: ", " }}
<br>
{% endif %}  
