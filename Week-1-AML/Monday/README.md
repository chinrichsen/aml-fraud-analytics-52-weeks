# Week 1 - Monday | 🛡️ Risk-Based AML Foundations

Welcome to **Week 1** of the 52-week AML and fraud analytics series.

This first week is about one of the most important ideas in financial crime compliance: the **risk-based AML framework**. Before you can tune rules, analyze suspicious behavior, or build advanced models, you need to understand the logic that sits underneath the whole program.

This week’s Monday topic focuses on **how a risk-based AML program works**, why it matters, and how it connects to downstream transaction monitoring. In simple terms, this is where the program starts: if the foundation is weak, everything built on top of it becomes less effective.

---

## 🎯 Why this topic matters

A strong AML program is not built on random alerts or isolated controls. It is built on a framework that identifies, understands, and prioritizes risk.

That means the institution must ask:
- Who is the customer?
- What is the expected activity?
- What products and channels are being used?
- What geography is involved?
- What is the customer’s overall risk profile?
- What behavior should be considered normal or unusual?

If these questions are not answered well at onboarding and during ongoing review, then the transaction monitoring process becomes noisier, less targeted, and harder to defend.

This is why the risk-based approach is so important. It is not just a compliance requirement — it is the logic that makes the rest of the AML program usable.

---

## 🧠 Core concept

A **risk-based AML framework** means that the institution does not treat every customer, product, or transaction the same way.

Instead, it applies more attention and stronger controls where risk is higher, and lighter controls where risk is lower.

This approach matters because financial institutions operate at scale. They cannot investigate everything equally. They need to prioritize:
- higher-risk customers,
- higher-risk products,
- unusual geographies,
- suspicious behaviors,
- and relationships that do not match expected patterns.

In practice, the risk-based model is what helps AML teams decide:
- what to monitor,
- how intensely to monitor it,
- and when to escalate.

---

## 🔍 How this connects to transaction monitoring

This week is not just about theory. It is about the operational flow from **KYC/CDD to transaction monitoring**.

The connection is straightforward:
1. The customer is onboarded.
2. KYC and CDD information is collected.
3. The institution forms an expected customer profile.
4. That profile becomes the baseline for monitoring.
5. Transactions are compared against that expected behavior.
6. Alerts are generated when activity looks inconsistent, risky, or suspicious.

So transaction monitoring does not operate in a vacuum. It depends on the quality of the upstream customer information.

If onboarding data is incomplete, inaccurate, or poorly maintained, the monitoring logic becomes weaker. That can lead to:
- more false positives,
- missed risk,
- poor segmentation,
- and weak investigative outcomes.

---

## 📌 What risk-based means in practice

A risk-based model typically considers multiple dimensions at once. For example:

- **Customer risk**: Who is the customer? What is their background, occupation, ownership structure, or business type?
- **Geographic risk**: Where are they located? Where do they send or receive funds?
- **Product risk**: What accounts, services, or instruments are being used?
- **Channel risk**: Are they using branch, digital, wire, cash, or third-party channels?
- **Behavioral risk**: Does the activity match the customer profile?
- **Relationship risk**: Are there unusual counterparties or connections?

These dimensions are combined into a broader view of risk. That view is then used to shape monitoring, review frequency, escalation thresholds, and investigative focus.

---

## 🧩 The analytics angle

From an analytics perspective, the risk-based AML model is the first layer of structure.

It gives analysts a way to:
- segment the customer base,
- prioritize monitoring,
- compare expected versus actual behavior,
- and identify where the program is producing the most noise.

This is where analytics begins to add value:
- by reducing blind spots,
- by improving alert quality,
- by highlighting mismatches between profile and behavior,
- and by helping teams focus on the riskiest activity.

Even at this early stage, good analytics work can improve program effectiveness. A clean foundation means better rules, better scoring, and better outcomes later.

---

## 💡 Practical example

Imagine two customers:

### Customer A
- salaried employee,
- local domestic activity,
- low transaction volume,
- consistent monthly behavior,
- limited counterparties.

### Customer B
- complex business structure,
- multiple jurisdictions,
- higher cash movement,
- irregular transfer patterns,
- new counterparties appearing frequently.

A risk-based AML program would not treat these two customers the same way.

Customer B would likely require more scrutiny, more monitoring attention, and possibly stronger review intensity. Customer A might still be monitored, but the expected behavior and alert sensitivity may differ.

This is the practical value of the risk-based approach: it helps the institution assign attention where it matters most.

---
## 📈 What the workbook or notebook should show

The notebook or workbook should remain simple and readable.

A strong first version could include:
- synthetic customer records,
- expected monthly activity,
- actual monthly activity,
- a few key risk flags,
- a basic rule or score,
- and a short explanation of the output.

The goal is to show the logic, not to model every possible AML scenario.

---

## 🔄 Why this matters

Transaction monitoring is more effective when it starts from a customer baseline.

If onboarding data is weak, the monitoring system has to rely on generic thresholds that may create too many false positives or miss meaningful behavior shifts. A risk-based approach helps focus attention where it matters most.

This is especially important for analytics work because the quality of the upstream data determines the quality of the downstream alerts, investigations, and reporting.

---

## 📚 Further reading

If you want to explore the ideas behind this exercise more deeply, these references are a good starting point:

- [FinCEN fact sheet on a risk-based AML/CFT program](https://www.fincen.gov/system/files/shared/Program-NPRM-FactSheet-508.pdf)
- [FINRA AML overview](https://www.finra.org/rules-guidance/key-topics/aml)
- [Risk-based approach to AML screening](https://dilisense.com/en/insights/what-is-a-risk-based-approach-in-aml-screening)
- [Embracing a risk-based approach to AML](https://financialcrimeacademy.org/risk-based-approach-to-aml-compliance/)
- [Understanding risk-based approach in AML for effective compliance](https://www.au10tix.com/blog/understanding-risk-based-approach-in-aml-for-effective-compliance/)
- [Combining KYC data with transaction monitoring for better risk insights](https://www.linkedin.com/pulse/combining-kyc-data-transaction-monitoring-better-risk-insights-izqff)
- [KYC integration guide: steps for financial institutions](https://shadowdragon.io/blog/kyc-integration/)
- [How to implement transaction monitoring: best practices for AML compliance](https://www.sanctions.io/blog/transaction-monitoring-aml-compliance-best-practices)
- [9 best practices for an efficient transaction monitoring system](https://complyadvantage.com/insights/transaction-monitoring-best-practices/)
- [Synthetic data in AML: promise, pitfalls, and persistent skepticism](https://amlpartners.com/insights/synthetic-data-in-aml/)
- [A synthetic data set to benchmark anti-money laundering methods](https://www.nature.com/articles/s41597-023-02569-2)
- [Your AI training strategies are risky: synthetic data generation](https://www.cxtoday.com/ai-automation-in-cx/synthetic-data-generation-is-your-compliance-shortcut/)

---
