Fraud Risk Decision Support

Logistic Regression | RapidMiner | EU Regulatory Framing

Executive Summary

This project implements an interpretable fraud risk classification model designed as a decision-support system, not an automated blocking tool.

Built using Logistic Regression in RapidMiner, the model assigns fraud risk predictions to banking transactions while prioritising:

Interpretability

Fraud recall (rare event detection)

Regulatory alignment (GDPR, EU banking context)

Human-in-the-loop oversight

The system demonstrates how AI can responsibly support fraud analysts in settlement risk management workflows.

Problem

Banking fraud detection faces:

Extremely imbalanced data (~0.12% fraud rate)

High transaction volumes

False positives from rule-based systems

Regulatory limits on automated decision-making

Accuracy alone is insufficient. Models must be explainable, auditable, and operationally practical.

Approach

Pipeline built in RapidMiner:

Data preparation and label assignment

Train/test split

Logistic Regression model training

Risk prediction on unseen data

Confusion matrix and performance evaluation

Logistic Regression was selected for its:

Transparency

Coefficient interpretability

Suitability for regulated financial environments

Key Insight

Given severe class imbalance, the focus is on:

Fraud recall (True Positive Rate)

Managing false positives

Supporting analyst prioritisation

This is framed as a risk scoring assistant, not an automated enforcement mechanism.

Governance Lens

Designed with:

GDPR Article 22 considerations

Human oversight requirements

Bias awareness

Auditability in mind

Fraud detection in finance is as much a governance challenge as a technical one.

Repository Contents

fraud_risk_decision_support.rmp – Reproducible RapidMiner pipeline

/visuals – Confusion matrix output

Project report (academic framing)

Academic Context

MSc Artificial Intelligence for Business
National College of Ireland
Module: Risk and Change Management

Takeaway

AI in financial services must balance performance with accountability.

This project demonstrates how interpretable models can support fraud risk management without compromising regulatory integrity.

This project demonstrates how interpretable models can responsibly support financial decision-making.
<img width="882" height="697" alt="Screenshot 2026-02-10 at 10 41 25 PM" src="https://github.com/user-attachments/assets/a2b89800-60c2-4e72-a355-47f5a81fe55d" />
<img width="549" height="390" alt="Screenshot 2026-02-11 at 1 10 48 AM" src="https://github.com/user-attachments/assets/d75236f5-040b-42ba-8348-7e2970c0b269" />
<img width="2048" height="1255" alt="Screenshot 2026-02-11 at 1 08 00 AM" src="https://github.com/user-attachments/assets/698b039b-ce95-4fb8-b29b-80f2bf9f0971" />
