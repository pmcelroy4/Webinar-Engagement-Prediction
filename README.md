# Webinar-Engagement-Prediction
Lead analysis project for a fictional company, ProfDev, which runs weekly webinars and seeks to identify high-potential prospects. Using engagement, survey responses, location, and lifecycle stage data, this project analyzes marketing interactions to surface the best leads for sales outreach.

# ProfDev Lead Scoring Analysis

This project analyzes marketing engagement data for a fictional company, ProfDev, which hosts weekly professional-development webinars. The goal is to identify high-quality leads who are most likely to convert into customers so sales teams can focus outreach efforts efficiently.

# Project Overview

As part of a Business Operations workflow, this analysis evaluates how webinar behavior, survey responses, and basic lead attributes correlate with downstream sales actions—specifically whether a lead ultimately booked a demo.

You’ll explore and model the data to surface the most promising prospects based on their interactions with ProfDev’s marketing funnel.

Dataset Description

Each row in the dataset represents a single lead. Key columns include:

Engagement Metrics

Number of webinars registered

Number of webinars attended

Average attendance duration

Count of webinars where attendance duration exceeded 50%

Survey Behavior

Post-webinar survey response

1 — lead expressed interest in speaking with the team

0 — no interest indicated

Lead Attributes

Geographic location

Lifecycle stage

1 — booked a sales demo

0 — did not book a demo

Objectives

Clean and explore the engagement dataset.

Engineer features to better capture lead quality.

Train classification models (e.g., logistic regression, decision trees) to predict demo-booking likelihood.

Interpret feature importance to understand what behaviors signal buying intent.

Surface the highest-potential leads for targeted sales outreach.

Key Findings

(Based on the notebook structure—expand or revise as needed.)

Post-webinar survey interest is one of the strongest predictors of demo booking.

Webinar engagement (attending more sessions, staying longer) correlates with higher conversion likelihood.

Location has less predictive power and may not materially improve model performance.

Repository Structure
├── market_analysis.ipynb   # Main analysis notebook
├── README.md               # Project documentation
└── data/                   # (Optional) Input dataset location

Tools & Libraries Used

Python

Pandas · NumPy

Scikit-learn

Matplotlib · Seaborn

Future Improvements

Deploy a production-ready lead scoring pipeline

Automate daily scoring using a scheduled workflow

Integrate with CRM systems (e.g., HubSpot, Salesforce)

Add real-time dashboards for marketing and sales teams
