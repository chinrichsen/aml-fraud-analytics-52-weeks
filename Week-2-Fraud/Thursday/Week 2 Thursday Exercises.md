# Week 2 Thursday Exercises — Account Takeover Behavioral Models

This folder contains the hands-on materials for **Week 2 Thursday** of the 52-week AML and fraud analytics series.

The theme for this week is **account takeover (ATO) behavioral models**. The key idea is that takeover fraud often shows up as a change in behavior rather than a single obvious event. A customer may suddenly use a new device, change IP location, reset a password, add payees quickly, or move money shortly after suspicious access. Those patterns can be strong indicators of compromise.

These exercises are important because they help the reader understand one of the most practical truths in fraud analytics:

> **ATO usually appears as a cluster of abnormal behaviors.**

The goal is not to build a production fraud engine. The goal is to create a clear learning artifact that shows how login, device, profile, and transaction changes can be combined into a meaningful behavioral model.

---

## What is included in this folder?

This folder includes:
- a synthetic dataset with ATO behavior indicators,
- an Exercise 1 solution file,
- an Exercise 2 solution file,
- and this instruction file.

The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.

---

## Why these exercises are important

ATO detection matters because takeover attacks often move quickly and quietly.

Examples include:
- new device usage,
- new IP addresses,
- repeated failed logins,
- password resets,
- rapid payee additions,
- profile changes,
- and transaction activity that starts right after access changes.

If fraud detection only looks at isolated events, it can miss the behavior cluster that defines an account takeover attack. These exercises help show how multiple signals can be combined into a stronger risk view.

---

## Exercise 1 — Classify ATO behavior

### Objective

Use the synthetic dataset to evaluate each customer’s activity and decide whether the behavior looks normal, elevated, or high risk.

### What you should do

1. Review each customer record in the synthetic dataset.
2. Compare current behavior against the customer baseline.
3. Identify signs of suspicious access or takeover.
4. Classify each case as normal, elevated, or high risk.
5. Recommend the most appropriate monitoring action.

### Why this exercise matters

This exercise is important because it teaches how ATO detection focuses on **behavioral change** rather than just one transaction or login event.

A customer may not show a single massive transfer, but if they suddenly use a new device, fail multiple logins, reset the password, and add payees quickly, the pattern can still be highly suspicious.

### Deliverable

Create a solution table with at least the following columns:
- `customer_id`
- `customer_name`
- `ato_score`
- `behavior_category`
- `recommended_action`
- `monitoring_rationale`

---

## Exercise 2 — Map fraud inputs to monitoring outputs

### Objective

Build a mapping file that connects ATO-related signals to downstream monitoring actions.

### What you should do

1. Build a mapping file with the following columns:
   - `fraud_input`
   - `risk_relevance`
   - `monitoring_output`
   - `example_use_case`
2. Include fields such as:
   - new device flag,
   - new IP flag,
   - login failures,
   - password reset,
   - payee additions,
   - email change,
   - phone change,
   - login geography change.
3. For each input, explain how it influences ATO monitoring.
4. Link each input to at least one downstream output such as:
   - ATO flag,
   - step-up authentication,
   - anomaly flag,
   - risk score,
   - escalation rule.
5. Save the output as a CSV or spreadsheet.

### Why this exercise matters

This exercise is important because it makes the connection between **behavioral signals** and **monitoring logic** explicit.

It helps the reader understand that ATO detection is not about one isolated indicator. It is about combining access, identity, device, and transaction signals into a pattern that looks more like an attacker than the legitimate account holder.

### Deliverable

Create a mapping table with at least the following columns:
- `fraud_input`
- `risk_relevance`
- `monitoring_output`
- `example_use_case`

---

## How to use the files

- Open the synthetic dataset and inspect the behavior patterns.
- Work through Exercise 1 before reviewing the solution file.
- Use the Exercise 2 mapping file to understand how fraud inputs translate into monitoring logic.
- Review the solution files to check your interpretation.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- recognize signs of account takeover behavior,
- compare current behavior to a baseline,
- identify when multiple suspicious signals form a takeover pattern,
- and explain how fraud signals should drive monitoring decisions.

That is a critical skill in fraud analytics, because a strong fraud program needs both **good behavioral signals** and **good decision logic**.
