{% for work in site.work %}
{% if work.category == page.category %}
## <b>{{ work.job-title }}</b>
### {{ work.employer }} - {{ work.location }}
*{{ work.start-date | date: %B %Y }} - {{ work.end-date | date: %B %Y }}*
{% if work.duties.size > 0 %}
Duties:

{% for duty in work.duties %}
- {{ duty }}
{% endfor %}
{% endif %}
{% endif %}
{% endfor %}