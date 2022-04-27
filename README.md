&nbsp;

<h1 align="center"><a href="https://nikahmadz.github.io/central">Central</a></h1>
<p align="center">Theme for GitHub Pages</p>

&nbsp;

***

**Central** helps you build websites on **GitHub**.
You can write your content in Markdown, HTML and Liquid using any code editor you like.
When you commit to your repository, **GitHub Pages** will build your website from the content of your repository files.

***

## Demo

**[Base](//nikahmadz.github.io/central/demo/base)**
**[Prime](//nikahmadz.github.io/central/demo/prime)**
**[Primer](//nikahmadz.github.io/central/demo/primer)**

## Getting started

Setup these files in your repository.
Then, [activate **GitHub Pages**](#activating-github-pages) to publish your website.

- `_config.yml`
  ```yml
  remote_theme: nikahmadz/central
  ```

- `index.md`
  ```markdown
  {% include hero/1.html %}
  ```

- `404.md`
  ```markdown
  {% include 404.md %}
  ```

## Activating GitHub Pages

1. Go to **GitHub Pages Settings** of your repository:
    `//github.com/<user-name>/<repo-name>/settings/pages`
2. Scroll down to the **Source** section.
3. Choose the source of your website files and hit **Save**.  eg: `main/(root)`

- Your app will be accessible at `//<user-name>.github.io/<repo-name>`.


## Writing content

**[GitHub Pages][]** uses [Jekyyll][jekyllrb.com] to build your website from the content of your repository files.
You can write your content in Markdown, HTML and Liquid using any code editor you like.
Check out these articles to familiarize your self on the basics :

- [GitHub Pages documentation][]
- [Markdown syntax][].
- Jekyll docs on [front-matter][], [writing posts][], and [creating pages][].
- [Liquid syntax][]

[GitHub Pages]: https://pages.github.com/
[GitHub Pages documentation]: https://docs.github.com/en/pages
[Markdown syntax]: https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
[jekyllrb.com]: https://jekyllrb.com/
[front-matter]: https://jekyllrb.com/docs/frontmatter/
[writing posts]: https://jekyllrb.com/docs/posts/
[creating pages]: https://jekyllrb.com/docs/pages/
[Liquid syntax]: https://shopify.github.io/liquid/


> `example-page.md`

```markdown
---
title: "Page title"
description: "Short description on the article."
permalink: # (optional: permalink)
layout: # layout-name
theme: # theme-name
---
<style>/* define custom style using html syntax */</style>

# Header 1
## Header 2
### Header 3

Write paragraph using Markdown syntax.  
Write in **Bold** and _Italic_ and `Code` text.

Apply custom styles using Liquid
{: .with-classes }

<div class="use-built-in-classes">With HTML syntax</div>

> Blockquote

- Bulleted
- List

1. Numbered
2. List

[Link](url)
[Footnote][^ref]
![Image](src)

{% if page.matter %}add logics{% endif %}

include ready-made-blocks like:
{% include edit.html %}


```

> More examples can be found in the [docs][] folder.

[docs]: https://github.com/nikahmadz/central/tree/main/docs

## Getting help

Having trouble with **GitHub Pages** ?  
Lets [discuss][] about it,
or [contact support][] to sort it out.

[discuss]: https://github.com/nikahmadz/central/discussions "Lets discuss about this project"
[contact support]: https://support.github.com/contact

## Sponsor

❤️ If you use this work and liked it, **please consider [supporting development][pay]**.

[pay]: https://nikahmadz.github.io/#!pay "See payment options"

## License

[MIT][] licensed - [nikahmadz][]

[MIT]: https://github.com/nikahmadz/central/blob/main/LICENSE "View license"
[nikahmadz]: https://nikahmadz.github.io "Visit my website"
