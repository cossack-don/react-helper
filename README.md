# react-help будущий справочник по часто используемым методам и подходам

реакт дока — осталось дочитать
— https://ru.reactjs.org/docs/hooks-reference.html </br>
— https://ru.reactjs.org/docs/implementation-notes.html </br>
— https://ru.reactjs.org/docs/design-principles.html </br>
- остальное дочитал

```mermaid

   flowchart LR
    
     C{React Senior Developer}
    C -->|React| D[React_routers] --> Redux --> Saga --> Thunk --> Next
    C -->|React packages| X[Hook_forms] --> Ant_Designer_UI --> Axios
    C -->|Core| E[JavaScript] --> TypeScript --> Webpack --> Unit_Tests
    C -->|Extra| G[Английский] --> Алгоритмы --> Архитектура --> Паттерны --> SOLID_KISS_DRY_OOP
    C -->|ken| W[MobX] --> Test
```

Задачники Code Wars / Leet Code

## Оглавление
1. [React](#React)
2. [Частые кейсы](#Частые-кейсы)
3. [Vanilla JS](#Vanilla-JS)
4. [Учебные ресурсы](#Учебные-ресурсы)
5. [Полезные библиотеки для React](#Полезные-библиотеки-для-React)
6. [Определения](#Определения)


## Определения
- Абстракция
- Карирование
- Имутабельность
- Инкапсуляция
- Декларативный подход
- императивный подход
- мемомизация
- композиция

## React
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
- 

## Частые кейсы
1. как передать данные из родителя в дочерний компонент (данные и событие)
2. как передать из дочернего компонента в родитель данные стейта или событие
3. условный и тернарный рендер компонентов


## Vanilla JS

- Event Loop
- что такое callback
- promise
- get,set
- рекурсия
- декораторы
- деструкторизация
- call, apply, bind
- this
- window
- spread
- тернарный оператор
- импортирование и экспорт файлов

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




spread

```js
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


чтобы получать стейт актуальный обновленный - setData((data) => data+2)
