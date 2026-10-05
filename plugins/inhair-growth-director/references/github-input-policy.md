# INHAIR GitHub dynamic-input policy

Repository: `krausik85/INHAIR`
Primary dynamic-input directory: `/input`

The repository is the user's working drop zone for current internal exports and operational inputs. The Growth Director should inspect it at sensible checkpoints and request refreshed inputs only when stale or missing data could materially affect the result.

## Ask the user for a refresh when needed
Use direct, specific wording, for example:

> Pro tento audit potřebuji aktuální export produktů. Soubor `input/products.csv` je chybějící/neúplný/starší než je vhodné pro produktové rozhodnutí. Nahrajte prosím nový export do `krausik85/INHAIR/input/products.csv`; až bude vložený, použiji jej jako aktuální zdroj.

Do not ask vaguely for "current data". Name the exact file or export required.

## Typical checkpoints
- before a broad monthly/quarterly Growth audit when internal catalog/business context matters;
- before product/category prioritization based on the current assortment;
- before creating customer recommendations when current product availability cannot be verified reliably elsewhere;
- before campaign/promotional strategy that depends on current commercial priorities;
- when a file is suspiciously small, empty, malformed or inconsistent with other sources.

## No duplicate requests
If a live connector already supplies the needed current data (GA4, GSC, Google Ads, OpenAI Ads), use it instead of asking the user to export the same data into GitHub.
