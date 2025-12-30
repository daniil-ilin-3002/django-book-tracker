# Book Tracker (Django)

Цель
- Личный трекер чтения: добавление книг (по ISBN/названию), подтягивание данных из Open Library, статусы чтения, заметки, рейтинг.
- REST API + админка, контейнеризация и базовые фоновые задачи.

Стек
- Django + DRF, Postgres, Redis, Celery (позже), Docker/Compose, pytest.

MVP (М1)
- Модели: Book, UserBook (миграции, админка).
- CRUD «мои книги» (без Celery), импорт книги по ISBN (минимальная логика).
- Docker: web + db; локальный запуск.
- Тесты базовых эндпойнтов.

М2
- Поиск через Open Library API, фоновые обновления метаданных (Celery beat).
- Документация OpenAPI (drf-spectacular/yasg).
- Фильтры/сортировки по статусам/рейтингу.

М3
- Авторизация (JWT), улучшенные фильтры, деплой на Render/Railway/VPS.
- Улучшенные тесты (моки внешних API), CI.

Чек-лист фич
- [ ] Модели Book/UserBook
- [ ] CRUD /api/userbooks
- [ ] Импорт по ISBN
- [ ] Поиск Open Library
- [ ] Фоновые задачи Celery
- [ ] JWT авторизация
- [ ] OpenAPI (Swagger)
- [ ] Docker/Compose
- [ ] CI (линт/тесты)
