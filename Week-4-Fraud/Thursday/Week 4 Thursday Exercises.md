# Week 4 Thursday Exercises — Fraud Propensity Scoring Techniques

This folder contains the hands-on materials for **Week 4 Thursday** of the 52-week AML and fraud analytics series.

The theme for this week is **fraud propensity scoring techniques**. The key idea is that synthetic identity cases often look normal in isolation, but become suspicious when you combine identity depth, reuse, linkage, and consistency into a single score or model.

These exercises are important because they help the reader understand one of the most practical truths in fraud analytics:

> **Fraud propensity scoring is most useful when it converts weak identity signals into a clear review decision.**

The goal is not to build a production fraud model. The goal is to create a clear learning artifact that shows how identity quality signals can be translated into a propensity score and a simple decision tree.

---

## What is included in this folder?

This folder includes:
- a synthetic fraud dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution notebook,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Synthetic identity fraud matters because the profile may not look obviously false.

Examples include:
- thin-file applications,
- short account age,
- mismatched identity details,
- reused phone, email, or address data,
- shared devices,
- high IP risk,
- and linked records across multiple identities.

If the institution does not score these signals together, the review process can miss suspicious identities that appear legitimate on the surface. These exercises help show how a pattern-based workflow can route customers to the right review path.

---

## Exercise 1 — Score fraud propensity

### Objective

Use the synthetic dataset to calculate a fraud propensity score and assign a risk band.

### What you should do

1. Review each customer record in the synthetic dataset.
2. Score the identity quality and reuse signals.
3. Calculate a propensity score using explicit formulas.
4. Assign a risk band such as Low, Medium, or High.
5. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how raw identity signals become a usable fraud risk view.

It also shows that different combinations of thin files, short account age, reuse, and linkage can produce very different risk outcomes. That is one of the most important ideas in synthetic identity detection.

### Example logic

A simple scoring logic could look like this:

`propensity_score = identity_depth + reuse_signals + linkage_signals + IP risk`

You can tune the thresholds and scoring weights to see how the output changes.

### Deliverable

Create a solution table with at least the following columns:
- `application_id`
- `customer_name`
- `propensity_score`
- `risk_band`
- `monitoring_action`

---

## Exercise 2 — Build the fraud propensity decision tree

### Objective

Build a simple decision tree in Python using the synthetic dataset and use it to classify customers into low-risk or potentially synthetic identity cases.

### What you should do

1. Use the same synthetic fraud dataset.
2. Define a target label based on the manual risk tier.
3. Train a decision tree classifier.
4. Review the decision rules that the model learns.
5. Apply the model to the customer cases.
6. Compare the predicted result against the expected result.

### Why this exercise matters

This exercise is important because it makes the fraud propensity logic explicit and easy to explain.

It also shows how a decision tree can mirror business logic in a readable form. That is especially useful in fraud analytics, where explainability matters as much as accuracy.

### Deliverable

Create a notebook output with at least the following:
- the synthetic fraud dataset,
- the target label definition,
- the trained decision tree,
- the learned decision rules,
- and the final prediction table.

---

## How to use the files

- Open the synthetic dataset and inspect the identity signals.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the decision tree supports fraud propensity scoring.
- Review the solution notebook to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize when an identity profile looks synthetic,
- understand how identity reuse and linkage affect fraud risk,
- explain why thin files and shared attributes matter,
- and use a decision tree to model a simple synthetic identity detection flow.

That is a critical skill in fraud analytics, because a strong detection model needs both **good identity signals** and **clear decision logic**.