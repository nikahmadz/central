---
title: "Test Page"
permalink: test
categories:
---

# {{ page.title }}

{% assign none = false %}
{% assign list = "John,Paul,George,Ringo" | split: "," %}

```yml
{{ none }}
{{ list }}
{% for v in "source,destination,safe" | split: "," -%}
{{ v }}: {{ site[v] }}
{% endfor %}

```

<div style="margin-top:4rem"></div>

***

{% include back.html %}
