# System Patterns

## Architecture Source

Высокоуровневая архитектура описана в `docs/README.md`. Детальные требования описаны в `PRD.md`.

## Component Pattern

Система проектируется как набор контейнеризированных сервисов:

- `camera-stream-handler` — специализированный сервис видеопотока.
- `compreface` — сервис распознавания лиц.
- `backend-api` — центральный координатор бизнес-логики.
- `postgres` — основное хранилище бизнес-данных.
- `tv-frontend` — клиент для ТВ-экрана.
- `admin-frontend` — клиент для администрирования.
- `reverse-proxy` — Nginx для HTTPS/WSS.

## Data Flow

Базовый поток:

```text
IP Camera → Stream Handler → CompreFace → Backend → WebSocket → TV Frontend
```

Альтернативный поток требует проверки задержек:

```text
IP Camera → Stream Handler → Backend → CompreFace → Backend → WebSocket → TV Frontend
```

## Backend Responsibilities

Backend должен оставаться центром бизнес-логики:

- сотрудники и профили лиц;
- anti-flood;
- журнал событий;
- audit log;
- роли и права;
- настройки ROI, similarity и камеры;
- WebSocket-события;
- `/health`.

## Reliability Pattern

- `/health` используется как простая диагностика MVP.
- Docker healthcheck должен добавляться для контейнеров, где это технически возможно.
- Ошибки камеры, CompreFace, backend и WebSocket логируются.

## Security Pattern

- Входная точка — Nginx.
- HTTPS/WSS с самоподписанными сертификатами.
- Секреты хранятся вне исходного кода.
- PostgreSQL и внутренние сервисы не публикуются наружу без необходимости.
- Права проверяются на backend.
