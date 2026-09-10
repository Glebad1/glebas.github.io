# glebas.github.io

MyBrain: общий слой для **Cursor** и **Claude Code**. Старый лендинг лежит в `build/`.

## Синхронизация агентов

| Файл | Кто читает |
|---|---|
| `AGENTS.md` | Cursor, Codex и другие агенты. Источник правды. |
| `CLAUDE.md` | Claude Code (одна строка `@AGENTS.md`). Не копировать правила сюда. |
| `.agents/skills/` | Скиллы. Cursor читает отсюда. |
| `.claude/skills/` | Симлинк на те же скиллы для Claude Code. |

Править только `AGENTS.md` и файлы в `.agents/skills/`.

Канон фриланса: `docs/profile.md`, `docs/profiles/upwork.md`, `docs/portfolio-freelance.md`.

Скилл откликов Upwork: `/upwork-client-comms` (после вставки джоба, инвайта или сообщения клиента).

Если включите GitHub Pages, источник должен быть **`/build`**, чтобы инструкции агентов не стали сайтом.
