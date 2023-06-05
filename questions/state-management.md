<h3>
  <img src="../assets/Redux.png" width="16" height="16" />
  <span>State management:</span>
</h3>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=792">Что такое Flux?</a>
  </summary>
    <br/>
  - Это архитектурный подход для обмена данными в пользовательских интерфейсах. В основе которого лежит однонаправленный поток данных. 
  1) Action(экшен тайп, пэйлоад) 
  2) Dispather(экшен) - доставляет данные об изменении в редьюсер 
  3) Reducer - чистая функция, не мутирует а возвращает новый стейт и потом происходит сравнение объектов и изменение.
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
  1) Единственный источник истины
  2) Состояние доступно только для чтения
  3) Изменение состояние производится только при помощи чистых функций + Иммутабельность данных за счет редьюсеров
</details>


<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=886">Что такое редьюсер (Reducer)?</a>
  </summary>
    <br/>
 - Это чистая функция которая принимает в качестве аргументов Action_type, payload и возвращает новое состояние для state
</details>


- [Разница между Redux и Flux?](https://youtu.be/81yRgVQ1ciM?t=819)
- [Ключевые концепции Redux?](https://youtu.be/HBSAjY-xh3k?t=408)
- [Что такое «единственный источник истины» (Single Source of Truth)?](https://youtu.be/HBSAjY-xh3k?t=517)
- [Разница между React State и Redux State?](https://youtu.be/HBSAjY-xh3k?t=638)
- [Как выглядит поток данных в Redux-приложении?](https://youtu.be/HBSAjY-xh3k?t=706)
- [Плюсы и минусы Redux?](https://youtu.be/HBSAjY-xh3k?t=767)
