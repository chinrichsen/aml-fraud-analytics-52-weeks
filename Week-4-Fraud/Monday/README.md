# Week 4 - Monday | 🕵️ Synthetic Identity Fraud Patterns


Welcome to **Week 4 Monday** of the 52-week AML and fraud analytics series.


This week moves deeper into fraud analytics and focuses on one of the most difficult fraud problems to detect: **synthetic identity fraud**. Unlike account takeover or card fraud, synthetic identity fraud often blends real and fake information so that the profile can look legitimate at first glance.


This Monday topic focuses on **synthetic identity patterns**, why they matter, and how structured detection logic can help identify suspicious identity creation and account behavior earlier in the lifecycle.


---


## 🎯 Why this topic matters


Synthetic identity fraud is dangerous because the profile may not look obviously false.


That means the team must ask:
- Is the identity internally consistent?
- Do the attributes match across sources?
- Are there signs of fabrication or reuse?
- Does the identity behave like a real customer?
- Are multiple identities linked through shared details?


If these questions are not answered well, the fraud program may allow fake identities to age into higher-value fraud events.


This is why synthetic identity detection matters. It helps the institution find problems early, before the fraud grows larger.


---


## 🧠 Core concept


Synthetic identity fraud happens when a fraudster combines real and fabricated identity elements to create a profile that can pass basic checks.


Instead of using a single stolen identity, the fraudster may mix:
- a real SSN with a fake name,
- a real address with a fabricated DOB,
- reused contact information,
- inconsistent employment or phone history,
- or multiple identities that share the same device or contact details.


These identities may appear valid on the surface, but they often contain subtle inconsistencies that can be detected through analytics.


In practice, synthetic identity detection helps fraud teams decide:
- which applications look suspicious,
- which identities may be linked,
- when to step up review,
- and how to prioritize investigation.


---


## 🔍 How this connects to fraud propensity scoring


This week is not just about theory. It is about the operational flow from **identity signals to fraud risk scoring**.


The connection is straightforward:
1. Identity attributes are collected during onboarding or review.
2. The model evaluates consistency, reuse, and anomaly signals.
3. Each signal contributes to a fraud propensity score.
4. The final score helps classify likely synthetic identity cases.
5. Higher-risk cases can be routed for review, decline, or monitoring.
6. The institution uses that output to support fraud prevention and decisioning.


So synthetic identity detection does not replace fraud scoring. It feeds into it and helps explain why an identity deserves more scrutiny.


If the signals are too weak, the program may miss fraud. If the signals are too broad, the team may create too many false positives.


---


## 📌 What synthetic identity patterns mean in practice


Synthetic identity models typically consider multiple dimensions at once. For example:


- **Identity consistency**: Do the name, DOB, SSN, address, and contact fields align?
- **Attribute reuse**: Are phone numbers, emails, or devices being reused across identities?
- **Velocity**: Are multiple applications appearing in a short time window?
- **Linkage**: Do several profiles share the same data points or behavioral patterns?
- **Stability**: Does the identity history look thin, new, or manufactured?
- **Behavioral fit**: Does the activity look like a real customer or a staged profile?


These signals are combined into a broader propensity score. That score is then used to guide review, escalation, or decline decisions.


---


## 🧩 The analytics angle


From an analytics perspective, synthetic identity detection is a great example of combining structured and behavioral signals into one fraud view.


It gives analysts a way to:
- standardize fraud review decisions,
- connect suspicious identities across records,
- identify patterns of reuse and fabrication,
- and understand which signals are most predictive of synthetic behavior.


This is where analytics adds value:
- by making the detection logic transparent,
- by supporting consistent investigation,
- by revealing how identities cluster together,
- and by helping teams justify review outcomes.


Even a simple rule-based model can create a meaningful first layer of defense.


---


## 💡 Practical example


Imagine two applicants:


### Applicant A
- stable identity history,
- consistent name, address, and phone details,
- normal velocity,
- no reuse across other records.


### Applicant B
- thin identity footprint,
- reused phone and device,
- mismatched attribute history,
- several linked records,
- short application history.


The institution would not treat these two applicants the same way.


Applicant B would likely receive a higher fraud propensity score and be routed for investigation. Applicant A might remain in a normal onboarding path with standard review intensity.


This is the practical value of synthetic identity modeling: it helps the institution separate legitimate applicants from suspicious identity constructions.


---


## 📈 What the workbook should show


The workbook should remain simple and readable.


A strong first version could include:
- synthetic identity records,
- identity quality and linkage features,
- a fraud propensity score,
- a risk tier output,
- and a short explanation of the result.


The goal is to show the logic, not to model every possible fraud scenario.


---


## 🔄 Why this matters


Synthetic identity fraud is most effectively managed when the detection logic is clear and consistent.


If the model only looks at one field, it can miss the broader pattern. A structured synthetic identity approach helps the institution align review intensity with the actual level of fraud risk.


This is especially important for analytics work because the quality of the score determines the quality of the investigation and escalation outcomes.


---


## 📚 Further reading


If you want to explore the ideas behind this exercise more deeply, these references are a good starting point:


- [Synthetic identity fraud: what it is and how to detect it](https://www.lexisnexisrisk.com/blog/synthetic-identity-fraud/)
- [Synthetic identity fraud detection in banking](https://www.sas.com/en_us/insights/articles/risk-fraud/synthetic-identity-fraud.html)
- [Understanding synthetic identity fraud](https://www.transunion.com/blog/identity-protection/synthetic-identity-fraud)
- [How synthetic identity fraud works](https://www.experian.com/blogs/insights/what-is-synthetic-identity-fraud/)
- [Synthetic identity and fraud risk management](https://www.acams.org/en/resources/fraud-prevention)
- [Identity verification and fraud analytics](https://www.fico.com/blogs/identity-verification-fraud-prevention)
- [Risk-based approach to identity fraud](https://www.finra.org/investors/insights/fraud)
- [How to build synthetic identity detection models](https://www.ibm.com/topics/fraud-detection)
- [Fraud propensity scoring techniques](https://www.amulet.com/blog/fraud-propensity-models)
- [Using linkage analysis to detect fraud patterns](https://www.sas.com/en_us/insights/articles/risk-fraud/network-analytics-fraud.html)