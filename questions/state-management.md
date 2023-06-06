<h3>
  <img src="../assets/Redux.png" width="16" height="16" />
  <span>State management:</span>
</h3>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=792">Что такое Flux?</a>
  </summary>
    <br/>
  - Это архитектурный подход для обмена данными в пользовательских интерфейсах. В основе которого лежит однонаправленный поток данных и мутация state <br/>
  1) Action(экшен тайп, пэйлоад)     <br/>
  2) Dispather(экшен) - доставляет данные об изменении в редьюсер     <br/>
  3) Store  <br/>
  4) View - отображение данных (конечная точка)
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=886">Что такое Redux?</a>
  </summary>
    <br/>
  - JavaScript библиотека для стейт мененджмента визуальных интерфейсов в основе которой заложена flux архитектура.
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=886">Ключевые принципы Redux?</a>
  </summary>
    <br/>
  1) Единственный источник истины    <br/>
  2) Состояние доступно только для чтения    <br/>
  3) Изменение состояние производится только при помощи чистых функций + Иммутабельность данных за счет редьюсеров
</details>


<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=886">Что такое редьюсер (Reducer)?</a>
  </summary>
    <br/>
 - Это чистая функция которая принимает в качестве аргументов Action_type, payload и возвращает новое состояние для state
</details>

<details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=819">Разница между Redux и Flux?</a>
  </summary>
    <br/>
 - Redux: иммутабельнеость состояния, только один store (single source of truth), dispather to reducer, midlware (типа санки, саги)     <br/>
  - Flux: мутабельность состояния, несколько store, dispather to state
</details>

<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=408">Ключевые концепции Redux?</a>
  </summary>
    <br/>
- Хранилище (Store)    <br/>
- Действия (Actions)    <br/>
- Редьюсеры (Reducers)  <br/>
- Селекторы (Selectors): Функции, которые извлекают определенные части состояния из хранилища.<br/>
- Middleware: Функции, которые расширяют функциональность Redux. Они позволяют обрабатывать действия перед их достижением редьюсерам, а также могут использоваться для логирования, асинхронных операций и других задач.<br/>
- Подписка и обновление: Компоненты могут подписываться на изменения состояния в хранилище и обновляться автоматически при изменении состояния.
</details>


<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=517">Что такое «единственный источник истины» (Single Source of Truth)?</a>
  </summary>
    <br/>
- Это хранилище данных, имеет постоянную структуру. единственный способ изменить это отправить экшен в редьюсер и получить обновление если подписаны на них определенные компоненты.
</details>

<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=638">Разница между React State и Redux State? (local and global state)</a>
  </summary>
    <br/>
- Состояние реакт хранится локально внутри компонента, передается через колбек.     <br/>
  - Глобальное состояние хранится отдельно и любой компонент может подписаться на получение данных от туда
</details>

<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=706">Как выглядит поток данных в Redux-приложении?</a>
  </summary>
    <br/>
-  View - Action - Dispatcher - Middleware(Thunks, Sagas) - Reducer - State
</details>

<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=767">Плюсы и минусы Redux?</a>
  </summary>
    <br/>
-  Плюсы: Получение состояния без передачи пропсов, отдельно визуализация и управление данными, 
  - Минусы: Много кода, расходы памяти на обновление состояния (создание новых стейтов)
</details>
