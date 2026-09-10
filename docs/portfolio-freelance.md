# Freelance portfolio canon — Gleb Vigursky

> Source of truth for case write-ups. Short profile copy: [profile.md](./profile.md).
> Upwork paste: [profiles/upwork.md](./profiles/upwork.md).
> **Insert by hand. Do not publish with a bot.** Rate: **$40/hr**.

Do not invent traffic, conversion, deflection, or revenue numbers. Do not claim sole authorship of the AlexHost marketing theme. Status page is a pilot.

---

## Commercial showcase (order of discovery)

### 1. HostBill client-area overlay (AlexHost)

- **Problem → solution → result.** Stock HostBill UI did not match the brand. Overlay via design tokens, CSS, ~60 JS modules, injected with a PHP hook. **No edits to 169 `.tpl` files.** Custom Google (OAuth2 + PKCE), Telegram Login, WebAuthn Passkey (not in the HostBill installer), method panel in Settings, Turnstile. Order-funnel analytics on the billing side. Live client area, UI in 6 languages.
- **Stack:** PHP, HostBill hooks, CSS/JS modules, OAuth2, WebAuthn, Turnstile
- **URL:** https://bill.alexhost.com/ (login: https://bill.alexhost.com/login/)
- **Do not mix** with the WordPress marketing site (case 2).
- **Upwork:** may mention overlay in Title/Overview without the billing URL until Gleb confirms.

### 2. alexhost.com + Polyglot Power Tools + HostBill configurators

- **Problem → solution → result.** Hosting catalog on **13 locales** (not 16). PPT (public repo): editor one-click → translation queue (HTML chunking, code-block protection). CPT services: Polylang links only, no AI on prices/CID. Menu/taxonomy sync, CLI audits. Configurators build HostBill order links by CID. Stock cron every 30 min. CID cluster updates.
- **Stack:** WordPress, Polylang, ACF, PHP, WP-CLI, HostBill API
- **URLs:** https://alexhost.com · https://github.com/gloutlaw/ppt
- **Not a prod demo:** https://dev.alexhost.com (noindex)
- Lead with PPT, configurators, CID/stock — not "I wrote the entire theme".

### 3. Profi Designs (NL)

- **Problem → solution → result.** Custom WordPress theme from scratch (no parent): token design system, CPT projects + 10 ACF sections, archive/single, services, contact, Polylang Pro. Production: 7 published real projects × EN+NL, request form, Yoast + JSON-LD LocalBusiness, Complianz, WebP/cache. No payments.
- **Stack:** WordPress, Polylang Pro, ACF, Yoast, custom theme
- **URL:** https://profidesigns.nl
- PPT on that site is **not** this plugin.

### 4. iPro Booking V4 calculator (London)

- **Problem → solution → result.** Custom wizard instead of "email the manager": 4 steps, 5 car classes, One Way / Hourly, up to 3 stops. Pricing engine: airport floor + overage, P2P miles, hourly, fixed stadium/polo/festival, VAT 20%, night tariff, Congestion Charge only where needed. Google Directions (shortest, Distance Matrix fallback), Places, flight check. QA: **47 of 67 routes wrong → 24/24 after the fix**. No in-form payments.
- **Stack:** custom JS/PHP, Google Places + Directions + Distance Matrix
- **URLs:** https://iprochauffeur.com/book-the-car-form/ · https://iprochauffeur.com · public snapshot https://github.com/gloutlaw/live-price-booking-v4 (wizard only)

### 5. AlexHost Status Page *(pilot)*

- **Problem → solution → result.** Public status page that should not die with the main stack: Node.js/Express SSR, probe quorum, incidents, maintenance, Email/Telegram subscribers, Last-Known-Good snapshot.
- **URL:** https://status.alexhost.com
- **Pilot:** one live probe. Multi-probe quorum and live Zabbix are not on yet. Say "pilot" in profiles.

### 6. Live-chat widget + RAG (AlexHost and Ava Hosting)

- **Problem → solution → result.** Self-hosted chat, no SaaS operator console: Vanilla JS widget, Socket.IO, Telegram operators, RAG with embeddings in MySQL. Two isolated instances, same codebase. Widget in 13 languages. Public AI answers only with supervised Telegram mode.
- **URLs:** https://alexhost.com/widget/widget.js · https://ava.hosting/widget/widget.js
- Separate from the WordPress `ai-faq-chat` plugin. Do not publish helped/not_helped counts as a deflection %.

---

## Anonymous / internal (do not put URLs in profiles)

### 7. Internal legal/document CRM *(medium)*

Small legal team: inbound official requests (deadlines, files, statuses) + internal document catalog. Express + MySQL, cookie sessions, React/TS SPA. Files on disk, not object storage. Auth: lockout, login rate limit, idle sessions, localhost behind nginx, noindex. In production: MySQL + disk (do not pretend Postgres/S3 shipped). **No URL, hostname, or screenshots.**

### 8. Telegram → Notion mentions bot *(medium)*

Mention in a work Telegram group → Notion card (text + media). Long polling, not the live-chat process. Multi-mention → multiple assignees; edited message updates the card. Fail-closed chat list. No public demo.

### Bybit alerts

Internal only. Never public. Keys/balances.

---

## Collect queue (not yet in the canon)

AVA hosting site/panel, universalcare.ch, kssautos, proflider.

---

## Profile drafts (do not publish with a bot)

- [profile.md](./profile.md) — shared source of truth (RU+EN)
- [profiles/upwork.md](./profiles/upwork.md) — Upwork paste

Rate/hourly: **$40/hr**.
