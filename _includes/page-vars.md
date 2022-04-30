###### page

```yml
{% for v in page -%}
{%- if v[0]!='content' and v[0]!='excerpt' -%}
{{ v[0] }}: {{ v[1] }}
{% endif %}{% endfor %}
content:
  size: {{ page.content.size | default:0 }}

excerpt:
  size: {{ page.excerpt.size | default:0 }}

tags: {{ page.tags | jsonify }}

published: {{ page.published }} # false # if you don't want to generate the post

```
