# my-singer

Учебный проект курса
[Kotlin Backend Developer](https://otus.ru/lessons/kotlin/).
Поток курса 2024-05.

my-singer - это онлайн-площадка для проведения конкурсов для музыкантов. 
Площадка позволяет организаторам таких онлайн-мероприятий в удобном интерфейсе организовать конкурс, назначать
судейскую коллегию, правила оценки работ и определения победителя на каждом этапе.
Для участников этих мероприятий будет удобный интерфейс для поиска активных мероприятий и сдачи своих работ на них.

## MVP

На этапе MVP будет доступен функционал:

1. Регистрация и авторизация пользователей
2. Организация онлайн конкурсов из одного или нескольких этапов по заранее заготовленным шаблонам
   - Отборочный этап
   - Play-Off
3. Управление этапами конкурса
4. Выдача прав пользователям на оценку работ в рамках одного или нескольких этапов своего конкурса
5. Выдача прав пользователям для модерации конкурса (Права организатора)
6. Загрузка/Скачивание/Прослушивание композиций на активные конкурсы и этапы к которым допущен участник
7. Выставление оценок работам сданным участниками на конкурс в формате true/false с текстовым комментарием


## Документация

1. Маркетинг и аналитика
    1. [Целевая аудитория](./docs/01-biz/01-target-audience.md)
    2. [Заинтересанты](./docs/01-biz/02-stakeholders.md)
    3. [Пользовательские истории](./docs/01-biz/03-bizreq.md)
2. Аналитика:
    1. [Функциональные требования](./docs/02-analysis/01-functional-requiremens.md)
    2. [Нефункциональные требования](./docs/02-analysis/02-nonfunctional-requirements.md)
3. Архитектура
   1. [api](./docs/03-architecture)
4. Тесты
5. Макеты фронтенда
    1. [Все пользователи](./docs/00-frontend-maket/01-all-users/frontend-all-users.md)
    2. [Организаторы](./docs/00-frontend-maket/02-organizer/frontend-organizer.md)
    3. [Участники](./docs/00-frontend-maket/03-player/frontend-player.md)
    4. [Судьи](./docs/00-frontend-maket/04-judge/frontend-judge.md)
6. Deployment
   1. [docker](./deploy)

