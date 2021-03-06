# react-stack-layout [![npm](https://img.shields.io/npm/v/@skbkontur/react-stack-layout.svg)](https://www.npmjs.com/package/@skbkontur/react-stack-layout) [![docs](https://img.shields.io/badge/docs-complete!-brightgreen.svg)](http://tech.skbkontur.ru/react-stack-layout/)

Библиотека для быстрого расположения контролов в вертикальный или горизонтальный стэки.
По сути представляет собой [layout manager](https://en.wikipedia.org/wiki/Layout_manager) из мира Desktop приложений.

## Обоснование

Очень часто при разработке бизнес логики нужно быстро выстроить контролы горизонтально друг за другом,
вырывания их, например, по базовой линии, не забывая при этом, что между ними должно быть небольшое
расстояние. Верстая такую логику много раз, появляется дублирование верстки.

В этой библиотеке я обобщил самые частые сценарии расположения контролов и создал несколько удобных
абстракций построенных поверх flexbox.

Плюс ещё маленький бонус: такой код понятен любому.

## Идея

Предположим, требуется расположить несколько контролов определённым образом. Вместо того, чтобы делать
добавочные стили к элементам, предлагается создать шаблон (или каркас) с placeholder-ами, внутри
которых разместить нужные элементы.

## Что имеем?

### Корневые элементы
* RowStack — располагает дочерние элементы в строку.
* ColumnStack — располагает дочерние элементы колонкой, друг под другом.

### Placeholder-ы
* Fit — принимает размер, соотвествующий своему контенту.
* Fill — занимает всю доступную область.
* Fixed — имеет фиксированный размер.

## Как использовать

### Установка

```
npm install @skbkontur/react-stack-layout
```

или

```
yarn add @skbkontur/react-stack-layout
```

и подключаем

```
import { ColumnStack, RowStack, Fill, Fit, Fixed } from "@skbkontur/react-stack-layout";
```

### [Документация](http://tech.skbkontur.ru/react-stack-layout/)

* [Как использовать](http://tech.skbkontur.ru/react-stack-layout/#how)
* [Сценарии использования](http://tech.skbkontur.ru/react-stack-layout/#usage)
* [Известные недостатки](http://tech.skbkontur.ru/react-stack-layout/#bugs)
* [API Reference](http://tech.skbkontur.ru/react-stack-layout/#api)

## Поиграть на CodeSandbox

[![Edit pmy55l4qrm](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/pmy55l4qrm)