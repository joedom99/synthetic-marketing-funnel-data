# Synthetic Marketing Funnel Dataset

![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)
![Dataset](https://img.shields.io/badge/type-synthetic%20dataset-lightgrey.svg)
![Rows](https://img.shields.io/badge/rows-100%2C000-brightgreen.svg)
![Focus](https://img.shields.io/badge/focus-imbalanced%20data-orange.svg)
![Use Case](https://img.shields.io/badge/use%20case-marketing%20analytics-blueviolet.svg)

This repository contains a synthetic, event-level marketing dataset designed to demonstrate **imbalanced data** and **signal-to-noise challenges** commonly encountered in real-world marketing analytics.

The dataset mirrors a typical digital marketing funnel, where meaningful outcomes (like conversions) are rare relative to overall activity.

This dataset is discussed in more detail in the article  
**_Why Many Marketing Models Fail: The Problem of Imbalanced Data_**  
https://blog.marketingdatascience.ai/why-many-marketing-models-fail-the-problem-of-imbalanced-data-ceb8123b80b3

---

## Dataset Overview

Each row represents a single ad impression and tracks progression through a marketing funnel.

### Funnel Ratios

Out of 100,000 impressions:

- 2,000 clicks (2% CTR)
- 100 leads (5% of clicks)
- 5 conversions (5% of leads)

Overall conversion rate: **0.005%**

This level of imbalance is intentional and reflects real marketing environments.

---

## File Description

### `synthetic_marketing_funnel_100k.csv`

**Columns:**

- `impression_id` – Unique identifier for each impression  
- `clicked` – Binary indicator (1 = click occurred)  
- `lead` – Binary indicator (1 = lead generated)  
- `converted` – Binary indicator (1 = conversion occurred)  
- `stage` – Highest funnel stage reached  
  (`Impression`, `Click`, `Lead`, `Conversion`)

---

## Intended Use Cases

This dataset is well-suited for:

- Demonstrating imbalanced classification problems
- Teaching confusion matrices and misleading accuracy metrics
- Exploring signal vs. noise in marketing data
- Practicing techniques such as class weighting, resampling, and threshold tuning
- Examples in Excel, R, and Python

---

## Important Notes

- This dataset is **synthetic** and contains no real customer or advertising data.
- It is intended for **educational and illustrative purposes only**.
- The imbalance is a feature, not a flaw.

---

## Related Content

This dataset accompanies articles and tutorials published at:  
**https://blog.marketingdatascience.ai**

---

## License

This project is licensed under the MIT License.
