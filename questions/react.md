<h3>
  <img src="../assets/React.png" width="16" height="16" />
  <span>React:</span>
</h3>

<details>
<summary><a href="https://youtu.be/7TvS0iKR3_c?t=638">Что такое React?</a></summary>
  <br/>
  - JavaScript библиотека с открытым исходным кодом, созданная компанией Facebook. В основе которой используется виртуал дом и компонентный подход для эффективной отрисовки пользовательских интерфейсов. 
</details>

<details>
<summary><a href="https://youtu.be/7TvS0iKR3_c?t=671">Перечислите особенности React?</a></summary>
    <br/>
- Virtual DOM  <br/>
- Компонентный подход <br/>
- Поддержка SSR <br/>
- One way of data flow <br/>
</details>

<details>
<summary><a href="https://youtu.be/7TvS0iKR3_c?t=740">Что такое Virtual DOM? Как он работает с React?</a></summary>
    <br/>
- Это упрощенная версия обычного DOM, который намного эффективнее смотрит что изменилось и перерисовывает в реальном DOM только то что изменилось, а не всю страницу 
</details>

<details>
<summary><a href="https://youtu.be/yvOXvZ8aEFo?t=526">Для чего нужен атрибут `key` при рендере списков? и почему нельзя использовать индекс</a></summary>
    <br/>
- Для того чтобы помочь более эффективно видеть изменения в списках и перерисовывать только те эелементы, у которых изменился ключ. если сделать индекс, то при добавлении в начало списка нового элемента будет неожидаемое поведение.
</details>

<details>
<summary><a href="https://youtu.be/yvOXvZ8aEFo?t=581">Что такое `PureComponent`?</a></summary>
    <br/>
- Это компонент, который не будет обновляться если у него не изменился локальный стейт или передаваемые пропсы. не смотря на перерисовку родительского компонента. (shouldComponentUpdate)
</details>

<details>
<summary><a href="https://youtu.be/yvOXvZ8aEFo?t=637">Что такое Компонент высшего порядка (Higher-Order Component/HOC)?</a></summary>
    <br/>
- Принимает как аргумент компонент и возвращает компонент. Этот паттер позволяет оптимизировать повторяющийся функционал путем создания HOC'a и потом обернуть им необходимые компоненты.
</details>

<details>
<summary><a href="https://youtu.be/yvOXvZ8aEFo?t=684">Разница между управляемыми (controlled) и не управляемыми (uncontrolled) компонентами?</a></summary>
    <br/>
- Примерами таких компонентов могут быть input or select. Неуправляемые компоненты опираются на DOM в качестве источника данных. В управляемых компонентах каждое изменение состояние компонента происходит через функцию обработчик и состояние храниться в стейте.
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=35">Методы жизненного цикла компонента в React?</a>
  </summary>
    <br/>
  Всего они делятся на 3 стадии:
1) Монтирование “mounting”
   - constructor (Установка state и присваивание props) 
   - getDerivedStateFromProps (посмотреть что лежит в пропсах, изменились ли они и присвоить их в стейт)
   - render()
   - componentDidMount (Вызывается один раз после рендера компонента)
3) Обновление “updating”
    - getDerivedStateFromProps (посмотреть что лежит в пропсах, изменились ли они и присвоить их в стейт)
    - shouldComponentUpdate (приходит nextProps, nextState и нужно вернуть булеан)
    - getSnapshotBeforeUpdate()
    - componentDidUpdate (вызывается после монтирования в DOM, приходят аргументы prevProps и prevState)
4) Размонтирования “unmounting”
    - componentWillUnMount (Вызывается перед размонтированием в DOM, можно удалить таймауты)
 5) Ошибки "errors"
    - getDerivedStateFromError() 
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=173">Фазы отрисовки компонента в React?</a>
  </summary>
    <br/>
  Всего есть 3 фазы:
