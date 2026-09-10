# Canonical profile — Gleb / Глеб

> Source of truth for platform drafts. Full case write-ups: [portfolio-freelance.md](./portfolio-freelance.md).
> Platform paste drafts: [profiles/upwork.md](./profiles/upwork.md).
> **Insert by hand. Do not publish with a bot.** Rate/hourly: **$40/hr**.

---

## Identity

| | |
|---|---|
| Name | Gleb Vigursky / Глеб Евгеньевич |
| Public role | Web-Developer (Marketing) — do not copy the rest of the AlexHost /about/ team list |
| Plugin / public git | `gloutlaw` — advertise `https://github.com/gloutlaw/ppt` (plus approved snapshots such as `live-price-booking-v4`) |
| Languages of copy | RU + EN below; Kwork = RU; LinkedIn/Upwork = EN unless noted |
| Hourly / package rate | $40/hr |
| LinkedIn | slug `vigurskiygleb`; location Chișinău, Moldova |

---

## Positioning (RU)

**WordPress/i18n для хостинга и кастомизация HostBill:** мультиязычный каталог (13 локалей), AI-плагин перевода, конфигураторы тарифов ↔ биллинг, overlay client area, live-chat и калькуляторы.

Кастомизирую HostBill и собираю мультиязычные WordPress-витрины хостинга. На проде AlexHost: overlay биллинга; сайт на 13 языках с плагином Polyglot Power Tools, конфигураторами тарифов и синхронизацией CID/стока; status page (пилот); live-chat. Также: Profi Designs (NL/EN), Booking V4 iPro. Внутренний CRM и Notion-бот — только как internal tools, без URL.

## Positioning (EN)

Multilingual WordPress for hosting (13 locales, AI i18n plugin, HostBill-linked configurators), HostBill client-area customization, live chat + RAG, and booking calculators. Production for hosting brands and an interior studio (NL).

I build multilingual hosting websites and customize HostBill. Production: alexhost.com (13 locales, Polyglot Power Tools, HostBill-linked configurators); HostBill client-area overlay; status page (pilot); live-chat widgets; Profi Designs (NL/EN); iPro Booking V4. Stack: PHP, WordPress, HostBill API, Node.js, Socket.IO, Maps APIs. I do not claim sole authorship of the entire AlexHost theme.

---

## Stack (production, confirmed)

- HostBill client area: overlay redesign without editing Smarty; PHP hooks; Google OAuth2 / Telegram / WebAuthn Passkey; Turnstile; order-funnel analytics
- WordPress: custom themes; Polylang; ACF; Yoast; AI i18n plugin (PPT: translation queue, menu/taxonomy sync, CLI, portable filters)
- Hosting catalog ↔ HostBill: configurators, CID clusters, stock/OOS cron
- Online calculators / booking wizards: pricing engine, Google Places + Directions + Distance Matrix, multi-step form, i18n
- Status page / monitoring (pilot): Node.js, Express SSR, probe quorum, incidents, Email/Telegram subscribers
- Live chat: widget, Socket.IO, Telegram operators, RAG (embeddings in MySQL, no vector DB), React admin, multi-brand
- Design system: CSS/JSON tokens, components, custom JS
- PHP, Node.js, MySQL, Redis, JS modules, Sass/CSS, i18n (including RTL)

---

## Showcase cases (6)

Do not paste the full CASE text into profiles. One problem → solution → result line + the public URL is enough. Details: [portfolio-freelance.md](./portfolio-freelance.md).

### 1. HostBill client-area overlay (AlexHost)

Stock HostBill did not match the brand. Overlay: design tokens, CSS, ~60 JS modules, inject via PHP hook; **no edits to 169 `.tpl` files**. Custom Google (OAuth2 + PKCE), Telegram Login, WebAuthn Passkey (not in the HostBill installer) + method panel in Settings + Turnstile. Order-funnel analytics on the billing side. Live client area, UI in 6 languages.

- **URL:** https://bill.alexhost.com/ (login: https://bill.alexhost.com/login/)
- **Do not mix** with the WordPress marketing site (case 2).

### 2. alexhost.com + Polyglot Power Tools + HostBill configurators

Hosting catalog on 13 locales. PPT (public repo, v2.4.0): editor one-click → translation queue (HTML chunking, code-block protection). CPT services: Polylang links only, no AI on prices/CID. Menu/taxonomy sync, CLI audits. Configurators build HostBill order links by CID. Stock cron every 30 min. CID cluster updates (Ryzen 78 posts, Moldova U 39). **Do not write "I wrote the entire theme alone"** (git authorship is mostly not a personal name). Lead with PPT, configurators, CID/stock.

- **URLs:** https://alexhost.com · https://github.com/gloutlaw/ppt
- **Not a prod demo:** https://dev.alexhost.com (noindex)

### 3. Profi Designs (NL)

Custom WordPress theme from scratch (no parent): token design system, CPT projects + 10 ACF sections, archive/single, services, contact, Polylang Pro. Production: 7 published real projects × EN+NL, request form, Yoast + JSON-LD LocalBusiness, Complianz, WebP/cache. No payments; prices on the services page.

- **URL:** https://profidesigns.nl
- PPT on that site is **not** this plugin (header: another team).

### 4. iPro Booking V4 calculator (London)

Custom wizard instead of "email the manager": 4 steps, 5 car classes, One Way / Hourly, up to 3 stops. Pricing engine: airport floor + overage, P2P miles, hourly, fixed stadium/polo/festival, VAT 20%, night tariff, Congestion Charge only where needed. Google Directions (shortest, Distance Matrix fallback), Places, flight check. QA: **47 of 67 routes wrong → 24/24 after the fix** (false airport floor, CCZ as multiplier, M25 detour). No in-form payments.

