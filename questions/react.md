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
  Всего они делятся на 3 стадии:    <br/>
1) Монтирование “mounting”    <br/>
   - constructor (Установка state и присваивание props)     <br/>
   - getDerivedStateFromProps (посмотреть что лежит в пропсах, изменились ли они и присвоить их в стейт)    <br/>
   - render()    <br/>
   - componentDidMount (Вызывается один раз после рендера компонента)    <br/>
3) Обновление “updating”    <br/>
    - getDerivedStateFromProps (посмотреть что лежит в пропсах, изменились ли они и присвоить их в стейт)    <br/>
    - shouldComponentUpdate (приходит nextProps, nextState и нужно вернуть булеан)    <br/>
    - getSnapshotBeforeUpdate()    <br/>
    - componentDidUpdate (вызывается после монтирования в DOM, приходят аргументы prevProps и prevState)    <br/>
4) Размонтирования “unmounting”    <br/>
    - componentWillUnMount (Вызывается перед размонтированием в DOM, можно удалить таймауты)    <br/>
 5) Ошибки "errors"    <br/>
    - getDerivedStateFromError()     <br/>
</details>

<details>
  <summary>
    <a href="https://youtu.be/RpcB5jnJvcI?t=173">Фазы отрисовки компонента в React?</a>
  </summary>
    <br/>
  Всего есть 3 фазы:    <br/>
1) Render - чистая фаза без сайд эффектов, может перезапускаться реактом несколько раз    <br/>
2) Pre-commit - Реакт читает дом через getSnapshotBeforeUpdate    <br/>
3) Commit - Изменяет дом и выполняет все сайд эффекты, в этот момент вызываются методы с приставкой DID    <br/>
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
  - Это нововведение, которые было добавлено в реакт с версией 16.8, которые позволяют использовать состояние, некоторые методы жизненого цикла компонентов и некоторые методы React (ref, context) в функциональных компонентах.    <br/>
   - useState (создание состояние компонента)    <br/>
   - useEffect (апдейт компонента / дидмаунт)    <br/>
   - useLayoutEffect (запускается после всех обновлений в дом дерева)    <br/>
   - useContext (создать контекст)    <br/>
   - useCallback (создать калбек)    <br/>
   - useMemo (мемоизировать функцию)    <br/>
   - useRef (создать ссылку)    <br/>
   - useReducer (использование редьюсера)    <br/>
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
    <a href="https://youtu.be/81yRgVQ1ciM?t=34">Что такое синтетические события в React?</a>
  </summary>
    <br/>
  - Это кроссбраузерная обертка для нативных евентов. все события с которыми работает рекат являются такими обертками.
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=69">Что такое React-ссылка (`ref`)?</a>
  </summary>
    <br/>
  - Это используется для получения ссылки на элемент из дом дерева, по сути аналог функции getElementById(). Для создания ссылки используется хук useRef() или функция createRef()
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=112">Разница между теневым (Shadow) и виртуальным (Virtual) DOM?</a>
  </summary>
    <br/>
  - Основная разница заключается в том, что они решают разные проблемы и находятся на разных уровнях абстракции.     <br/>
   - Virtual DOM для поиска различий и эффективной синхронизации изменений
   - Shadow DOM для создания веб елементов с собественным стилями и поведением типа псевдоэлементов before:: after::
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=112">Назовите преимущества использования React?</a>
  </summary>
    <br/>
  - Virtual DOM    <br/>
  - Возможность рендера на клиенте и на сервере    <br/>
  - JSX    <br/>
  - Низкий порог входа    <br/>
  - Простая интеграция с фреймворками и библиотеками    <br/>
  - Комьюнити и библиотеки с готовыми решениями    <br/>
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=224">Что такое условный рендеринг (Conditional Rendering)? Как его выполнить?</a>
  </summary>
    <br/>
  - Это отрисовка компонетна или элемента в зависимости от входного условия isLoading ? <Prelocader/> : null
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=265">Что такое компонент-переключатель (Switching Component)?</a>
  </summary>
    <br/>
  - Это паттерн, которые отрисовывает один из компонентов, которые есть в списке в зависимости от входных данных 
