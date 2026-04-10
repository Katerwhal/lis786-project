{% for w in site.collections.work.docs %}
  <p>{{ w.job-title }}</p>
{% endfor %}

{% assign order = site.data.work-order %}
{% for filename in order %}
  {% assign work = site.collections.work.docs | where_exp: "item", "item.path contains filename" | first %}

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