###### page

```yml
{% for v in page %}{% if v[0]!='content' -%}
{{ v[0] }}: {{ v[1] }}
{% endif %}{% endfor %}
content:
  size: {{ page.content.size | default:0 }}

```
