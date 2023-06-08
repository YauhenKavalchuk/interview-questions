<h3>
  <img src="../assets/WWW.png" width="16" height="16" />
  <span>Web API:</span>
</h3>

<details>
<summary><a href="https://youtu.be/w-vUj0gHGgg?t=422"></a>Что такое `HTTP`?</summary>
    <br/>
  - протокол, являющийся стандартом для отправки и получения запросов от клиента к серверу.
</details>

<details>
<summary><a href="https://youtu.be/w-vUj0gHGgg?t=483"></a>Из чего состоит `HTTP`-запрос?</summary>
    <br/>
  - Method: get, post, put, delete    <br/>
  - Path: /hello.com <br/>
  - Version of protocol: https1 / http2 <br/>
  - Headers  <br/>
  - Body, если post or put 
</details>

<details>
<summary><a href="https://youtu.be/xZLxdts7ZW4?t=31"></a>Разница между `HTTP` и `HTTPS`?</summary>
    <br/>
  - тоже самое, но только с безопасной передачей данных за счет установки зашифрованного соединения. 
</details>

<details>
<summary><a href="https://youtu.be/G4iYlbilozM?t=488"></a>Что такое `HTTP` cookie? Для чего они используются?</summary>
    <br/>
  - так как http протокол без сохранения состояния, то есть запросы на сервере не запоминаются от кого они пришли в прошлый раз, то для этого используется куки в которых мы можем передавать какую то доп информацию или идентификатор пользователя.

</details>

<details>
<summary><a href="https://youtu.be/-mWa7erZu64?t=265"></a>Разница между `HTTP/1`  и `HTTP/2`?</summary>
    <br/>
 - улучшнання версия с приоритизацией, сжатием заголвков, повышенной безопасностью.
</details>

<details>
<summary><a href="https://youtu.be/-mWa7erZu64?t=378"></a>Как работает мультиплексирование в `HTTP/2`?</summary>
    <br/>

</details>

<details>
<summary><a href="https://youtu.be/__neFkxAO9s?t=409"></a>Что такое “трехстороннее рукопожатие” (Triple handshake)?</summary>
    <br/>

</details>

<details>
<summary><a href="https://youtu.be/trriSYNrHw4?t=234"></a>Разница между протоколами `TCP` и `UDP`?</summary>
    <br/>
- протоколы для передачи данных между клиентом и сервером.   <br/>
  - TCP используется когда необходимо точно и в определенном порядке передать данные в ущерб времени (получение html or css)
  - UDP не гаранитрует доставку данных (напрмер видео звонок)
</details>

<details>
<summary><a href="https://youtu.be/yvOXvZ8aEFo?t=237"></a>Что такое `WebSocket`? В чем принцип его работы?</summary>
    <br/>
- протокол для обеспечения передачи данных и установки постоянного соединения между клиентом и сервером, данные передаются в обоих направлениях в виде пакетов без разрыва соединения. const socket = new Socket('ws://address'). (4 события: open, message, close, error)
</details>

<details>
<summary><a href="https://youtu.be/xZLxdts7ZW4?t=98"></a>Разница между Long-Polling, Websockets и Server-Sent Events?</summary>
    <br/>
  - polling/long polling это отправка запроса с клиента и ожидание ответа   <br/>
  - websocket это установка соедиенения между клиентом и сервером   <br/>
  - SSE отправка сервером событий, если данные изменились   <br/>
</details>

<details>
<summary><a href="https://youtu.be/V-m0sQ-hW58?t=727"></a>Что такое Service Workers?</summary>
    <br/>
 - по сути прокси между клиентом и сервером, основной задачей которого является обработка сетевых запросов(кэш), синхронизация обновлений кода, работы в автономном режиме (no internet)
</details>

<details>
<summary><a href="https://youtu.be/V-m0sQ-hW58?t=811"></a>Что такое Web Workers?</summary>
    <br/>
