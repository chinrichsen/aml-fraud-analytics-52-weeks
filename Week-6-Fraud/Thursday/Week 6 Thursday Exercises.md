# Week 6 Thursday Exercises — Friendly Fraud & First-Party Fraud Signals


This folder contains the hands-on materials for **Week 6 Thursday** of the 52-week AML and fraud analytics series.

The theme for this week is **friendly fraud and first-party fraud signals**. The key idea is that some suspicious activity only becomes visible after the transaction, when disputes, chargebacks, refunds, and return patterns are combined into a clear monitoring rule or model.

These exercises are important because they help the reader understand one of the most practical truths in fraud analytics:

> **Friendly fraud is most useful to detect when dispute and return signals are turned into a clear review decision.**

The goal is not to build a production fraud platform. The goal is to create a clear learning artifact that shows how customer dispute behavior can be translated into friendly fraud detection logic.

---

## What is included in this folder?

This folder includes:
- a synthetic dispute and refund dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution notebook,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Friendly fraud matters because the original payment may not look suspicious, but later dispute behavior can reveal abuse.

Examples include:
- repeated chargebacks,
- excessive refund requests,
- return abuse,
- dispute abuse,
- loss concentration on the same customer or card,
- and behavior that is inconsistent with the expected customer profile.

If the institution does not score these signals together, the review process can miss suspicious first-party abuse that appears routine at first. These exercises help show how a pattern-based workflow can route disputes and returns to the right review path.

---

## Exercise 1 — Detect friendly fraud with SQL

### Objective

Use the synthetic dataset to identify friendly fraud risk in SQL and assign an alert band.

### What you should do

1. Review each customer record in the synthetic dataset.
2. Flag high dispute, refund, or return behavior.
3. Compare current activity to customer history or loss patterns.
4. Calculate a friendly fraud score using explicit SQL logic.
5. Assign an alert band such as Low, Medium, or High.
6. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how post-transaction dispute behavior becomes a usable fraud monitoring view.

It also shows that a combination of chargebacks, refunds, returns, and repeated losses can be more suspicious than a single isolated event.

### Example logic

A simple friendly fraud logic could look like this:

`friendly_fraud_score = chargeback_behavior + refund_behavior + return_behavior + loss_history + dispute_pattern`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `customer_id`
- `customer_name`
- `friendly_fraud_score`
- `risk_band`
- `recommended_action`

---

## Exercise 2 — Predict first-party fraud risk with Python

### Objective

Build a simple decision tree in Python to classify customers into Low, Medium, or High first-party fraud risk.

### What you should do

1. Use the same synthetic dispute and refund dataset.
2. Define a target label based on the manual review tier.
3. Train a decision tree classifier.
4. Review the decision rules that the model learns.
5. Apply the model to the customer cases.
6. Compare the predicted result against the expected result.

### Why this exercise matters

This exercise is important because it makes first-party fraud logic explicit and easy to explain.

It also shows how a decision tree can mirror fraud business rules in a readable form. That is especially useful in fraud analytics, where explainability matters as much as accuracy.

### Example logic

A simple model could use:

`predicted_risk = decision_tree(chargeback_count, refund_count, return_rate, dispute_rate, loss_history)`

You can tune the depth and feature set to see how the output changes.

### Deliverable

Create a notebook output with at least the following:
- the synthetic dispute and refund dataset,
- the target label definition,
- the trained decision tree,
- the learned decision rules,
- and the final prediction table.

---

## How to use the files

- Open the synthetic dataset and inspect the dispute and refund signals.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the decision tree supports friendly fraud detection.
- Review the solution notebook to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize when customer dispute behavior looks suspicious,
- understand how chargebacks and refunds affect fraud risk,
- explain why return abuse and loss history matter,
- and use SQL or Python to model a simple friendly fraud detection flow.

That is a critical skill in fraud analytics, because a strong monitoring design needs both **good post-transaction signals** and **clear decision logic**.