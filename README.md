# Predicting Purchase Value Using Session-Level Behavioral Data

## Overview
This project focuses on predicting customer purchase value using multi-session behavioral data from a large-scale digital commerce platform. By analyzing user engagement patterns, acquisition channels, device characteristics, and geographic context, the model estimates the monetary value of each session to support data-driven marketing and personalization strategies.

## Problem Statement
Understanding and predicting purchase value at the session level enables businesses to optimize marketing spend, prioritize high-value users, and improve engagement strategies. The objective of this project is to build a regression model that accurately estimates purchase value based on user behavior across digital touchpoints.

## Dataset
The dataset contains anonymized **session-level data** from a digital commerce platform. Each row represents a unique user session.

### Feature Categories
- **User Behavior & Session Metrics:** page views, total hits, visit counts, bounce indicators, session timing
- **Device & Technical Attributes:** device type, operating system, browser, screen size, language
- **Traffic & Marketing Source:** acquisition channel, campaign, medium, referral path, ad interaction signals
- **Geographical Context:** country, region, city, continent, and location-based clusters
- **Identifiers:** user and session identifiers enabling multi-session analysis

**Target Variable:**  
- `purchaseValue` — total amount spent during a given session

## Evaluation Metric
Model performance is evaluated using **R² (coefficient of determination)**, measuring how well predicted purchase values explain variance in actual outcomes.

## Approach
- Data cleaning and preprocessing of behavioral and categorical features
- Exploratory analysis to understand engagement and purchase patterns
- Feature selection and transformation for regression modeling
- Train–test split and baseline modeling
- Regression model training and evaluation using R²

## Key Results
- User engagement signals (such as session activity and page views) were strong predictors of purchase value
- Acquisition source and device characteristics contributed meaningfully to revenue prediction
- The model demonstrated reasonable explanatory power given the sparsity and skew typical of purchase value data

## Tools & Technologies
Python (Pandas, NumPy, Scikit-learn), data visualization libraries

## Repository Contents
- `analysis.ipynb`: End-to-end workflow covering preprocessing, modeling, and evaluation
