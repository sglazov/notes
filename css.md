# CSS

- See: http://philipwalton.github.io/solved-by-flexbox/
- See: https://github.com/AllThingsSmitty/css-protips/tree/master/translations/ru-RU
- See: http://codeguide.co
- See: http://cssnext.io/

## Стандартный стиль для ссылок

```css
a[href]:not([class]) {
  color: #0000FF;
  text-decoration: underline;
}
```

### Стили для поломанныx изображений

See: https://bitsofco.de/styling-broken-images/

## Clearfix

```css
.group:before, .group:after { content: " "; display: table; }
.group:after { clear: both; }
.group { zoom: 1; } /* IE 6/7 (trigger hasLayout) */
```

## Hide text

```css
.hide-text {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
}
```

## :lang

See: https://developer.mozilla.org/en-US/docs/Web/CSS/:lang
