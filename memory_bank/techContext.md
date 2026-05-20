# Tech Context

## Repository Map

Текущее состояние репозитория:

- `PRD.md` — основной PRD/ТЗ документ.
- `AGENTS.md` — актуальные правила работы агента и Memory Bank.
- `docs/README.md` — источник архитектурной правды.
- `docs/server-setup.html` — пошаговая инструкция настройки Ubuntu-сервера с кнопками копирования команд.
- `memory_bank/` — операционная память проекта.
- `.gitignore` — исключения для секретов, runtime-данных, сборок и временных файлов.

Прикладные директории сервисов пока отсутствуют.

## Target Platform

- Ubuntu Server LTS 22.04 или 24.04.
- Docker Compose.
- CPU-only распознавание без GPU.
- Локальная сеть 1 Гбит/с.

## Planned Stack

- CompreFace для распознавания лиц.
- Python OpenCV/PyAV для Stream Handler.
- Backend: Node.js NestJS/Fastify или Python FastAPI; окончательный выбор не зафиксирован.
- PostgreSQL.
- Frontend: React/Vue/Vanilla JS; окончательный выбор не зафиксирован.
- Nginx reverse proxy.
- Самоподписанные TLS-сертификаты.

## Tooling Rules

- Использовать `bun` как пакетный менеджер для JS/TS частей после появления кода.
- Markdown-файлы не проверять через Biome.
- Сервер разработки не запускать, не останавливать и не проверять его статус без запроса пользователя.

## Current Implementation Status

Код сервисов ещё не создан. Репозиторий находится на стадии требований, архитектурной фиксации и Memory Bank initialization.
