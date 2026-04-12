---
name: business-analytics
description: Analyze a dataset with regression, discover patterns, and build a professional browser-based dashboard
---

# Business Analytics Skill

When the user provides a dataset or points to a CSV file, follow this pipeline:

## Step 1: Inspect
- Read the dataset. Report shape, dtypes, head, and missing values.
- Summarize key variables and suggest which are outcomes vs. predictors.
- Ask the user to confirm the target variable and any controls before proceeding.

## Step 2: Regression
- Run a regression of the target variable on the main predictor.
- Then add controls (market, category, time) and compare coefficients.
- Interpret the result in business terms (e.g., elasticity, lift, ROI).

## Step 3: Explore
- Identify 2–3 interesting patterns in the data (trends, segments, outliers).
- Generate charts for each pattern.

## Step 4: Save Code
- Save all analysis code as `analysis.py` in the workspace so the user can review and reproduce.

## Step 5: Dashboard
- Build a single-file `dashboard.html` that opens in any browser with no dependencies.
- Include: regression results, key charts, and a summary of findings.
- Use clean, professional styling.

## Rules
- Always show the user the regression output before building the dashboard.
- Never drop rows without explaining why.
- Keep the dashboard self-contained — inline all CSS and JS, no external CDN.
