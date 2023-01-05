# hugo-pure-personal

A personal Hugo theme based on purecss.io, focused cleanliness, speed and responsiveness.

A live version of this theme together with my [hugo-photoswipe5-gallery](https://www.thkukuk.de/blog/hugo-photoswipe5-gallery/) can be found [on my personal homepage](https://www.thkukuk.de/).


## Features

* Page load speed optimizations (mobile 98/100, dekstop 100/100 on PageSpeed)
* Small (using [pure CSS](https://purecss.io))
* Responsive Sidebar
* Responsive Layout
* Configurable social links and RSS
* Data privacy
* Support for JSON-LD (JavaScript Object Notation for Linked Data)
* Custom date/time format

## Getting Started
People who have no experience with Hugo it's recommendet to read at leat the [Quick Start](https://gohugo.io/getting-started/quick-start/) guide.
Else, download or clone the theme into the `themes` directory:

```bash
$ cd themes && git clone https://github.com/thkukuk/hugo-pure-personal.git
```

Then reference it in your `config`:

```TOML
theme = "hugo-pure-personal"
```

## Customizing
A `config.toml` file with all necessary options should be created:

```toml
baseURL = "https://www.example.com/"
languageCode = "en-us"
title = "John Doe"
theme = ["hugo-pure-personal"]
copyright="Copyright © 2022-{year} John Doe"

[taxonomies]
  tag = "tags"
  category = "categories"

[params]
  breadcrumb = true
  # Enable table of contents, this can be overridden by page level parameter toc.
  toc = true
  #accentColor = "#FD3519"

[params.intro]
  main = "John Doe"
  sub = ":wink:"

[params.sidebar]
  logo = "/images/John-Doe-Portrait-256x256.webp"

[params.assets]
  favicon = "/favicon.ico"
  customCSS = ""

[menu]

[[menu.main]]
  identifier = "blog"
  name = "Blog"
  url = "/blog/"
  weight = 1

[[menu.main]]
  identifier = "recipes"
  name = "Recipes"
  url = "/recipes/"
  weight = 2

[[menu.main]]
  identifier = "about"
  name = "About"
  url = "/about/"
  weight = 3

[[menu.social]]
  name = 'GitHub'
  url = 'https://github.com/'
  weight = 1

[[menu.social]]
  name = 'LinkedIn'
  url = 'https://www.linkedin.com/'
  weight = 2

[[menu.social]]
  name = 'Email'
  url = 'mailto:john.doe@example.com'
  weight = 3

[[menu.social]]
  name = 'RSS'
  url = '/index.xml'
  weight = 4

[sitemap]
  changefreq = "monthly"
  filename = "sitemap.xml"
  priority = 0.5

# syntax highlight settings
[markup]
  [markup.highlight]
    style = "friendly"
```

## Contributing
Contributions are always welcome.

**Features**:
If you are adding a feature, fork the repository and submit a PR. Please make sure to add documentation for your new feature.

**Issues/Bugs**:
Submit a new issue with information about your issue and/or bug. If you
have a solution, then submit a new PR.

## License
MIT License. See the [LICENSE](LICENSE).
