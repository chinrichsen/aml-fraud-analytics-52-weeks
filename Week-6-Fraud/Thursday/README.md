# Week 6 Thursday | 🛒 Friendly Fraud & First-Party Fraud Signals

Welcome to **Week 6 Thursday** of the 52-week AML and fraud analytics series.

This week continues the fraud analytics theme and focuses on **friendly fraud** and **first-party fraud signals**. These cases matter because the transaction may look legitimate at first, but the dispute, return, chargeback, or behavioral pattern later suggests that the loss did not come from a traditional external fraudster.

This Thursday topic focuses on **friendly fraud / first-party fraud**, why it matters, and how institutions use structured signals to identify transactions that may be disputed, abused, or intentionally misrepresented by the customer.

---

## 🎯 Why this topic matters

Friendly fraud matters because the transaction itself may not look obviously suspicious.

That means the team must ask:
- Did the customer actually authorize the purchase?
- Is there a pattern of excessive refunds or chargebacks?
- Does the account show return abuse or dispute abuse?
- Is the customer behavior inconsistent with prior history?
- Are there signs of intentional misuse rather than accidental error?

If these questions are not answered well, the fraud program may treat the case as a normal customer issue and miss an important first-party fraud pattern.

This is why friendly fraud analytics matters. It helps the institution identify suspicious post-transaction behavior before losses and operational friction grow larger.

---

## 🧠 Core concept

Friendly fraud, also called first-party fraud in many cases, happens when the cardholder or account holder claims a transaction was unauthorized, disputes a valid purchase, or otherwise misrepresents the event to receive a financial benefit.

Instead of relying only on authorization signals, the institution evaluates patterns such as:
- repeated chargebacks,
- high refund activity,
- excessive return behavior,
- dispute patterns across merchants or channels,
- customer tenure and behavioral consistency,
- and loss history tied to the same account or customer.

These signals do not prove fraud on their own, but they help identify activity that deserves further review.

In practice, first-party fraud analytics helps fraud teams decide:
- which disputes should be challenged,
- which accounts should be monitored more closely,
- when a customer’s behavior becomes materially unusual,
- and how to prioritize investigation resources.

---

## 🔍 How this connects to fraud rules

This week is not just about theory. It is about the operational flow from **customer behavior to dispute risk decisioning**.

The connection is straightforward:
1. The institution defines friendly-fraud monitoring objectives based on loss and abuse risk.
2. Rules are built to detect chargeback, refund, and dispute abuse behavior.
3. Transaction history, return activity, and case outcomes are evaluated together.
4. The resulting alerts are reviewed for relevance and quality.
5. Higher-risk cases can be escalated for investigation or account action.
6. The institution tunes the rules to improve effectiveness and reduce false positives.

So first-party fraud analytics does not sit apart from fraud operations. It feeds directly into them and helps explain why certain patterns deserve review.

If the rule is too narrow, it may miss abuse. If it is too broad, it may flag ordinary customers who simply had a bad experience.

---

## 📌 What friendly fraud analytics means in practice

Strong friendly-fraud scenarios usually combine several dimensions at once. For example:

- **Chargeback behavior**: Is the account showing repeated dispute activity?
- **Refund and return patterns**: Are returns or refunds unusually frequent?
- **Customer consistency**: Does the behavior fit the customer’s prior history?
- **Loss concentration**: Are losses clustered on the same cardholder or account?
- **Channel and merchant context**: Do certain merchants, channels, or products show abnormal dispute rates?
- **Timing and sequence**: Does the behavior follow a pattern of purchase, use, dispute, and reattempt?

These elements are combined into rules that can generate alerts for analyst review. The goal is not just to identify disputes, but to identify them in a way that is explainable and operationally useful.

---

## 🧩 The analytics angle

From an analytics perspective, friendly fraud is a strong example of turning post-transaction signals into practical detection logic.

It gives analysts a way to:
- standardize what suspicious dispute behavior looks like,
- connect fraud typologies to system rules,
- compare alert quality across scenarios,
- and understand which parameters drive the most useful results.

This is where analytics adds value:
- by making fraud logic transparent,
- by supporting more consistent investigations,
- by helping teams tune thresholds and loss windows,
- and by showing whether a rule produces signal or noise.

Even a simple first-party fraud rule can be valuable if it is clearly defined and aligned to real risk.

---

## 💡 Practical example

Imagine two customers:

### Customer A
- one isolated refund request,
- normal purchase history,
- no repeated chargebacks,
- and behavior that fits the customer’s past pattern.

### Customer B
- repeated disputes across multiple purchases,
- high refund and return activity,
- prior losses on the same account,
- and a pattern that does not fit the expected customer profile.

The institution would not treat these two customers the same way.

Customer B would likely trigger a friendly-fraud rule for further review because the pattern suggests possible first-party abuse. Customer A might remain within expected behavior and not require escalation.

This is the practical value of friendly fraud analytics: it helps the institution separate ordinary customer activity from patterns that deserve fraud investigation.

---

## 📈 What the workbook should show

The workbook should remain simple and readable.

A strong first version could include:
- dispute and return records,
- chargeback and refund fields,
- customer history and loss indicators,
- a risk flag output,
- and a short explanation of the result.

The goal is to show the logic, not to model every possible dispute or abuse scenario.

---

## 🔄 Why this matters

Friendly fraud is most effectively managed when the detection logic is clear, risk-based, and tunable.

If the system only applies static thresholds without context, it can miss important patterns or create unnecessary false positives. A structured first-party fraud approach helps the institution align detection output with investigative value.

This is especially important for analytics work because the quality of the rule determines the quality of the alerts, reviews, and escalation outcomes.

---

## 📚 Further reading

If you want to explore the ideas behind this topic more deeply, these references are a good starting point:

- [What Is Friendly Fraud?](https://www.mastercard.us/en-us/business/insights/friendly-fraud.html)
- [Chargeback Fraud and Dispute Abuse](https://www.visa.com/chargeback-reason-codes.html)
- [First-Party Fraud Overview](https://www.feedzai.com/blog/what-is-first-party-fraud/)
- [Refund Abuse and Return Fraud](https://www.sift.com/resources/friendly-fraud)
- [Managing Chargebacks and Disputes](https://www.electronicpaymentsinternational.com/)
- [Fraud Analytics and Dispute Monitoring](https://www.sas.com/en_us/insights/articles/fraud/fraud-detection.html)
- [Behavioral Analytics for Fraud Detection](https://www.ibm.com/topics/fraud-detection)
- [Customer Abuse and First-Party Risk](https://www.lexisnexisrisk.com/)
- [Risk-Based Fraud Monitoring](https://www.niceactimize.com/resources/)
- [E-commerce Fraud Prevention Best Practices](https://www.riskified.com/learning/)