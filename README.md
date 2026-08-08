# Manufacturing Analytics

An end-to-end manufacturing analytics project focused on **quality engineering, defect analysis, CAPA management, and predictive maintenance**, developed using **Power BI, DAX, Python, and Machine Learning**.

The project demonstrates how manufacturing data can be transformed into actionable insights to identify **where quality losses are occurring, why they are occurring, and which machines may require preventive attention**.

---

## Project Overview

The project is structured around two major analytical areas:

### 1. Manufacturing Quality Analytics

A Power BI-based quality engineering dashboard designed to provide a structured view of manufacturing quality performance.

The dashboard enables analysis of:

- Quality KPIs
- Rejected units
- Defect trends
- Top defects and Pareto analysis
- Defect categorization
- Root cause frequency
- Section-level performance
- Station-level performance
- Shift-wise analysis
- CAPA tracking
- CAPA closure performance
- Quality loss analysis

The objective is to move from:

**"How many defects do we have?"**

to:

**"Where are the defects occurring, what are the major contributors, and where should the quality team act first?"**

---

### 2. Predictive Maintenance

A Python-based machine learning component was developed as an extension of the manufacturing analytics framework.

The objective is to estimate the probability of machine failure using machine operating parameters such as:

- Tool Wear
- Torque
- Process Temperature
- Air Temperature
- Rotational Speed

The resulting failure probabilities are integrated into Power BI to provide a machine-level risk view and support preventive maintenance prioritization.

---

# Manufacturing Quality Analytics

## Quality Engineering Dashboard

The Power BI dashboard is designed around the typical quality investigation workflow:

```text
Overall Quality Performance
          ↓
Identify Major Defects
          ↓
Pareto Analysis
          ↓
Identify Affected Section / Station
          ↓
Investigate Root Causes
          ↓
Track CAPA
          ↓
Monitor Improvement

