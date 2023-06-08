<h3>
  <img src="../assets/JavaScript.png" width="16" height="16" />
  <span>JavaScript:</span>
</h3>

<details>
<summary><a href="https://youtu.be/ycYp7CYOnO0?t=471">Типы данных в JavaScript?</a></summary>
  <br/>
  - String, Number, Boolean, Object, Symbol, Undefined, null, Bigint
</details>

<details>
<summary><a href="https://youtu.be/ycYp7CYOnO0?t=529">Разница между `==` и `===` (нестрогое/строгое равенство)?</a></summary>
  <br/>
  - == приводит к одному типу и сравнивает по типу   <br/>
  - === сравнивает по типу и по значению
</details>

<details>
<summary><a href="https://youtu.be/ycYp7CYOnO0?t=577">Что такое Strict mode в JavaScript?</a></summary>
  <br/>
  - strict mode заменияет исключениями некоторые ошибки, которые js интерпретатор пропускает по умолчанию <br/>
  - подключить можно в начале скрипта прописать "strict mode" и он по дефолту в module
</details>

<details>
<summary><a href="https://youtu.be/ycYp7CYOnO0?t=632">Разница между function declaration и function expression?</a></summary>
    <br/>
  - function declaration создана при помощи ключевого слова function и не была присвоена в переменную (может быть вызвана до ее объявления, тк интерпретатор создает ее до выполнения кода hoisting)  <br/>
  - function expression функция присвоенная в переменную
</details>

<details>
<summary><a href="https://youtu.be/G7hLwudGWL4?t=552">Что такое поднятие (Hoisting)?</a></summary>
    <br/>
  - функционал подьема переменных (var) или function declaration в глобальную область видимости. (тк интерпретатор js сначало объявляет все переменные данные ему в js файле, а потом инициализирует)
</details>

<details>
<summary><a href="https://youtu.be/1eIRTdgzHtw?t=282">Что такое область видимости (Scope)?</a></summary>
    <br/>
  - это место от куда мы имеем доступ к переменными или функциям. Существует три типа: глобальная, локальная/функциональная, блочная {let i = 0}.
</details>

<details>
<summary><a href="https://youtu.be/1eIRTdgzHtw?t=362">Разница между `var`, `let` и `const`?</a></summary>
    <br/>
  - var применяется hoisting, es5 глобальная область видимости
  - let блочная область видимости/ можно изменять
  - const блоачная область видимости/ нельзя изменять
</details>

<details>
<summary><a href="https://youtu.be/1eIRTdgzHtw?t=426">Что такое функции высшего порядка (Higher Order Functions)?</a></summary>
    <br/>
  - это функции, которые в качестве аргумента принимают другую функцию или возвращают функцию. примеры map, reduce, forEach
</details>

<details>
<summary><a href="https://youtu.be/1eIRTdgzHtw?t=426">Что такое распространение события (Evenet Propagation)?</a></summary>
    <br/>
  - это происходит после нажатия кнопки, то событие начинает опускаться с window до элемента на который тыкнули итого три фазы (capturing, targer, bubbling)
</details>

<details>
<summary><a href="https://youtu.be/1eIRTdgzHtw?t=426">Что такое делегация события (Evenet Delegation)?</a></summary>
    <br/>
  - это вместо того, чтобы вешать слушатель события на элемент, мы вешаем на родителя и смотрим на какой таргет было нажатие. 
</details>

<details>
<summary><a href="https://youtu.be/kx3dR6ztICU?t=284">Что такое замыкание (Closure)?</a></summary>
    <br/>
  - мы знаем, что переменные созданные внутри функции не доступны снаружи функции, но они удаляются после того, как функция была выполнена. Но мы можем из этой функции вернуть функцию, предварительно создав переменную и получится, что она замкнулась внутри.
</details>

<details>
<summary><a href="https://youtu.be/rlWgI7AvV18?t=507">Что обозначает `this` в JavaScript?</a></summary>
    <br/>
  - это конекст вызова или ссылка на значение объекта, который вызывает/выполняет функцию (по умолчанию это window)
</details>

<details>
<summary><a href="https://youtu.be/rlWgI7AvV18?t=548">Разница между `.call()`, `.apply()` и `bind()`?</a></summary>
    <br/>
  - tellName.bind(object, firstName, lastName) // object.tellName()    <br/>
  - someFunc.call(object, firstName, lastName)  // Ivan Kurochkin <br/>
   - someFunc.apply(object, [firstName, lastName])  // Ivan Kurochkin
