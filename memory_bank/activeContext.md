# Active Context

## Current Focus

Инициализация Memory Bank по актуальным правилам AGENTS.md из репозитория `Ravva/projects-tracker`.

## Current Task

- Скачан и сохранён актуальный `AGENTS.md`.
- Создаётся обязательная структура `memory_bank`.
- Проверяется наличие раздела `## Project Deliverables` в `memory_bank/projectbrief.md`.
- Таблица deliverables должна иметь колонки `ID | Deliverable | Status | Weight` и сумму Weight ровно 100.
- Обновляется `docs/README.md` как источник архитектурной правды.
- После исправлений требуется commit и push всех файлов.

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
