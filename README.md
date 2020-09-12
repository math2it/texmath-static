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

## References

- [Official docs](https://www.11ty.dev/docs/).

## Cheat sheet

### Frontmatter

Basics

``` yaml
---
title: Title of the post
description: description of the post
date: 2020-09-11
layout: layouts/post.njk
---
```

Tags

``` yaml
---
tags:
  - default

# or
tags: [tag 1, tag 2]
---
```

### Code

Need [this plugin](https://www.11ty.dev/docs/plugins/syntaxhighlight/). List of suppo[rted languages](https://prismjs.com/#languages-list).

Highlight lines

~~~ js
``` text/1-2,4
// this is a command
function myCommand() {
	let counter = 0;
	counter++;
}
```
~~~

### Navigation

Next / Previous posts

``` html
<ul>
  {%- set nextPost = collections.posts | getNextCollectionItem(page) %}
  {%- if nextPost %}<li>Next: <a href="{{ nextPost.url | url }}">{{ nextPost.data.title }}</a></li>{% endif %}
  {%- set previousPost = collections.posts | getPreviousCollectionItem(page) %}
  {%- if previousPost %}<li>Previous: <a href="{{ previousPost.url | url }}">{{ previousPost.data.title }}</a></li>{% endif %}
</ul>
```

### Others