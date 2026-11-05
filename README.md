# Денис Артемьев — Go Backend Developer

Пишу backend на Go: HTTP API по OpenAPI-контракту, PostgreSQL и Redis, интеграции с внешними сервисами. Уделяю внимание транзакциям, конкурентному доступу к данным и обработке ошибок.

**Ищу стажировку или позицию junior Go backend developer.**

[![Telegram](https://img.shields.io/badge/Telegram-@redukeee-26A5E4?style=flat&logo=telegram&logoColor=white)](https://t.me/redukeee)

## Проекты

### [GorkyCode](https://github.com/ArtemST2006/GorkyCode/tree/main/backend) — backend голосового ассистента

`Go` `Chi` `OpenAPI` `PostgreSQL` `pgvector` `Redis` `OAuth 2.0` `WebSocket`

Командный проект: ассистент для задач, напоминаний и встреч. Go-backend принимает запросы клиентов, хранит данные в PostgreSQL и Redis и обращается к отдельному AI-сервису.

- HTTP API на Chi, код сгенерирован по OpenAPI-контракту.
- PostgreSQL (pgx, Squirrel) для записей, Redis для сессий и контекста диалога.
- Синхронизация с Google Calendar через OAuth 2.0.
- WebSocket-уведомления, напоминания, поиск записей с pgvector.
- Модульные и интеграционные тесты.

**Мой вклад:** интеграция с календарём, получение списка записей, типы записей — [мои коммиты](https://github.com/ArtemST2006/GorkyCode/commits/main/?author=redukeee-hse).

[Архитектура и запуск](https://github.com/ArtemST2006/GorkyCode#readme) · [Документация backend](https://github.com/ArtemST2006/GorkyCode/blob/main/backend/README.md)

### [Trip Service](https://github.com/redukeee-hse/trip-service/tree/homework/01) — HTTP API сервиса поездок

`Go` `Chi` `oapi-codegen` `PostgreSQL` `pgxpool` `goose` `Docker`

Учебный сервис: создание, получение и завершение поездок. Основной упор — на корректность при параллельных запросах.

- Изменение поездки и запись истории статусов в одной транзакции.
- Идемпотентное создание по заголовку `Idempotency-Key`.
- Блокировка строки при завершении поездки; уникальный индекс не даёт водителю иметь две активные поездки.
- Таймауты, graceful shutdown, health/readiness endpoints, многостадийная Docker-сборка.

[Код и запуск](https://github.com/redukeee-hse/trip-service/tree/homework/01) · [Решения по транзакциям и конкурентности](https://github.com/redukeee-hse/trip-service/blob/homework/01/README.md#решения)

## Стек

| Направление | Инструменты |
|---|---|
| HTTP API | Go, net/http, Chi, OpenAPI, oapi-codegen |
| Данные | PostgreSQL, pgx / pgxpool, Squirrel, goose |
| Кэш и сессии | Redis, go-redis |
| Интеграции | OAuth 2.0, Google Calendar API, WebSocket |
| Тесты и запуск | testing, httptest, Docker, Docker Compose, Make |

Также работал с Java и Python. Дома — NixOS + Hyprland: [конфигурация](https://github.com/redukeee-hse/nixos-config) с Home Manager и скриптами установки и обновления.

## Контакты

Telegram: [@redukeee](https://t.me/redukeee) · [Все репозитории](https://github.com/redukeee-hse?tab=repositories)
