# Week 5 Monday Exercises — Transaction Monitoring Scenario Design


This folder contains the hands-on materials for **Week 5 Monday** of the 52-week AML and fraud analytics series.

The theme for this week is **transaction monitoring scenario design**. The key idea is that suspicious activity often looks ordinary in isolation, but becomes suspicious when you combine thresholds, velocity, aggregation, segmentation, and pattern logic into a clear monitoring rule or model.

These exercises are important because they help the reader understand one of the most practical truths in AML analytics:

> **Transaction monitoring is most useful when it converts scattered transaction behavior into a clear review decision.**

The goal is not to build a production AML monitoring platform. The goal is to create a clear learning artifact that shows how transaction behavior can be translated into scenario logic and a simple decision tree.

---

## What is included in this folder?

This folder includes:
- a synthetic AML transaction dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution notebook,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Transaction monitoring matters because suspicious activity rarely announces itself clearly.

Examples include:
- cash deposits just below reporting thresholds,
- repeated activity within short time windows,
- unusual spikes in transaction frequency,
- activity inconsistent with the expected customer profile,
- high-risk geography or channel usage,
- and customer behavior that suggests structuring or smurfing.

If the institution does not score these signals together, the review process can miss suspicious activity that appears routine on the surface. These exercises help show how a pattern-based workflow can route transactions to the right review path.

---

## Exercise 1 — Build a SQL scenario rule

### Objective

Use the synthetic dataset to create a transaction monitoring scenario in SQL and assign an alert band.

### What you should do

1. Review each transaction record in the synthetic dataset.
2. Score threshold proximity, cash behavior, velocity, and risk indicators.
3. Calculate a scenario score using explicit SQL logic.
4. Assign an alert band such as Low, Medium, or High.
5. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how raw transaction behavior becomes a usable AML monitoring view.

It also shows that different combinations of threshold behavior, high activity, and risk flags can produce very different alert outcomes. That is one of the most important ideas in transaction monitoring design.

### Example logic

A simple scenario logic could look like this:

`scenario_score = threshold_pattern + cash_activity + velocity + risk_country_flag`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `transaction_id`
- `customer_name`
- `scenario_score`
- `risk_band`
- `recommended_action`

---

## Exercise 2 — Build the transaction monitoring decision tree

### Objective

Build a simple decision tree in Python using the synthetic dataset and use it to classify transactions into low-risk or potentially suspicious activity cases.

### What you should do

1. Use the same synthetic AML transaction dataset.
2. Define a target label based on the manual review tier.
3. Train a decision tree classifier.
4. Review the decision rules that the model learns.
5. Apply the model to the transaction cases.
6. Compare the predicted result against the expected result.

### Why this exercise matters

This exercise is important because it makes the transaction monitoring logic explicit and easy to explain.

It also shows how a decision tree can mirror business logic in a readable form. That is especially useful in AML analytics, where explainability matters as much as accuracy.

### Deliverable

Create a notebook output with at least the following:
- the synthetic AML transaction dataset,
- the target label definition,
- the trained decision tree,
- the learned decision rules,
- and the final prediction table.

---

## How to use the files

- Open the synthetic dataset and inspect the transaction signals.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the decision tree supports AML scenario design.
- Review the solution notebook to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize when transaction behavior looks suspicious,
- understand how thresholds and velocity affect AML risk,
- explain why aggregation and repeat activity matter,
- and use a decision tree to model a simple transaction monitoring detection flow.

That is a critical skill in AML analytics, because a strong monitoring design needs both **good transaction signals** and **clear decision logic**.