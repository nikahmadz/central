---
title: "Test Page"
permalink: test
categories:
---

# {{ page.title }}

{% assign none = false %}
{% capture senarai %}
source,
destination,
safe
{% endcapture %}
{% assign list = senarai | split: ", " %}

```yml
{{ none }}
{{ list | array_to_sentence_string }}
{{ senarai }}
{% for v in list -%}
{{ v }}: {{ site[v] }}
{% endfor %}

```

<div style="margin-top:4rem"></div>

***

{% include back.html %}
