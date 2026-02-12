# SaaS Retention Analytics

## Client Background
A subscription-based SaaS company wants to better understand customer churn and retention patterns. Leadership is concerned about declining retention and wants to identify the key drivers of churn and opportunities to improve customer engagement.

Stakeholders:
- Executive leadership (retention and growth)
- Finance (revenue impact of churn)
- Product team (engagement and onboarding)
- Customer Success (at-risk accounts)

---

## North Star Metrics
Primary Metrics:
- Financial churn rate
- Active customer rate

Supporting Metrics:
- Engagement churn rate
- Silent churn rate
- Revenue per customer
- Cohort retention trends

---

## Executive Summary
- Financial churn is approximately 43% across customers.
- Churn rates are relatively consistent across plan tiers, suggesting pricing alone is not the main driver.
- Cohort analysis shows churn is stable across signup periods.
- Silent churn (customers paying but inactive) represents a significant retention risk.

Key Recommendation:
- Trigger outreach and engagement workflows for customers inactive for 30+ days.

---

## Data Structure & ERD

Datasets:
- customers.csv
- subscriptions.csv
- transactions.csv
- user_activity.csv

Relationships:
- Customers → Subscriptions (1-to-many)
- Customers → Transactions (1-to-many)
- Customers → User Activity (1-to-many)

Customer is the central entity used to build a customer-level feature table.

---

## Insights Deep Dive

### Churn by Plan
Churn rates are similar across Basic, Standard, and Premium tiers, indicating retention challenges are likely driven by engagement or product value rather than pricing alone.

### Cohort Analysis
Financial churn remains relatively stable across signup cohorts, suggesting onboarding quality is consistent but overall retention requires improvement.

### Silent Churn
A large portion of customers continue to pay but are inactive, indicating a strong opportunity for re-engagement campaigns.

---

## Project Structure

