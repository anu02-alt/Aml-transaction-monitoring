# Aml-transaction-monitoring
AML transaction monitoring system combining rule based typologies with ML anomaly detection.
# AML Transaction Monitoring Model
**Author:** Anushka Shinde | MS Finance, Boston University

## Overview
An end-to-end Anti Money Laundering (AML) transaction monitoring system 
built in Python. Combines rule-based typologies with a Machine Learning 
anomaly detection model to risk-score 500 banking transactions.

## What This Project Does
- Generates 500 synthetic banking transactions
- Applies 7 rule-based AML red flags (structuring, high-risk countries, 
  smurfing, shell companies, prior SAR, and more)
- Trains an Isolation Forest ML model to score each transaction 0–100
- Exports a formatted Excel report with executive summary, alert sheet, 
  and methodology documentation

## AML Typologies Covered
| Red Flag | Description |
|---|---|
| Structuring | Amounts $9,000–$9,999 to avoid CTR filing |
| High-Risk Country | FATF-listed jurisdictions |
| Unusual Amount | 5x above customer's historical average |
| Shell Company + Wire | High-risk entity type combinations |
| Prior SAR | Previously reported customers |
| New Account High Value | <1 year old accounts with large transactions |
| Excessive Frequency | Smurfing detection |

## Tech Stack
- Python (pandas, numpy, scikit-learn, openpyxl)
- Machine Learning: Isolation Forest (unsupervised anomaly detection)
- Output: Formatted Excel report

## Files
- `Stage1` → Data generation
- `Stage2` → Rule-based red flags
- `Stage3` → ML risk scoring
- `Stage4` → Excel report generation
- `AML_Transaction_Monitoring_Report.xlsx` → Final output

## Background
This project is informed by my experience as a Forensic and Financial 
Crime Executive at Deloitte, where I analyzed complex financial datasets 
to identify anomalies, risk indicators, and patterns supporting AML investigations.
