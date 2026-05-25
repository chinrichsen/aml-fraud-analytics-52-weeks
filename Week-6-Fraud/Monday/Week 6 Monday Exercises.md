# Week 6 Monday Exercises — Card-Not-Present (CNP) Fraud Analytics


This folder contains the hands-on materials for **Week 6 Monday** of the 52-week AML and fraud analytics series.

The theme for this week is **card-not-present (CNP) fraud analytics**. The key idea is that suspicious card activity often looks ordinary when viewed only through the payment amount, but becomes suspicious when you combine device risk, channel behavior, billing and shipping mismatch, velocity, authentication failures, and merchant context into a clear monitoring rule or model.

These exercises are important because they help the reader understand one of the most practical truths in fraud analytics:

> **CNP fraud is most useful to detect when digital signals are turned into a clear review decision.**

The goal is not to build a production fraud platform. The goal is to create a clear learning artifact that shows how card-not-present transaction behavior can be translated into CNP fraud detection logic.

---

## What is included in this folder?

This folder includes:
- a synthetic CNP transaction dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution notebook,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Card-not-present fraud matters because the cardholder is not physically present, so the institution must rely on digital and behavioral signals instead of face-to-face verification.

Examples include:
- new or risky devices,
- billing and shipping mismatches,
- repeated authorization attempts,
- unusual velocity,
- suspicious merchant categories,
- and customer behavior that does not fit the expected payment profile.

If the institution does not score these signals together, the review process can miss suspicious activity that appears normal on the surface. These exercises help show how a pattern-based workflow can route transactions to the right review path.

---

## Exercise 1 — Detect CNP fraud with SQL

### Objective

Use the synthetic dataset to identify card-not-present fraud risk in SQL and assign an alert band.

### What you should do

1. Review each transaction record in the synthetic dataset.
2. Flag transactions with risky device, channel, or authentication behavior.
3. Compare billing and shipping country or address-related signals.
4. Calculate a CNP fraud score using explicit SQL logic.
5. Assign an alert band such as Low, Medium, or High.
6. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how raw CNP transaction behavior becomes a usable fraud monitoring view.

It also shows that a combination of device risk, mismatch signals, velocity, and authentication failures can be more suspicious than a single isolated feature.

### Example logic

A simple CNP fraud logic could look like this:

`cnp_score = device_risk + mismatch + velocity + auth_fail + merchant_risk`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `txn_id`
- `customer_name`
- `cnp_score`
- `risk_band`
- `recommended_action`

---

## Exercise 2 — Predict CNP fraud risk with Python

### Objective

Build a simple decision tree in Python to classify CNP transactions into Low, Medium, or High fraud risk.

### What you should do

1. Use the same synthetic CNP transaction dataset.
2. Define a target label based on the manual review tier.
3. Train a decision tree classifier.
4. Review the decision rules that the model learns.
5. Apply the model to the transaction cases.
6. Compare the predicted result against the expected result.

### Why this exercise matters

This exercise is important because it makes CNP fraud logic explicit and easy to explain.

It also shows how a decision tree can mirror fraud business rules in a readable form. That is especially useful in fraud analytics, where explainability matters as much as accuracy.

### Example logic

A simple model could use:

`predicted_risk = decision_tree(device_risk, billing_shipping_mismatch, velocity, auth_fail, merchant_category)`

You can tune the depth and feature set to see how the output changes.

### Deliverable

Create a notebook output with at least the following:
- the synthetic CNP transaction dataset,
- the target label definition,
- the trained decision tree,
- the learned decision rules,
- and the final prediction table.

---

## How to use the files

- Open the synthetic dataset and inspect the transaction signals.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the decision tree supports CNP fraud detection.
- Review the solution notebook to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize when card-not-present transaction behavior looks suspicious,
- understand how device and mismatch signals affect fraud risk,
- explain why velocity and authentication failures matter,
- and use SQL or Python to model a simple CNP fraud detection flow.

That is a critical skill in fraud analytics, because a strong monitoring design needs both **good digital signals** and **clear decision logic**.