</details>
  
 <details>
  <summary>
    <a href="">Разница между `React` и `ReactDOM`?</a>
  </summary>
    <br/>
   - React содержит методы для взаимодействия с элементами и создания компонентов    <br/>
   - React DOM содержит методы для управления дом элементами содержащимися на странице    <br/>
   - Были разделены в разные библиотеки для того чтобы компоненты могли создаваться как для веб так и для мобилы
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=370">Разница между компонентом и контейнером? (Conatainer & Presentational)</a>
  </summary>
    <br/>
   - Presentational component чистый функциональный или классовый компонент основной задачей является визуализация данных   <br/>
   - Conatainer component в которых содержится сложная логика управления/состояния/связывание других компонентов   <br/>
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=370">Разница между компонентом и контейнером? (Conatainer & Presentational)</a>
  </summary>
    <br/>
   - Presentational component чистый функциональный или классовый компонент основной задачей является визуализация данных   <br/>
   - Conatainer component в которых содержится сложная логика управления/состояния/связывание других компонентов   <br/>
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=413">Как React обрабатывает, или ограничивает использование пропсов определенного типа?</a>
  </summary>
    <br/>
   - Использует сторонние библиотеки/языки типа TypeScrip/PropsTypes
</details>
  
 <details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=469">Что такое строгий режим в React? Его преимущества?</a>
  </summary>
    <br/>
   - Для определения потенциальных проблем приложения, который включает доп проверки и предупреждения для компонентов, которые происходят только в dev mode. Типа устаревшее API.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=532">Что такое «бурение пропсов» (Prop Drilling)? Как его избежать?</a>
  </summary>
    <br/>
   - Так как поток данных однонаправленный, то есть от корневого элемента к дочерним. то чтобы передать от первого уровня вложенности в 3 или 4 можно использовать контекст или редакс.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=597">Что такое «опрос» (Polling)? Как его реализовать в React?</a>
  </summary>
    <br/>
   - Это отправка запросов в api через определенный интервал и в случае появление изменений, то визуализации для пользователя. например уведомления. (setInterval)
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=663">Разница между элементом и компонентом?</a>
  </summary>
    <br/>
   - Компонент это шаблон, который может быть функцией или классом и у него есть методы жизненного цикла или хуки так же может быть состояние и пропсы   <br/>
   - Элемент это то что возвращается из компонента, объект описывающий виртуальное представление дом узла
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/81yRgVQ1ciM?t=763">Что такое `ReactDOMServer`?</a>
  </summary>
    <br/>
    - Позволяет рендерить компоненты в виде статической html разметки, используется на js сервере для SSR
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=36">Что такое предохранители (Error Boundaries)?</a>
  </summary>
    <br/>
    - Это компоненты которые перехватывают вознишие ошибки в дереве потомков и отображают соответствующий контент или выводят лог    <br/>
  - Перехватывают во время рендеринга getDerivedStateFromError(error), componentDidCatch(error)
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=103">Что такое «ленивая» (Lazy) функция?</a>
  </summary>
    <br/>
    - Это функция которая позволяет создавать компоненты при помощи динамического импорта, что позволяет уменьшить размер бандла, посколько загружаются только те компоненты, которые загружаются на UI в данный момент.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=149">Разница между рендерингом и монтированием?</a>
  </summary>
    <br/>
    - Монтирование компонента происходит только один раз после выполнения рендера и означает встраивание в дом. А ренедер происходит каждый раз при изменении состояния или пропсов компонента. 
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=191">Что такое `сhildren`?</a>
  </summary>
    <br/>
    - это пропс позволяющий передавать компоненты другим компонентам как обычные пропсы. childrenMap, childrenToArray, childrenCount. 
</details>
  
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=239">Что такое события указателя (Pointer Events)?</a>
  </summary>
    <br/>
    - Это кроссплатформенные события, которые позволяют обрабатывать прикосновения, клики мыши или нажатие стилусом
</details>
  
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=301">Что такое инверсия наследования (Inheritance Inversion)?</a>
  </summary>
    <br/>
    - Это паттерн. который при помощи HOC позволяет наследоваться от оборачиваемого компонента и контролировать стейт или рендеринг.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/HBSAjY-xh3k?t=355">Как в React реализовать двустороннее связывание данных?</a>
  </summary>
    <br/>
    - Специально запутанный вопрос. На самом деле нужно рассказать как управлять не управляемыми элементами типа input.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/xZLxdts7ZW4?t=664">Разница между классовым и функциональным компонентами?</a>
  </summary>
    <br/>
    - Функциональные это компоненты без стейта и основная функция просто отображать контент     <br/>
    - У классовых компонентов есть жизненные циклы, метод рендер и стейт
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/xZLxdts7ZW4?t=754">Разница между `useEffect()` и `componentDidMount()`?</a>
  </summary>
    <br/>
    - useEffect это в функциях (можно получить flicker нужно использовать useLayoutEffect - хук который вызывается до отображения контента)
    - componentDidMount в классовых компонентах и вызывается до отображения контента на странице.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/xZLxdts7ZW4?t=819">Преимущества хуков?</a>
  </summary>
    <br/>
    - С ними легче работать, легче читать, чем HOC, которые усложняют понимание работы компонента. вся логика в одном месте    <br/>
    - Позволяет создавать собственные хуки тем самым объеденять в функции повторяющуюся логику между другими компонентами
