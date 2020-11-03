# texmath-static [![Netlify Status](https://api.netlify.com/api/v1/badges/c187bcca-9464-4b2d-98d3-06982d8c1fe4/deploy-status)](https://app.netlify.com/sites/eloquent-goldstine-e9aa03/deploys)

*A static version for texmath.* -- __11ty version__.

__Demo__: https://eloquent-goldstine-e9aa03.netlify.app

## TODO

Don't design, testing to create components first! Directly test or reference to a source.

- [x] All basic fotmat in markdown (heading, blockquote, list, bold, italic,...)
  - [ ] Using html tags inside markdown doc -> [this](https://github.com/markdown-it/markdown-it#init-with-presets-and-options)
  - [ ] Cucstom container (eg. `::: warning` becomes `<div class="warning"></div>`)
  - [ ] Footnote -> [this](https://github.com/markdown-it/markdown-it-footnote)
  - [ ] use `===text===` for rendering to `<mark>text</mark>` -> [this](https://github.com/markdown-it/markdown-it-mark)
  - [ ] keyboard by `[[Ctrl]]` --> [this](https://www.npmjs.com/package/@gerhobbelt/markdown-it-kbd)
  - [ ] Task list like github -> [this](https://www.npmjs.com/package/@hackmd/markdown-it-task-lists)
  - [ ] many [more](https://www.npmjs.com/search?q=keywords%3Amarkdown-it-plugin&page=2&perPage=20)
- [ ] Hover heading links -> [plugin](https://www.npmjs.com/package/markdown-it-github-headings).
  - use option `prefixHeadingsIds: false`
- [ ] Excerpt for posts. -> [this tut](https://www.11ty.dev/docs/data-frontmatter-customize/#example-parse-excerpts-from-content)
- [ ] Insert images
  - [ ] Insert inside markdown file with custom folder.
  - [ ] Reponsive images. -> plugins [eleventy-img](https://github.com/11ty/eleventy-img) and [eleventy-plugin-images-responsiver](https://www.npmjs.com/package/eleventy-plugin-images-responsiver).
  - [ ] Lazy load images -> check [this plugin](https://www.npmjs.com/package/eleventy-plugin-lazyimages).
  - [ ] Custom image size inside markdown, like `![](/link/img.png =200x200)` -> [this plugin](https://www.npmjs.com/package/markdown-it-imsize).
- [ ] Create a custom inline shortcode (for example, for highlight text, keyboard,...)
- [ ] Create a custom block shortcode (for example, hide/show box)
- [ ] Insert custom javascript blocks (for example, reference-mode button)
- [x] Insert math equations (katex)
  - [x] [markdown-it-katex](https://github.com/waylonflinn/markdown-it-katex)
    - [x] Using updated version (12), currently 0.5.1. -> use [this](https://github.com/iktakahiro/markdown-it-katex/) instead!
    - **Or?** using katex directly in `<head>`
  - **later** -- [markdown-it-mathjax](https://github.com/classeur/markdown-it-mathjax)
- [x] Insert syntax highlight for inline/block codes.
- [ ] Custom class for blocks in markdown like `{:.class_name}`. -> try [this plugin](https://www.npmjs.com/package/markdown-it-attrs)? (it uses `{.class_name}` instead -> use [custom delimiters](https://www.npmjs.com/package/markdown-it-attrs#custom-delimiters)).
  - Check [this](https://github.com/11ty/eleventy/issues/697) also.
- [ ] Migrate from wordpress (less modification as possible)
- [ ] Pagination.
- [ ] Navigation.
- [ ] Multi-users/authors.
- [ ] Embed Youtube videos based on its URL. -> check [this plugin](https://www.npmjs.com/package/eleventy-plugin-youtube-embed).
- [ ] SEO friendly?
- [ ] Keep links from Wordpress.
- [ ] Popular posts? Related posts?
- [ ] Search.
- [ ] Series of posts.
- [ ] Comment system.
- [ ] Upvote button.
- [x] Tags
- [ ] Categories
- [ ] Custom urls (with/without `/posts/` or with/without days)
- [x] Previous / Next post
- [ ] Table of contents (TOC) -> use [this plugin](https://www.npmjs.com/package/eleventy-plugin-toc).
- [x] 404 page.
- [x] Bootstrap -> **don't use in texmath / dinhanhthi.com!**
  - [x] If wanna use, read [this note](https://dinhanhthi.com/11ty-nunjucks#bootstrap--11ty).
  - **optional** -- Separatedly components.
  - **optional** -- Using [Bootstrap native](https://thednp.github.io/bootstrap.native/).
  - [x] Remove bootstrap from test!
- [ ] Without bootstrap
  - [ ] Collapse with native JS -> [ref](https://medium.com/dailyjs/mimicking-bootstraps-collapse-with-vanilla-javascript-b3bb389040e7)
- [ ] Create a custom plugin in 11ty -> check [Creating an 11ty Plugin - SVG Embed Tool - bryanlrobinson.com](https://bryanlrobinson.com/blog/creating-11ty-plugin-embed-svg-contents/)
t.

## Tools

- [11ty](https://www.11ty.dev/)
- [Nunjucks](https://mozilla.github.io/nunjucks/) (mozilla)

## Starters

- [eleventy-base-blog](https://github.com/11ty/eleventy-base-blog)

## Build & run this theme

``` bash
# install nodejs
# https://github.com/nodesource/distributions/blob/master/README.md#installation-instructions

npm install
# modify informations in _data/metadata.json
npm start
# localhost:8080/
```

## References

- [Official docs](https://www.11ty.dev/docs/).

## Cheat sheet

Read [this note](https://dinhanhthi.com/11ty-nunjucks).