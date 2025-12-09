![](https://heatbadger.vercel.app/github/readme/contributte/rankface/?deprecated=1)

<p align=center>
    <a href="https://bit.ly/ctteg"><img src="https://badgen.net/badge/support/gitter/cyan"></a>
    <a href="https://bit.ly/cttfo"><img src="https://badgen.net/badge/support/forum/yellow"></a>
    <a href="https://contributte.org/partners.html"><img src="https://badgen.net/badge/sponsor/donations/F96854"></a>
</p>

<p align=center>
    Website 🚀 <a href="https://contributte.org">contributte.org</a> | Contact 👨🏻‍💻 <a href="https://f3l1x.io">f3l1x.io</a> | Twitter 🐦 <a href="https://twitter.com/contributte">@contributte</a>
</p>

## Disclaimer

| :warning: | This project is no longer being maintained.
|---|---|

![](https://badgen.net/github/license/contributte/rankface)

## About

Rank-Face was a simple PHP library for checking your webpage rank/position across multiple search engines and services.

## Features

The library provided methods to check:

- **Google PageRank** - Page ranking from Google (0-10 scale)
- **Google Cache Rank** - Cache ranking from Google
- **Seznam S-Rank** - Czech search engine Seznam's S-Rank
- **Alexa Traffic Rank** - Global traffic ranking from Alexa
- **Yahoo Backlinks** - Number of backlinks indexed by Yahoo
- **Yahoo Indexed Pages** - Number of pages indexed by Yahoo

## Usage

```php
<?php

require_once 'RankFace.php';
require_once 'services/RankService.php';
require_once 'services/GoogleService.php';
require_once 'services/SeznamService.php';
require_once 'services/YahooService.php';
require_once 'services/AlexaService.php';

$rankFace = new RankFace();

echo 'Google PageRank: ' . $rankFace->getGooglePageRank('example.com') . '/10<br>';
echo 'Google Cache Rank: ' . $rankFace->getGoogleCacheRank('example.com') . '/10<br>';
echo 'Seznam SRank: ' . $rankFace->getSeznamSRank('example.com') . '/10<br>';
echo 'Alexa TrafficRank: ' . $rankFace->getAlexaTrafficRank('example.com') . '<br>';
echo 'Yahoo indexed pages: ' . $rankFace->getYahooPages('example.com') . '<br>';
echo 'Yahoo backlinks: ' . $rankFace->getYahooBacklinks('example.com') . '<br>';
```

A demo preview file is included in `preview.php`.

## Development

This package was maintained by these authors.

<a href="https://github.com/f3l1x">
  <img width="80" height="80" src="https://avatars2.githubusercontent.com/u/538058?v=3&s=80">
</a>

-----

Consider to [support](https://contributte.org/partners.html) **contributte** development team.
Also thank you for using this package.
