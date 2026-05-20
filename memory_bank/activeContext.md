# Active Context

## Current Focus

Проект находится на стадии документирования. PRD/ТЗ утверждён, Memory Bank инициализирован, подготовлена HTML-инструкция по настройке серверной части.

## Current Task

- Завершена и сохранена пошаговая HTML-инструкция `docs/server-setup.html` с кнопками копирования команд.
- Инструкция покрывает: подготовку Ubuntu, Docker, firewall, клонирование, .env, TLS-сертификат, Nginx, проверку камеры, запуск и эксплуатацию.

## Active Decisions

- Имя основного требований-документа остаётся `PRD.md`.
- `docs/README.md` содержит высокоуровневую архитектуру и ссылается на `PRD.md`.
- Канонический процент готовности проекта считается только по `memory_bank/projectbrief.md`.
- На текущем этапе реализована документационная база; прикладной код ещё отсутствует.

## Next Steps

1. Реализовать Docker-инфраструктуру и Nginx reverse proxy.
2. Подготовить backend skeleton и `/health`.
3. Интегрировать CompreFace и Stream Handler.
4. Реализовать Admin frontend и TV frontend.
