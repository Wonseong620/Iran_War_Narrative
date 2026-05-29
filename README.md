# Iran War Narrative — Multi-Lingual Media Dataset

A cross-lingual media-narrative dataset and lead-lag network visualization for the
2026 Iran crisis, covering news in **English, Persian, Arabic, and Chinese**.

## Contents

| File | Description |
|---|---|
| `dataset_iran_war_news_4languages_.json` | Public dataset (58,530 articles, metadata + LLM labels) |
| `index.html` | Interactive lead-lag network of economic sub-topics across the four languages |

## Live visualization

The interactive network is published via GitHub Pages:
**https://wonseong620.github.io/Iran_War_Narrative/**

## Dataset schema

Each record contains:

| Field | Description |
|---|---|
| `language` | Source language: `en`, `pe`, `ar`, `ch` |
| `id` | Article identifier |
| `published_at` | Publication timestamp |
| `source`, `provider`, `publisher_location` | Outlet metadata |
| `title` | Article headline |
| `url` | Article URL |
| `war_related` | Binary flag (1 = war-related) |
| `type_risk` | Risk type label |
| `negativity` | Sentiment negativity score (0–1) |
| `subtopic` | Primary sub-topic (12-label scheme) |
| `economic_subtopic` | Economic sub-topic (9 economic labels, else blank) |
| `llm_confidence` | Classifier confidence |

**Sub-topic scheme (12 labels):** `oil_energy`, `sanctions`, `transport_shipping`,
`currency_banking`, `supply_chain`, `food_security`, `macroeconomy`,
`general_economy`, `protest_strike`, `military`, `nuclear`, `none`.

## Data availability note

Raw article text (full body, fact/opinion extracts, and translations) is subject to
licensing restrictions and is **not** publicly redistributed. This release contains
article metadata and derived LLM labels only.

## Citation

If you use this dataset, please cite the accompanying manuscript (forthcoming, *Economics
of Peace and Security Journal*).
