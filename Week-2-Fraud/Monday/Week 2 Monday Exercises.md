# Week 2 Monday Exercises — Velocity Fraud Detection Patterns

This folder contains the hands-on materials for **Week 2 Monday** of the 52-week AML and fraud analytics series.

The theme for this week is **velocity fraud detection patterns**. The key idea is that fraud often shows up as speed, repetition, or a sudden change in behavior. A customer who suddenly logs in many times, adds multiple payees, changes devices, or sends transactions much faster than normal may be showing signs of account takeover or another fast-moving fraud event.

These exercises are important because they help the reader understand one of the most practical truths in fraud analytics:

> **Fraud often appears first as an unusual burst of activity.**

The goal is not to build a production fraud engine. The goal is to create a simple, clear learning artifact that shows how velocity patterns can be used to identify suspicious behavior and prioritize review.

---

## What is included in this folder?

This folder includes:
- a synthetic dataset with velocity and account takeover indicators,
- an Exercise 1 solution file,
- an Exercise 2 solution file,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

Velocity-based detection matters because many fraud scenarios happen quickly.

Examples include:
- rapid login attempts,
- repeated failed logins,
- sudden transaction bursts,
- multiple payee additions,
- device changes,
- IP changes,
- and behavior that is far above the customer’s normal baseline.

If fraud detection only looks at isolated events, it can miss the sequence and speed that define the attack. These exercises help show how timing and repetition can become powerful signals.

---

## Exercise 1 — Classify velocity behavior

### Objective

Use the synthetic dataset to evaluate each customer’s activity and decide whether the pattern looks normal, elevated, or high risk.

### What you should do

1. Review each customer record in the synthetic dataset.
2. Compare current activity against the customer baseline.
3. Identify signs of unusual velocity.
4. Classify each case as normal, elevated, or high risk.
5. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how fraud detection can focus on **behavioral speed** rather than just transaction content.

A customer may not be spending unusual amounts, but if they are logging in many times, changing payees, or shifting devices rapidly, the pattern can still be highly suspicious.

### Deliverable

Create a solution table with at least the following columns:
- `customer_id`
- `customer_name`
- `velocity_score`
- `behavior_category`
- `recommended_action`
- `monitoring_rationale`

---

## Exercise 2 — Map fraud inputs to monitoring outputs

### Objective

Build a mapping file that connects fraud-related signals to downstream monitoring actions.

### What you should do

1. Build a mapping file with the following columns:
   - `fraud_input`
   - `risk_relevance`
   - `monitoring_output`
   - `example_use_case`
2. Include fields such as:
   - login attempts,
   - transaction bursts,
   - payee additions,
   - device changes,
   - IP changes,
   - failed logins,
   - baseline activity.
3. For each input, explain how it influences fraud monitoring.
4. Link each input to at least one downstream output such as:
   - velocity threshold,
   - anomaly flag,
   - risk score,
   - step-up authentication,
   - ATO flag.
5. Save the output as a CSV or spreadsheet.

### Why this exercise matters

This exercise is important because it makes the link between **fraud signals** and **monitoring logic** explicit.

It helps the reader understand that a fraud system should not only ask whether activity happened, but also **how fast**, **how often**, and **how differently** it happened compared to the customer baseline.

### Deliverable

Create a mapping table with at least the following columns:
- `fraud_input`
- `risk_relevance`
- `monitoring_output`
- `example_use_case`

---

## How to use the files

- Open the synthetic dataset and inspect the activity patterns.
- Work through Exercise 1 before reviewing the solution file.
- Use the Exercise 2 mapping file to understand how fraud inputs translate into monitoring logic.
- Review the solution files to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize velocity-based fraud patterns,
- compare current behavior to a baseline,
- identify signs of account takeover or suspicious rapid activity,
- and explain how fraud signals should drive monitoring decisions.

That is a critical skill in fraud analytics, because a strong fraud program needs both **good behavioral signals** and **good decision logic**.
