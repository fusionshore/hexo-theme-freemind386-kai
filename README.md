# Hexo-Theme-Freemind386-kai

![screenshot](./screenshot.png)

Freemind386-kai aims at fully taking advantages of Bootstrap.

- modified from https://github.com/blackshow/hexo-theme-freemind.386
- inspired by https://github.com/maxlefou/hugo.386

- [Demo](http://fusionshore.github.io)

## Requirements

- Hexo >= 3.0
- [hexo-tag-bootstrap](https://github.com/wzpan/hexo-tag-bootstrap) >= 0.0.8 (optional)

## Features

- **Bootstrap** - get the power of Twitter Bootstrap with minimal hassle;
- **Tag plugins** - luxuriant Bootstrap tag plugins, provided by [hexo-tag-bootstrap](https://github.com/wzpan/hexo-tag-bootstrap), including:
  - textcolor - a paragraph of text with specified color;
  - button - a button with target links, text and specified color;
  - label - a label with text and specified color;
  - badge - a badge with text;
  - alert - alert messages with text and specified color;
- **Local Search Engine** - a build-in local search engine, with the help of [hexo-generator-search](https://github.com/paichyperiondev/hexo-generator-search).

## Install

1. install theme (using git submodule):

```sh
$ git submodule add git@github.com:fusionshore/hexo-theme-freemind386-kai.git themes/freemind386-kai
```

2. install [hexo-tag-bootstrap](https://github.com/wzpan/hexo-tag-bootstrap) (_optional_):

```sh
$ npm install hexo-tag-bootstrap --save
```

3. install [hexo-generator-search](https://github.com/paichyperiondev/hexo-generator-search) (_optional_):

```sh
$ npm install hexo-generator-search --save
```

4. Create pages

This theme offers you the customized Categories, Tags and About pages. But you need to manually create these page at your 'source' folder.

For example, to create a `Categories` page, you may create a `index.html` file at `source/categories/` folder with the following contents:

```
title: Categories
layout: categories
---
```

Tags and About pages are created in a similar way, except that the layouts are `tags` and `page` respectively.

Alternatively you can create About page using the following command:

```sh
$ hexo new page about
```

Note that only About page can be created in that way.

## Enable

Modify `theme` setting in your `_config.yml` to `freemind386-kai`.

## Update

```sh
$ cd themes/freemind386-kai
$ git pull
```

## Configuration

```
slogan: Enter your slogan.

menu:
  - title: Archives
    url: archives
    intro: All the articles.
    icon: fa fa-archive
  - title: Categories
    url: categories
    intro: All the categories.
    icon: fa fa-folder
  - title: Tags
    url: tags
    intro: All the tags.
    icon: fa fa-tags
  - title: About
    url: about
    intro: About me.
    icon: fa fa-user

links:
  - title: My Github
    url: http://www.github.com/foo
    intro: My Github account.
    icon: fa fa-github
  - title: My LinkedIn
    url: http://www.linkedin.com/in/bar
    intro: My Linkin account.
    icon: fa fa-linkedin

widgets:
- search
- category
- tagcloud
- recent_posts
- links

rss: atom.xml
favicon: favicon.png
fancybox: true
duoshuo_shortname:

# analytics
google_analytics:
  enable: false
  siteid:
baidu_tongji:
  enable: false
  siteid:

# Search
swiftype_key:
```

- **slogan** - slogan display at the index page
- **menu** - Navigation menu
- **links** - reference links at the links widget
- **widgets** - Widgets displaying in sidebar
- **rss** - RSS link
- **fancybox** - Enable [Fancybox](http://fancyapps.com/fancybox/)
- **duoshuo_shortname** - DuoShuo ID, if you prefer to use duoshuo instead of Disqus
- **analytics** - Analytics ID. Supports both Google Analytics and Baidu Tongji.
- **swiftype_key** - Swifttype key to enable local searching. Leave it blank or comment this line if you want to use build-in local search engine.

If you prefer to use disqus, the setting of disqus should be placed at your **root** `_config.yml`:

```
# Disqus
disqus_shortname:
```

## Front-Matter

There are some new front-matter settings in Freemind386-kai that you can use to decorate your articles.

- **description** - a short description about the articles that will be display at the top of the post
- **feature** - sets a feature image that will be show at the index page
- **toc** - renders a table of contents

For example:

```
title: Tag Plugins
date: 2014-03-16 10:17:16
tags: plugins
categories: Docs
description: Introduce tag plugins in freemind.
feature: images/tag-plugins/plugins.jpg
toc: true
---
```

## License

This theme is provided under [MIT License](http://opensource.org/licenses/MIT).

## Credits

- The theme is built based on [Freemind](http://wzpan.github.io/hexo-theme-freemind/) and [BOOTSTRA.386](http://kristopolous.github.io/BOOTSTRA.386/);
- The beautiful icons are from [Font Awesome](http://fortawesome.github.io/Font-Awesome/icons/).
