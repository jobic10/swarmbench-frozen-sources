# OpenFoodFacts category-benchmark snapshot

A byte-stable snapshot of 216 packaged-food products across 18 retail
categories, taken from the Open Food Facts v2 search API on 2026-07-06 and
frozen here so agent containers fetch an identical copy each run.

- `index.json` — the 18 categories, each with its list of product codes and the
  raw-URL pattern for the per-product files.
- `products/<code>.json` — one trimmed record per product (name, brand,
  quantity, serving size, NOVA group, Nutri-Score, additive tags, allergen
  tags, ingredients text, and per-100g / per-serving nutriment values).
- `reference/nutrient_guidelines.json` — UK front-of-pack "red/high" thresholds
  (per 100 g for solids, per 100 ml for drinks).
- `reference/additives_classes.json` — E-number to functional-class lookup for
  the additives present in this snapshot.

Data © Open Food Facts contributors, made available under the Open Database
License (ODbL) v1.0 (https://opendatacommons.org/licenses/odbl/1-0/). Product
names and brands are trademarks of their respective owners.
