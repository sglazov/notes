# Элементы вёрстки контента

Для блогов [А—К](#a-k) и [B.SP](#bsp) всем внешним ссылкам обязательно указывать атрибуты `rel="nofollow"` и `target="_blank"`. Для [рассылки](#Рассылка) используется только `target="_blank"`.

----

## A—K

### Рамка
```html
<div class="hipsterquote" style="border: 5px solid #ca2017; text-align: center; font-size: 16px; font-weight: bold; padding: 15px 10px 15px 10px; width: 100%; margin-bottom: 2em; max-width: 800px;border-radius: 5px;">
  Текст в рамке
</div>
```

### Вставка видео

В коде `iframe` или `embed` видео желательны атрибуты `width="100%" height="380"`.

```html
<div class="video-container">
  Код видео
</div>
```

### Картинка

```html
<p class="img-center" style="text-align: center;">
  <img style="width: auto;" src="" alt="" width="" height="" />
</p>
```

#### Картинка с подписью

```html
<p class="img-center" style="text-align: center;">
  <img style="width: auto;" src="" alt="" width="" height="" />
  <span class="img__caption img-center__caption" style="display: block; font-size: 12px; padding-top: 2px; color: #b5b2b2; font-style: italic;">Текст подписи</span>
</p>
```

### Врезка в тексте

```html
<div class="hipsterbox" class="" style="margin: 25px 0; padding: 12px 15px 13px; font-size: 17px; line-height: 24px;border: 1px solid rgba(0,0,0,0.08); border-radius: 4px; background: #fff9cd; box-shadow: 0 1px 15px rgba(0,0,0,0.1); font-family: 'Arial','Helvetica Neue',sans-serif;">
  Текст врезки
</div>
```

### Большой текст по центру

```html
<p class="big-text" style="text-align: center; font-size: 28px; font-weight: 300; line-height: 1;">Текст</p>
```

----

## B.SP

### Текст в рамке

```html
<div class="help-me" style="border: 5px solid #ffa200;text-align: center;font-size: 18px;font-weight: bold;padding: 12px 15px 12px 15px;width: 100%;margin-bottom: 2em;max-width: 840px;border-radius: 3px;">
  Текст в рамке
</div>
```

### Картинка

Картинки по ширине лучше всего делать — `width: 840px`.

```html
<p style="text-align: center;">
  <img style="padding: 3px; border: 1px solid #ccc;width:auto;max-width:840px;height:auto;border-radius:3px;" src="" alt="" width="" height="" />
</p>
```

#### Картинка с подписью

```html
<p class="img-center" style="text-align: center;">
  <img style="padding: 3px; border: 1px solid #ccc;width:auto;max-width:840px;height:auto;border-radius:3px;" src="" alt="" width="" height="" />
  <span class="img__caption img-center__caption" style="display: block; font-size: 12px; color: #b5b2b2; font-style: italic;padding-top: 5px;">Текст подписи</span>
</p>
```

### Таблицы

К сожалению, таблицы в записи нужно вставлять криво:

```html
<table style="border: 1px solid #ccc;width: 100%;margin-bottom: 10px;">
  <tbody>
    <tr>
      <td style="padding: 10px;border: 1px solid #ccc;font-weight: bold;width: 300px;"></td>
      <td style="padding: 10px;border: 1px solid #ccc;font-weight: bold;"></td>
    </tr>
    <tr>
      <td style="padding: 10px;border: 1px solid #ccc;"></td>
      <td style="padding: 10px;border: 1px solid #ccc;"></td>
    </tr>
  </tbody>
</table>
```

### Выделение текста

```html
<span class="mark" style="color: #c60; background: #fff8d0;padding: 3px 4px 2px 4px;">текст</span>
```

### Блок кода

```html
<pre>
  <code class="html">
    листинг кода
  </code>
</pre>
```
Для подстветки кода используется [highlight.js](https://highlightjs.org/).

----

## Рассылка

### Картинки

Картинки новостей должны быть 800×150, 800×200. Картинки мероприятий должны быть квадратными.

```html
<center>
   <table style="border: 1px solid #ccc;" cellpadding="0" cellspacing="0">
      <tbody>
         <tr>
            <td><img style="display: block;" attach="" src="" alt=""></td>
         </tr>
      </tbody>
   </table>
   <i style="font-size: 10px;padding-top:6px;display:block;">Текст подписи картинки</i>
</center>
```

### Спойлеры

Каждый спойлер — со *своим* ID (`spoiler_1`, `spoiler_2`).

```html
<div id="spoiler_id" style="display: none;">
   {Текст спойлера}
</div>
<span class="as_adash" onclick="showhideObj('spoiler_id');">Показать подробности</span>
```

### Таблицы

```html
<table cellpadding="0" cellspacing="0" border="0" class="table_in_subscribe" align="center" width="90%">
```

### Код в тексте рассылки

Бывает, что в рассылке мы показываем кусок кода для примера, а он не отображается, тогда его надо обернуть в тег `<xmp>`.
