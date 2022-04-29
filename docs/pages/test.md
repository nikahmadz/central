---
title: "Test Page"
permalink: test
categories:
---

# {{ page.title }}

{% assign none = false %}
{% assign list = ['a'] %}

```yml
{{ none }}
{{ list }}
{% for v in ['source','destination','safe'] -%}
{{ v }}
{% endfor %}

```

<div style="margin-top:4rem"></div>

***

{% include back.html %}
