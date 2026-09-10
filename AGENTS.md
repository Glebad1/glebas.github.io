# MyBrain — shared agent instructions

This repository is Gleb Vigursky's MyBrain workspace (`glebas.github.io`).
`build/` is an old 2019 HTML landing. Do not treat it as the freelance portfolio.

These instructions are the always-on layer for **Cursor** (reads `AGENTS.md`) and **Claude Code** (`CLAUDE.md` imports this file). Edit this file only; do not duplicate the rules in `CLAUDE.md`.

## How to talk

- Talk to Gleb in **Russian**. Step-by-step click guides when filling a website UI.
- Client-facing drafts (Upwork, LinkedIn, email) in **English**, unless the client wrote Russian.
- Insert by hand. **Never publish, submit, scrape, or boost with a bot.**
- Do not invent metrics, English level, freelance start date, cases, or URLs.

## Identity (public)

- Name: **Gleb Vigursky**. GitHub: **`gloutlaw`**. In-house: AlexHost SRL from March 2023. Freelance is separate (Profi Designs, iPro).
- Rate: **$40/hr** (range discussed: $35–50). Do not undercut to match cheap payroll.
- Availability: about 15–20 hours/week when relevant.
- Public plugin repo to advertise: `https://github.com/gloutlaw/ppt` only, unless a cleaned snapshot was explicitly approved (e.g. `live-price-booking-v4`).

## Honesty

- Not sole author of the AlexHost marketing theme.
- **13 locales**, not 16.
- Status page is a **pilot** (one probe).
- WooCommerce, n8n, Automation, Ecommerce: not showcase skills and not cases until a real one ships.
- Employer live URLs (`alexhost.com`, `bill.alexhost.com`, status) are OK on LinkedIn. On Upwork, HostBill overlay may appear in Title/Overview **without** the billing URL until Gleb confirms.
- Internal CRM, Telegram→Notion, Bybit: anonymous or omitted. No hostnames, no keys.

## Canon (read, do not invent)

1. `docs/profile.md` — source of truth
2. `docs/profiles/upwork.md` — Upwork paste draft
3. `docs/portfolio-freelance.md` — case write-ups

Canon is the **profile and proof list**, not a cage. Stretch jobs are allowed if the pitch stays honest.

## Skills (Claude + Cursor)

Project skills live in **`.agents/skills/`** (Agent Skills standard; Cursor loads this natively).

Claude Code loads **`.claude/skills/`**, which is a symlink to the same folders. Edit the files under `.agents/skills/` only.

When Gleb pastes an Upwork job, invite, screening questions, or a client message, use **`upwork-client-comms`**.

## Secrets

Never publish, log, or commit tokens, API keys, `.env`, `wp-config`, `ppt-settings`, cookies, session IDs, or client PII. If they appear, replace with placeholders.

## GitHub Pages

If Pages is enabled, publish **`/build` only**. Agent files at the repo root must not become the live site.
