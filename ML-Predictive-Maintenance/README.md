# Manufacturing Analytics & Predictive Maintenance

An end-to-end manufacturing analytics project combining Power BI, DAX, Python and Machine Learning to analyse manufacturing quality and predict potential machine failures.

## Project Overview

This project demonstrates two complementary analytics applications:

1. Manufacturing Quality Analytics
2. Predictive Maintenance

The quality analytics component uses Power BI and DAX to analyse defects, root causes, CAPA performance, rejection trends and manufacturing sections. The predictive maintenance component uses Python and Random Forest to estimate machine failure probability based on machine sensor parameters.

## Predictive Maintenance

### Objective

Predict the probability of machine failure using:

- Tool Wear
- Torque
- Process Temperature
- Air Temperature
- Rotational Speed

### Machine Learning Workflow

```text
Raw Sensor Data
↓
Exploratory Data Analysis
↓
Class Imbalance Analysis
↓
Train/Test Split
↓
SMOTE on Training Data
↓
Random Forest
↓
Failure Probability
↓
Risk Classification
↓
Power BI Dashboard




## Handling Class Imbalance

The dataset contains a very small number of failure observations compared with normal observations.
SMOTE (Synthetic Minority Over-sampling Technique) was therefore applied only to the training dataset to improve learning of the minority failure class.

## Model Output

The model generates:

- Predicted Failure Probability
- Predicted Failure
- Risk Flag

A probability threshold of 0.30 is used to identify machines requiring further maintenance attention.

## Feature Importance

Random Forest feature importance is used to identify which sensor variables contribute most strongly to the model's predictions.
In this synthetic dataset, Tool Wear was the most influential feature.

## Power BI Dashboard

The predictions are integrated into a Power BI dashboard containing:

- Total Failures
- Failure Rate
- MTBF
- Machines at High Risk
- Failure Type Distribution
- Machine Risk Plot
- Predicted Failure Probability
- Risk Flag
- Feature Importance

## Important Limitation

This project uses a synthetic dataset containing very few failure events. Therefore, the model should be considered a proof-of-concept rather than a production-ready predictive maintenance system. A production implementation would require substantially more real-world failure data, validation across multiple machines and operating conditions, continuous monitoring, model retraining and an appropriate business-driven risk threshold.

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Matplotlib
- Power BI
- DAX
- GitHub

## Repository Structure

Manufacturing-Analytics/
│
├── README.md
├── predictive_maintenance.ipynb
└── requirements.txt
