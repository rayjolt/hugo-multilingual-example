An example of how to make a multilingual site with [Hugo](https://gohugo.io/), the super-fast static website generator.

## Overview

Hugo has had support for multilingual content since version 0.17. Hugo's multilingual mode has [good documentation](https://gohugo.io/content/multilingual/), but sometimes it can be helpful to see an example. This repository shows a common configuration for making a multilingual site with Hugo.

Another purpose of this repository is for testing [Hugo themes](http://themes.gohugo.io/). All Hugo themes are not created equal with regard to internationalisation (i18n); in fact most just hard-code the English strings into the HTML templates, making multilingual sites impossible. Using such themes with this example should make it easier to see what they need to change to implement good i18n.

## Usage

To see how this repository looks with a certain theme, just clone it, then clone the theme into a subdirectory of the `themes` directory.

``` console
$ git clone https://github.com/rayjolt/hugo-multilingual-example.git
$ cd hugo-multilingual-example
$ git clone https://github.com/example/some-hugo-theme.git themes/some-hugo-theme
```

You can then test the site using Hugo's built-in server.

``` console
$ hugo server -t some-hugo-theme
```
