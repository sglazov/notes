# HTML

- See: http://htmlreference.io/

----

## Figure

```html
<figure>
    <img src="">
    <figcaption>Isabel loves the fluffy felines</figcaption>
</figure>
```

## Picture
See: https://github.com/seokirill/posthtml-webp

Before:

```html
<img src="image.jpg">
```

After:

```html
<picture>
    <source type="image/webp" srcset="image.jpg.webp">
    <img src="image.jpg">
</picture>
```