1) Render - чистая фаза без сайд эффектов, может перезапускаться реактом несколько раз
2) Pre-commit - Реакт читает дом через getSnapshotBeforeUpdate
3) Commit - Изменяет дом и выполняет все сайд эффекты, в этот момент вызываются методы с приставкой DID
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=271">Что такое React Reconciliation?</a>
  </summary>
    <br/>
  - Это алгоритм по которому происходит сравнение старого и нового виртуал дома и добавление соответсвующих изменений в реальный DOM. Сравнение начинается рекурсивно с корневого элемента и если оно изменилось, то перерисовывается вся нода.
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=342">Что такое портал (`Portal`)?</a>
  </summary>
    <br/>
  - Компонент, который рендерит свое содержиимое в произвольную часть DOM дерева. Например модальное окно или чат поверх всего layot'a. Создается при помощи React.createPortal(children, element)
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=390">Что такое контекст (`Context`)?</a>
  </summary>
    <br/>
  - Это способ глобального управления состоянием для более легкого обмена состоянием между глубоко вложенными компонентами, чем только. Создается через React.createContext() и компонент, которому необходимо соединение с контекстом оборачивается в <Provider> и передается через useContext хуком.
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=475">Что такое React хуки (Hooks)?</a>
  </summary>
    <br/>
  - Это нововведение, которые было добавлено в реакт с версией 16.8, которые позволяют использовать состояние, некоторые методы жизненого цикла компонентов и некоторые методы React (ref, context) в функциональных компонентах.
   - useState (создание состояние компонента)
   - useEffect (апдейт компонента / дидмаунт)
   - useLayoutEffect (запускается после всех обновлений в дом дерева)
   - useContext (создать контекст)
   - useCallback (создать калбек)
   - useMemo (мемоизировать функцию)
   - useRef (создать ссылку)
   - useReducer (использование редьюсера)
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=571">Что Такое `JSX`?</a>
  </summary>
    <br/>
  - Расшифровывается аббревиатура как javascript xml. Конвертируемый Babel весь написанный JSX в функции React.createElement, так что по сути это синтаксический сахар, созданный для упрощения процесса создания компонентов. 
</details>
    
<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=621">Разница между состоянием(`state`) и пропсами(`props`)?</a>
  </summary>
    <br/>
  - Это два JavaScript объекта. Props это входные аргументы для компонента, которые передаются от вышестоящего компонента. А state это локальная переменная по сути которая контролируется этим компонентом.
</details>
      
<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=689">Что такое React Fiber?</a>
  </summary>
    <br/>
  - Это новая версия алгоритма reconsilation, который предоставляет более гибкую и масштабируемую основу для работы с компонентами React. Основное преимущество это то что процесс согласования(reconciliation) компонентов происходит поэтапно (incrementally), что в общем влияет на перфоманс. 
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=689">Что такое React Fiber?</a>
  </summary>
    <br/>
  - Специальный тег JSX котрый не отрисовывается в DOM. Плюс в том, что он быстрее и использует меньше памяти, так же плюс в CSS при flex and grid
</details>
  

