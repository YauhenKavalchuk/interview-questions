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

- [Ключевые концепции Redux?](https://youtu.be/HBSAjY-xh3k?t=408)
- [Что такое «единственный источник истины» (Single Source of Truth)?](https://youtu.be/HBSAjY-xh3k?t=517)
- [Разница между React State и Redux State?](https://youtu.be/HBSAjY-xh3k?t=638)
- [Как выглядит поток данных в Redux-приложении?](https://youtu.be/HBSAjY-xh3k?t=706)
- [Плюсы и минусы Redux?](https://youtu.be/HBSAjY-xh3k?t=767)