</details>


<details>
<summary><a href="https://youtu.be/rlWgI7AvV18?t=401">Что такое чистая функция?</a></summary>
    <br/>
  - одна из концепций функционального программирования удовлетовраяющая двум основым требованиям: no side effects, при одни и тех же аргументах возвращает одинковые значения.
</details>


<details>
<summary><a href="https://youtu.be/kx3dR6ztICU?t=396">Что такое IIFE? (Immediatly invoke function expression)</a></summary>
    <br/>
  - это функция которая вызывает сама себя: (() => hello!)()
</details>

<details>
<summary><a href="https://youtu.be/IooJ3P2VUYs?t=100">Почему результат сравнения 2х объектов это `false`?</a></summary>
    <br/>
  - потому что объекты сравниваются по адресу в котором они хранятся в памяти, а так как каждый объект это два разных адреса в памяти, то поэтому false. 
</details>

<details>
<summary><a href="https://youtu.be/G4iYlbilozM?t=149">Как работает boxing/unboxing в JavaScript?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/nvktMVFM0_M?t=30">Что такое мемоизация? Реализуйте базовую логику функции для мемоизации?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/nvktMVFM0_M?t=280">Как передаются параметры в функцию: по ссылке или по значению?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/ngyOYuTrUk8?t=445">Плюсы и минусы иммутабельности? Как достичь иммутабельности в JS?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/V-m0sQ-hW58?t=98">JavaScript статически, или динамически типизированный язык?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/VYQl2GhbCUs?t=706">Что такое выражения (expression) и инструкции (statement) в JavaScript?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/lZNWrW39ELM?t=232">Разница между явным и неявным преобразованием (Implicit and Explicit Coercion)?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/3NGkctg4lsE?t=744">Каким образом можно обмениваться кодом между файлами?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/trriSYNrHw4?t=786">Как работает «сборщик мусора» в JavaScript?</a></summary>
    <br/>
</details>

<details>
<summary><a href="https://youtu.be/w-vUj0gHGgg?t=125">Для чего используется ключевое слово `new`?</a></summary>
    <br/>
</details>




