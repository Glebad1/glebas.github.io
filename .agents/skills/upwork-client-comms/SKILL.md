---
name: upwork-client-comms
description: >-
  Qualify Upwork jobs and invites against Gleb's canon, draft proposals, and
  answer clients in the same professional tone. Use when the user pastes a job,
  invite, screening questions, or a client message. Do not publish to Upwork.
---

# Upwork client comms (Gleb)

Combo skill. Not messages-only. Not a bot.

Load this when there is a job, invite, screening form, or a client question. Drafts stay in chat or this folder. The human pastes. Never submit, scrape, or auto-send on Upwork.

## Canon (read, do not invent)

Read before writing anything the client will see:

1. [docs/profile.md](../../../docs/profile.md)
2. [docs/profiles/upwork.md](../../../docs/profiles/upwork.md)
3. [docs/portfolio-freelance.md](../../../docs/portfolio-freelance.md)

Canon is the **profile and proof list**, not a cage. Rate **$40/hr**. Stage: **no-history** (no JSS, no Top Rated, no earnings story).

**Take / grow:** custom WordPress we can actually build (CPT, custom plugin, URL/SEO hygiene, import, overlays, calculators). Stretch jobs are allowed. We grow by shipping them, then add the case to the canon after it is live.

**Still never:** invent a case, invent listings or %, claim Woo/directory/HostBill work we did not ship, use another city-page plugin when they forbade it.

## Always this order

1. Analyze the offer.
2. Match the canon. Verdict first.
3. Propose on Fit, Weak fit, or Stretch (growth). Honest gap + first milestone.
4. Answer later questions in the same voice.

Skip means no proposal unless the user asks for a polite no. Skip is for lie-required briefs, banned plugins, or work we cannot do safely (not "missing from the portfolio").

## 1. Analyze

Pull, do not fluff:

- Task in one sentence
- Stack and deliverables
- Size (URLs, catalog, hours, duration)
- Hourly vs fixed, rate band vs $40
- Screening questions (answer all or do not apply)
- Client signals: hire rate, avg hourly paid, interviews already open, timezone
- Red flags: plugin-only brief, Woo/checkout, "senior + takeover", invent content, mass-redirect thin URLs, work outside canon

If the listing is incomplete, say what is missing. Do not invent the missing parts.

## 2. Match

Output **5–8 lines**, then stop or continue:

```
Verdict: Fit | Stretch | Weak fit | Skip
Why: …
Proof we may cite: … (live URLs from the canon only)
Gap we will not fake: …
Risk: scope / first-JSS / competition / rate
Connects: spend or save
First slice: …
```

### Stretch (default for growth)

Same engineering class (custom WP, PHP, MySQL, import, rewrites, SEO, live takeover of WP — not necessarily HostBill/i18n). We have not shipped this exact product yet. Apply. Say the closest live work, say the gap, book a small first slice. After it ships, add the case to the canon.

Examples: US city directory, plugin-off migration at scale, Woo audit/takeover if they accept an honest "no prior Woo store, strong live WP/PHP" pitch.

### Hard Skip

- They demand another directory/city plugin or city-name find-and-replace
- They require a lie (fake directory, fake Woo takeover, sole authorship of AlexHost)
- Invent listings / scrape junk into the index
- CRM / Bybit / secrets / `dev.alexhost.com`

WooCommerce is **Stretch or Skip by blast radius**, not a portfolio ban. Live payments + "describe the Woo takeover you did" with no such job = Stretch only if the pitch stays honest. Do not add Woo to the public profile until a real case exists.

### Weak fit

Stretch plus a bad table (19 interviews already, avg pay far below $40, huge fixed unknown). Still draft if Gleb wants to spend Connects.

### Fit

Hosting catalog, HostBill overlay, i18n plugin, custom theme (Profi), live-price calculator. Still scope before promising a date.

## 3. Proposal / invite

English. No em dashes. No JSS / Top Rated / invented %. Professional, direct, Solution Oriented.

Structure:

1. Two opening lines: restate their problem; one live fact from the canon.
2. How you would do **this** job (migration, data model, cutover). No generic WP speech.
3. Answers to every screening question, numbered as they asked.
4. Four to six scope questions if anything is still open.
5. Offer: **$40/hr** and honest weekly hours. Or a first milestone (audit / one template / import sample). No "whole catalog in N weeks" without counts.

Allowed proof URLs (pick 1–2 that match):

- https://alexhost.com
- https://github.com/gloutlaw/ppt
- https://bill.alexhost.com/
- https://profidesigns.nl
- https://iprochauffeur.com/book-the-car-form/
- https://status.alexhost.com (say **pilot**)

Templates: [templates.md](./templates.md).

## 4. Client questions

Same voice as the proposal. Do not widen the offer after they reply.

Default English. Russian only if they write Russian.

Cover: screening follow-up, access/staging, weekly (done / blocker / next), scope change with a new estimate, polite decline.

## Bans (from the canon)

Never write: Bybit; CRM hostname; keys, tokens, `.env`, wp-config, ppt-settings; any `gloutlaw` repo except `ppt` and approved public snapshots; sole authorship of the AlexHost theme; traffic/conversion/deflection %; full About-page team; 2019 GitHub HTML landings; chat helped/not_helped counts; PPT on Profi Designs; mixing HostBill overlay with the WP site; mixing the Node chat widget with `ai-faq-chat`.

Do not list WooCommerce as a skill or a case.
