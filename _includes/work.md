{% assign order = site.collections.work.order %}
{% for filename in order %}
  {% assign work = site.work | where: "name", filename | first %}

{% if work.category == page.category %}
## <u>{{ work.job-title }}</u>
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