# Week 6 - Monday | 💳 Card-Not-Present (CNP) Fraud Analytics

Welcome to **Week 6 Monday** of the 52-week AML and fraud analytics series.

This week moves into **fraud analytics** and focuses on one of the most common card fraud problems: **card-not-present (CNP) fraud**. CNP fraud happens when the cardholder is not physically present, so the transaction must be evaluated using digital and behavioral signals rather than face-to-face verification.

This Monday topic focuses on **CNP fraud analytics**, why it matters, and how structured detection logic can help identify suspicious online or remote card activity earlier in the payment lifecycle.

---

## 🎯 Why this topic matters

CNP fraud matters because the card is often valid, but the transaction context is not.

That means the team must ask:
- Is the purchase channel consistent with the customer profile?
- Does the device or browser look familiar?
- Is the transaction amount or timing unusual?
- Are there signs of velocity or repeated attempts?
- Does the activity fit the cardholder’s normal behavior?

If these questions are not answered well, the fraud program may allow stolen or compromised card credentials to be used online before the case is detected.

This is why CNP fraud analytics matters. It helps the institution identify suspicious remote payment behavior before losses grow larger.

---

## 🧠 Core concept

Card-not-present fraud happens when a payment is made without the physical card being presented.

Instead of relying on chip, swipe, or in-person verification, the institution evaluates signals such as:
- device reputation,
- shipping and billing mismatch,
- transaction velocity,
- unusual merchant behavior,
- digital identity consistency,
- and repeated failed authentication or authorization attempts.

These signals do not prove fraud on their own, but they help identify activity that deserves further review.

In practice, CNP analytics helps fraud teams decide:
- which transactions should be challenged,
- which payments should be stepped up for authentication,
- when a transaction is too risky to approve,
- and how to prioritize investigation resources.

---

## 🔍 How this connects to fraud rules

This week is not just about theory. It is about the operational flow from **CNP signals to fraud decisioning**.

The connection is straightforward:
1. The institution defines CNP monitoring objectives based on fraud risk.
2. Rules are built to detect suspicious online or remote payment behavior.
3. Device, channel, velocity, and identity signals are evaluated together.
4. The resulting alerts or declines are reviewed for relevance and quality.
5. Higher-risk cases can be escalated for investigation or step-up verification.
6. The institution tunes the rules to improve effectiveness and reduce false positives.

So CNP analytics does not sit apart from fraud operations. It feeds directly into them and helps explain why certain payments deserve review.

If the rule is too narrow, it may miss fraud. If it is too broad, it may block too many legitimate customers.

---

## 📌 What CNP analytics means in practice

Strong CNP fraud scenarios usually combine several dimensions at once. For example:

- **Device reputation**: Is the device known, risky, or new?
- **Channel behavior**: Is the transaction coming from a web, mobile, or app channel?
- **Velocity**: Are multiple attempts occurring in a short period of time?
- **Identity consistency**: Do the customer, payment, and delivery details align?
- **Merchant context**: Is the merchant type or purchase pattern unusual?
- **Behavioral fit**: Does the activity resemble the customer’s normal payment profile?

These elements are combined into rules that can generate alerts or declines for analyst and fraud review. The goal is not just to block transactions, but to block or challenge them in a way that is explainable and operationally useful.

---

## 🧩 The analytics angle

From an analytics perspective, CNP fraud is a strong example of turning digital signals into practical detection logic.

It gives analysts a way to:
- standardize what suspicious online card activity looks like,
- connect fraud typologies to system rules,
- compare alert quality across scenarios,
- and understand which parameters drive the most useful results.

This is where analytics adds value:
- by making fraud logic transparent,
- by supporting more consistent investigations,
- by helping teams tune thresholds and velocity windows,
- and by showing whether a rule produces signal or noise.

Even a simple CNP rule can be valuable if it is clearly defined and aligned to real risk.

---

## 💡 Practical example

Imagine two customers:

### Customer A
- familiar device,
- normal purchase channel,
- typical transaction amount,
- and a pattern that matches historical behavior.

### Customer B
- new device,
- shipping and billing mismatch,
- multiple attempts in a short time window,
- and a pattern that does not fit the expected cardholder profile.

The institution would not treat these two customers the same way.

Customer B would likely trigger a CNP fraud rule for further review because the pattern suggests elevated risk. Customer A might remain within expected behavior and not require escalation.

This is the practical value of CNP fraud analytics: it helps the institution separate ordinary remote card activity from patterns that deserve fraud investigation.

---

## 📈 What the workbook should show

The workbook should remain simple and readable.

A strong first version could include:
- card transaction records,
- device and channel fields,
- fraud thresholds and pattern logic,
- an alert flag output,
- and a short explanation of the result.

The goal is to show the logic, not to model every possible card fraud scenario.

---

## 🔄 Why this matters

CNP fraud is most effectively managed when the detection logic is clear, risk-based, and tunable.

If the system only applies static thresholds without context, it can miss important patterns or create unnecessary false positives. A structured CNP fraud approach helps the institution align detection output with investigative value.

This is especially important for analytics work because the quality of the rule determines the quality of the alerts, reviews, and escalation outcomes.

---

## 📚 Further reading

If you want to explore the ideas behind this topic more deeply, these references are a good starting point:

- [Card-Not-Present Fraud: What It Is and How to Detect It](https://www.ftc.gov/business-guidance/blog/2023/06/fighting-card-not-present-fraud)
- [Card-Not-Present Fraud Overview](https://www.fico.com/blogs/card-not-present-fraud)
- [E-commerce Fraud and Risk Signals](https://www.visa.com/security.html)
- [Digital Identity and Fraud Prevention](https://www.experian.com/blogs/insights/category/fraud-prevention/)
- [Online Payment Fraud Detection](https://www.mastercard.us/en-us/vision/cybersecurity.html)
- [Device Intelligence in Fraud Detection](https://www.lexisnexisrisk.com/insights/resources/what-is-device-intelligence/)
- [Fraud Analytics and Transaction Monitoring](https://www.sas.com/en_us/insights/articles/fraud/fraud-detection.html)
- [Risk-Based Authentication and Step-Up Controls](https://www.ibm.com/topics/fraud-detection)
- [Behavioral Analytics for Fraud Detection](https://www.feedzai.com/blog/fraud-detection/)
- [E-commerce Fraud Prevention Best Practices](https://www.niceactimize.com/resources/)