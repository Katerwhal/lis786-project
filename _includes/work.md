{% for work in site.work %}
{% if work.category == page.category %}
## <u>{{ work.job-title }}</u>
### {{ work.employer }}
### {{ work.location }}
*{{ work.start-date | date: %B %Y }} - {{ work.end-date | date: %B %Y }}*
{% if page.duties.size > 0 %}
{% for duty in page.duties %}
Duties:

- {{ duty }}
{% endfor %}
{% endif %}
{% endif %}
{% endfor %}