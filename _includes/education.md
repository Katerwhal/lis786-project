{% for education in site.education %}
{% if education.category == page.category %}
## <b>{{ education.degree }}</b>
### {{ education.location }}
*{{ education.start-date | date: %B %Y }} - {{ education.end-date | date: %B %Y }}*
{{ education.other }}
{% endif %}
{% endfor %}