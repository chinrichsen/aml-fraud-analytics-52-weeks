# Week 5 - Thursday | 🧾 Structuring & Smurfing Detection Rules


Welcome to **Week 5 Thursday** of the 52-week AML and fraud analytics series.


This week continues the AML monitoring theme and focuses on one of the most important suspicious activity typologies in transaction monitoring: **structuring and smurfing**. These typologies matter because they often involve transactions that are intentionally kept below obvious reporting thresholds, which makes them harder to detect without the right scenario logic.


This Thursday topic focuses on **structuring and smurfing detection rules**, why they matter, and how institutions turn transaction patterns into alerts that can be reviewed, tuned, and escalated when necessary.


---


## 🎯 Why this topic matters


Structuring and smurfing matter because suspicious activity can be hidden inside seemingly ordinary transaction behavior.


That means the team must ask:
- Are transactions occurring just below reporting thresholds?
- Is the customer repeating similar deposits or withdrawals?
- Are there multiple transactions across a short time window?
- Does the activity look designed to avoid detection?
- Are there signs that multiple accounts, people, or channels are involved?


If these questions are not answered well, the monitoring program may miss behavior that is deliberately designed to evade AML controls.


This is why **structuring and smurfing** detection matters. It helps the institution identify activity that may be fragmented, repeated, or spread across accounts in a way that suggests intentional threshold avoidance.


---


## 🧠 Core concept


Structuring is the breaking up of transactions for the purpose of evading reporting and recordkeeping requirements, while smurfing is a related tactic that typically uses multiple individuals or accounts to distribute the activity.


In practice, this often looks like:
- multiple cash deposits just below a reporting threshold,
- repeated activity within a short period of time,
- several related transactions that add up to a material amount,
- or coordinated behavior across accounts or actors.


These transactions may not be suspicious one by one. But when they are viewed together, they can reveal a pattern that deserves review.


In practice, **structuring and smurfing** detection helps AML teams decide:
- which patterns should trigger alerts,
- which thresholds should be monitored,
- when repeated activity becomes meaningful,
- and how to prioritize investigation resources.


---


## 🔍 How this connects to scenario rules


This week is not just about theory. It is about the operational flow from **monitoring logic to structuring and smurfing detection**.


The connection is straightforward:
1. The institution defines transaction monitoring objectives based on AML risk.
2. Scenario rules are built to detect threshold avoidance and repeated transaction behavior.
3. Amounts, frequencies, time windows, and customer context are evaluated together.
4. The resulting alerts are reviewed for relevance and quality.
5. Higher-value patterns can be escalated for investigation and possible SAR review.
6. The institution tunes the rules to reduce false positives and improve detection strength.


So structuring and smurfing detection does not sit apart from AML investigations. It feeds directly into them and helps explain why certain transaction patterns deserve review.


If the rule is too narrow, it may miss suspicious behavior. If it is too broad, it may generate large volumes of low-value alerts.


---


## 📌 What structuring rules mean in practice


Strong structuring and smurfing scenarios usually combine several dimensions at once. For example:


- **Threshold proximity**: Are transactions just below a meaningful reporting threshold?
- **Velocity**: Are multiple transactions occurring in a short period of time?
- **Aggregation**: Do repeated smaller transactions add up over a lookback window?
- **Customer segmentation**: Does the behavior fit the customer profile?
- **Channel and geography**: Are there unusual locations, cash channels, or corridors involved?
- **Network patterns**: Are multiple accounts or actors linked through shared behavior?


These elements are combined into rules that can generate alerts for analyst review. The goal is not just to detect activity, but to detect activity in a way that is explainable and operationally useful.


---


## 🧩 The analytics angle


From an analytics perspective, structuring and smurfing detection is a strong example of turning AML policy into practical monitoring logic.


It gives analysts a way to:
- standardize what suspicious threshold avoidance looks like,
- connect AML typologies to system rules,
- compare alert quality across scenarios,
- and understand which parameters produce the most useful results.


This is where analytics adds value:
- by making monitoring logic transparent,
- by supporting more consistent investigations,
- by helping teams tune thresholds and time windows,
- and by showing whether a rule produces signal or noise.


Even a simple structuring or smurfing rule can be valuable if it is clearly defined and aligned to real risk.


---


## 💡 Practical example


Imagine two customers:


### Customer A
- one cash deposit above the normal reporting threshold,
- no repeated pattern,
- no unusual aggregation,
- and no related activity across accounts.


### Customer B
- several cash deposits just below the threshold,
- repeated activity over a short time window,
- similar amounts across multiple days,
- and a pattern that appears designed to avoid reporting triggers.


The institution would not treat these two customers the same way.


Customer B would likely trigger a structuring or smurfing scenario for further review because the activity suggests intentional threshold avoidance. Customer A might remain within expected behavior and not require escalation.


This is the practical value of structuring and smurfing detection: it helps the institution separate ordinary activity from patterns that deserve AML investigation.


---


## 📈 What the workbook should show


The workbook should remain simple and readable.


A strong first version could include:
- customer transaction records,
- transaction amount and date fields,
- threshold and aggregation logic,
- an alert flag output,
- and a short explanation of the result.


The goal is to show the logic, not to model every possible AML scenario.


---


## 🔄 Why this matters


Structuring and smurfing detection is most effective when the scenario logic is clear, risk-based, and tunable.


If the system only applies static thresholds without context, it can miss important patterns or create unnecessary alert volumes. A structured rule design approach helps the institution align monitoring output with investigative value.


This is especially important for analytics work because the quality of the rule determines the quality of the alerts, reviews, and escalation outcomes.


---


## 📚 Further reading


If you want to explore the ideas behind this topic more deeply, these references are a good starting point:


- [Suspicious Activity Reporting (Structuring)](https://www.fincen.gov/resources/statutes-regulations/administrative-rulings/suspicious-activity-reporting-structuring)
- [BSA/AML Manual – Appendix G: Structuring](https://bsaaml.ffiec.gov/manual/Appendices/08)
- [Anti-Money Laundering (AML) Transaction Monitoring Rules and Best Practices](https://www.sanctions.io/blog/anti-money-laundering-aml-transaction-monitoring-rules-and-best-practices)
- [Structuring and Smurfing Explained: Strengthening AML Compliance](https://www.netbankaudit.com/resources/structuring-and-smurfing-explained)
- [What is the difference between smurfing & structuring?](https://complyadvantage.com/insights/structuring-vs-smurfing/)
- [Structuring vs Smurfing in AML: Key Risks & Detection Tactics](https://www.facctum.com/blog/structuring-vs-smurfing-in-aml-key-risks-detection-tactics)
- [Smurfing in AML: key alert triggers every bank should monitor](https://www.trapets.com/resources/blog/smurfing-in-aml-key-alert-triggers-every-bank-should-monitor)
- [Smurfing: How Criminals Launder Money](https://www.unit21.ai/fraud-aml-dictionary/smurfing-money-laundering)
- [Smurfing in Money Laundering - azakaw](https://www.azakaw.com/blog/smurfing)
- [Smurfing and Structuring in AML: How to Detect and Report It](https://www.tookitaki.com/compliance-hub/smurfing-structuring-aml-detection-reporting)