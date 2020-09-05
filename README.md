# texmath-static
*A static version for texmath.* -- __11ty version__.

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