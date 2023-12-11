# Дипломная работа по профессии «Frontend-разработчик»

### Цели дипломной работы

В этой дипломной работе вы создадите сайт для бронирования билетов в кинотеатр и разработаете информационную систему для администрирования залов, сеансов и предварительного бронирования билетов.

В результате выполнения дипломной работы вы:
- разработаете сайт бронирования билетов онлайн,
- разработаете административную часть сайта.

### Инструменты и дополнительные материалы, которые пригодятся для выполнения работы

- [Макеты страниц в Figma](https://www.figma.com/file/UuE7u3KnLq7DE4Dt4dK6rY/%D0%94%D0%B8%D0%B7%D0%B0%D0%B9%D0%BD-%D0%BC%D0%B0%D0%BA%D0%B5%D1%82?type=design&node-id=0%3A1&mode=design&t=CDgOE2svq5UvT5Wx-1)
- [Информация по API](./md/api.md).

### Описание проекта

#### 1. Сущности

- **Кинозал** – помещение, в котором демонстрируются фильмы. Режим работы определяется расписанием на день. Зал — прямоугольный, состоит из `N*M` различных зрительских мест.

- **Зрительское место** – место в кинозале. Зрительские места могут быть VIP и обычные.

- **Фильм** – информация о фильме заполняется администратором. Фильм связан с сеансом в кинозале.

- **Сеанс** – это временной промежуток, в котором в кинозале будет показываться фильм. На сеанс могут быть забронированы билеты.

- **Билет**  – QR-код c уникальным кодом бронирования, в котором обязательно указаны: Дата, Время, Название фильма, Зал, Ряд, Место, Стоимость, Фраза _"Билет действителен строго на свой сеанс"_.
  
Для генерации QR-кода можно использовать [QRCreator.js](https://github.com/slesareva-gala/QR-Code)

#### 2. Роли пользователей системы

-   Гость — неавторизованный посетитель сайта.
-   Администратор — авторизованный пользователь.

#### 3. Возможности гостя
-   Просмотр расписания
-   Просмотр информации о фильмах
-   Выбор места в кинозале
-   Бронирование билета

#### 4. Возможности администратора
-   Создание или редактирование залов.
-   Создание или редактирование списка фильмов.
-   Настройка цен.
-   Создание или редактирование расписания сеансов фильмов.

### Этапы разработки

1. Выполнить верстку предоставленных [макетов]((https://www.figma.com/file/BwhoRUEU4ikdbjjxFOrO7v/%D0%94%D0%B8%D0%B7%D0%B0%D0%B9%D0%BD-%D0%BC%D0%B0%D0%BA%D0%B5%D1%82?type=design&node-id=0-1&mode=design&t=j9bYnoV4gt8q03IU-0))  
   * Верстка должна корректно отображаться в браузере chrome на устройствах с шириной экрана **320px** и более.  
   * В наименовании CSS-классов желательно придерживаться методологии [БЭМ](https://ru.bem.info/methodology/quick-start/)
   * Верстка должна быть валидной ([Валидатор](https://validator.w3.org/)). 
   * Для быстрой адаптации рекомендуем вам воспользоваться [системой сеток BootStrap](https://getbootstrap.su/docs/5.0/layout/grid/).
2. Разработка класс API для взаимодействия с [Backend](./md/api.md).
3. Программирование админской части сайта.
4. Программирование клиентской части сайта.

### Правила приема работы

В личном кабинете отправлена ссылка на ваш ***Git-репозиторий***, в котором содержатся:
- все файлы проекта,
- файл Readme со ссылкой на ваш проект, опубликованный на ***githubPage***,
- описание стэка технологий, используемых вами в процессе работы над проектом.





