# Week 3 - Monday | 🧮 CRR Model Inputs & Weighting

Welcome to **Week 3 Monday** of the 52-week AML and fraud analytics series.

This week moves from fraud detection into a key AML decisioning topic: **customer risk rating (CRR)**. Before an institution can make strong EDD decisions, it needs to understand which customer inputs matter most and how those inputs should be weighted in the risk model.

This Monday topic focuses on **CRR model inputs**, why weighting matters, and how a structured risk view can help drive better escalation decisions.

---

## 🎯 Why this topic matters

A strong CRR framework is not built on one field alone. It is built on the ability to combine multiple customer attributes into a consistent risk view.

That means the institution must ask:
- What type of customer is this?
- Where are they located?
- What products and channels are they using?
- What is their expected activity?
- Are there any adverse or complexity flags?
- Which inputs should carry the most weight?

If these questions are not answered well, then the risk rating process becomes inconsistent, harder to defend, and less useful for downstream monitoring.

This is why model inputs and weighting matter. They help turn customer information into a structured risk decision.

---

## 🧠 Core concept

A **customer risk rating model** is designed to estimate how much AML risk a customer presents based on a set of inputs.

Instead of relying on a single review or subjective judgment, the model combines structured factors such as:
- customer type,
- geography,
- products,
- channels,
- ownership structure,
- expected activity,
- source of funds,
- adverse media,
- and other risk indicators.

Each input does not always have the same importance. Some factors are more predictive of risk than others, so weighting helps the model reflect that difference.

In practice, CRR helps AML teams decide:
- how to classify the customer,
- how often to review them,
- when to escalate,
- and whether EDD is needed.

---

## 🔍 How this connects to EDD

This week is not just about theory. It is about the operational flow from **risk inputs to enhanced due diligence**.

The connection is straightforward:
1. Customer onboarding or periodic review data is collected.
2. The model evaluates the relevant risk inputs.
3. Each input contributes to the overall risk score.
4. The final score determines the customer’s risk tier.
5. Higher-risk customers are routed for stronger due diligence.
6. The institution uses that output to support AML decisions.

So CRR does not operate in a vacuum. It feeds directly into review frequency, escalation paths, and EDD intensity.

If the model underweights important factors, high-risk customers may look lower-risk than they should. If it overweights minor factors, the program may create unnecessary noise.

---

## 📌 What CRR inputs mean in practice

A CRR model typically considers multiple dimensions at once. For example:

- **Customer type**: Is the customer retail, business, nonprofit, or something more complex?
- **Geography**: Are they domestic, cross-border, or linked to higher-risk jurisdictions?
- **Product usage**: Are they using cash-heavy, wire-heavy, or complex products?
- **Channel usage**: Do they rely on branch, digital, or third-party channels?
- **Expected activity**: Does the actual behavior match what was disclosed?
- **Risk flags**: Are there adverse media, PEP, sanctions proximity, or entity complexity signals?

These inputs are combined into a broader risk score. That score is then used to shape review decisions and monitoring expectations.

---

## 🧩 The analytics angle

From an analytics perspective, CRR is one of the clearest examples of structured risk modeling.

It gives analysts a way to:
- standardize customer review decisions,
- compare risk across customer segments,
- identify which inputs drive the score,
- and understand where the model may be too loose or too strict.

This is where analytics adds value:
- by making the risk logic transparent,
- by supporting consistent decisioning,
- by revealing which factors matter most,
- and by helping teams justify review outcomes.

Even at this stage, good analytics can improve governance and reduce subjective variability.

---

## 💡 Practical example

Imagine two customers:

### Customer A
- local retail customer,
- simple account structure,
- domestic activity,
- low-volume expected transactions,
- no adverse flags.

### Customer B
- business customer,
- multiple jurisdictions,
- cross-border activity,
- complex ownership structure,
- higher expected movement of funds,
- adverse media concerns.

A CRR model would not treat these two customers the same way.

Customer B would likely receive a higher risk rating and a more frequent review cycle. Customer A might be assigned a lower rating with lighter review intensity.

This is the practical value of weighting: it helps the institution distinguish between lower-risk and higher-risk customers in a consistent way.

---

## 📈 What the notebook or workbook should show

The notebook or workbook should remain simple and readable.

A strong first version could include:
- synthetic customer input records,
- a few CRR model factors,
- weighted scores,
- a simple risk tier output,
- and a short explanation of the output.

The goal is to show the logic, not to model every possible AML scenario.

---

## 🔄 Why this matters

Customer risk rating is more effective when it reflects meaningful differences in customer profiles.

If the model gives equal weight to every field, it may miss the factors that really drive risk. A weighted CRR approach helps focus attention where it matters most.

This is especially important for analytics work because the quality of the score determines the quality of the due diligence, review cadence, and escalation outcomes.

---

## 📚 Further reading

If you want to explore the ideas behind this exercise more deeply, these references are a good starting point:

- [Customer Risk Rating: The Complete Guide](https://www.complyadvantage.com/insights/customer-risk-rating/)
- [Customer risk profiling for AML compliance](https://www.flagright.com/post/customer-risk-profiling-a-key-to-aml-compliance)
- [Top customer risk profiling techniques to enhance compliance accuracy](https://www.prospero.systems/insights/top-customer-risk-profiling-techniques-to-enhance-compliance-accuracy)
- [Understanding risk-based approach in AML for effective compliance](https://www.au10tix.com/blog/understanding-risk-based-approach-in-aml-compliance/)
- [How to build a customer risk rating model](https://www.sas.com/en_us/insights/articles/risk-fraud/customer-risk-rating-model.html)
- [Risk-based approach to AML compliance](https://www.finra.org/rules-guidance/key-topics/aml)
- [Customer due diligence under the CDD final rule](https://www.fincen.gov/resources/statutes-and-regulations/cdd-final-rule)
- [Risk-based customer due diligence](https://www.lexisnexisrisk.com/blog/customer-risk-rating/)
- [AML risk rating model best practices](https://www.sanctions.io/blog/aml-risk-rating/)
- [Customer risk rating and EDD decisioning](https://www.acams.org/en/resources/risk-based-approach)

