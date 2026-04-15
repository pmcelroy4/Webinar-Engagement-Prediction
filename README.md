# Webinar Engagement Lead Scoring Model

This project analyzes webinar engagement data for a fictional company, ProfDev, which runs weekly professional-development webinars. The goal is to identify high-potential leads who are most likely to convert into a business opportunity, enabling more efficient and targeted sales outreach.

The analysis focuses on behavioral engagement signals such as webinar attendance, duration, survey responses, and geographic attributes to predict whether a lead will convert.

---

# Project Overview

As part of a marketing analytics and business operations workflow, this project builds a supervised classification model to predict lead conversion (i.e., whether a user books a demo).

The workflow includes:
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Feature engineering and encoding
- Handling class imbalance
- Model training (Logistic Regression)
- Model evaluation using multiple metrics beyond accuracy
- Feature interpretation and business insight generation

A key focus of this project is addressing **class imbalance**, which initially resulted in misleadingly high accuracy but poor predictive performance for the minority class.

---

# Dataset Description

Each row represents a unique lead interacting with ProfDev’s webinar funnel.

## Engagement Metrics
- Number of webinar registrations
- Number of webinars attended
- Average webinar attendance duration
- Number of sessions with >50% attendance duration

## Survey Behavior
- Post-webinar survey response indicating interest in speaking with the team
  - 1 = expressed interest
  - 0 = no interest / no response

## Target Variable
- Opportunity (binary classification target)
  - 1 = booked a demo / converted
  - 0 = did not convert

---

# Modeling Approach

## Baseline Model
A Logistic Regression model was trained to establish a baseline for conversion prediction.

## Class Imbalance Handling
The dataset exhibited significant class imbalance, with far fewer positive conversions than non-conversions. To address this, **oversampling (upsampling the minority class)** was applied to improve model learning and recall for the positive class.

## Evaluation Strategy
Model performance was evaluated using:
- Accuracy (baseline reference only)
- Confusion Matrix
- Precision, Recall, and F1-score
- ROC Curve and AUC
- Precision-Recall Curve (important for imbalanced classification)

---

# Key Findings

- Survey engagement (expressed interest in speaking with ProfDev) is the strongest predictor of conversion.
- Webinar engagement behaviors (attendance frequency and duration) also contribute meaningfully to prediction performance.
- Geographic features were less predictive and risk introducing overfitting or reduced generalization.
- The initial high accuracy masked poor minority-class performance, highlighting the importance of using **recall, ROC-AUC, and PR curves** for evaluation.

---

# Repository Structure

```bash
.
├── market_analysis.ipynb
├── data/
├── README.md