# Antora Default UI Hugo Theme

[![GitHub contributors](https://img.shields.io/github/contributors/basil/antora-default-ui-hugo-theme.svg?color=blue)](https://github.com/basil/antora-default-ui-hugo-theme/contributors)
[![GitHub stars](https://img.shields.io/github/stars/basil/antora-default-ui-hugo-theme.svg)](https://github.com/basil/antora-default-ui-hugo-theme/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/basil/antora-default-ui-hugo-theme.svg)](https://github.com/basil/antora-default-ui-hugo-theme/network/members)
[![MPL 2.0 License](https://img.shields.io/badge/License-MPL%202.0-blue.svg)](https://github.com/basil/antora-default-ui-hugo-theme/blob/master/LICENSE)
<!-- [![GitHub release](https://img.shields.io/github/release/basil/antora-default-ui-hugo-theme.svg)](https://github.com/basil/antora-default-ui-hugo-theme/releases) -->

A Hugo theme based on the [Antora default UI](https://gitlab.com/antora/antora-ui-default), with full support for [Asciidoctor](https://asciidoctor.org/). **([_Demo_](https://antora-default-ui-hugo-theme.netlify.app/))**

## Screenshot

![screenshot](https://raw.githubusercontent.com/basil/antora-default-ui-hugo-theme/master/images/screenshot.png)

## Prerequisites

Before starting, ensure that you have [installed Hugo](https://gohugo.io/getting-started/quick-start/#step-1-install-hugo) and [created a new site](https://gohugo.io/getting-started/quick-start/#step-2-create-a-new-site).

Also ensure that you have [installed Asciidoctor](https://asciidoctor.org/docs/install-toolchain/).

## Installation

Clone the theme repository from GitHub into your site's `themes` directory:

```bash
$ git clone https://github.com/basil/antora-default-ui-hugo-theme.git themes/antora-default-ui-hugo-theme
```

Alternatively, add the theme as a [Git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules):

```bash
$ git submodule add https://github.com/basil/antora-default-ui-hugo-theme.git themes/antora-default-ui-hugo-theme
```

Then, add the theme to your site's configuration file (`config.toml`):

```toml
theme = "antora-default-ui-hugo-theme"
```

For more information, consult the [Hugo documentation](https://gohugo.io/getting-started/quick-start/#step-3-add-a-theme).

## Configuration

Configure the Asciidoctor attributes in your site's configuration file (`config.toml`) for use with this theme:

```toml
[markup]
  [markup.asciidocext]
    [markup.asciidocext.attributes]
      "icons" = "font"
      "source-highlighter" = "highlightjs"
  [markup.highlight]
    # Disable Goldmark Chroma syntax highlighter
    codeFences = false
```

Optionally, configure a copyright line for this theme's footer:

```toml
copyright = "Copyright &copy; 2020 First Last. All rights reserved."
```

Optionally, configure a URL for use with this theme's **Edit this page** feature:

```toml
[params]
  editThisPage = "https://github.com/organization/repository/edit/master/content/"
```

### Customization

Custom CSS can be added to `assets/css/custom.css`.

### Syntax Highlighting

This theme uses [highlight.js](https://highlightjs.org/) for syntax highlighting. The version of highlight.js shipped in this theme supports all of the highlight.js common languages and AsciiDoc. To add support for additional languages, [download a custom package](https://highlightjs.org/download/) with the desired languages and place it in `assets/js/vendor/highlight.pack.js`.

## License

Released under the [Mozilla Public License, Version 2.0](https://github.com/basil/antora-default-ui-hugo-theme/blob/master/LICENSE) (MPL-2.0).

## Acknowledgements

- [Dan Allen](https://github.com/mojavelinux), [Asciidoctor](https://asciidoctor.org/) Project Lead & [Antora](https://antora.org/) Project Co-Lead
