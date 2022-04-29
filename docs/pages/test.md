---
title: "Test Page"
permalink: test
categories:
---

# {{ page.title }}

{% assign none = false %}
{% assign list = [
'a'
] %}

```yml
{{ none }}
{{ list }}
{% for v in [
'source',
'destination',
'safe'
] -%}
{{ v }}
{% endfor %}
source: {{ site.source }}
destination: {{ site.destination }}
safe: {{ site.safe }}
disable_disk_cache: {{ site.disable_disk_cache }}
ignore_theme_config: {{ site.ignore_theme_config }}
exclude: {{ site.exclude }}
include: {{ site.include }}
keep_files: {{ site.keep_files }}
```

<div style="margin-top:4rem"></div>

***

{% include back.html %}
