# Сетки

`tpl-grid` – Сетка для контентный блоков. "Дети" такой сетки подчиняются ее правилам, им не надо дополнительно указывать размеры.

```js 
{
	block: 'tpl-grid',
	content: [
	{ elem: 'fraction' },
	{ elem: 'fraction' },
	{ elem: 'fraction' }]
}
```

## Сетка с равными секциями

Для такой сетки понадобится указать только количество секций в строке. [Пример](https://codepen.io/whitepapertools/pen/5dc797f4ecf179d175ac940ceb11f893/)

Модификатор | Значение                                        | Описание
----------- | ----------------------------------------------- | --------------------------
ratio       | 1-1 / 1-1-1 / 1-1-1-1 / 1-1-1-1-1 / 1-1-1-1-1-1 | Колличество секций в сетке

## Колоночная сетка

Чтобы описать колоночную сетку, нужно указать несколько модификаторов: количество колонок, расстояние между колонками и расстояние между строками. Расстояния регулируются темой.

Если на твоем проекте сетка с другим количеством колонок, создай нужное значение модификатора на уровне проекта.

Модификатор | Значение                                | Описание
----------- | --------------------------------------- | --------------------------------------
columns     | 10 / 12                                 | Количество возможных колонок в сетке
col-gap     | none / third / half / two-thirds / full | Относительная ширина межколонника
row-gap     | none / third / half / two-thirds / full | Относительная высота межстрочника

## Элемент fraction

В колоночной сетке элементы `fraction` имеют модификатор на ширину в колонках. [Пример](https://codepen.io/whitepapertools/pen/1b5f9e70fdae42bf89878e5a3694d34e/)

Модификатор | Значение                                         | Описание
----------- | ------------------------------------------------ | --------------------------
col         | 1 / 2 / 3 / 4 / 5 / 6 / 7 / 8 / 9 / 10 / 11 / 12 | Ширина элемента в колонках