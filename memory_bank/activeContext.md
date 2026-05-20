# Active Context

## Current Focus

Документация обновлена: добавлена поддержка USB/встроенной камеры как альтернативы IP-камере. Stream Handler теперь работает в двух режимах: RTSP (продакшен) и V4L2 (разработка/тестирование).

## Current Task

- PRD, README и HTML-инструкция приведены в соответствие.
- В `.env` добавлен параметр `VIDEO_SOURCE` (rtsp / v4l2).
- В server-setup.html добавлен раздел проверки USB-камеры через v4l2-ctl и ffmpeg.
- Чек-лист дополнен пунктами для V4L2.

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
