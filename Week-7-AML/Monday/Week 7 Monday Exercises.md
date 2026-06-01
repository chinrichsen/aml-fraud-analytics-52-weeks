# Week 7 Monday Exercises — Geographic Risk Corridor Analysis


This folder contains the hands-on materials for **Week 7 Monday** of the 52-week AML and fraud analytics series.

The theme for this week is **geographic risk corridor analysis**. The key idea is that suspicious activity often looks ordinary when viewed in isolation, but becomes more suspicious when you combine origin and destination geography, corridor risk, customer profile fit, transaction concentration, and jurisdiction-based exposure into a clear monitoring rule or model.

These exercises are important because they help the reader understand one of the most practical truths in AML analytics:

> **Geographic risk is most useful to detect when location signals are turned into a clear review decision.**

The goal is not to build a production AML platform. The goal is to create a clear learning artifact that shows how cross-border transaction behavior can be translated into geographic risk detection logic.

---

## What is included in this folder?

This folder includes:
- a synthetic geographic corridor dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution notebook,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Geographic risk matters because the transaction may be routine on its own, but the corridor can reveal AML exposure.

Examples include:
- activity involving higher-risk jurisdictions,
- repeated flows through the same corridor,
- unusual cross-border patterns,
- sudden changes in origin or destination geography,
- transaction clustering in a specific route,
- and customer behavior that does not fit the expected geographic profile.

If the institution does not score these signals together, the review process can miss suspicious activity that appears normal on the surface. These exercises help show how a pattern-based workflow can route transactions to the right review path.

---

## Exercise 1 — Detect geographic risk with SQL

### Objective

Use the synthetic dataset to identify geographic risk in SQL and assign an alert band.

### What you should do

1. Review each transaction or customer record in the synthetic dataset.
2. Flag corridors involving higher-risk jurisdictions or unusual cross-border activity.
3. Compare origin and destination geography against the expected customer profile.
4. Calculate a geographic risk score using explicit SQL logic.
5. Assign an alert band such as Low, Medium, or High.
6. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how raw geography becomes a usable AML monitoring view.

It also shows that a combination of corridor risk, profile mismatch, activity concentration, and corridor change can be more suspicious than a single isolated country flag.

### Example logic

A simple geographic risk logic could look like this:

`geo_score = corridor_risk + profile_mismatch + corridor_change + activity_concentration + high_risk_jurisdiction`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `corridor_id`
- `customer_name`
- `geo_score`
- `risk_band`
- `recommended_action`

---

## Exercise 2 — Predict geographic risk with Python

### Objective

Build a simple decision tree in Python to classify geographic corridors into Low, Medium, or High AML risk.

### What you should do

1. Use the same synthetic geographic corridor dataset.
2. Define a target label based on the manual review tier.
3. Train a decision tree classifier.
4. Review the decision rules that the model learns.
5. Apply the model to the corridor cases.
6. Compare the predicted result against the expected result.

### Why this exercise matters

This exercise is important because it makes geographic risk logic explicit and easy to explain.

It also shows how a decision tree can mirror AML business rules in a readable form. That is especially useful in AML analytics, where explainability matters as much as accuracy.

### Example logic

A simple model could use:

`predicted_risk = decision_tree(high_risk_jurisdiction, profile_mismatch, corridor_change_flag, txn_count_30d, total_amount_30d)`

You can tune the depth and feature set to see how the output changes.

### Deliverable

Create a notebook output with at least the following:
- the synthetic geographic corridor dataset,
- the target label definition,
- the trained decision tree,
- the learned decision rules,
- and the final prediction table.

---

## How to use the files

- Open the synthetic dataset and inspect the geographic signals.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the decision tree supports geographic risk detection.
- Review the solution notebook to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize when geographic activity looks suspicious,
- understand how corridor and jurisdiction signals affect AML risk,
- explain why profile fit and corridor changes matter,
- and use SQL or Python to model a simple geographic risk detection flow.

That is a critical skill in AML analytics, because a strong monitoring design needs both **good geographic signals** and **clear decision logic**.