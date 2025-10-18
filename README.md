“A Trustworthy and Explainable Deep Learning Framework for Multi-Level Anxiety Severity Assessment and Binary Risk Screening.”

📋 Overview

The project presents a reliable, interpretable, and robust transformer-based deep learning framework designed to assess anxiety severity and risk using heterogeneous psychosocial data. The dataset integrates validated psychological questionnaires (GAD-7, PHQ-9), demographic variables, and academic stress indicators.

🧩 Key Highlights

Model Architecture: Transformer-based neural network optimized for tabular inputs, featuring linear input projections, multi-head self-attention, feedforward layers, residual connections, and dropout-based regularization.

Feature Selection: ANOVA F-test used to select the top 31 predictors for multiclass and 27 for binary classification.

Evaluation Protocol: Stratified 5-fold cross-validation with testing on a held-out dataset.

Performance:

Multiclass setting: Accuracy = 92.00 ± 0.45%, Macro F1 = 89.67 ± 0.38%, AUC-ROC = 0.9234 ± 0.0041

Binary setting: Accuracy = 99.26 ± 0.21%, Macro F1 = 99.16 ± 0.19%, AUC-ROC = 0.9723 ± 0.0028

🧮 Robustness, Uncertainty & Explainability

Adversarial Robustness: Evaluated using FGSM and PGD perturbations, showing minimal degradation.

Uncertainty Quantification: Performed using Monte Carlo Dropout, providing both sample-level and overall predictive confidence.

Explainable AI (XAI): Implemented via SHAP for local and global explanations on both clean and adversarial samples.

Human-in-the-loop Component: A referral mechanism is integrated to flag uncertain predictions for expert review.
