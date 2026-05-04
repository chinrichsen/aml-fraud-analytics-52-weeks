# Week 3 Monday Exercises — CRR Model Inputs & Weighting

This folder contains the hands-on materials for **Week 3 Monday** of the 52-week AML and fraud analytics series.

The theme for this week is **customer risk rating (CRR)**. The key idea is that risk ratings are not based on one field alone. A good CRR model combines multiple customer inputs, applies weights, and produces a consistent risk view that can support due diligence and escalation.

These exercises are important because they help the reader understand one of the most practical truths in AML analytics:

> **Moving the weights can change the risk rating.**

The goal is not to build a production risk engine. The goal is to create a clear learning artifact that shows how customer attributes can be translated into a risk score and how different weighting schemes can change the final rating.

---

## What is included in this folder?

This folder includes:
- a synthetic customer dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution file,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

CRR matters because AML teams need a structured way to identify which customers require more scrutiny.

Examples include:
- different customer types,
- domestic vs. cross-border activity,
- product and channel differences,
- source of funds,
- ownership complexity,
- adverse media,
- PEP exposure,
- and sanctions proximity.

If the model does not weight inputs carefully, it may understate high-risk customers or overstate low-risk ones. These exercises help show how scoring logic changes when weights are adjusted.

---

## Exercise 1 — Calculate the CRR score

### Objective

Use the synthetic dataset to calculate a customer risk score using a weighted formula.

### What you should do

1. Review each customer record in the synthetic dataset.
2. Assign a score to each risk input.
3. Apply a weighted formula to calculate the CRR score.
4. Convert the score into a risk tier such as Low, Medium, or High.
5. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how CRR models turn customer information into a numeric risk view.

It also shows that changing the weight of a single factor can change the final score and potentially the risk tier. That is one of the most important ideas in model design and tuning.

### Example formula

A simple CRR formula could look like this:

`CRR Score = (Customer Type × 0.20) + (Geography × 0.15) + (Product × 0.15) + (Channel × 0.10) + (Source of Funds × 0.10) + (Ownership Complexity × 0.10) + (Adverse Media × 0.10) + (PEP × 0.05) + (Sanctions × 0.05)`

You can tune the weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `customer_id`
- `customer_name`
- `crr_score_formula`
- `risk_tier`
- `monitoring_action`

---

## Exercise 2 — Compare two weighting schemes

### Objective

Recalculate the CRR score using two different sets of weights and observe how the final risk tier changes.

### What you should do

1. Use the same synthetic customer dataset.
2. Apply Weight Set A.
3. Apply Weight Set B.
4. Compare the resulting scores and risk tiers.
5. Identify which customers changed risk tiers when the weights were adjusted.

### Why this exercise matters

This exercise is important because it shows that a CRR model is not static.

When weights change, the model can prioritize different risk drivers. For example, a scheme that emphasizes geography more heavily may push cross-border customers higher, while another scheme that emphasizes adverse media more heavily may change the ranking of customers with reputation concerns.

### Deliverable

Create a comparison table with at least the following columns:
- `customer_id`
- `customer_name`
- `score_weights_a`
- `tier_weights_a`
- `score_weights_b`
- `tier_weights_b`
- `tier_changed`

---

## How to use the files

- Open the synthetic dataset and inspect the customer attributes.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how tuning weights affects the rating.
- Review the solution files to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- calculate a simple CRR score,
- understand how different customer inputs contribute to the score,
- see how changing weights affects the final rating,
- and explain how CRR supports review and due diligence decisions.

That is a critical skill in AML analytics, because a strong risk model needs both **good inputs** and **good weighting logic**.
