# Week 3 - Thursday | 🚨 EDD Triggers for High-Risk Customers


Welcome to **Week 3 Thursday** of the 52-week AML and fraud analytics series.


This week continues the customer risk rating theme and moves from model inputs into the next operational step: **enhanced due diligence (EDD) triggers**. Once a customer has been scored and classified as higher risk, the institution still needs a clear decision path for when to escalate, review more deeply, and apply stronger controls.


This Thursday topic focuses on **EDD triggers for high-risk customers**, why they matter, and how a simple decision tree can help translate risk scores into review actions.


---


## 🎯 Why this topic matters


A high-risk rating by itself does not complete the process. The institution still needs to decide what happens next.


That means the team must ask:
- Is the customer above the EDD threshold?
- Are there additional risk signals that justify escalation?
- Should the review cadence change?
- Does the case need analyst intervention?
- What specific actions should follow the trigger?


If these questions are not answered clearly, then the risk rating is not very useful operationally.


This is why EDD triggers matter. They connect the score to action.


---


## 🧠 Core concept


Enhanced due diligence is the deeper review layer that follows a higher-risk customer assessment.


Instead of treating every customer the same way, the institution uses risk thresholds and trigger conditions to determine when stronger review is needed. These triggers can include:
- high CRR score,
- adverse media,
- PEP exposure,
- sanctions proximity,
- cross-border complexity,
- ownership opacity,
- unusual activity,
- or multiple elevated risk indicators together.


Each trigger helps the AML team decide whether the case should stay in standard review or move into EDD.


In practice, EDD helps AML teams decide:
- who needs a deeper review,
- what additional information should be collected,
- when to escalate,
- and how to document the rationale.


---


## 🔍 How this connects to the CRR model


This week is not just about theory. It is about the operational flow from **customer risk score to EDD decisioning**.


The connection is straightforward:
1. Customer data is scored through the CRR model.
2. The customer is assigned a risk tier.
3. High-risk customers are tested against EDD triggers.
4. Additional conditions may reinforce the escalation decision.
5. The case is routed to enhanced review or standard review.
6. The institution uses that output to support AML governance and monitoring.


So EDD does not replace CRR. It extends CRR into a decision tree that tells the institution what to do next.


If the triggers are too strict, the program may miss important customers. If they are too loose, the team may create unnecessary escalation volume.


---


## 📌 What EDD triggers mean in practice


EDD triggers typically consider multiple dimensions at once. For example:


- **CRR threshold**: Is the customer’s score above the cutoff?
- **Adverse media**: Are there negative news or reputation issues?
- **PEP status**: Is the customer politically exposed?
- **Sanctions proximity**: Is there a link to sanctioned persons or entities?
- **Geography**: Is the customer tied to higher-risk jurisdictions?
- **Ownership complexity**: Is the ownership structure opaque or layered?
- **Expected activity**: Does the behavior match what was disclosed?
- **Other risk flags**: Are there unusual events that justify a deeper review?


These triggers are combined into a broader decisioning flow. That flow is then used to determine whether the customer should receive EDD, standard review, or a lower-intensity review path.


---


## 🧩 The analytics angle


From an analytics perspective, EDD decisioning is a great example of turning model output into a business rule.


It gives analysts a way to:
- translate score thresholds into action,
- document escalation logic,
- test whether triggers are too sensitive or too weak,
- and support governance with transparent decision rules.


This is where analytics adds value:
- by clarifying the relationship between score and action,
- by making escalation logic consistent,
- by showing which triggers are most influential,
- and by helping teams defend review outcomes.


Even a simple decision tree can make the process much more explainable.


---


## 💡 Practical example


Imagine two customers:


### Customer A
- moderate CRR score,
- no adverse media,
- domestic activity,
- simple ownership structure,
- no PEP or sanctions concerns.


### Customer B
- high CRR score,
- adverse media present,
- cross-border activity,
- layered ownership structure,
- PEP exposure.


The institution would not treat these two customers the same way.


Customer B would likely be routed to EDD and receive stronger review intensity. Customer A might remain in standard review, even if the score is elevated but not high enough to trigger escalation.


This is the practical value of triggers: they help the institution distinguish between elevated risk and truly high-risk cases.


---


## 📈 What the workbook should show


The workbook should remain simple and readable.


A strong first version could include:
- synthetic customer records,
- a CRR score output,
- a risk tier output,
- EDD trigger logic,
- a decision tree,
- and a short explanation of the result.


The goal is to show the logic, not to create a production decision engine.


---


## 🔄 Why this matters


EDD is most effective when the trigger logic is clear and consistent.


If the escalation rules are vague, different analysts may treat similar customers differently. A structured EDD decision tree helps the institution align review intensity with the actual level of risk.


This is especially important for analytics work because the quality of the trigger logic determines the quality of the escalation, review, and governance outcomes.


---


## 📚 Further reading


If you want to explore the ideas behind this exercise more deeply, these references are a good starting point:


- [Enhanced Due Diligence (EDD) in AML](https://www.complyadvantage.com/insights/enhanced-due-diligence/)
- [Customer Due Diligence and Enhanced Due Diligence](https://www.fincen.gov/resources/statutes-and-regulations/cdd-final-rule)
- [Risk-based customer due diligence](https://www.lexisnexisrisk.com/blog/customer-risk-rating/)
- [EDD and AML risk management](https://www.sanctions.io/blog/enhanced-due-diligence/)
- [EDD requirements and best practices](https://www.acams.org/en/resources/risk-based-approach)
- [How to build an EDD framework](https://www.sas.com/en_us/insights/articles/risk-fraud/customer-risk-rating-model.html)
- [Risk-based approach to AML compliance](https://www.finra.org/rules-guidance/key-topics/aml)
- [Customer risk profiling for AML compliance](https://www.flagright.com/post/customer-risk-profiling-a-key-to-aml-compliance)
- [EDD review triggers and escalation logic](https://www.au10tix.com/blog/understanding-risk-based-approach-in-aml-compliance/)
- [Why trigger-based escalation improves AML governance](https://www.prospero.systems/insights/top-customer-risk-profiling-techniques-to-enhance-compliance-accuracy)
