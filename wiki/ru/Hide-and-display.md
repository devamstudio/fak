# Система скрытия и отображения контента

Самый просто способ скрыть элемент на странице — использовать атрибут `hidden`. Следующим образом:

```html
<div hidden>...</div>
```

Данный подход рекомендован стандартами W3C. Но нередко возникают ситуации, когда надо взять сокрытие в свои руки. Мы предлагаем 2 подхода.

## Скрыть и показать для разрешений

В рамках данной концепции можно использовать атрибут `hidden` для того, чтобы скрыть элемент для всех разрешений. После, необходимо его отобразить, например, для больших мониторов. Тогда можно использовать такую конструкцию:

```html
<div class="g-visible__xl" hidden>...</div>
```

Данный подход валиден, работает по принципу `display:block!important`. Но иногда бывает ситуация, когда надо скрыть строго для одного разрешения. Тогда, как нам кажется, не смысла перечислять все «разрешенные» медиазпросы классами.

## Скрыть в одном разрешении

В таком случае есть классы типа `g-hidden`. Как и `g-visible`, он требует модификатора. И выглядит это следующим образом:

```html
<div class="g-hidden__xl">...</div>
```
Таким образом данный `div` будет скрыт только для медиазапроса типа `xl`, т.е. для больших мониторов от 1440px рабочей области браузера.