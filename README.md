# texmath-static [![Netlify Status](https://api.netlify.com/api/v1/badges/c187bcca-9464-4b2d-98d3-06982d8c1fe4/deploy-status)](https://app.netlify.com/sites/eloquent-goldstine-e9aa03/deploys)

*A static version for texmath.* -- __11ty version__.

__Demo__: https://eloquent-goldstine-e9aa03.netlify.app

## TODO

Don't design, testing to create components first! Directly test or reference to a source.

- [x] All basic fotmat in markdown (heading, blockquote, list, bold, italic,...)
- [ ] Insert images (lazy load, different position, directly or from markdown post files,...)
- [ ] Create a custom inline shortcode (for example, for highlight text, keyboard,...)
- [ ] Create a custom block shortcode (for example, hide/show box)
- [ ] Insert custom javascript blocks (for example, reference-mode button)
- [x] Insert math equations (katex)
  - [x] [markdown-it-katex](https://github.com/waylonflinn/markdown-it-katex)
    - [x] Using updated version (12), currently 0.5.1. -> use [this](https://github.com/iktakahiro/markdown-it-katex/) instead!
    - **Or?** using katex directly in `<head>`
  - **later** -- [markdown-it-mathjax](https://github.com/classeur/markdown-it-mathjax)
- [x] Insert syntax highlight for inline/block codes.
- [ ] Custom markdown parser (for example, use `===text===` for rendering to `<mark>text</mark>`).
- [ ] Migrate from wordpress (less modification as possible)
- [ ] Pagination.
- [ ] Navigation.
- [ ] Multi-users/authors.
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
- [ ] Table of contents.
- [x] 404 page.
- [x] Bootstrap -> **don't use in texmath / dinhanhthi.com!**
  - [x] If wanna use, read [this note](https://dinhanhthi.com/11ty-nunjucks#bootstrap--11ty).
  - **optional** -- Separatedly components.
  - **optional** -- Using [Bootstrap native](https://thednp.github.io/bootstrap.native/).
  - [x] Remove bootstrap from test!
- [ ] Without bootstrap
  - [ ] Collapse with native JS -> [ref](https://medium.com/dailyjs/mimicking-bootstraps-collapse-with-vanilla-javascript-b3bb389040e7)

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