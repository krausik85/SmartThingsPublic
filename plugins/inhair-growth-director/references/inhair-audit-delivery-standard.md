# INHAIR audit delivery standard

This standard defines the minimum quality of every substantial INHAIR audit.

## Core principle
**Finding a problem is only half of the job. The audit must tell the user exactly how to correct it.**

Apply `inhair-audit-priority-order.md` before ranking ordinary SEO/content findings.

## Mandatory demand-first order
Default sequence:
1. P1A — missing assets with proven demand/value;
2. P1B — query/content gaps;
3. P2 — weak existing assets;
4. P3 — enrichment.

Critical analytics, legal, trust or indexation failures may override this sequence.

## Required report structure
### 1. Audit header / baseline
State audit date, source freshness, live data ranges, sources used and limitations.

### 2. Executive summary
Summarize the highest-value findings, with special emphasis on:
- what is missing completely;
- which missing assets already have measurable demand;
- which query gaps can be closed quickly;
- what should not be changed.

### 3. Priority roadmap
Use P1A/P1B/P2/P3 and practical execution order.

### 4. Finding detail
Each issue must include:
**WHAT IS WRONG / EVIDENCE / AFFECTED SCOPE / BUSINESS-SEARCH IMPACT / EXACT FIX / WHERE-HOW / METHOD / DEPENDENCIES / CONFIDENCE / VALIDATION**

### 5. Current -> recommended diff
For text/field changes always provide current value when reliably verified and the complete proposed value.

### 6. Mandatory implementation export
When file creation is available, every substantial audit must produce a **downloadable XLSX and/or CSV**, not only chat prose.

Preferred sheets:
- `01_Chybejici_metadata_kategorie`
- `02_Kategorie_bez_FAQ`
- `03_Produkty_search_demand_bez_metadata`
- `04_Produkty_query_content_gap`
- `05_Chybejici_interni_odkazy`
- `06_P2_optimalizace`
- `07_Konkurence`
- `08_Tracking_Ads`

Preferred columns:
`issue_id,priority,entity_type,sku,url,query,impressions,clicks,ctr,position,field,current_value,recommended_value,action,admin_location,method,evidence,business_impact,confidence,dependency,validation,status`

`recommended_value` may never say only improve/rewrite/optimize/review/fix.

### 7. Verification wave
Define refresh data, comparison window, baseline vs after, success criteria and next decision.

## Category FAQ
Do not add FAQ mechanically. Prioritize when real GSC query demand, commercial importance or customer decision friction supports it. Export the complete ready-to-paste FAQ.

## Product SEO
Do not optimize all products equally. Prioritize products with search demand/value. Map query clusters to missing verified product information and close the smallest supported gap.

## Confidence
HIGH = directly verified.
MEDIUM = strong evidence, one material fact needs confirmation.
LOW = hypothesis.
BLOCKED FOR IMPLEMENTATION = exact fix cannot safely be specified yet.

## Healthy-state reporting
Include KEEP / DO NOT CHANGE. Do not manufacture work.
