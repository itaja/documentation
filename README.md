# Itaja documentation

Developer documentation for [Itaja](https://www.getitaja.com) — the merchant of
record and monetization infrastructure for African SaaS.

Built on [Mintlify](https://mintlify.com). Pages are MDX files with YAML
frontmatter; configuration lives in `docs.json`.

## Design

The design system is normative and lives in
[`DESIGN.md`](./DESIGN.md) — *Malachite & Cuivre*. Brand tokens applied to this
site via `docs.json`:

| Token | Value | Role |
|---|---|---|
| Malachite `#0E5F52` | `colors.primary` | links, emphasis |
| Malachite claire `#5FB8A3` | `colors.light` | dark-mode emphasis |
| Malachite profonde `#0A4A40` | `colors.dark` | buttons, hover |
| Ivoire `#FAF8F3` | background (light) | canvas |
| Nuit minérale `#0A1F1B` | background (dark) | canvas |
| Rubik | body font | paragraphs, UI |
| Bricolage Grotesque | heading font | titles |

The logo mark is the *portique* (two posts and an arch): `logo/light.svg` in
nuit minérale on ivory, `logo/dark.svg` in ivory on nuit minérale. The copper
`#C0703A` is a fill color only — it never appears as text.

## Structure

The docs are **trilingual**: English at the root (default), French in `fr/`,
Spanish in `es/` — same file names and structure in each directory. Language
switcher and per-language navigation labels are configured in `docs.json`
(`navigation.languages`).

```
├── docs.json                    # site configuration (brand tokens, i18n navigation)
├── index.mdx · quickstart.mdx   # English (default)
├── merchant-of-record/          # the MoR section (en)
├── guides/index.mdx             # coming soon (en)
├── api-reference/index.mdx      # coming soon (en)
├── fr/                          # French mirror
│   ├── index.mdx · quickstart.mdx
│   ├── merchant-of-record/ …
│   ├── guides/index.mdx
│   └── api-reference/index.mdx
└── es/                          # Spanish mirror (same shape)
```

Navigation is organized in three tabs — **Documentation**, **Guides**, and
**API Reference** — per language, configured in `docs.json`.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint):

```bash
npm i -g mint
```

Run at the root of this repository, where `docs.json` lives:

```bash
mint dev
```

Preview at `http://localhost:3000`.

## Publishing

Changes deploy automatically through the Mintlify GitHub app when pushed to
`main`. No local deployment commands are needed or allowed.

## Troubleshooting

- Dev environment not running: `mint update` to get the latest CLI.
- Page loads as a 404: make sure you run `mint dev` from the folder with a
  valid `docs.json`.

[Mintlify documentation](https://mintlify.com/docs)
