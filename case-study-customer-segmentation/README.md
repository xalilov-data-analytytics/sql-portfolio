# Customer Transaction Amount Segmentation (Percentile-Based)

## Overview
This SQL case study demonstrates how transaction amounts can be segmented into categories using percentile-based logic.
The goal is to transform raw transactional data into meaningful business insights by identifying customer spending levels.

The solution calculates percentiles (P10–P90) and assigns each transaction into a corresponding category such as low, medium, or high value.

---

## Business Objective
Financial institutions and businesses often need to understand customer behavior.
Instead of using fixed thresholds, this project uses data-driven segmentation to classify transaction amounts relative to the overall distribution.

This helps answer questions such as:
- Who are low-spending customers?
- Who are high-value customers?
- How are transaction values distributed?

---

## Methodology

### Step 1 — Calculate Percentiles
Percentiles (10% to 90%) are calculated using `PERCENTILE_CONT` on transaction amounts.

### Step 2 — Categorize Transactions
Each transaction is compared with percentile thresholds and assigned to a category:
- Below Threshold
- 0–10 Percentile
- 10–20 Percentile
- ...
- 80–90 Percentile
- 90–100 Percentile (highest value transactions)

### Step 3 — Aggregate Results
The final output aggregates:
- number of entities in each category
- minimum transaction amount
- maximum transaction amount

---

## Technical Skills Demonstrated
- SQL analytical functions
- Window/ordered set functions
- Data segmentation logic
- CASE expressions
- Aggregations
- Business interpretation of data

---

## Data Privacy
All table names, column names, and business identifiers are fully anonymized.
The original business logic and analytical structure are preserved for portfolio demonstration purposes.

---

## Tools
- SQL (Oracle compatible syntax)
- GitHub for version control
