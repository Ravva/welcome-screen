# Progress

## Current Status

Проект находится на стадии спецификации и первичной инициализации репозитория. Созданы `PRD.md`, `.gitignore`, актуальный `AGENTS.md`, `docs/README.md` и базовая структура Memory Bank.

## Completed

- Подготовлен PRD/ТЗ для MVP системы Welcome Screen.
- Настроен git-репозиторий и remote `origin`.
- Создан `.gitignore`.
- Инициализирован Memory Bank.
- Создан `docs/README.md` как источник архитектурной правды.
- Создан `Project Deliverables` с суммой Weight ровно 100.

## Known Issues / Open Questions

- Прикладный код сервисов ещё не реализован.
- Не выбран окончательный backend stack: Node.js NestJS/Fastify или Python FastAPI.
- Не выбран окончательный frontend stack: React/Vue/Vanilla JS.
- Не определён срок хранения фото неизвестных лиц и snapshot-изображений.
- Не закрыты юридические требования по биометрическим данным.
- Не выбран канал уведомлений администратора о неизвестных лицах.
- Не выбрана стратегия переполнения очереди приветствий.

## Контроль изменений

- last_checked_commit: `6c7bd3c`
- Последний проверенный git commit до инициализации Memory Bank: `f1e7235`.
- Сравнение `git log f1e7235.. --oneline` перед правками: новых коммитов не было.
- Memory Bank и `docs/README.md` синхронизированы с коммитом `6c7bd3c`.

## Changelog

### 2026-05-20

- Загружены правила AGENTS.md из `Ravva/projects-tracker`.
- Создан локальный `AGENTS.md`.
- Создана директория `memory_bank` с обязательными файлами.
- Добавлен `docs/README.md` с архитектурным обзором.
- В `memory_bank/projectbrief.md` добавлен обязательный раздел `## Project Deliverables`.
- Выполнена арифметическая самопроверка Weight: сумма равна 100.
- Обновлён `last_checked_commit` после коммита инициализации Memory Bank.
