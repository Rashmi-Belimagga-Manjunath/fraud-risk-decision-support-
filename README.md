Fraud Risk Decision Support System

Logistic Regression | RapidMiner | EU Regulatory Framing

Project Overview

This project develops a fraud risk classification model designed as a decision-support system, not an automated blocking tool.

Using Logistic Regression in RapidMiner, the model assigns fraud risk predictions to banking transactions while prioritising:

Interpretability

Recall for fraud cases

Regulatory alignment (GDPR, EU banking context)

Human-in-the-loop oversight

The objective is not full automation, but structured support for fraud analysts operating in regulated financial environments.

Problem Context

Fraud detection in banking is challenging due to:

Extremely large transaction volumes

Highly imbalanced data (fraud cases are rare)

High false-positive rates in traditional rule-based systems

Regulatory constraints on automated decision-making

Under GDPR (Article 22) and EU financial governance requirements, automated decisions affecting customers must be explainable and subject to human oversight.

This project demonstrates how AI can be responsibly integrated into settlement risk management workflows.

Dataset

The model uses a publicly available banking transactions dataset containing:

Transaction type (PAYMENT, TRANSFER, CASH_OUT, DEBIT)

Transaction amount

Account balance information

Fraud indicator (isFraud)

Key Observations

Fraud rate ≈ 0.12%

Severe class imbalance

High variance in transaction amounts

Presence of extreme outliers

This imbalance makes recall (detecting fraud cases) more important than raw accuracy.

Methodology

The RapidMiner pipeline includes:

Data Retrieval

Data Type Conversion

Label Assignment (isFraud as target variable)

Train/Test Split

Logistic Regression model training

Model application on test data

Performance evaluation (Confusion Matrix + Classification Metrics)

Why Logistic Regression?

Logistic Regression was chosen because:

It is interpretable

Coefficients can be explained to auditors

Suitable for regulated environments

Supports accountability and transparency

Model Evaluation

Performance was assessed using:

Confusion Matrix

Precision

Recall

Classification Accuracy

Given the severe class imbalance, emphasis was placed on:

Fraud recall (True Positive Rate)

Reduction of false positives

Practical usefulness in analyst workflows

📊 Confusion matrix screenshot available in the /visuals folder.

Business & Operational Impact

If deployed as decision-support:

Prioritises high-risk transactions for analyst review

Reduces manual workload

Minimises unnecessary customer friction

Supports faster settlement for legitimate transactions

Maintains regulatory compliance

The model is intentionally framed as a support mechanism — not a fully automated enforcement system.

Ethical & Governance Considerations

Bias risk in transaction data

Risk of disproportionate impact on certain users

GDPR Article 22 implications

Need for human-in-the-loop review

Requirement for auditability

Responsible AI design is central to financial system deployment.

Tools Used

RapidMiner Studio

Logistic Regression (H2O implementation)

Confusion Matrix Performance Evaluation

GitHub (documentation & reproducibility)

Repository Structure
fraud-risk-decision-support/
│
├── visuals/
│   └── confusion_matrix.png
│
├── Fraud_Risk_Decision_Support_Report.pdf
├── fraud_risk_decision_support.rmp
├── README.md


.rmp file allows full reproducibility in RapidMiner

Report contains detailed academic framing

Visuals folder contains performance outputs

Academic Context

Programme: MSc Artificial Intelligence for Business
Institution: National College of Ireland
Module: Risk and Change Management

This project reflects a governance-aware AI implementation approach suitable for regulated industries.

Key Takeaway

Fraud detection is not just a machine learning problem — it is a governance problem.

AI systems in banking must optimise not only for predictive performance, but for:

Explainability

Accountability

Regulatory compliance

Human oversight

This project demonstrates how interpretable models can responsibly support financial decision-making.
<img width="882" height="697" alt="Screenshot 2026-02-10 at 10 41 25 PM" src="https://github.com/user-attachments/assets/a2b89800-60c2-4e72-a355-47f5a81fe55d" />
<img width="549" height="390" alt="Screenshot 2026-02-11 at 1 10 48 AM" src="https://github.com/user-attachments/assets/d75236f5-040b-42ba-8348-7e2970c0b269" />
<img width="2048" height="1255" alt="Screenshot 2026-02-11 at 1 08 00 AM" src="https://github.com/user-attachments/assets/698b039b-ce95-4fb8-b29b-80f2bf9f0971" />