- **URLs:** live form https://iprochauffeur.com/book-the-car-form/ · site https://iprochauffeur.com · **Upwork sample:** https://github.com/gloutlaw/live-price-booking-v4 (wizard-only public snapshot)

### 5. AlexHost Status Page *(pilot)*

Node.js/Express SSR status page that should not die with the main stack: probe quorum, incidents, maintenance, Email/Telegram subscribers, Last-Known-Good snapshot. Live: https://status.alexhost.com (HTTP 200). **Pilot:** one live probe; multi-probe quorum and live Zabbix are not on yet. Say "in development / pilot" in profiles.

### 6. Live-chat widget + RAG (AlexHost and Ava Hosting)

Self-hosted chat, no SaaS operator console: Vanilla JS widget, Socket.IO, Telegram operators, RAG with embeddings in MySQL. Two isolated instances, same codebase. Widget in 13 languages. Public AI answers only with supervised Telegram mode.

- **URLs:** https://alexhost.com/widget/widget.js · https://ava.hosting/widget/widget.js
- Separate from the WordPress `ai-faq-chat` plugin. Do not publish internal helped/partial/not_helped counts as a "deflection %".

---

## Anonymous / internal tools (2)

Use only as "internal tools". **No URLs, hostnames, screenshots, or names.**

### 7. Internal legal/document CRM *(medium)*

Small legal team: inbound official requests (deadlines, files, statuses) + internal document catalog. Express + MySQL, cookie sessions, React/TS SPA. Files on disk, not object storage. Auth: lockout, login rate limit, idle sessions, localhost behind nginx, noindex. In production: MySQL + disk (the spec mentioned Postgres/S3; do not pretend those shipped).

### 8. Telegram → Notion mentions bot *(medium)*

Mention in a work Telegram group → Notion card (text + media). Long polling, not the live-chat process. Multi-mention → multiple assignees; edited message updates the card. Fail-closed chat list. No public demo.

---

## Featured / portfolio URLs (public)

Use these in LinkedIn Featured and Upwork portfolio. Skip CRM, Notion bot, Bybit, and `dev.alexhost.com`.

1. https://alexhost.com
2. https://github.com/gloutlaw/ppt
3. https://bill.alexhost.com/
4. https://profidesigns.nl
5. https://github.com/gloutlaw/live-price-booking-v4 (Upwork this pass). Live form exists but is not the Upwork link.
6. https://status.alexhost.com (label as **pilot**)
7. Widgets: `https://alexhost.com/widget/widget.js`, `https://ava.hosting/widget/widget.js`

---

## Short bullets (RU)

- Кастомизирую HostBill client area без форка ядра и без правок Smarty-шаблонов
- Overlay UI: дизайн-токены, CSS-слой, JS-модули, инжект через PHP-хуки
- Подключаю вход Google, Telegram и Passkey (WebAuthn) + панель методов входа в Settings
- Делаю онлайн-калькуляторы и многошаговый booking: живая цена, Google Maps API, тарифные правила
- Собираю аналитику воронки заказа и захват click ID на стороне биллинга
- Делаю мультиязычные WP-сайты хостеров: 13 локалей, AI-перевод, sync меню/таксономий
- Связываю каталог с HostBill: конфигураторы, CID, сток/OOS
- Делаю сайты под ключ на кастомной теме WordPress: дизайн-система, CPT/ACF, NL/EN
- Собираю публичные status page: кворум probe, инциденты, подписки (сейчас пилот)
- Делаю self-hosted live-chat: виджет, Telegram-операторы, RAG, мультибренд без форка
- Собираю внутренние CRM и ботов: workflow + файлы, Telegram → Notion (без публикации URL и имён)

## Short bullets (EN)

- HostBill client area customization without forking core or Smarty templates
- Overlay UI, PHP hooks, Google/Telegram/Passkey sign-in
- Live pricing calculators and multi-step booking wizards (Maps APIs, tariff rules)
- Order-funnel analytics and ad click-ID capture on the billing side
- Multilingual hosting WordPress: AI i18n plugin, menu/taxonomy sync, HostBill configurators and stock
- Full-cycle custom WordPress themes: design system, CPT/ACF, NL/EN
- Public status pages: probe quorum, incidents, Email/Telegram subscribers (pilot)
- Self-hosted live chat: widget, Telegram operators, RAG, multi-brand isolation
- Internal tools: small CRM workflows, Telegram→Notion task bots (anonymized in public profiles)

---

## Bans (never in public profiles)

- Bybit portfolio monitor (weak; keys/balances)
- URL / hostname of the police/legal CRM
- Keys, `.env`, wp-config, ppt-settings screenshots, tokens, cookies, session IDs
- Git remotes under `gloutlaw` except public `ppt` and approved snapshots
- "I wrote the entire AlexHost theme alone"
- Invented traffic %, conversion %, deflection %, revenue
- Copying the whole About-page team
- GitHub HTML landings from 2019 (`glebas.github.io` and siblings)
- Chat-widget helped/partial/not_helped counts as marketing metrics
- Claiming PPT on Profi Designs
- Mixing HostBill overlay (case 1) with the WP site (case 2)
- Mixing chat-widget Node app with the WP `ai-faq-chat` plugin

## Gaps

- Hourly rate: **$40/hr** (Upwork profile)
- HostBill overlay: no git on the 2019 theme; no before/after screenshots without PII
- alexhost.com: no business metrics in repo; ~210 truncated FAQ is debt, not a win; PPT license header GPL vs `composer.json` proprietary (agree before offering the plugin)
- Status page is a pilot (1 probe)
- CRM / Notion bot: anonymous only
- Queue not yet collected: AVA hosting site/panel, universalcare.ch, kssautos, proflider
- LinkedIn: Experience title must not stay "AI Automation"; Featured / photo / banner still open
