<style> .markdown-body .highlight pre{max-height:400px} </style>

###### site

```yml
title: {{ site.title }}
description: {{ site.description }}

theme: {{ site.theme }}
remote_theme: {{ site.remote_theme }}

author: {{ site.author }}
favicon: {{ site.favicon }}
manifest: {{ site.manifest }}
color_scheme: {{ site.color_scheme }}
theme_color: {{ site.theme_color }}
header: {{ site.header }}
cloudflare_analytics: {{ site.cloudflare_analytics }}
google_analytics: {{ site.google_analytics }}

time: {{ site.time }}
timezone: {{ site.timezone }}
encoding: {{ site.encoding }}
url: {{ site.url }}
baseurl: {{ site.baseurl }}
source:      {{ site.source }}
destination: {{ site.destination }}
safe: {{ site.safe }}
disable_disk_cache: {{ site.disable_disk_cache }}
ignore_theme_config: {{ site.ignore_theme_config }}
include: {{ site.include | jsonify }}
exclude: {{ site.exclude | jsonify }}
keep_files: {{ site.keep_files | jsonify }}
plugins_dir: {{ site.plugins_dir | jsonify }}
layouts_dir: {{ site.layouts_dir }}
show_drafts: {{ site.show_drafts }}
future: {{ site.future }}
unpublished: {{ site.unpublished }}
lsi: {{ site.lsi }}
limit_posts: {{ site.limit_posts }}
force_polling: {{ site.force_polling }}
verbose: {{ site.verbose }}
quiet: {{ site.quiet }}
incremental: {{ site.incremental }}
profile: {{ site.profile }}
strict_front_matter: {{ site.strict_front_matter }}

```

###### site.github

```yml
project_title:   {{ site.github.project_title }}
project_tagline: {{ site.github.project_tagline }}
baseurl: {{ site.github.baseurl }}
api_url: {{ site.github.api_url }}
build_revision: {{ site.github.build_revision }}
environment:    {{ site.github.environment }}
hostname:       {{ site.github.hostname }}
pages_env:      {{ site.github.pages_env }}
pages_hostname: {{ site.github.pages_hostname }}
owner_name:     {{ site.github.owner_name }}
owner_url:          {{ site.github.owner_url }}
owner_gravatar_url: {{ site.github.owner_gravatar_url }}
repository_name: {{ site.github.repository_name }}
repository_nwo:  {{ site.github.repository_nwo }}
repository_url:  {{ site.github.repository_url }}
clone_url:       {{ site.github.clone_url }}
issues_url:      {{ site.github.issues_url }}
releases_url:    {{ site.github.releases_url }}
wiki_url:        {{ site.github.wiki_url }}
tar_url:         {{ site.github.tar_url }}
zip_url:         {{ site.github.zip_url }}
url: {{ site.github.url }}
language: {{ site.github.language }}
contributors: {{ site.github.contributors.size | default:0 }}
organization_members: {{ site.github.organization_members }}
private: {{ site.github.private }}
public_repositories: {{ site.github.public_repositories.size | default:0 }}
releases: {{ site.github.releases.size | default:0 }}
show_downloads: {{ site.github.show_downloads }}
source: {{ site.github.source }}

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

###### site.posts

```yml
size: {{ site.posts.size | default:0 }}
{% if site.posts %}{{ site.posts[0] | jsonify }}{% endif %}
```

###### site.pages

```yml
size: {{ site.pages.size | default:0 }}
```

###### site.tags

```yml
size: {{ site.tags.size | default:0 }}
{% if site.tags %}yes{% endif %}
```

###### site.categories

```yml
size: {{ site.categories.size | default:0 }}
```
