<style> .markdown-body .highlight pre{max-height:400px} </style>

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
api_url: {{ site.github.api_url }}
baseurl: {{ site.github.baseurl }}
build_revision: {{ site.github.build_revision }}
clone_url: {{ site.github.clone_url }}
contributors: {{ site.github.contributors.size | default:0 }}
environment: {{ site.github.environment }}
hostname: {{ site.github.hostname }}
issues_url: {{ site.github.issues_url }}
language: {{ site.github.language }}
organization_members: {{ site.github.organization_members }}
owner_gravatar_url: {{ site.github.owner_gravatar_url }}
owner_name: {{ site.github.owner_name }}
owner_url: {{ site.github.owner_url }}
pages_env: {{ site.github.pages_env }}
pages_hostname: {{ site.github.pages_hostname }}
private: {{ site.github.private }}
project_title: {{ site.github.project_title }}
project_tagline: {{ site.github.project_tagline }}
public_repositories: {{ site.github.public_repositories.size | default:0 }}
releases: {{ site.github.releases.size | default:0 }}
releases_url: {{ site.github.releases_url }}
repository_name: {{ site.github.repository_name }}
repository_nwo: {{ site.github.repository_nwo }}
repository_url: {{ site.github.repository_url }}
show_downloads: {{ site.github.show_downloads }}
source: {{ site.github.source | default:null }}
url: {{ site.github.url }}
wiki_url: {{ site.github.wiki_url }}
tar_url: {{ site.github.tar_url }}
zip_url: {{ site.github.zip_url }}

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

###### site.posts

```yml
{% for v in site.posts -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
# content:
# excerpt:
# published: false # if you don't want to generate the post
# tags

```

###### site.pages

```yml
{% for v in site.pages -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### site.tags

```yml
{% for v in site.tags -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```

###### site.categories

```yml
{% for v in site.categories -%}
{{ v[0] }}: {{ v[1] }}
{% endfor %}
```
