<h3>
  <img src="../assets/JavaScript.png" width="16" height="16" />
  <span>Async JS:</span>
</h3>

<details>
<summary><a href="https://youtu.be/kx3dR6ztICU?t=681">Разница между синхронными и асинхронными функциями?</a></summary>
    <br/>
- Синхронные функции блокируют выполнение операций javaScript, а асинхронные нет
</details>

<details>
<summary><a href="https://youtu.be/IooJ3P2VUYs?t=612">Что такое same-origin policy в контексте JavaScript?</a></summary>
    <br/>
- Это ограничение на выполнение запросов на домены отличные от домена с которого было загружено приложение. Для разрешения таких запросов используется cors в заголовках header
</details>

<details>
<summary><a href="https://youtu.be/w-vUj0gHGgg?t=293">Что такое цикл событий (event loop) и как он работает?</a></summary>
    <br/>
- Это бесконечный цикл для выполнения синхронных и асинхронных операций в JS. состоит из Stack, Web API, Callback queue, Event loop
</details>

<details>
<summary><a href="https://youtu.be/hL5yFo9Pms4?t=249">Разница между микро и макрозадачами в event loop?</a></summary>
    <br/>
- Макро задачи выполняются после того стек вызова пуст и это задачи типа timeout, events.
  - Микро задачи выполняются перед макро задачами после опустошения стека вызова setMicroTask, async, promise callback.
</details>

<details>
<summary><a href="https://youtu.be/hL5yFo9Pms4?t=330">Расскажите о `queueMicrotask`?</a></summary>
    <br/>
- Микро задачи выполняются перед макро задачами после опустошения стека вызова setMicroTask, async, promise callback.
</details>

<details>
<summary><a href="https://youtu.be/G4iYlbilozM?t=371"></a>Что такое промисы (Promises)?</summary>
    <br/>
- это объекты в JavaScript, которые представляют собой результат асинхронной операции, которая может быть завершена успешно (resolved) или с ошибкой (rejected) в будущем. Промисы используются для управления асинхронным кодом и облегчают работу с колбэками и цепочкой асинхронных операций.
</details>

<details>
<summary><a href="https://youtu.be/XtQPrt8G0n8?t=782"></a>Разница между `Promise.all()`, `Promise.any()` и `Promise.race()`?</summary>
    <br/>
- Promise.all() - Разрешается только тогда, когда все промисы из массива успешно разрешены (resolved). если reject хоть один, то выкидывает ошибку.    <br/>
  - Promise.allSettled() - Разрешается только тогда, когда все промисы из массива успешно разрешены (resolved). если reject хоть один, даже если будет ошибка.    <br/>
  - Promise.any() - Разрешается, когда хотя бы один из промисов из массива успешно разрешается (resolved).   <br/>
  - Promise.race() - Разрешается, когда первый промис из массива разрешается или отклоняется.
</details>

<details>
<summary><a href="https://youtu.be/t0sdlbA6yA8?t=599"></a>Как выполнить несколько асинхронных операций последовательно?</summary>
    <br/>
- Цепочка из then в которой вызваются последовательно асинхронные операции в зависимости от прошлых результатов.   <br/>
  - Async/await
</details>


- [Что такое AJAX?](https://youtu.be/IooJ3P2VUYs?t=547)
- [Плюсы и минусы использовании Ajax?](https://youtu.be/yvOXvZ8aEFo?t=352)
- [Подходы при работе с асинхронным кодом?](https://youtu.be/yvOXvZ8aEFo?t=410)
- [Преимущества использовании промисов вместо колбэков?](https://youtu.be/yvOXvZ8aEFo?t=481)
- [Что такое callback-функция? Что такое Callback Hell?](https://youtu.be/V-m0sQ-hW58?t=348)
- [Что такое `async/await`?](https://youtu.be/V-m0sQ-hW58?t=417)
- [Плюсы и минусы асинхронного программирования в JavaScript?](https://youtu.be/t0sdlbA6yA8?t=460)
- [Проблемы при использовании callback-функций?](https://youtu.be/t0sdlbA6yA8?t=540)
- [Какие проблемы может вызвать неправильное использование асинхронности в JavaScript?](https://youtu.be/t0sdlbA6yA8?t=657)
