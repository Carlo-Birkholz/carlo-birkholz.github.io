## Teaching

{% for item in site.data.teaching.main %}
- **{{ item.course }}** — {{ item.periods | join: ", " }}
{% endfor %}
