# Week 1 Thursday — Hands-On Exercises

This folder contains the hands-on materials for **Week 1 Thursday** of the AML and fraud analytics series.

The purpose of these exercises is to show a simple but very important truth in financial crime analytics:

> **Alert quality is only as good as the data feeding the monitoring system.**

When upstream data is incomplete, stale, duplicated, or misclassified, the downstream alert environment becomes less reliable. These exercises are designed to make that relationship visible and practical.

---

## What is included in this folder?

This folder includes:
- a synthetic dataset with intentional data quality issues,
- an Exercise 1 solution file,
- an Exercise 2 solution file,
- and this instruction file.

The goal is not to simulate a full production AML environment. The goal is to create a clear learning artifact that helps readers understand how upstream data problems affect alert quality.

---

## Why these exercises are important

This topic matters because transaction monitoring depends on the quality of the input data.

If customer records are missing key fields, if risk ratings are stale, if transaction codes are wrong, or if customer updates are delayed, the monitoring engine may produce:
- false positives,
- missed alerts,
- weak segmentation,
- poor escalation decisions,
- and lower investigative confidence.

That means data quality is not just a technical concern. It is a **financial crime control issue**.

---

## Exercise 1 — Identify the data quality issue

### Objective

Inspect each record in the synthetic dataset and determine what data quality issue is present.

### What you should do

1. Review each record in the dataset.
2. Identify the data quality issue.
3. Explain how the issue could affect alert quality.
4. Decide whether the problem is likely caused by the rule itself or by upstream data.
5. Suggest the most likely remediation.

### Why this exercise matters

This exercise is important because it teaches that bad alerts are not always caused by bad rules.

In many cases, the real issue is upstream: a missing geography field, a stale risk rating, a duplicate customer profile, or incorrect transaction coding. If analysts only look at the alert, they may miss the true root cause.

### Deliverable

Create a solution table with at least the following columns:
- `record_id`
- `customer_id`
- `issue_flag`
- `monitoring_issue`
- `root_cause`
- `alert_quality_assessment`
- `recommended_fix`

---

## Exercise 2 — Map data quality issues to monitoring outcomes

### Objective

Build a mapping file that connects data quality problems to their downstream monitoring impact.

### What you should do

1. Build a mapping file with the following columns:
   - `data_issue`
   - `where_it_occurs`
   - `monitoring_impact`
   - `likely_alert_outcome`
   - `possible_control`
2. Include issues such as:
   - missing geography,
   - stale risk rating,
   - duplicate customer record,
   - incorrect transaction coding,
   - missing expected activity,
   - delayed onboarding update.
3. For each issue, explain how it changes monitoring behavior.
4. Link each issue to at least one downstream consequence such as:
   - false positives,
   - missed alerts,
   - mis-segmentation,
   - weak escalation,
   - reduced investigation confidence.
5. Save the output as a CSV file.

### Why this exercise matters

This exercise is important because it makes the connection between **data quality** and **alert quality** explicit.

A control failure may begin long before the alert appears. In AML, the monitoring system often reflects the quality of the upstream data environment, so understanding this link is essential for both analysts and control owners.

### Deliverable

Create a mapping table with at least the following columns:
- `data_issue`
- `where_it_occurs`
- `monitoring_impact`
- `likely_alert_outcome`
- `possible_control`

---

## How to use the files

- Open the dataset and inspect the records.
- Work through the exercises before looking at the solutions.
- Use the solution files to check your understanding.
- Use the mapping file as a reference for how upstream defects can translate into monitoring problems.

---

## Learning outcome

By the end of these exercises, the reader should be able to:
- identify common upstream data quality problems,
- explain how those problems affect alert quality,
- distinguish between a rule problem and a data problem,
- and describe how monitoring controls depend on the reliability of customer and transaction data.

That is a critical skill in AML analytics, because a strong monitoring program needs both **good logic** and **good data**.
