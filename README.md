# react-help будущий справочник по часто используемым методам и подходам

реакт дока — осталось дочитать
— https://ru.reactjs.org/docs/hooks-reference.html
— https://ru.reactjs.org/docs/implementation-notes.html
— https://ru.reactjs.org/docs/design-principles.html
— https://ru.reactjs.org/docs/faq-ajax.html  и весь раздел FAQ

Задачники Code Wars / Leet Code

## Оглавление

## React

## Частые кейсы

## Vanilla JS

## Учебные ресурсы
1. https://metanit.com/web/react/ - Metanit
2. https://ru.reactjs.org/ - ru React Docs
3. https://beta.reactjs.org/ - en React Docs new - function structure

## Полезные библиотеки для React

1. Yup - валидация
2. react hook forms
3. react
4. nano store
5. react routers


Добавить памятку work life balans
+ перерывы во время работы 

- хуки
- реактивность 
- философия
- свои хуки
- частые кейсы шаблоны  например от родителям к ребёнку и наобо
рот
- можно добавить полезные учебники по реакту основные
- можно добавить примеры с код пен
- нужны примеры с функциональным подходом
- можно добавить новую доку реакта с функциональным подходом


1. как передать данные из родителя в дочерний компонент (данные и событие)
2. как передать из дочернего компонента в родитель данные стейта или событие
3. условный и тернарный рендер компонентов
4. хук use effect
5. use state 
6. use memo



native js
1 деструкторизация
2 спред оператор
3 тернарный оператор
4 импортирование компонентов и виды импортов
5 Каллбек это


Хуки (сделать подробное описание, промеры + код пен и возможно сравнение со вью
Посмотреть, может каких то хуков не хватает

- useState ( слежка-реактивности за данными, get и set)

- useEffect ( можно использовать как wathcer, и хук onMaunt)

- useCallback ( при создание компонента по новой, функция передается по ссылке, а не создается заново)

- useMemo ( кеширует и вычеслительные действия, например computed)

- useRef ( вместо querySelector)

- useReducer ( мини redux, состояние приложения)

- useContext ( provide, inject - можно с родителя передать в глубь необходимые данные без лишних props)

- useLayoutEffect ( срабатывает до монтирования в дом)

- useImperativeHande - необходимо использовать ref + forwardRef и можно получить элемент в другом компоненте и обновлять его из другого компонента

- cuatomHook react ( можно создать свои хуки используя, встроенные и так же можно создавать хуки и в них использовать свои, что создал) - вынесение логки


Core Vanilla JavaScript

- Promise
- this
- call, apply, bind
- window
- async, await
- fetch
- get,set
- exports, imports

- 

spread 
1. У нас есть один массив const a = [1, 2, 3] который мы хотим модифицировать, добавив несколько значений:

const a = [1, 2, 3];
const b = [...a, 4, 5, 6]; // [1, 2, 3, 4, 5, 6]

Теперь у нас новый массив b который содержит все значения a, плюс свои.

2. Также можно создать копию массива:
const c = [...a];

3. spread также работает и для объектов. Клонировать объект можно так:
const newObj = { ...oldObj };

4. Используя строки, оператор распространения spread создает массив с каждым символом в строке:
const hey = "hey";
const arrayized = [...hey]; // ['h', 'e', 'y']

5. У этого оператора есть несколько довольно полезных свойств.
Наиболее важным из них является возможность очень просто использовать массив в качестве аргумента функции:

const f = (one, two) => {
  console.log(one, two); // 1, 2
};
const a = [1, 2];
f(...a);
```


Матчить - это https://habr.com/ru/company/sberbank/blog/354564/
иммутабельность - В программировании неизменяемым (англ. immutable) называется объект, состояние которого не может быть изменено после создания.

В функциональном программировании все (в случае чистых языков) или почти все (в случае «нечистых» — англ. impure — языков) данные в программе, как локальные, так и глобальные, являются неизменяемыми. С одной стороны, это существенно повышает стабильность программ за счёт упрощения формальной верификации программ. С другой, это затрудняет решение ряда задач (из которых наиболее часто отмечается задача реализации интерфейса пользователя, который в своей сути представляет собой изменяемое состояние), что вынуждает усложнять системы типов языка — например, монадами или уникальными типами.

https://formik.org/  - для работы с формами - наподобие react hook forms


## Vanilla JavaScript

- Event Loop
- что такое callback
- promise
- get,set
- рекурсия
- декораторы
- call, apply, bind
- this
- window
- spread
- Абстракция
- Карирование
- Имутабельность
- Инкапсуляция
- Декларативный подход
- императивный подход
- мемомизация

## Core stack React

- React 16.8+
- Redux or Nano store
- React Routers
- Saga
- Thunk
- TypeScript
- JavaScript ES6+
- Webpack
- Unit tests (Jest, Testing Library)
- Паттерны
- Алгоритмы
- Архитектура
- SOLID, KISS, DRY, ООП
