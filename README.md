# texmath-static

*A static version for texmath.* -- __11ty version__.

## TODO

Don't design, testing to create components first! Directly test or reference to a source.

- [ ] All basic fotmat in markdown (heading, blockquote, list, bold, italic,...)
- [ ] Insert images (lazy load, different position, directly or from markdown post files,...)
- [ ] Create a custom inline shortcode (for example, for highlight text, keyboard,...)
- [ ] Create a custom block shortcode (for example, hide/show box)
- [ ] Insert custom javascript blocks (for example, reference-mode button)
- [ ] Insert math equations (katex)
- [ ] Insert syntax highlight for inline/block codes.
- [ ] Custom markdown parser (for example, use `===text===` for rendering to `<mark>text</mark>`).
- [ ] Migrate from wordpress (less modification as possible)
- [ ] Pagination.
- [ ] Multi-users/authors.
- [ ] SEO friendly?
- [ ] Popular posts? Related posts?
- [ ] Search.
- [ ] Series of posts.
- [ ] Commen system.
- [ ] Upvote button.

## Tools

- [11ty](https://www.11ty.dev/)
- [Nunjucks](https://mozilla.github.io/nunjucks/) (mozilla)

## Starters

- [eleventy-base-blog](https://github.com/11ty/eleventy-base-blog)

## Build & run this theme

``` bash
npm install
# modify informations in _data/metadata.json
npx eleventy
npx eleventy --serve
# localhost:8080/

# or build auto when template changes
npx eleventy --watch

# or in debug mode
DEBUG=* npx eleventy
```