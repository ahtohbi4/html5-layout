HTML5 Layout
==============

[![GitHub version][github-version-img]][github-version] [![Travis Build Status][travis-img]][travis]

[github-version-img]: https://badge.fury.io/gh/ahtohbi4%2Flayout.svg
[github-version]: https://badge.fury.io/gh/ahtohbi4%2Flayout
[travis-img]: https://travis-ci.org/ahtohbi4/layout.svg
[travis]: https://travis-ci.org/ahtohbi4/layout

> Base HTML5 layout.

Installation
-----------------

```Ctrl+c``` + ```Ctrl+v```

Components
--------------------

#### Charset *(required)*
Charset of page content.
```html
<meta charset="utf-8">
```

#### Page title *(required)*
Title which is showing in browser's tab.
```html
<title>%title%</title>
```

#### SEO page description
Google will sometimes use the meta description of a page in search results snippets. [Lern more...](https://support.google.com/webmasters/answer/35624?hl=en#1)
```html
<meta name="description" content="%description%">
```

#### SEO page keywords
May be taken into account when the [Yandex robot determines if a page matches a search query](https://yandex.ru/support/webmaster/controlling-robot/html.xml?ncrnd=2477#metatags). But Google [does not use it](https://googlewebmastercentral.blogspot.ru/2009/09/google-does-not-use-keywords-meta-tag.html) in web ranking.
```html
<meta name="keywords" content="%keywords%">
```

#### Open Graph
Base meta:
```html
<meta property="og:type" content="website">
<meta property="og:url" content= "/path/to/target/page/">
<meta property="og:title" content="%title%">
<meta property="og:image" content="/path/to/image.jpg">
```
Additional meta:
```html
<meta property="og:description" content="%description%">
<meta property="og:determiner" content="%determiner%">
<meta property="og:locale" content="en_EN">
<meta property="og:locale:alternate" content="ru_RU">
<meta property="og:site_name" content="%name%">
<meta property="og:audio" content="/path/to/audio/file.mp3">
<meta property="og:video" content="/path/to/video/file.avi">
```

Tests
--------------------

Always check your pages with official W3C [validator](https://validator.w3.org/nu/).

License
--------------------

MIT © Alexander Antonov <alexandr-post@yandex.ru>
