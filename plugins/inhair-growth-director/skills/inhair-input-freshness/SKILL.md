---
name: inhair-input-freshness
description: Freshness gate for dynamic INHAIR.cz internal inputs stored in the private GitHub repository krausik85/INHAIR. Use before substantial audits, strategy, assortment/product recommendations, category work or any task whose result could materially change with newer internal exports or business inputs.
---

# INHAIR Input Freshness Gate

Use the private GitHub repository **krausik85/INHAIR**, especially `/input`, as the governed workspace for dynamic user-supplied inputs.

## Purpose
Do not make the user repeat current internal data in chat when it can be read from the repository. At the same time, do not silently base important recommendations on stale exports.

## Required behavior
Before a substantial INHAIR task that depends on dynamic internal inputs:
1. Inspect `krausik85/INHAIR/input` and the relevant README/instructions.
2. Identify which files are actually relevant to the task.
3. Check whether the relevant input exists, is plausibly complete and is fresh enough for the decision.
4. If fresh enough, use it without asking the user to re-upload it.
5. If missing, empty, obviously incomplete, conflicting or materially stale, explicitly ask the user to refresh that specific input in the repository.
6. State exactly which file/export is needed and why.

## Reasonable freshness defaults
These are defaults, not rigid expiry rules:
- live GA4/GSC/Google Ads/OpenAI Ads: use the connected live source; do not ask for duplicate exports;
- product/category/catalog exports: normally consider refresh when older than about **14 days** for product-level, availability, URL or assortment decisions;
- current campaign, promotion, price, stock or merchandising inputs: normally refresh when older than about **7 days** if material to the task;
- strategic priorities, business constraints, margin/ROAS guardrails or quarterly plans: normally refresh when older than about **30 days**, or sooner if the user signals a change;
- stable templates, brand voice and evergreen rules: do not ask for updates merely because time has passed.

Freshness is contextual. A six-week-old product export may still be adequate for an evergreen copy-style task, but not for an exact current product recommendation.

## Do not nag
Do not ask for updated inputs on every turn. Ask only when the missing/stale input could materially alter the answer or implementation.

When several related inputs are stale, consolidate the request into one concise update request instead of interrupting repeatedly.

## Current repository convention
Primary dynamic input location: `krausik85/INHAIR/input/`.
Existing README says exports may include files such as `products.csv`, `categories.csv`, `urls.csv`, `sitemap.xml`, `search_console.csv`, `ga4_landing_pages.csv`, and that the file schema must be inspected rather than assumed.

Never assume a column exists. Inspect the actual file structure first.

## Conflict policy
When repository input conflicts with live first-party data or the current INHAIR website:
- prefer live first-party data for measured performance;
- prefer current live product/page facts for public availability/content when directly verifiable;
- flag the conflict if it affects a recommendation;
- ask the user for an updated internal input when the internal business truth cannot be inferred safely.
