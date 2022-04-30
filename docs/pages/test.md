---
title: "Test Page"
permalink: test
categories:
---

# {{ page.title }}

```yml
{%- assign list = "source,destination" | split:"," -%}
{% for v in list %}{{ v }}: {{ site[v] }}
{% endfor -%}

```

<div style="margin-top:4rem"></div>

***

{% include back.html %}
