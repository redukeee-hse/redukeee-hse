# Денис Артемьев — Go Backend Developer

Разрабатываю backend на Go: HTTP API, работу с PostgreSQL и Redis, интеграции с внешними сервисами. В проектах использую Chi, pgx, Squirrel и OpenAPI; уделяю внимание транзакциям, конкурентным операциям и обработке ошибок.

**Открыт к предложениям:** стажировка или junior Go backend · [Telegram @redukeee](https://t.me/redukeee)

## Основной стек

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

| Направление | Инструменты |
|---|---|
| HTTP API | Go, net/http, Chi, OpenAPI, oapi-codegen |
| Хранение данных | PostgreSQL, pgx / pgxpool, Squirrel, goose |
| Сессии и временное состояние | Redis, go-redis |
| Интеграции | OAuth 2.0, Google Calendar API, WebSocket |
| Проверка и запуск | testing, httptest, Docker, Docker Compose, Make |

## Go-проекты

### [GorkyCode — backend голосового ассистента](https://github.com/ArtemST2006/GorkyCode/tree/main/backend)

Командный проект для управления задачами, напоминаниями и встречами. Backend на Go обрабатывает запросы, работает с PostgreSQL и Redis и взаимодействует с отдельным AI-сервисом.

- HTTP API на Chi с генерацией кода по OpenAPI-контракту.
- PostgreSQL, pgx и Squirrel для хранения записей; Redis для сессий и контекста диалога.
- Интеграция с Google Calendar через OAuth 2.0.
- WebSocket-уведомления, напоминания и поиск записей с pgvector.
- В репозитории есть модульные и интеграционные тесты.

Мой вклад включает работу с календарём, получением списка записей и типами записей: [коммиты](https://github.com/ArtemST2006/GorkyCode/commits/main/?author=redukeee-hse).

[Архитектура и запуск](https://github.com/ArtemST2006/GorkyCode#readme) · [Документация backend](https://github.com/ArtemST2006/GorkyCode/blob/main/backend/README.md)

### [Trip Service — HTTP API сервиса поездок](https://github.com/redukeee-hse/trip-service/tree/homework/01)

Учебный Go-сервис создания, получения и завершения поездок. Реализация и подробный README находятся в ветке **homework/01**.

- Chi, OpenAPI и oapi-codegen для HTTP-слоя.
- PostgreSQL, pgxpool, Squirrel и миграции goose.
- Транзакции для изменения поездок и записи истории статусов.
- Идемпотентность создания по Idempotency-Key.
- Блокировка строки при завершении поездки и уникальный индекс для активной поездки водителя.
- Таймауты, graceful shutdown, health/readiness endpoints и многостадийная Docker-сборка.

[Код и инструкция запуска](https://github.com/redukeee-hse/trip-service/tree/homework/01) · [Решения по транзакциям и конкурентности](https://github.com/redukeee-hse/trip-service/blob/homework/01/README.md#решения)

## Дополнительно

Поддерживаю [конфигурацию NixOS + Hyprland](https://github.com/redukeee-hse/nixos-config) с Home Manager и скриптами установки и обновления. Ранее работал с Java и Python; сейчас основной фокус — Go backend.

## Контакты

Telegram: [@redukeee](https://t.me/redukeee) · GitHub: [все репозитории](https://github.com/redukeee-hse?tab=repositories)
