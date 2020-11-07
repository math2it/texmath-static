---
title: Insert images
description: Testing everything about inserting images
date: 2020-10-29
tags: [default, code]
layout: layouts/post.njk
---

## Insert normally

Try to inset an image from `/img/` (normally, without any effect):

``` js
![Nancy](/img/nancy2.jpg)
// image is store in /img/
```

![Nancy](/img/nancy2.jpg)

## Custom sizes

Custom im size inside markdown?

``` js
![test](/img/nancy.jpg =100x200)
```

![test](/img/nancy.jpg =100x200)

Auto height?

``` js
![test](/img/nancy.jpg =100x)
```

![test](/img/nancy2.jpg =100x)

Auto width?

``` js
![test](/img/nancy.jpg =x200)
```

![test](/img/nancy.jpg =x200)

## Try lazy load

Below image is very heavy!

![Very weight image](/img/hard_img.jpg)

## References

- [James Doc - Responsive images in Eleventy](https://jamesdoc.com/blog/2018/rwd-img-11ty/)
