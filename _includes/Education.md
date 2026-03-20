{% for education in site.education %}
{{ education.degree }}
{{ education.date }}
{{ education.location }}
{{ education.other }}
{% endfor %}