</details>
  
  
<details>
  <summary>
    <a href="https://youtu.be/xZLxdts7ZW4?t=873">Правила (ограничения) использования хуков?</a>
  </summary>
    <br/>
    - С ними легче работать, легче читать, чем HOC, которые усложняют понимание работы компонента. вся логика в одном месте    <br/>
    - Позволяет создавать собственные хуки тем самым объеденять в функции повторяющуюся логику между другими компонентами
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/GZUy2i6QN7o?t=257">Что такое `useReducer()`?</a>
  </summary>
    <br/>
    - Это хук принимающий в качестве аргуметов редьюсер(как в редаксе по экшен тайп) и начальный стейт и возвращающий текущий стейт и dispatch функцию    <br/>
  const [state, dispatch] = useReducer(initialState, reducer);
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/GZUy2i6QN7o?t=449">Расскажите о хуках `useCallback()`, `useMemo()`?</a>
  </summary>
    <br/>
    - useCallback(() => callback, [depend]) возвращает мемоизированную колбек функцию, которая изменяется только от зависимостей     <br/>
    - useMemo(result, [depend]) возвращает мемоизированное вычесление и в отличии от useCallback может принимать любой аргумент
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/XtQPrt8G0n8?t=847">Что такое Reselect и как он работает?</a>
  </summary>
    <br/>
    - Библиотека для мемоизации селекторов из redux. если ничего не изменилось то компонент не делает рендер.
</details>
  
<details>
  <summary>
    <a href="https://youtu.be/DgevxmyzymQ?t=166">Разница между `memo` и `useMemo`?</a>
  </summary>
    <br/>
    - Memo это компонетн высшего порядка который принимает на вход другой компонент и смотрит изменились ли пропсы и если нет, то не будет перерисовываться    <br/>
  - useMemo хук для мемоизации функций, которые вызываются каждый раз заного при изменении зависимостей
</details>
  
- [Что такое поднятие состояния вверх (Lifting State Up)?](https://youtu.be/ngyOYuTrUk8?t=700)
- [Что делает метод `shouldComponentUpdate`?](https://youtu.be/ngyOYuTrUk8?t=748)
- [Разница между `createElement()` и `cloneElement()`?](https://youtu.be/ngyOYuTrUk8?t=816)
- [Как реализовать однократное выполнение операции при начальном рендеринге?](https://youtu.be/GZUy2i6QN7o?t=321)
- [Что такое распределенный компонент?](https://youtu.be/GZUy2i6QN7o?t=386)
- [Как отрендерить HTML код в React-компоненте?](https://youtu.be/GZUy2i6QN7o?t=572)
- [Зачем в `setState()` нужно передавать функцию?](https://youtu.be/GZUy2i6QN7o?t=627)
- [Для чего предназначен метод `registerServiceWorker()` в React?](https://youtu.be/GZUy2i6QN7o?t=665)
- [Чем React Router отличается от обычной маршрутизации?](https://youtu.be/GZUy2i6QN7o?t=710)
- [Какие хуки были добавлены в React Router версии 5?](https://youtu.be/GZUy2i6QN7o?t=765)
- [Как передавать пропсы в React Router?](https://youtu.be/GZUy2i6QN7o?t=841)
- [Назовите основную цель React Fiber?](https://youtu.be/DgevxmyzymQ?t=30)
- [Какие типы данных может возвращать `render`?](https://youtu.be/DgevxmyzymQ?t=90)
- [Является ли React реактивным?](https://youtu.be/DgevxmyzymQ?t=291)
- [Техники оптимизации перфоманса React?](https://youtu.be/__neFkxAO9s?t=606)
- [Лучшие практики безопасности в React?](https://youtu.be/__neFkxAO9s?t=694)
