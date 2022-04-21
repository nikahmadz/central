&nbsp;

<h1 align="center"><a href="https://nikahmadz.github.io/central">Central</a></h1>
<p align="center">Theme for GitHub Pages</p>

&nbsp;

***

**Central** helps you build websites on **GitHub**.
You can write your content using any code editor you like.
When you commit your code to your repository, **GitHub Pages** will build your website from the content of your files.

***

## Usage

Set these files in your repository.
Then, activate **GitHub Pages** to publish your website.

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

**[GitHub Pages][]** uses [Jekyyll][jekyllrb.com] to build your website from the content of your files.
You can write in Markdown and HTML using any code editor you like.
Check out these articles to familiarize your self on the basics:
- [Official documentation][] of GitHub Pages
- [Basic writing and formatting syntax][basics].
- Jekyll docs on [front-matter][], [writing posts][], and [creating pages][].

[GitHub Pages]: https://pages.github.com/
[Official documentation]: https://docs.github.com/en/pages "GitHub Pages Documentation"
[basics]: https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
[jekyllrb.com]: https://jekyllrb.com/
[front-matter]: https://jekyllrb.com/docs/frontmatter/ "Read more"
[writing posts]: https://jekyllrb.com/docs/posts/
[creating pages]: https://jekyllrb.com/docs/pages/

###### `example-page.md`
```markdown
---
title: "Page title"
description: "Short description on the article."
permalink: # (optional: permalink)
layout: # layout-name
theme: # theme-name
---
<style>/* defining custom style using html syntax */</style>

# Header 1
## Header 2
### Header 3

A paragraph using Markdown syntax.  
**Bold** and _Italic_ and `Code` text

> Blockquote

- Bulleted
- List

1. Numbered
2. List

[Link](url)
[Footnote][^ref]
![Image](src)

{% include ready-made-blocks.html %}


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
