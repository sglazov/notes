# Элементы вёрстки проектов

Для блогов *А—К* и *B.SP* всем внешним ссылкам обязательно указывать атрибуты `rel="nofollow"` и `target="_blank"`. Для рассылки используется только `target="_blank"`.

----

## A—K

### Рамка
```html
<div style="border: 5px solid #ca2017; text-align: center; font-size: 16px; font-weight: bold; padding: 15px 10px 15px 10px; width: 100%; margin-bottom: 2em; max-width: 800px;border-radius: 5px;">
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
<p style="text-align: center;">
  <img style="width: auto;" src="" alt="" width="" height="" />
</p>
```

#### Картинка с подписью

```html
<p style="text-align: center;">
  <img style="width: auto;" src="" alt="" width="" height="" />
  <span style="display: block; font-size: 12px; padding-top: 2px; color: #b5b2b2; font-style: italic;">Текст подписи</span>
</p>
```

----

## B.SP

### Текст в рамке

```html
<div class="help-me" style="border: 5px solid #ffa200;text-align: center;font-size: 18px;font-weight: bold;padding: 12px 15px 2px 15px;width: 100%;margin-bottom: 2em;max-width: 840px;border-radius: 3px;">
  Текст в рамке
</div>
```

### Картинка

```html
<p style="text-align: center;">
  <img style="padding: 3px; border: 1px solid #ccc;width:auto;height:auto;border-radius:3px;" src="" alt="" width="" height="" />
</p>
```

#### Картинка с подписью

```html
<p style="text-align: center;">
  <img style="padding: 3px; border: 1px solid #ccc;width:auto;height:auto;border-radius:3px;" src="" alt="" width="" height="" />
  <span style="display: block; font-size: 12px; color: #b5b2b2; font-style: italic;padding-top: 5px;">Текст подписи</span>
</p>
```

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
