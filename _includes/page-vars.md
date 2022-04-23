###### page

```yml
{% for v in page %}{% if v[0]!='content' -%}
{{ v[0] }}: {{ v[1] }}
{% endif %}{% endfor %}
content:
  size: {{ page.content.size | default:0 }}

excerpt:
  size: {{ page.excerpt.size | default:0 }}

tags: {{ page.tags }}

published: # false # if you don't want to generate the post

```
