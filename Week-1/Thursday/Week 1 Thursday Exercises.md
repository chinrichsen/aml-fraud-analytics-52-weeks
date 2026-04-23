# Week 1 Monday Exercises

These two exercises are designed to help the reader move from **conceptual AML knowledge** to **practical analytical thinking**.

A risk-based AML framework is important because transaction monitoring does not work well in isolation. Monitoring quality depends on the quality of the upstream customer context, including who the customer is, what activity is expected, which products and channels are used, and whether the profile carries higher-risk characteristics.

In other words, if onboarding data is weak, expected behavior is weak, and the monitoring process becomes noisier, less targeted, and harder to defend. These exercises are important because they make that connection visible.

---

## Exercise 1 — Build the baseline

### Why this exercise is important

This exercise is important because it teaches one of the core ideas behind risk-based AML: **customer context should shape monitoring expectations**.

A monitoring engine should not treat every customer the same way. A domestic salaried retail customer, a cross-border business, and a high-net-worth client with mixed funding sources do not present the same type of risk and should not be monitored with identical expectations.

This exercise helps the reader understand how onboarding fields can be turned into a practical baseline for monitoring. It also shows why two customers with similar transaction volumes may deserve different levels of scrutiny if their underlying profiles are materially different.

### Objective

Use the synthetic customer dataset to create a basic monitoring baseline.

### Tasks

1. Review each customer profile in the synthetic dataset.
2. Identify which fields are most useful for initial risk assessment.
3. Create a simple risk category such as **Low**, **Medium**, or **High**.
4. Define expected behavior based on the customer profile.
5. Compare expected behavior against the sample activity values.
6. Document which customers would likely receive more monitoring attention and explain why.

### Suggested fields to review

- `customer_type`
- `geography`
- `product_type`
- `channel`
- `source_of_funds`
- `expected_monthly_txn_count`
- `actual_monthly_txn_count`
- `expected_monthly_txn_amount_usd`
- `actual_monthly_txn_amount_usd`
- `adverse_flags`

### Expected output

Create a small analytical table with at least the following columns:

- `customer_id`
- `risk_category`
- `expected_behavior_summary`
- `monitoring_attention`
- `monitoring_rationale`

---

## Exercise 2 — Map KYC inputs to monitoring outputs

### Why this exercise is important

This exercise is important because it makes the bridge between **KYC/CDD inputs** and **transaction monitoring design** explicit.

In many AML programs, onboarding information is collected, but the operational link between customer data and monitoring logic is not always clearly documented. This exercise helps show that KYC is not just a compliance formality. It is an operational input into alert design, risk scoring, review prioritization, and escalation workflows.

It is also important from an analytics perspective because it helps analysts explain *why* a field matters, *how* it affects monitoring logic, and *where* it should influence downstream controls.

### Objective

Create a mapping file that connects onboarding attributes to monitoring outputs.

### Tasks

1. Build a mapping file with the following columns:
   - `kyc_input`
   - `risk_relevance`
   - `monitoring_output`
   - `example_use_case`
2. Include fields such as:
   - geography
   - customer type
   - product type
   - channel
   - source of funds
   - expected activity
   - adverse flags
3. For each input, explain how it affects monitoring design.
4. Link each input to at least one downstream output such as:
   - risk score
   - alert threshold
   - review frequency
   - escalation rule
   - typology flag
5. Save the output as a CSV or spreadsheet.

### Expected output

Create a mapping table that clearly explains how customer information gathered during onboarding can influence downstream monitoring rules, review intensity, and investigative prioritization.

---

## Files used in these exercises

- `week1_synthetic_customer_dataset.csv`
- `week1_exercise1_solution.csv`
- `week1_exercise2_solution.csv`

## Final note

These exercises are intentionally simple. The goal is not to simulate a full production AML program. The goal is to build a clear analytical foundation that shows how customer context feeds monitoring logic.
