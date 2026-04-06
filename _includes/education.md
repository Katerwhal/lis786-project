{% for education in site.education %}
{% if education.category == page.category %}
## {{ education.degree }}
##### {{ education.location }}
*{{ education.start-date | date: %B %Y }} - {{ education.end-date | date: %B %Y }}*
{{ education.other }}
{% endif %}
{% endfor %}