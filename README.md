# Manufacturing Analytics & Predictive Maintenance

An end-to-end manufacturing analytics project combining **Power BI, DAX, Python and Machine Learning** to analyse manufacturing quality performance and identify potential machine-failure risks.

The project demonstrates how manufacturing data can be transformed into actionable insights for **quality monitoring, defect analysis, CAPA tracking and predictive maintenance**.

---

## Project Overview

The project consists of two interconnected analytics components:

### 1. Manufacturing Quality Analytics

A Power BI dashboard designed to provide visibility into manufacturing quality performance, including:

- Overall Equipment Effectiveness (OEE)
- First Pass Yield (FPY)
- Defect analysis
- Defect Pareto analysis
- Root cause analysis
- CAPA tracking
- Rejection analysis
- Station and section-level performance
- Quality trends over time

### 2. Predictive Maintenance

A Python-based machine learning model developed to estimate the probability of machine failure using machine sensor parameters.

The model output is integrated into Power BI to identify machines requiring further attention based on their predicted failure risk.

---

# Predictive Maintenance

## Objective

The objective of the predictive maintenance component is to estimate machine-failure risk based on operating and process parameters.

The model uses the following features:

- Tool Wear (min)
- Torque (Nm)
- Process Temperature (K)
- Air Temperature (K)
- Rotational Speed (RPM)

The target variable is:

`Machine_Failure`

---

## Machine Learning Workflow

```text
Manufacturing Sensor Data
          ↓
Exploratory Data Analysis
          ↓
Class Imbalance Analysis
          ↓
Train / Test Split
          ↓
SMOTE on Training Data
          ↓
Random Forest Classifier
          ↓
Failure Probability
          ↓
Risk Classification
          ↓
Power BI Dashboard

