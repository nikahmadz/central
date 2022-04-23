<style> .markdown-body .highlight pre{max-height:400px} </style>

```yml
github_edit_link: {{ github_edit_link "Edit this page" }}

```

###### site

```yml
theme: {{ site.theme }}
remote_theme: {{ site.remote_theme }}
title: {{ site.title }}
description: {{ site.description }}
author: {{ site.author }}
favicon: {{ site.favicon }}
manifest: {{ site.manifest }}
time: {{ site.time }}
url: {{ site.url }}
baseurl: {{ site.baseurl }}
color_scheme: {{ site.color_scheme }}
theme_color: {{ site.theme_color }}
cloudflare_analytics: {{ site.cloudflare_analytics }}
google_analytics: {{ site.google_analytics }}
header: {{ site.header }}

```

###### site.github

```yml
{% for v in site.github -%}
{%- if v[0]!='license' and v[0]!='owner' and v[0]!='latest_release' and v[0]!='versions' and v[0]!='sass' -%}
{{ v[0] }}: {{ v[1] }}
{% endif %}{% endfor %}

```

###### site.github.license

```yml
{% for v in site.github.license -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### site.github.owner

```yml
{% for v in site.github.owner -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### site.github.latest_release

{% if site.github.latest_release %}
```yml
{% for v in site.github.latest_release %}{% if v[0]!='author' -%}
{{ v[0] }}: {{ v[1] }}
{% endif %}{% endfor %}
author:
  {% for v in site.github.latest_release.author -%}
  {{ v[0] }}: {{ v[1] }}
  {% endfor %}
```
{% endif %}

###### site.github.versions

```yml
{% for v in site.github.versions -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### site.sass

```yml
{% for v in site.sass -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### layout

```yml
{% for v in layout -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### page

```yml
{% for v in page %}{% if v[0]!='content' -%}
{{ v[0] }}: {{ v[1] }}
{% endif %}{% endfor %}
author:
# content-size: {{ page.content.size | default:0 }}

```
