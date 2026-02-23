
  {% for item in site.data.navigation %}
## [{{ item.category }}]({{ item.url | relative_url }})
{% endfor %}
{{ include.description }}
