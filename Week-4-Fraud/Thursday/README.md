# Week 4 - Thursday | 🧠 Fraud Propensity Scoring Techniques


Welcome to **Week 4 Thursday** of the 52-week AML and fraud analytics series.


This week continues the synthetic identity theme and moves from pattern recognition into the next analytical step: **fraud propensity scoring**. Once suspicious identity signals have been identified, the institution still needs a structured way to translate those signals into a score, a risk tier, or a review decision.



This Thursday topic focuses on **fraud propensity scoring techniques**, why they matter, and how a simple decision tree can help turn identity signals into a clearer fraud risk assessment.



---



## 🎯 Why this topic matters



Synthetic identity fraud is not always obvious from one field alone. The real challenge is deciding how to combine multiple weak signals into a meaningful fraud view.



That means the team must ask:
- Which signals matter most?
- How should identity signals be weighted?
- What score separates low-risk from suspicious cases?
- Which cases should be reviewed first?
- How can the score support investigation and escalation?



If these questions are not answered clearly, the fraud program may identify patterns but still fail to prioritize cases effectively.



This is why propensity scoring matters. It connects suspicious signals to action.



---



## 🧠 Core concept



Fraud propensity scoring is the process of assigning a likelihood score to a case, applicant, or account based on observed risk signals.



Instead of relying on one red flag, the model combines multiple features such as:
- thin-file profile,
- short account age,
- mismatched identity fields,
- reused phone, email, or address,
- shared device,
- IP risk,
- linked records,
- and other identity anomalies.



These features can be combined into a risk score or used in a simple classification model. The goal is to estimate how likely it is that the case represents synthetic identity behavior.



In practice, propensity scoring helps fraud teams decide:
- which applications should be reviewed first,
- which cases may require step-up verification,
- when to decline or hold,
- and how to document the rationale behind the decision.



---



## 🔍 How this connects to the Monday topic



This week is not just about theory. It is about the operational flow from **synthetic identity patterns to propensity scoring**.



The connection is straightforward:
1. Identity signals are collected from the application or customer record.
2. The model evaluates reuse, linkage, consistency, and profile depth.
3. Each signal contributes to a propensity score.
4. The final score helps classify likely synthetic identity cases.
5. Higher-risk cases can be routed for review, decline, or monitoring.
6. The institution uses that output to support fraud prevention and decisioning.



So propensity scoring does not replace pattern detection. It builds on it and helps explain why a case deserves more scrutiny.



If the scoring logic is too narrow, the program may miss important fraud cases. If it is too broad, the team may create too many false positives.



---



## 📌 What propensity scoring means in practice



Fraud propensity models typically consider multiple dimensions at once. For example:



- **Identity depth**: Is the profile thin, new, or incomplete?
- **Attribute consistency**: Do the name, address, phone, and device signals align?
- **Reuse**: Are contact details or devices shared across multiple applications?
- **Linkage**: Do multiple records point to the same underlying identity cluster?
- **Velocity**: Are there multiple applications in a short window?
- **Environment risk**: Is the IP, device, or session context suspicious?



These signals are combined into a broader fraud score. That score is then used to guide review, escalation, or decisioning.



---



## 🧩 The analytics angle



From an analytics perspective, fraud propensity scoring is a great example of turning raw signals into an operational model.



It gives analysts a way to:
- standardize review decisions,
- prioritize suspicious identities,
- test which features are most predictive,
- and explain why a case received a certain score or tier.



This is where analytics adds value:
- by making the scoring logic transparent,
- by helping teams compare cases consistently,
- by showing how linked records influence the score,
- and by supporting repeatable review outcomes.



Even a simple decision tree can create a useful first layer of fraud scoring.



---



## 💡 Practical example



Imagine two applicants:



### Applicant A
- stable identity history,
- consistent contact details,
- no shared devices,
- no linkage across other records.



### Applicant B
- thin-file profile,
- reused phone and email,
- shared device,
- multiple linked records,
- suspicious IP context.



The institution would not treat these two applicants the same way.



Applicant B would likely receive a higher fraud propensity score and be routed for investigation. Applicant A might remain in a normal onboarding path with standard review intensity.



This is the practical value of propensity scoring: it helps the institution separate routine applications from suspicious synthetic identity cases.



---



## 📈 What the workbook should show



The workbook should remain simple and readable.



A strong first version could include:
- synthetic identity records,
- identity quality and linkage features,
- a fraud propensity score,
- a risk tier output,
- and a short explanation of the result.



The goal is to show the logic, not to build a production fraud engine.



---



## 🔄 Why this matters



Fraud propensity scoring is most effective when the logic is clear and consistent.



If the model only looks at one signal, it can miss the broader pattern. A structured propensity approach helps the institution align review intensity with the actual level of fraud risk.



This is especially important for analytics work because the quality of the score determines the quality of the investigation and escalation outcomes.



---



## 📚 Further reading



If you want to explore the ideas behind this exercise more deeply, these references are a good starting point:



- [Fraud propensity modeling overview](https://www.fico.com/blogs/fraud-propensity-modeling)
- [Synthetic identity fraud and scoring](https://www.lexisnexisrisk.com/blog/synthetic-identity-fraud/)
- [How to detect and prevent synthetic identity fraud](https://www.sas.com/en_us/insights/articles/risk-fraud/synthetic-identity-fraud.html)
- [Identity verification and fraud analytics](https://www.transunion.com/blog/identity-protection/synthetic-identity-fraud/)
- [Fraud risk scoring techniques](https://www.ibm.com/topics/fraud-detection)
- [Using linkage analysis in fraud detection](https://www.sas.com/en_us/insights/articles/risk-fraud/network-analytics-fraud.html)
- [Understanding identity fraud signals](https://www.acams.org/en/resources/fraud-prevention)
- [Machine learning for fraud prevention](https://www.fraud.com/post/machine-learning-fraud-detection)
- [Risk-based fraud review frameworks](https://www.finra.org/investors/insights/fraud)
- [Fraud scoring and prioritization](https://www.oracle.com/financial-services/fraud-prevention/)