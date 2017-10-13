# CSS

- See: http://philipwalton.github.io/solved-by-flexbox/
- See: https://github.com/AllThingsSmitty/css-protips/tree/master/translations/ru-RU
- See: http://codeguide.co
- See: http://cssnext.io/
- See: https://drafts.csswg.org/
- See: https://www.w3.org/Style/CSS/current-work
- See: https://wsd.events/2016/11/26/pres/you-dont-know-css/
- See: http://www.cheetyr.com/css-selectors
- See: http://cssreference.io/
- See: https://necolas.github.io/normalize.css/
- See: https://github.com/CSSSR/sputnik/blob/master/docs/CSS/Readme.md

## Сетка

See: http://flexboxgrid.com/
See: https://css-tricks.com/snippets/css/complete-guide-grid/
See: https://developer.mozilla.org/ru/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout

## Стандартный стиль для ссылок

```css
a[href]:not([class]) {
  color: #0000FF;
  text-decoration: underline;
}
```

## Стили для поломанныx изображений

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

## @supports

See: https://developer.mozilla.org/ru/docs/Web/CSS/@supports

## :lang

See: https://developer.mozilla.org/en-US/docs/Web/CSS/:lang
