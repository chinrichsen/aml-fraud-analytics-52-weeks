# Week 3 Thursday Exercises — EDD Triggers for High-Risk Customers


This folder contains the hands-on materials for **Week 3 Thursday** of the 52-week AML and fraud analytics series.


The theme for this week is **EDD triggers for high-risk customers**. The key idea is that a high customer risk rating is not the end of the process. Once a customer reaches a high-risk threshold, the institution still needs to determine whether that customer should move into enhanced due diligence, standard review, or another escalation path.


These exercises are important because they help the reader understand one of the most practical truths in AML decisioning:


> **A high risk score only becomes useful when it drives a clear routing decision.**


The goal is not to build a production decision engine. The goal is to create a clear learning artifact that shows how CRR thresholds and trigger checks can be translated into an EDD decision tree and a simple routing framework.


---


## What is included in this folder?


This folder includes:
- a synthetic customer risk dataset,
- an Exercise 1 solution file,
- an Exercise 2 solution notebook,
- and this instruction file.


The files are designed to be easy to understand, easy to explain, and easy to extend in future weeks.


---


## Why these exercises are important


EDD matters because AML teams need a structured way to decide when a customer requires deeper review.


Examples include:
- high CRR scores,
- adverse media,
- PEP exposure,
- sanctions concern,
- cross-border complexity,
- ownership opacity,
- and other escalation triggers.


If the institution does not separate these triggers clearly, the review process can become inconsistent and harder to defend. These exercises help show how a threshold-based workflow can route customers to the right review path.


---


## Exercise 1 — Route customers to EDD or standard review


### Objective


Use the synthetic dataset to determine whether each customer should be routed to enhanced due diligence or standard review.


### What you should do


1. Review each customer record in the synthetic dataset.
2. Check whether the CRR score is above the defined threshold.
3. Evaluate the trigger buckets separately.
4. Determine whether adverse media, PEP, or sanctions concern is present.
5. Route the customer to either EDD or standard review.
6. Recommend the most appropriate monitoring action.


### Why this exercise matters


This exercise is important because it teaches how risk scores become operational decisions.


It also shows that the routing logic should not depend on only one trigger. A customer may have no adverse media but still require EDD because of PEP status or sanctions concern. That is one of the most important ideas in escalation design.


### Example logic


A simple routing logic could look like this:


`IF CRR Score > Threshold AND (Adverse Media OR PEP OR Sanctions) THEN Route to EDD`


`IF CRR Score > Threshold AND none of the trigger buckets are positive THEN Route to Standard Review`


You can tune the threshold and trigger conditions to see how the output changes.


### Deliverable


Create a solution table with at least the following columns:
- `customer_id`
- `customer_name`
- `crr_score_0_100`
- `adverse_media`
- `pep`
- `sanctions`
- `edd_decision`
- `review_frequency`
- `recommended_action`


---


## Exercise 2 — Build the EDD decision tree


### Objective


Build a simple decision tree in Python using the synthetic dataset and use it to classify customers into EDD or standard review.


### What you should do


1. Use the same synthetic customer risk dataset.
2. Define a target label based on the routing logic.
3. Train a decision tree classifier.
4. Review the decision rules that the model learns.
5. Apply the model to the customer cases.
6. Compare the predicted routing result against the expected result.


### Why this exercise matters


This exercise is important because it makes the routing logic explicit and easy to explain.


It also shows how a decision tree can mirror business logic in a readable form. That is especially useful in AML analytics, where explainability matters as much as accuracy.


### Deliverable


Create a notebook output with at least the following:
- the synthetic dataset,
- the target label definition,
- the trained decision tree,
- the learned decision rules,
- and the final prediction table.


---


## How to use the files


- Open the synthetic dataset and inspect the risk factors.
- Work through Exercise 1 before reviewing the solution file.
- Use Exercise 2 to understand how the decision tree supports the routing logic.
- Review the solution notebook to check your interpretation.


---


## Learning outcome


By the end of these exercises, the reader should be able to:
- recognize when a CRR score should trigger escalation,
- understand how separate trigger buckets affect routing decisions,
- explain why PEP, sanctions, and adverse media should remain distinct checks,
- and use a decision tree to model a simple EDD routing flow.


That is a critical skill in AML analytics, because a strong risk model needs both **good thresholds** and **clear decision logic**.
