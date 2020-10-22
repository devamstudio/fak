# Добро пожаловать в вики проекта FA-Kit!

Мы создали этот проект в качестве противовеса уже порядком перегруженному Bootstrap. К слову, интегрировать flexbox мы начали еще в старой версии, собранной на Less. А теперь добавили еще и поддержку grid.

На данный момент структура проекта следующая:

## Основа (Base)

1. [Сброс](/devamstudio/fa-kit/wiki/Grid)
1. [Сетка](/devamstudio/fa-kit/wiki/02-Grid)
1. [Типографика](/devamstudio/fa-kit/wiki/)
1. [Оформление текста](/devamstudio/fa-kit/wiki/04-Text-formatting)
1. [Медиа-контент](/devamstudio/fa-kit/wiki/07-Media)
1. [Утилиты](/devamstudio/fa-kit/wiki/03-Utilites)
1. [Система отображения\скрытия контента](/devamstudio/fa-kit/wiki/05-Hide-and-display)
1. [Призрачные классы для SASS](/devamstudio/fa-kit/wiki/06-Ghosts)

## Элементы дизайна\интерфейс (UI)

1. Блоки
1. Формы и поля ввода
1. Кнопки
1. Оформление модальных окон
1. Уведомления и предупреждения
1. Хлебные крошки
1. Пагинация

## Наименование классов

Преследуя цели — исключить конфликтность и повысить читаемость (делая акцент на BEM), наименование классов происходит у нас по принципу:

Приставка → Блок → Элемент → Модификатор. По умолчанию приставки в сборке нет, классы выглядят, как `.container`. Но при желании можно в конфигурации добавить приставки и выглядеть это будет следующим образом:

На примере образования класса контейнера: `.g-container`. Где `g-` — приставка, а `container` — блок.

Также, дабы исключить ошибки в формировании элементов и модификаторов, мы используем двойной дефис. Например: `.g-container--whide`, где `--wide` — модификатор.

***

В проекте реализована система настройки наименования классов. При сборке из исходников, предусмотрена возможность установки своих базовых классов и их приставок. **Но не модификаторов**.

В файле `/sass/config/class.sass` выведены настройки для всех классов, что представлены в проекте.

В начале идет перечень префиксов. Предусмотрен префикс для дизайн-блоков, его можно добавить в конечную сборку проекта, перенося дизайн из макетов. Это позволит исключить конфликты в классах.

В то же время существует 2 используемых в проекте префикса:

1. `g-` — используется для маркировки «глобальных» блоков.
1. `b-` — обычная маркировка блоков. В основном используется в описании интерфейса.

# Цели

Данный проект не претендует на активное использование, навязывание, рекламу. Это наша открытая командная библиотека для оперативной и удобной верстки наших проектов. Это значит, что если вам не зашло, об этом не обязательно говорить, сравнивать с другими и т.д. Тем не менее, мы совсем не против прислушаться к сообществу, и улучшить проект.