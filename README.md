# texmath-static [![Netlify Status](https://api.netlify.com/api/v1/badges/c187bcca-9464-4b2d-98d3-06982d8c1fe4/deploy-status)](https://app.netlify.com/sites/eloquent-goldstine-e9aa03/deploys)

*A static version for texmath.* -- __11ty version__.

## TODO

Don't design, testing to create components first! Directly test or reference to a source.

- [x] All basic fotmat in markdown (heading, blockquote, list, bold, italic,...)
- [ ] Insert images (lazy load, different position, directly or from markdown post files,...)
- [ ] Create a custom inline shortcode (for example, for highlight text, keyboard,...)
- [ ] Create a custom block shortcode (for example, hide/show box)
- [ ] Insert custom javascript blocks (for example, reference-mode button)
- [ ] Insert math equations (katex)
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
- [ ] Commen system.
- [ ] Upvote button.
- [x] Tags
- [ ] Categories
- [ ] Custom urls (with/without `/posts/` or with/without days)
- [x] Previous / Next post
- [ ] Table of contents.
- [x] 404 page.
- [x] Bootstrap
  - [ ] Separatedly components.

## Tools

- [11ty](https://www.11ty.dev/)
- [Nunjucks](https://mozilla.github.io/nunjucks/) (mozilla)

## Starters

- [eleventy-base-blog](https://github.com/11ty/eleventy-base-blog)

## Build & run this theme

``` bash
npm install
# modify informations in _data/metadata.json
npm start
# localhost:8080/
```

## References

- [Official docs](https://www.11ty.dev/docs/).

## Cheat sheet

Read [this note](https://dinhanhthi.com/11ty-nunjucks).