- [Что такое синтетические события в React?](https://youtu.be/81yRgVQ1ciM?t=34)
- [Что такое React-ссылка (`ref`)? Как создать ссылку?](https://youtu.be/81yRgVQ1ciM?t=69)
- [Разница между теневым (Shadow) и виртуальным (Virtual) DOM?](https://youtu.be/81yRgVQ1ciM?t=112)
- [Назовите преимущества использования React?](https://youtu.be/81yRgVQ1ciM?t=170)
- [Что такое условный рендеринг (Conditional Rendering)? Как его выполнить?](https://youtu.be/81yRgVQ1ciM?t=224)
- [Что такое компонент-переключатель (Switching Component)?](https://youtu.be/81yRgVQ1ciM?t=265)
- [Разница между `React` и `ReactDOM`?](https://youtu.be/81yRgVQ1ciM?t=305)
- [Разница между компонентом и контейнером?](https://youtu.be/81yRgVQ1ciM?t=370)
- [Как React обрабатывает, или ограничивает использование пропсов определенного типа?](https://youtu.be/81yRgVQ1ciM?t=413)
- [Что такое строгий режим в React? Его преимущества?](https://youtu.be/81yRgVQ1ciM?t=469)
- [Что такое «бурение пропсов» (Prop Drilling)? Как его избежать?](https://youtu.be/81yRgVQ1ciM?t=532)
- [Что такое «опрос» (Polling)? Как его реализовать в React?](https://youtu.be/81yRgVQ1ciM?t=597)
- [Разница между элементом и компонентом?](https://youtu.be/81yRgVQ1ciM?t=663)
- [Что такое `ReactDOMServer`?](https://youtu.be/81yRgVQ1ciM?t=763)
- [Что такое предохранители (Error Boundaries)?](https://youtu.be/HBSAjY-xh3k?t=36)
- [Что такое «ленивая» (Lazy) функция?](https://youtu.be/HBSAjY-xh3k?t=103)
- [Разница между рендерингом и монтированием?](https://youtu.be/HBSAjY-xh3k?t=149)
- [Что такое `сhildren`?](https://youtu.be/HBSAjY-xh3k?t=191)
- [Что такое события указателя (Pointer Events)?](https://youtu.be/HBSAjY-xh3k?t=239)
- [Что такое инверсия наследования (Inheritance Inversion)?](https://youtu.be/HBSAjY-xh3k?t=301)
- [Как в React реализовать двустороннее связывание данных?](https://youtu.be/HBSAjY-xh3k?t=355)
- [Разница между классовым и функциональным компонентами?](https://youtu.be/xZLxdts7ZW4?t=664)
- [Разница между `useEffect()` и `componentDidMount()`?](https://youtu.be/xZLxdts7ZW4?t=754)
- [Преимущества хуков?](https://youtu.be/xZLxdts7ZW4?t=819)
- [Недостатки хуков?](https://youtu.be/__neFkxAO9s?t=793)
- [Правила (ограничения) использования хуков?](https://youtu.be/xZLxdts7ZW4?t=873)
- [Что такое поднятие состояния вверх (Lifting State Up)?](https://youtu.be/ngyOYuTrUk8?t=700)
- [Что делает метод `shouldComponentUpdate`?](https://youtu.be/ngyOYuTrUk8?t=748)
- [Разница между `createElement()` и `cloneElement()`?](https://youtu.be/ngyOYuTrUk8?t=816)
- [Что такое `useReducer()`?](https://youtu.be/GZUy2i6QN7o?t=257)
- [Как реализовать однократное выполнение операции при начальном рендеринге?](https://youtu.be/GZUy2i6QN7o?t=321)
- [Что такое распределенный компонент?](https://youtu.be/GZUy2i6QN7o?t=386)
- [Расскажите о хуках `useCallback()`, `useMemo()`, `useImperativeHandle()`, `useLayoutEffect()`?](https://youtu.be/GZUy2i6QN7o?t=449)
- [Как отрендерить HTML код в React-компоненте?](https://youtu.be/GZUy2i6QN7o?t=572)
- [Зачем в `setState()` нужно передавать функцию?](https://youtu.be/GZUy2i6QN7o?t=627)
- [Для чего предназначен метод `registerServiceWorker()` в React?](https://youtu.be/GZUy2i6QN7o?t=665)
- [Чем React Router отличается от обычной маршрутизации?](https://youtu.be/GZUy2i6QN7o?t=710)
- [Какие хуки были добавлены в React Router версии 5?](https://youtu.be/GZUy2i6QN7o?t=765)
- [Как передавать пропсы в React Router?](https://youtu.be/GZUy2i6QN7o?t=841)
- [Что такое Reselect и как он работает?](https://youtu.be/XtQPrt8G0n8?t=847)
- [Назовите основную цель React Fiber?](https://youtu.be/DgevxmyzymQ?t=30)
- [Какие типы данных может возвращать `render`?](https://youtu.be/DgevxmyzymQ?t=90)
- [Разница между `memo` и `useMemo`?](https://youtu.be/DgevxmyzymQ?t=166)
- [Что такое синтетические события (SyntheticEvent) в React?](https://youtu.be/DgevxmyzymQ?t=235)
- [Является ли React реактивным?](https://youtu.be/DgevxmyzymQ?t=291)
- [Техники оптимизации перфоманса React?](https://youtu.be/__neFkxAO9s?t=606)
- [Лучшие практики безопасности в React?](https://youtu.be/__neFkxAO9s?t=694)
