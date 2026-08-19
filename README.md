TELECOM CHURNQUEST
Excel-based customer churn analysis for a telecom company, built with pivot tables, pivot charts, and an interactive dashboard.
Problem & Background
The telecom company is experiencing customer churn. This analysis examines call, usage, and plan data for 10,276 customers to identify why customers are leaving and where retention efforts will have the greatest impact.
Approach
The response combines three elements:
Data Analysis — usage patterns, plan types, and service-call history are analysed to pinpoint high-risk customer segments.
Data-Driven Insights — recurring churn triggers (plan type, service friction, usage intensity) are identified and quantified.
Stakeholder Action — findings are framed as concrete, department-actionable recommendations (retention, pricing, service).
Goals
Reduce the overall churn rate.
Identify the factors that most strongly promote churn and target them with suitable retention action.
Methodology
Data source: Local telecom customer dataset (10,276 records, 19 fields)
Data wrangling: Understanding, cleaning, and structuring the raw data
Data analysis: Pivot tables to surface trends and patterns across 13 KPIs
Data visualisation: Pivot charts and a consolidated dashboard
Dataset
10,276 customer records with 19 fields covering state, account length, area code, international/voice-mail plan flags, day/evening/night/international minutes-calls-charges, customer service calls, and churn status. Full field definitions are in the `DATA DICTIONARY` sheet.
Workbook Structure
Sheet	Contents
`DATA`	Raw customer-level dataset (10,276 rows × 19 columns)
`DATA DICTIONARY`	Field-by-field definitions of every column in `DATA`
`KPI`	Index of the 13 business questions analysed
`KPI1` – `KPI13`	One pivot table + chart per KPI, each with an Insight and a recommended Action
`DASHBOARD`	Consolidated view combining the key charts from all 13 KPIs
KPIs & Findings
Overall churn rate — 13.96% of customers churned (1,435 of 10,276).
State-wise churn — by rate, New Jersey (27.0%) and California (26.4%) are highest-risk; by raw count, West Virginia (326), Minnesota (261) and Idaho (248) see the most churn.
Account length vs. churn — nearly identical: 101.9 months (churned) vs. 99.9 months (retained). Tenure is not a meaningful predictor.
International plan vs. churn — the strongest driver found: 42.2% of international-plan customers churn vs. 11.0% of those without the plan, a ~4x gap.
Customer service calls vs. churn — flat around 11% churn for 0–3 calls, then spikes to 44–100% at 4 or more calls — a clear escalation tipping point.
Day call charges vs. churn — churned customers average $35.41 vs. $29.88 for retained customers.
Evening call charges vs. churn — smaller gap: $17.82 (churned) vs. $16.87 (retained).
Night call charges vs. churn — smaller gap: $9.29 (churned) vs. $8.98 (retained).
International call charges vs. churn — modest gap: $2.87 (churned) vs. $2.75 (retained).
Total day minutes vs. churn — churned customers average 208.3 minutes vs. 175.6 for retained customers.
Voice-mail plan vs. churn — protective effect: 7.6% churn for subscribers vs. 16.3% for non-subscribers.
International minutes vs. churn — slightly higher for churned customers (10.6 vs. 10.2 minutes).
Total day calls vs. churn — retained customers place more day calls in aggregate than churned customers.
Technical Processes
Data cleaning
Pivot tables
Pivot charts
Dashboard design
Conclusion
Churn affects 13.96% of the customer base, warranting focused reduction strategies.
Account tenure has little bearing on churn — the driver lies elsewhere.
International plan subscription is the single strongest churn signal (42.2% vs. 11.0% churn), and warrants a review of that plan's pricing and value proposition.
Repeated customer service contact is a tipping-point signal — churn risk holds steady through 3 calls, then rises sharply from the 4th call onward, pointing to a first-contact-resolution gap.
Voice-mail plan adoption is associated with meaningfully lower churn, suggesting it functions as a retention lever.
Call charges (evening, night, international) differ only modestly by churn status; day usage shows the clearest gap.
How to Use This Workbook
Open `KPI` for a quick index of all 13 analyses.
Open any `KPI1`–`KPI13` sheet to see that pivot table, its chart, and the Insight/Action notes above it.
Open `DASHBOARD` for the consolidated view.
Refresh pivot tables via Data > Refresh All if the source data in `DATA` is updated.
Tools Used
Microsoft Excel — PivotTables, PivotCharts, and dashboard design.
Project Owner
Chetan
