&nbsp;

<h1 align="center"><a href="https://nikahmadz.github.io/central">Central</a></h1>
<p align="center">Theme for GitHub Pages</p>

&nbsp;

***

**Central** helps you build websites on **GitHub**.
You can write your content in Markdown and HTML using any code editor you like.
When you commit your code to your repository, **GitHub Pages** will build your website from the content of your files.

***

## Getting started

Create these files on your repository.
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

## Publishing your website

1. Go to **GitHub Pages Settings** of your repository:
    `//github.com/<user-name>/<repo-name>/settings/pages`
2. Scroll down to the **Source** section.
3. Choose the source of your website files and hit **Save**.  eg: `main/(root)`

- Your app will be accessible at `//<user-name>.github.io/<repo-name>`.


## Getting help

Having trouble with **GitHub Pages** ?  
Lets [discuss][] about it,
or [contact support](https://support.github.com/contact) to sort it out.

[discuss]: https://github.com/nikahmadz/central/discussions "Lets discuss about this project"


## Sponsor

❤️ If you use this work and liked it, **please consider [supporting development][pay]**.

[pay]: https://nikahmadz.github.io/#!pay "See payment options"

## License

[MIT][] licensed - [nikahmadz][]

[MIT]: https://github.com/nikahmadz/central/blob/main/LICENSE "View license"
[nikahmadz]: https://nikahmadz.github.io "Visit my website"
