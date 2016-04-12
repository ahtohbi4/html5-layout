HTML5 Layout
==

[![GitHub version][github-version-img]][github-version] [![Travis Build Status][travis-img]][travis]

[github-version-img]: https://badge.fury.io/gh/ahtohbi4%2Flayout.svg
[github-version]: https://badge.fury.io/gh/ahtohbi4%2Flayout
[travis-img]: https://travis-ci.org/ahtohbi4/layout.svg
[travis]: https://travis-ci.org/ahtohbi4/layout

> Base HTML5 layout.

Installation
--

`Ctrl+c` + `Ctrl+v`

Components
--

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

#### Twitter Cards
```html
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@username">
<meta name="twitter:title" content="%title%">
<meta name="twitter:description" content="%description%">
<meta name="twitter:image" content="/path/to/image.jpg">
```

#### Google instructions
```html
<meta name="google" content="notranslate">
```

#### Mobile viewport scale
```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

#### Phone number detection by device
```html
<meta name="format-detection" content="telephone=no">
```

#### Cononical link
```html
<link rel="canonical" href="/cannonical/link/to/current/page/">
```

#### Alternate link
```html
<link rel="alternate" hreflang="ru" href="/path/to/alternate/ru/language/of/current/page/">
<link rel="alternate" hreflang="ar" href="/path/to/alternate/ar/language/of/current/page/">
...
```

#### Prefetch DNS
Identifies a DNS query to resolve the background, so that requests can occur more quickly. [Lern more...](http://www.w3.org/TR/resource-hints/#dfn-prefetch)
```html
<link rel="dns-prefetch" href="//example.com">
```

#### Pre connect
Initiating an early connection, which includes the DNS lookup, TCP handshake, and optional TLS negotiation,
allows the user agent to mask the high latency costs of establishing a connection. [Lern more...](http://www.w3.org/TR/resource-hints/#preconnect)
```html
<link rel="preconnect" href="//example.com" crossorigin="use-credentials">
```

#### Prefetch of resources
Identifies a resource file, such as an image or a CSS stylesheet, to be downloaded into the cache. [Lern more...](http://www.w3.org/TR/resource-hints/#prefetch)
```html
<link rel="prefetch" href="//example.com/path/to/next/page/or/single/resource/" crossorigin="use-credentials">
```

#### Pre render of next page
Identifies a webpage to load in the background, in case the user wants to navigate to it next. [Lern more...](http://www.w3.org/TR/resource-hints/#prerender)
```html
<link rel="prerender" href="//example.com/path/to/next/page/">
```

#### Browser MS configuration
```html
<meta name="msapplication-config" content="/browserconfig.xml">
```
Other meta by Microsoft
```html
<meta name="application-name" content="%name%">
<meta name="msapplication-badge" content="frequency=60; polling-uri=http://example.com/path/to/polling.xml">
```

#### CSS for layout
> Use a some number of subdomains to parallel downloads.

```html
<link rel="stylesheet" href="//st1.example.com/path/to/first-view-style.css">
```

#### Google Analytics code
```js
<script>(function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){(i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)})(window,document,'script','//www.google-analytics.com/analytics.js','ga');ga('create','%id%','auto');ga('send','pageview');</script>
```

Tests
--------------------

Always check your pages with official W3C [validator](https://validator.w3.org/nu/).

License
--------------------

MIT © Alexander Antonov <alexandr-post@yandex.ru>
