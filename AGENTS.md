# Documentation project instructions

## About this project

- Developer documentation for [Itaja](https://www.getitaja.com), built on
  [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter; configuration lives in `docs.json`
- The design system is normative: [`DESIGN.md`](./DESIGN.md) — *Malachite &
  Cuivre*. Brand tokens are applied in `docs.json` (colors, fonts, background,
  logo). Do not introduce colors or fonts outside that file and `DESIGN.md`.

## Terminology

- Use **merchant of record** on first mention, then **MoR** is acceptable
- Use **payout** (not "withdrawal") for merchant reversals
- Use **payment provider** or **PSP** — pick one per page and stay consistent
- Use **settled**, **pending**, and **failed** for payment statuses
- Product name is **Itaja**; never "ITAJA" in prose

## Style preferences

- Write in **English** — developer docs are English even though the marketing
  site is trilingual
- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Amounts are written in ink, tabular figures, ISO 4217 code in capitals after
  the amount: `25 000 XOF` — never `25 000 F`, never a bare symbol

## Content boundaries

- Itaja is in **private beta** (since September 2026). Do not write as if the
  product were generally available.
- Never invent statistics, market figures, customer names, testimonials, or
  usage numbers. Verified claims only.
- Do not document endpoints, dashboard paths, or credentials that are not
  confirmed by the engineering team.
- Legal fields that depend on the operating entity (RCCM, jurisdiction) stay
  unfilled until the entity choice is final.