- это скрипты, которые позволяют создавать отдельные от основного потоки и выполнять в них сложные вычеслени либо работу с данными и при этом это не будет останавливать основной поток. используется для оптимизации и улучшения произвродительности.
</details>

<details>
<summary><a href="https://youtu.be/__neFkxAO9s?t=521"></a>Что такое Web Worklet?</summary>
    <br/>
 - типа веб воркеров, только используются для оптимизации процесса отрисовки браузером веб страницы (расчет размера блоков на основе css, отрисовку)
</details>

<details>
<summary><a href="https://youtu.be/-mWa7erZu64?t=663"></a>Что такое `SSL`/`TLS`? Зачем они используются в веб-разработке?</summary>
    <br/>
- это протоколы шифорования и защиты передачи данных. для подтверждения подлинности сервера с которым было установлено соединение, чтобы избежать аттаки MITM. при отправке вычесляется хэш функция и цифровой подписи для того, чтобы не изменили в пути.
</details>

<details>
<summary><a href="https://youtu.be/-mWa7erZu64?t=570"></a>Механизм устанавки сеанса между клиентом и сервером?</summary>
    <br/>

</details>

<details>
<summary><a href="https://youtu.be/ngyOYuTrUk8?t=152"></a>Что такое CDN?</summary>
    <br/>

</details>

<details>
<summary><a href="https://youtu.be/70VnuTXi4Wk?t=720"></a>Что такое IP-адрес?</summary>
    <br/>
- уникальный и числовой идентификатор устройства в компьютерной сети, работающий по протоколу IP.
</details>

<details>
<summary><a href="https://youtu.be/70VnuTXi4Wk?t=779"></a>Разница между host и domain?</summary>
    <br/>
 - domain это человекочитаемое название, которое привязывается к ip адресу    <br/>
  - host это место размещения веб сайта на сервере
</details>

<details>
<summary><a href="https://youtu.be/-mWa7erZu64?t=735"></a>Разница между идентификацией, аутентификацией, авторизацией?</summary>
    <br/>
 - идентификация это установление личности, отвечает на вопрос КТО ЭТО?     <br/>
  - аутентификацией это процедура подтверждения личности при помощи проверки пароля, отвечает на вопрос ПРАВДА ЛИ ЭТО ТЫ? <br/>
  - авторизация процедура для проверки прав личности доступа к определенными данным, отвечает на вопрос МОЖНО ЛИ ЭТО ДЕЛАТЬ? <br/>
</details>

<details>
<summary><a href="https://youtu.be/DZjIcc6KdjE?t=419"></a>Что такое OWASP Top 10?</summary>
    <br/>
 - OWASP организация занимающаяся содействием безопасности веб приложений. TOP 10 список самых популярных уязвимостей веб приложений. 
</details>



- [Какие методы может иметь `HTTP`-запрос?](https://youtu.be/G4iYlbilozM?t=419)
- [Разница между `PUT`- и `POST`-запросами?](https://youtu.be/ngyOYuTrUk8?t=29)
- [Как работает `JSONP`?](https://youtu.be/trriSYNrHw4?t=178)
- [Что такое IndexedDB в браузере? Преимущества IndexedDB?](https://youtu.be/V-m0sQ-hW58?t=653)
- [Что Такое API?](https://youtu.be/ngyOYuTrUk8?t=98)
- [Разница между URI и URL?](https://youtu.be/70VnuTXi4Wk?t=844)
- [Почему очищать кэш важно? Как это можно сделать?](https://youtu.be/N1wPX5Z4HKE?t=30)
- [Виды аутентификации?](https://youtu.be/-mWa7erZu64?t=770)
- [Что такое безопасные (Secure) и HttpOnly cookies?](https://youtu.be/ovV8GhIkzBE?t=158)
- [Что такое межсайтовый скриптинг (XSS)?](https://youtu.be/ovV8GhIkzBE?t=292)
- [Методы повышения безопасности веб-приложений?](https://youtu.be/DZjIcc6KdjE?t=347)