- [Разница между `null` и `undefined`?](https://youtu.be/G7hLwudGWL4?t=511)
- [Как превратить любой тип данных в булевый? Перечислите ложные значения в JS?](https://youtu.be/CjdCxxqObaM?t=368)
- [Методы строк в JavaScript?](https://youtu.be/CjdCxxqObaM?t=415)
- [Методы массивов в JavaScript?](https://youtu.be/CjdCxxqObaM?t=538)
- [Разница между `.forEach()` и `.map()`?](https://youtu.be/rlWgI7AvV18?t=456)
- [Почему в JS функции называют объектами первого класса?](https://youtu.be/rlWgI7AvV18?t=624)
- [Как определить наличие свойства в объекте?](https://youtu.be/kx3dR6ztICU?t=226)
- [Что такое псевдомассив `arguments`?](https://youtu.be/kx3dR6ztICU?t=442)
- [Разница между host-объектами и нативными объектами?](https://youtu.be/kx3dR6ztICU?t=484)
- [Что такое прототипное наследование? Как создать объект без прототипа?](https://youtu.be/IooJ3P2VUYs?t=154)
- [Почему расширение нативных JavaScript-объектов это плохая практика?](https://youtu.be/IooJ3P2VUYs?t=202)
- [Что такое `NaN`? Как определить, что значение равно `NaN`?](https://youtu.be/IooJ3P2VUYs?t=266)
- [Что такое объектная обертка (Wrapper Objects)?](https://youtu.be/w-vUj0gHGgg?t=26)
- [Как в JavaScript создать объект?](https://youtu.be/w-vUj0gHGgg?t=83)
- [Операторы «И» и «ИЛИ» (`&&` и `||`)?](https://youtu.be/G7hLwudGWL4?t=617)
- [Для чего используется оператор двойного отрицания (`!!`)?](https://youtu.be/G4iYlbilozM?t=26)
- [Для чего используется оператор остатка (`%`)?](https://youtu.be/G4iYlbilozM?t=88)
- [Как проверить, является ли значение массивом?](https://youtu.be/G4iYlbilozM?t=68)
- [Разница между оператором `in` и методом `.hasOwnProperty()`?](https://youtu.be/nvktMVFM0_M?t=102)
- [Разница между глубокой (deep) и поверхностной (shallow) копиями объекта? Как сделать каждую из них?](https://youtu.be/nvktMVFM0_M?t=125)
- [Что такое цепочка вызовов функций (chaining)? Как реализовать такой подход?](https://youtu.be/nvktMVFM0_M?t=200)
- [Что такое необъявленная переменная?](https://youtu.be/nvktMVFM0_M?t=236)
- [Что такое прототип объекта в JavaScript?](https://youtu.be/yvOXvZ8aEFo?t=287)
- [Как работает метод `Object.create()`?](https://youtu.be/V-m0sQ-hW58?t=28)
- [Разниц между `Object.freeze()` и `Object.seal()`?](https://youtu.be/xZLxdts7ZW4?t=374)
- [Разница между методами `.slice()` и `.splice()`?](https://youtu.be/XtQPrt8G0n8?t=679)
- [Как работают методы `.find()`, `.findIndex()` и `.indexOf()`?](https://youtu.be/xZLxdts7ZW4?t=488)
- [Плюсы и минусы использования `use strict`?](https://youtu.be/xZLxdts7ZW4?t=549)
- [Разница между методами `.push()`, `.pop()`, `.shift()` и `.unshift()`?](https://youtu.be/ngyOYuTrUk8?t=385)
- [Типы всплывающих окон в JavaScript?](https://youtu.be/ngyOYuTrUk8?t=515)
- [Типы объектов JavaScript?](https://youtu.be/ngyOYuTrUk8?t=595)
- [Парадигмы программирования в JavaScript?](https://youtu.be/ngyOYuTrUk8?t=653)
- [Типы ошибок в JavaScript?](https://youtu.be/ovV8GhIkzBE?t=754)
- [Разница между `typeof` и `instanceof`?](https://youtu.be/ovV8GhIkzBE?t=835)
- [Что такое регулярное выражение (Regular Expression)?](https://youtu.be/V-m0sQ-hW58?t=146)
- [Что такое рекурсия?](https://youtu.be/V-m0sQ-hW58?t=220)
- [Что такое прототип (Prototype) объекта?](https://youtu.be/V-m0sQ-hW58?t=290)
- [Какие методы используются в регулярных выражениях?](https://youtu.be/XtQPrt8G0n8?t=495)
- [Что такое полифил (polyfill)?](https://youtu.be/XtQPrt8G0n8?t=557)
- [Что такое `switch/case`? Правила использования `switch/case`?](https://youtu.be/XtQPrt8G0n8?t=600)
- [Типы функций по способности принимать другие функции?](https://youtu.be/XtQPrt8G0n8?t=726)
- [Разница между `.some()` и `.every()`?](https://youtu.be/VYQl2GhbCUs?t=762)
- [Как сгенерировать случайное число в JavaScript?](https://youtu.be/VYQl2GhbCUs?t=801)
- [Типы операторов в JavaScript?](https://youtu.be/lZNWrW39ELM?t=30)
- [Разница между параметром и аргументом функции?](https://youtu.be/lZNWrW39ELM?t=144)
- [Правила задания имён для переменных и функций в JavaScript?](https://youtu.be/lZNWrW39ELM?t=173)
- [Для чего применяется метод `Array.from()`?](https://youtu.be/lZNWrW39ELM?t=328)
- [Назовите способы преобразования массива в объект?](https://youtu.be/lZNWrW39ELM?t=389)
- [Разница между `Object` и `Map`?](https://youtu.be/nbWY5W-9OEo?t=214)
- [Что такое каррирование?](https://youtu.be/nbWY5W-9OEo?t=295)
- [Для чего используются метод `Object.seal()`?](https://youtu.be/nbWY5W-9OEo?t=354)
- [Для чего используется свойство `.dataset`?](https://youtu.be/3NGkctg4lsE?t=680)
- [Что такое утечки памяти?](https://youtu.be/3NGkctg4lsE?t=815)
- [Назовите основные типы утечек памяти в JavaScript?](https://youtu.be/3NGkctg4lsE?t=874)
- [Как работает контекст выполнения (execution context) в JavaScript?](https://youtu.be/nTE4qvSvxXY?t=704)
- [Разница между примитивом и объектом?](https://youtu.be/nTE4qvSvxXY?t=791)
- [Типы таймеров в JavaScript?](https://youtu.be/G7hLwudGWL4?t=690)
