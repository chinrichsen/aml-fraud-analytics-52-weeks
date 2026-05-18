# Week 5 - Monday | 🚨 Transaction Monitoring Scenario Design

Welcome to **Week 5 Monday** of the 52-week AML and fraud analytics series.

This week shifts back into **AML analytics** and focuses on one of the most practical parts of transaction monitoring: **scenario design**. A transaction monitoring program is only as useful as the logic behind the scenarios it runs, so this topic is about how to translate AML risk into rules that are structured, explainable, and operationally useful.

This Monday topic focuses on **transaction monitoring scenario design**, why it matters, and how institutions turn broad AML concerns into detection logic that can identify unusual or suspicious activity for review.

---

## 🎯 Why this topic matters

Transaction monitoring matters because suspicious activity rarely announces itself clearly.

That means the team must ask:
- What customer behavior should be considered unusual?
- Which transactions indicate elevated AML risk?
- How should thresholds be set?
- Which typologies should the scenario target?
- How can the alert be useful without overwhelming investigators?

If these questions are not answered well, the monitoring program may either miss suspicious activity or generate too many low-value alerts.

This is why scenario design matters. It helps the institution create a monitoring framework that is aligned to risk, practical for analysts, and easier to tune over time.

---

## 🧠 Core concept

A transaction monitoring scenario is a defined rule or logic set that looks for behavior associated with money laundering or other suspicious financial activity.

Instead of reviewing every transaction manually, the institution creates targeted scenarios such as:
- large cash activity,
- rapid movement of funds,
- unusual wire transfers,
- sudden changes in customer behavior,
- structuring below reporting thresholds,
- or activity inconsistent with the expected customer profile.

These scenarios do not prove misconduct on their own, but they help identify activity that deserves further review.

In practice, scenario design helps AML teams decide:
- which patterns should trigger alerts,
- which thresholds are appropriate,
- when customer behavior is materially unusual,
- and how to prioritize investigation resources.

---

## 🔍 How this connects to structuring rules

This week is not just about theory. It is about the operational flow from **scenario design to targeted structuring detection**.

The connection is straightforward:
1. The institution defines monitoring objectives based on AML risk.
2. Scenario logic is built to detect activity patterns that may indicate suspicious behavior.
3. Thresholds, lookback windows, and segmentation rules are applied.
4. The resulting alerts are reviewed for relevance and quality.
5. Higher-value patterns, including structuring behavior, can be escalated for investigation.
6. The institution tunes the scenarios to improve effectiveness and reduce noise.

So scenario design does not sit apart from AML investigations. It feeds directly into them and helps explain why certain activity deserves review.

If the scenario is too narrow, it may miss suspicious behavior. If it is too broad, it may generate large volumes of alerts with little investigative value.

---

## 📌 What scenario design means in practice

Strong transaction monitoring scenarios usually combine several dimensions at once. For example:

- **Threshold logic**: Is transaction activity above, below, or near a meaningful threshold?
- **Velocity**: Are multiple transactions occurring in a short period of time?
- **Aggregation**: Do smaller transactions add up to a material amount over a lookback window?
- **Customer segmentation**: Does the scenario behave differently for retail, business, or high-risk customers?
- **Expected behavior**: Is the activity consistent with the customer profile?
- **Geography and channel**: Do certain locations, corridors, or delivery channels raise additional concern?

These elements are combined into rules that can generate alerts for analyst review. The goal is not just to detect activity, but to detect activity in a way that is explainable and operationally useful.

---

## 🧩 The analytics angle

From an analytics perspective, transaction monitoring scenario design is a strong example of turning policy expectations into practical detection logic.

It gives analysts a way to:
- standardize what suspicious activity looks like,
- connect AML typologies to system rules,
- compare alert quality across scenarios,
- and understand which parameters drive the most useful results.

This is where analytics adds value:
- by making monitoring logic transparent,
- by supporting more consistent investigations,
- by helping teams tune thresholds and time windows,
- and by showing whether a scenario produces signal or noise.

Even a simple scenario can be valuable if it is clearly defined and aligned to real risk.

---

## 💡 Practical example

Imagine two customers:

### Customer A
- periodic cash deposits,
- transaction amounts consistent with historical behavior,
- no unusual spike in activity,
- and no obvious threshold avoidance pattern.

### Customer B
- multiple cash deposits just below a reporting threshold,
- repeated activity within a short time window,
- branch activity spread across locations,
- and a pattern that does not fit the expected customer profile.

The institution would not treat these two customers the same way.

Customer B would likely trigger a scenario for further review because the pattern suggests possible structuring. Customer A might remain within expected behavior and not require escalation.

This is the practical value of scenario design: it helps the institution separate ordinary activity from patterns that deserve AML investigation.

---

## 📈 What the workbook should show

The workbook should remain simple and readable.

A strong first version could include:
- customer transaction records,
- transaction amount and date fields,
- scenario thresholds and aggregation logic,
- an alert flag output,
- and a short explanation of the result.

The goal is to show the logic, not to model every possible AML scenario.

---

## 🔄 Why this matters

Transaction monitoring is most effective when the scenario logic is clear, risk-based, and tunable.

If the system only applies static thresholds without context, it can miss important patterns or create unnecessary alert volumes. A structured scenario design approach helps the institution align monitoring output with investigative value.

This is especially important for analytics work because the quality of the scenario determines the quality of the alerts, reviews, and escalation outcomes.

---

## 📚 Further reading

If you want to explore the ideas behind this topic more deeply, these references are a good starting point:

- [Transaction Monitoring Systems and Segmentation](https://www.occ.treas.gov/topics/supervision-and-examination/bsa/index-bsa.html)
- [Guidance on a Risk-Based Approach](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Risk-based-approach-guidance.html)
- [Suspicious Activity Monitoring and Reporting](https://www.fincen.gov/resources/statutes-regulations/guidance)
- [AML Transaction Monitoring Best Practices](https://www.sas.com/en_us/insights/analytics/anti-money-laundering.html)
- [How AML Monitoring Scenarios Are Tuned](https://www.niceactimize.com/blog/transaction-monitoring-threshold-setting/)
- [Using Analytics in AML Detection](https://www.oracle.com/financial-services/aml-financial-crime-compliance/)
- [Structuring and Smurfing Overview](https://www.fincen.gov/resources/statutes-regulations/administrative-rulings)
- [Financial Crime Monitoring Programs](https://www.acams.org/en/resources/aml-glossary)
- [Risk-Based Alert Generation in AML](https://www.ibm.com/think/topics/anti-money-laundering)
- [Scenario Tuning and Alert Optimization](https://www.feedzai.com/blog/transaction-monitoring/)