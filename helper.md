# Элементы вёрстки контента

Для блогов [А—К](#a-k), [B.SP](#bsp) и [BWA](#bwa) всем внешним ссылкам обязательно указывать атрибуты `rel="nofollow"` и `target="_blank"`. Для [рассылки](#Рассылка) используется только `target="_blank"`.

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

### Картинка-превью

```html
<img style="padding-right: 10px;padding-bottom: 10px;float: left;width: 340px;" src="" alt="" width="" height="" />
```

### Картинка

```html
<p class="img-center" style="text-align: center;">
  <img style="width: auto;" src="" alt="" width="" height="" />
</p>
```

### Кликабельная картинка

Для того, чтобы сработало увеличение картинки по клику нужно вставлять картинку с ссылкой на медиафайл и к ссылке добавить класс `image-popup`.

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

### Таблицы

Для вставки таблицы используется семантическая разметка таблицы (с использованием `thead`, `th`, `tbody` и других семантичных тегов).

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
Для подстветки кода используется [highlight.js](https://highlightjs.org/). Список поддерживаемых вариантов подстветски синтаксиса есть на странице [highlightjs.org/static/demo/](https://highlightjs.org/static/demo/). Для удобного автоматического форматирования блоков кода использую редактор: [Online HTML Editor &#128221;](https://html-online.com/editor/).

----

## BWA

### Цитаты

```html
<blockquote>
  Текст цитаты
</blockquote>
```

#### Цитаты в кавычки

```html
<blockquote class="quote">
  Текст цитаты с кавычками
</blockquote>
```

### Картинки

Для вставки полноразмерных картинок нужно обернуть картинку в тег `<p>`, а для самого изображения добавить класс `.wideresize`:

```html
<p><img src="" alt="" width="" height="" class="wideresize"></p>
```

#### Картинка с подписью

Используется для оформления скриншотов интерфейса, графиков и всего смыслового и важного:

```html
<p class="img_labeled">
  <img src="" alt="" width="" height=""><br>
  <span>Подпись к изображению</span>
</p>
```

### Вставка видео

В коде `iframe` или `embed` видео желательны атрибуты `width="100%" height="360"`.

```html
<div class="video-container">
  Код видео
</div>
```

----

## Рассылка

### Текст во врезке

```html
<div class="waring-message">Текст во врезке</div>
```

### Картинки

#### Картинка с подписью

```html
<p class="img-text">
  <img src="" alt="" style="margin-top: 3px;border-bottom: solid 1px #fdfdfd;" width="" height="">
  <span class="img-text__caption">Описание картинки</span>
</p>
```

Картинки в тексте рассылки должны быть 800×150, 800×200. Картинки мероприятий должны быть квадратными.

#### Картинки в рассылке для письма

```html
<center style="Margin: 2em 0;">
  <img src="" width="" style="-ms-interpolation-mode: bicubic; max-width: ; width: 100%;height:auto;">
</center>
```

Значение в свойстве `max-width` должно быть равно атрибуту `width=""`.

<details>
  <summary>Старый вариант для писем</summary>

```html
<center>
   <table style="border: 1px solid transparent;max-width: ;" cellpadding="0" cellspacing="0">
      <tbody>
         <tr>
            <td><img src="" alt="" width="" style="display: block;  max-width: ; width: 100%;height:auto;"></td>
         </tr>
      </tbody>
   </table>
   <i style="font-size: 10px;padding-top:6px;display:block;">Текст подписи картинки</i>
</center>
```

Значение в свойстве `max-width` у таблицы и у картинки должно быть равно атрибуту `width=""`.
</details>

### Спойлеры

Каждый спойлер — со *своим* порядковым ID: `spoiler1`, `spoiler2`.

```html
<span onclick="showhideObj('spoilerId');" class="as_adash">Развернуть</span>
<div id="spoilerId" style="display: none;">
   Текст в спойлере
</div>
```

### Таблицы

```html
<div class="table-responsive">
  <table border="0" cellpadding="0" cellspacing="0" class="table table-striped" style="width: 100%;max-width: 100%;">
     <caption>Схемы интеграции: достоинства и недостатки.</caption>
     <thead>
        <tr>
           <th></th>
        </tr>
     </thead>
     <tbody>
        <tr>
           <td></td>
        </tr>
     </tbody>
  </table>
</div>
```

Если ячейкам нужно задать выравнивание текста — нужно добавлять соответствующий класс к `<td>` или `<tr>`: `text-left`, `text-right` или `text-center`.

### Код в тексте рассылки

Бывает, что в рассылке мы показываем кусок кода для примера, а он не отображается, тогда его надо обернуть в тег `<xmp>`.
