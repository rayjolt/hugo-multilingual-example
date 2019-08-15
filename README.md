An example of how to make a multilingual site with [Hugo](https://gohugo.io/), the super-fast static website generator.

## Overview

Hugo has had support for multilingual content since version 0.17. Hugo's multilingual mode has [good documentation](https://gohugo.io/content/multilingual/), but sometimes it can be helpful to see an example. This repository shows a common configuration for making a multilingual site with Hugo.

Another purpose of this repository is for testing [Hugo themes](http://themes.gohugo.io/). All Hugo themes are not created equal with regard to internationalisation (i18n); in fact most just hard-code the English strings into the HTML templates, making multilingual sites impossible. Using such themes with this example should make it easier to see what they need to change to implement good i18n.

## Usage

To see how this repository looks with a certain theme, clone it, then clone the theme into a subdirectory of the `themes` directory.

``` console
$ git clone https://github.com/rayjolt/hugo-multilingual-example.git
$ cd hugo-multilingual-example
$ git clone https://github.com/example/some-hugo-theme.git themes/some-hugo-theme
```

You can then test the site using Hugo's built-in server.

``` console
$ hugo server -t some-hugo-theme
```

### Bilingual sites

The `master` branch contains content and configuration for three languages. If you want to use only two languages, you can check out the `bilingual` branch.

``` console
$ git checkout bilingual
```

## Theme i18n checklist

Things to do when making a theme i18n-ready:
1. Move all hard-coded strings to [i18n files](https://gohugo.io/content/multilingual/#translation-of-strings).
2. Add a language switcher to the site navigation.
3. Make all links in templates [language-relative](https://gohugo.io/content/multilingual/#multilingual-themes-support).
4. Add [links to translated content](https://gohugo.io/content/multilingual/#link-to-translated-content).
5. Set the correct `lang` attribute on the `html` element.
6. Set `lang` attributes for any content that is not in the page's default language, e.g. links in the language switcher.
7. For languages with right-to-left (RTL) scripts, add `dir="rtl"` to the `html` element. (Note: as of April 2017, this is [not well-supported in Hugo](https://github.com/spf13/hugo/issues/3255).)
8. [Flip the CSS](https://hacks.mozilla.org/2015/09/building-rtl-aware-web-apps-and-websites-part-1/) for RTL scripts.
