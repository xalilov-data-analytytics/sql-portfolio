# Case Study: External Inflows to Student Cards (Under Age 18)

## Business Problem
Banks must monitor transactions performed on student cards owned by customers under 18 years old.
In some cases, these cards receive frequent incoming transfers from third parties, which may indicate that the card is being used by someone else or represents a potential risk behavior.

The purpose of this analysis is to detect and analyze such external inflows.

---

## Objectives
- Identify customers under 18 who own student cards
- Detect incoming transactions from external accounts
- Calculate total inflow amounts
- Classify customer behavior based on inflow activity
- Provide data for monitoring and risk control

---

## Data Description
The dataset contains anonymized banking transaction data including:

- customer_id
- card_type
- transaction_type
- amount
- transaction_date

All identifiers are masked to preserve confidentiality.

---

## Analysis Steps
1. Select customers under 18 with student cards
2. Filter incoming transactions from external accounts
3. Aggregate transaction amounts
4. Analyze inflow behavior patterns
5. Prepare data for monitoring and risk detection

---

## SQL Skills Used
- CASE WHEN logic
- JOIN operations
- CTE (WITH clause)
- Aggregations (SUM, COUNT)
- Filtering and business rule implementation

---

## Business Value
This analysis helps the bank to:
- detect possible third-party card usage
- monitor financial activity of minors
- support fraud and compliance teams
- identify suspicious transaction patterns early
