# INHAIR Growth Director — Claude Code plugin

Soukromý řídicí agent pro INHAIR.cz převedený z verze 0.5.1 do formátu pluginu Claude Code.

## Obsah
- `skills/` — 17 rolí (growth director, audit director, SEO, GEO/AIO, paid, FAQ, produkty, poradna, chat, QA…). Claude je spouští automaticky podle popisu úkolu.
- `references/` — 12 původních referenčních souborů (včetně 3 HTML šablon) + `claude-adaptation.md` (routing a pravidla pro Claude Code).
- `commands/` — slash příkazy:
  - `/inhair-growth-director:inhair <zadání>` — obecný vstupní bod,
  - `/inhair-growth-director:audit [rozsah]` — komplexní demand-first audit s exportem,
  - `/inhair-growth-director:chat <dotaz zákazníka>` — rychlá odpověď do chatu.

## Instalace
```
/plugin marketplace add krausik85/SmartThingsPublic
/plugin install inhair-growth-director@krausik85-plugins
```
Lokální test bez marketplace: `claude --plugin-dir ./plugins/inhair-growth-director`.

## Konektory
Plugin neobsahuje žádné přihlašovací údaje. GA4, Search Console, Google Ads a privátní repozitář `krausik85/INHAIR` používá jen přes konektory (MCP servery), které máte v Claude sami připojené a autorizované.
