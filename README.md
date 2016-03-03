# Haughty

### A simple and retro styled Hexo theme, was forked from [Minos](https://github.com/ppoffice/hexo-theme-minos).
#### >> [Preview](http://track.zekeair.xyz/)

![Haughty - the Hexo theme](http://zekeair.github.io/images/figures/haughty.jpg)

## Installation

### Install

``` bash
$ git clone https://github.com/zekeair/hexo-theme-haughty.git themes/haughty
```

**Haughty requires Hexo 3.0 and above.**

### Enable

Modify `theme` setting in `_config.yml` to `haughty`.

### Update

``` bash
cd themes/haughty
git pull
```

## Configuration

### Theme configuration example
```
# Header
logo_text: # Logo text
menu:
  archives: archives
  categories: categories
  tags: tags
  about: about

# Left Panel
name: # Your name
email: # Your email
description: # Some description
github: # Relative github site path
twitter: # Relative twitter site path
panel_menu: 
  about: about
  books: tags/books-sheet

# Content
excerpt_link: Read More
toc: false #  Whether to show the table of contents in articles
fancybox: true

# Miscellaneous
google_analytics: UA-71748521-1
comment_provider: disqus
favicon: /favicon.png
```

- **excerpt_link** - Cooperate with <!-- more --\> tag to show only part of the article in index pages.
- **toc** - Whether to show the table of contents in articles.
- **fancybox** - Enable [Fancybox].
- **google_analytics** - Google Analytics ID.
- **favicon** - Favicon path.

Don't forget to rename `_config.yml.example` to `_config.yml` to enable theme config!

## Custom Categories & Tags Pages

To enable custom categories page and tags page, just copy the `categories` folder and `tags` folder under your theme's `_source` foler into your site's `source` folder. Then edit theme's _config.yml and add the following lines:
```
# Header
menu:
  ...
  Categories: categories # -> add this line
  Tags: tags # -> and add this line
  ...
```

## Languages

English and Simplified Chinese are the default languages of the theme. You can add translations in the `languages` folder and change the default language in site's `_config.yml`.

``` yml
language: zh-CN
```

## Features

### Custom Categories & Tags Pages

Get your categories and tags listed in single pages to make your blog more methodic.

### Responsive Layout

Haughty knows on what screen size you are browsering the website, and reorganize the layout to fit your device.

![](http://zekeair.github.io/images/figures/haughty-responsive.jpg)

### Fancybox

Haughty uses [Fancybox] to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```
![img caption](img url)
```

### Monokai Sublime Syntax Highlight

Thanks to [Highlight.js](https://highlightjs.org/).

## Development

### Requirements

- [Grunt] 0.4+
- Hexo 3.0+

### Grunt tasks

- **default** - Download [Fancybox] and [Font Awesome].
- **fontawesome** - Only download [Font Awesome].
- **fancybox** - Only download [Fancybox].
- **clean** - Clean temporarily files and downloaded files.

[Hexo]: http://zespia.tw/hexo/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
[Grunt]: http://gruntjs.com/