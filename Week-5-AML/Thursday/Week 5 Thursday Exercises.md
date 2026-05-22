```md
# Week 5 Thursday Exercises — Structuring & Smurfing Detection Rules


This folder contains the hands-on materials for **Week 5 Thursday** of the 52-week AML and fraud analytics series.

The theme for this week is **structuring and smurfing detection rules**. The key idea is that suspicious transaction behavior often looks ordinary in isolation, but becomes suspicious when you combine threshold proximity, repeated activity, aggregation, segmentation, and pattern logic into a clear monitoring rule.

These exercises are important because they help the reader understand one of the most practical truths in AML analytics:

> **Structuring and smurfing are most useful to detect when fragmented transaction behavior is turned into a clear review decision.**

The goal is not to build a production AML monitoring platform. The goal is to create a clear learning artifact that shows how transaction behavior can be translated into structuring and smurfing detection logic.

---

## What is included in this folder?

This folder includes:
- a synthetic AML transaction dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution file,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Structuring and smurfing matter because suspicious activity rarely announces itself clearly.

Examples include:
- cash deposits just below reporting thresholds,
- repeated activity within short time windows,
- unusual spikes in transaction frequency,
- activity inconsistent with the expected customer profile,
- high-risk geography or channel usage,
- and customer behavior that suggests structuring or smurfing.

If the institution does not score these signals together, the review process can miss suspicious activity that appears routine on the surface. These exercises help show how a pattern-based workflow can route transactions to the right review path.

---

## Exercise 1 — Detect structuring with SQL

### Objective

Use the synthetic dataset to identify structuring behavior in SQL and assign an alert band.

### What you should do

1. Review each transaction record in the synthetic dataset.
2. Flag transactions that appear just below reporting thresholds.
3. Aggregate customer activity across a lookback window.
4. Calculate a structuring score using explicit SQL logic.
5. Assign an alert band such as Low, Medium, or High.
6. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how raw transaction behavior becomes a usable AML monitoring view.

It also shows that repeated small deposits or withdrawals can be more suspicious than a single large transaction when the pattern indicates intentional threshold avoidance.

### Example logic

A simple structuring logic could look like this:

`structuring_score = threshold_proximity + repeat_cash_activity + aggregation + velocity`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `transaction_id`
- `customer_name`
- `structuring_score`
- `risk_band`
- `recommended_action`

---

## Exercise 2 — Detect smurfing with SQL

### Objective

Use the synthetic dataset to identify smurfing behavior in SQL and assign an alert band.

### What you should do

1. Review transaction clusters across multiple customers or linked records.
2. Look for repeated small transactions spread across accounts, channels, or time windows.
3. Identify commonalities such as shared timing, shared counterparties, or repeated cash behavior.
4. Calculate a smurfing score using explicit SQL logic.
5. Assign an alert band such as Low, Medium, or High.
6. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because smurfing often appears as distributed structuring across multiple actors, which makes it harder to spot with a single-record view.

It also shows that a networked or clustered pattern can be more revealing than a standalone transaction pattern.

### Example logic

A simple smurfing logic could look like this:

`smurfing_score = shared_activity + repeated_small_transactions + linked_entities + short_time_window`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `cluster_id`
- `customer_name`
- `smurfing_score`
- `risk_band`
- `recommended_action`

---

## How to use the files

- Open the synthetic dataset and inspect the transaction signals.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the SQL rules support AML detection of smurfing behavior.
- Review the solution file to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize when transaction behavior looks like structuring,
- understand how repeated small transactions can create AML risk,
- explain why distributed activity may indicate smurfing,
- and use SQL to model simple threshold-avoidance detection flows.

That is a critical skill in AML analytics, because a strong monitoring design needs both **good transaction signals** and **clear decision logic**.
```