# INHAIR audit priority order — demand-first gap filling

This policy is mandatory for broad SEO/GEO/AIO/content audits.

## Core rule
Do **not** begin by rewriting assets that already exist and perform acceptably.

The first audit wave must find **missing assets or missing answers on URLs that already have evidence of demand or commercial importance**.

Prioritize with:
**GSC query + impressions + position + page state + GA4/commercial value + implementation effort**.

## P1A — MISSING COMPLETELY
Audit these first:
- missing TITLE;
- missing META DESCRIPTION;
- missing/invalid H1 where material;
- important category with no useful introductory/basic description;
- important category with no FAQ despite real question/decision intent;
- product with real organic demand but missing SEO metadata or useful product content;
- product/category with no relevant internal link path despite measurable demand;
- other essential SEO/content field that is genuinely absent.

Do not prioritize an empty field merely because it is empty. It becomes high priority when the page has measurable demand, commercial value, or strategic importance.

### Required output
For each P1A finding, provide the finished asset:
- NEW TITLE;
- NEW META DESCRIPTION;
- exact H1 if needed;
- full FAQ questions + answers via FAQ Agent;
- ready-to-paste content block;
- exact internal-link source + anchor + destination;
- exact field/admin location.

## P1B — DEMAND EXISTS, PAGE DOES NOT ANSWER IT
Next find pages where GSC/Ads/market evidence shows a real query/decision need but the page does not serve it.

Examples:
- product ranks for `[product] použití` but has no use instructions;
- product ranks for `[product] recenze` but lacks credible decision-support information;
- category ranks for question queries but has no FAQ;
- brand page ranks for product-line names but gives no route to those lines;
- query cluster indicates `pro koho`, `jak použít`, `na co`, `rozdíl`, `odstín`, `oxidant`, etc., but the page does not answer it.

Do not rewrite the entire page automatically. Add or replace the **smallest exact asset that closes the proven gap**.

## P2 — EXISTS BUT IS WEAK
Only after P1A/P1B:
- weak title;
- weak meta description;
- inaccurate or overbroad H1/intro;
- weak information architecture;
- low CTR where metadata already exists;
- weak internal linking;
- imprecise FAQ/content;
- cannibalization or structural optimization requiring refinement rather than filling an absence.

## P3 — ENRICHMENT / EXPANSION
After the above:
- competitor-inspired enrichment;
- GEO/AIO enrichment;
- deeper internal linking;
- extra supporting content;
- CRO experiments;
- optional structured enhancements.

## Category FAQ rule
Do not add FAQ mechanically to every category.

Prioritize FAQ when one or more applies:
- GSC exposes real question/decision queries;
- category has meaningful impressions/traffic/revenue;
- customers need selection guidance;
- competitor/search evidence shows a material information gap;
- FAQ can resolve product-choice friction.

The output must contain the actual FAQ in approved INHAIR HTML/template format, not “add FAQ”.

## Product SEO rule
Do not optimize every product equally.

Prioritize products with:
- non-trivial GSC impressions/clicks;
- identifiable product-name/brand/SKU query demand;
- queries indicating missing information;
- commercial value in GA4/Ads;
- strategic assortment importance.

For each product, compare query demand against current page content. Close only supported gaps and never invent ingredients, claims, use instructions, technical parameters or compatibility.

## Export-first audit delivery
Every substantial audit must, when file creation is available, deliver a **downloadable implementation export** in addition to the chat summary.

Preferred workbook sheets:
1. `01_Chybejici_metadata_kategorie`
2. `02_Kategorie_bez_FAQ`
3. `03_Produkty_search_demand_bez_metadata`
4. `04_Produkty_query_content_gap`
5. `05_Chybejici_interni_odkazy`
6. `06_P2_optimalizace`
7. `07_Konkurence`
8. `08_Tracking_Ads` when relevant

Every actionable row should include, as applicable:
`priority, url, sku, query, impressions, clicks, ctr, position, ga4_value, field, current_value, recommended_value, action, admin_location, evidence, confidence, validation`

The downloadable file is the implementation source of truth; the chat response summarizes priorities and links to it.
