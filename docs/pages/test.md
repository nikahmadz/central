---
title: "Test Page"
permalink: test
categories:
---

# {{ page.title }}

{% assign none = false %}
{% assign list = "source,destination,safe" | split: "," %}

```yml
{{ none }}
{{ list | array_to_sentence_string }}
{% for v in list -%}
{{ v }}: {{ site[v] }}
{% endfor %}

```

<div style="margin-top:4rem"></div>

***

{% include back.html %}
