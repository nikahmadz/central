###### page

```yml
title: {{ page.title }}

layout: {{ page.layout }}
theme: {{ page.theme }}

url:           {{ page.url }}
dir:           {{ page.dir }}
name:          {{ page.name }}
path:          {{ page.path }}
relative_path: {{ page.relative_path }}
permalink:     {{ page.permalink }}
date: {{ page.date }}
published: {{ page.published }} # false # if you don't want to generate the post

content:
  size: {{ page.content.size | default:0 }}

output:
  size: {{ page.output.size | default:0 }}

excerpt:
  size: {{ page.excerpt.size | default:0 }}

tags: {{ page.tags | jsonify }}
categories: {{ page.categories }}
category: {{ page.category }}
collection:    {{ page.collection }}

```
