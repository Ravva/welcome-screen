# Project Brief

## Project Name

Welcome Screen — модуль автоматического распознавания лиц и вывода приветствий.

## Goal

Создать локальную Docker-based систему для автоматической фиксации сотрудников и посетителей на входе в здание, распознавания лиц на сервере без GPU и отображения персонального или нейтрального приветствия на ТВ-экране с целевой задержкой до 1.2 секунды.

## Scope

MVP включает одну IP-камеру, один ТВ-экран, локальное распознавание через CompreFace, Stream Handler, Backend API, PostgreSQL, Admin frontend, TV frontend, Nginx HTTPS/WSS с самоподписанными сертификатами и `/health` для диагностики.

## Out of Scope

В MVP не входят мобильное приложение, СКУД, юридически значимый учёт рабочего времени, распознавание эмоций, пол/возраст, облачная аналитика, несколько камер, несколько ТВ-экранов, BI и полноценный мониторинг Prometheus/Grafana.

## Project Deliverables

| ID | Deliverable | Status | Weight |
|---|---|---|---:|
| WS-01 | PRD, архитектурный обзор и Memory Bank | completed | 10 |
| WS-02 | Docker-инфраструктура, Nginx HTTPS/WSS и конфигурация окружения | pending | 15 |
| WS-03 | Stream Handler для RTSP, ROI, сэмплирования и передачи кадров | pending | 15 |
| WS-04 | Интеграция CompreFace и калибровка CPU-only распознавания | pending | 15 |
| WS-05 | Backend API, бизнес-логика, anti-flood, audit log и `/health` | pending | 20 |
| WS-06 | PostgreSQL-модель данных, хранение сотрудников, фото и логов | pending | 10 |
| WS-07 | Admin frontend для сотрудников, фото, логов, ролей и настроек | pending | 10 |
| WS-08 | TV frontend с режимом ожидания, WSS и очередью приветствий | pending | 5 |

Арифметическая самопроверка Weight: 10 + 15 + 15 + 15 + 20 + 10 + 10 + 5 = 100.

## Completion Calculation

Канонический процент выполнения проекта считается только по таблице `Project Deliverables`. Сейчас завершён deliverable WS-01 весом 10, поэтому документально подтверждённая готовность проекта: 10%.
