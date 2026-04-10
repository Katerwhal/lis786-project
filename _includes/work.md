{% assign order = site.collections.work.order %}

{% for filename in order %}
  <p>{{ filename }}</p>
  {% assign work = site.work | where: "name", filename | first %}
  <p>{{ work }}</p>
{% endfor %}