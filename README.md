
# Fitness Subscription Analytics 

## Executive Summary
This project delivers a comprehensive subscription and transaction analytics solution built in **Tableau**. The dashboard suite evaluates core subscription dynamics, customer retention behaviors, 12-month revenue forecasts, and unit economics (Customer Acquisition Cost vs. Cumulative Lifetime Value) across customer cohorts.

---

## Key Business Findings & Answers

### 1. Customer Cohort Analysis (`cohort_analysis.PNG`)
* **Business Question:** *After how many months do customers typically cancel their subscriptions?*
* **Key Finding:** Retention tracking across monthly cohorts (e.g., January 2024 through December 2025) highlights a significant customer churn drop-off occurring between **Month 2 and Month 3**. For instance, in the January 2024 cohort, active users drop from 122 at Month 2 down to 78 at Month 3. Customers who persist past Month 3 demonstrate remarkably stable, long-term retention out to 24 months.

### 2. Revenue Forecast (`revenue_forecast.png`)
* **Business Question:** *What is the expected subscription revenue over the next 12 months? Does the revenue forecast show evidence of seasonality?*
* **Key Finding:** Utilizing exponential smoothing with a 12-month seasonal cycle, historical monthly revenue (ranging from $7,008 in Jan 2024 up to $275,624 in Dec 2025) is projected to grow further. Over the next 12 forecasted months (February 2026 to January 2027), projected monthly revenue ranges from $223,206 up to a peak of $356,210 in December 2026, totaling approximately **$3.37M**.
* **Seasonality Evidence:** Yes, the forecast clearly demonstrates strong **annual seasonality**, reflecting predictable spikes during the year-end holiday season (November/December peaks) and subsequent resets/dips at the start of each year.

### 3. CAC vs. LTV Analysis (`cac_vs_ltv.PNG`)
* **Business Question:** *How long does it take for the 2024 and 2025 cohorts to recover their customer acquisition cost?*
* **Key Finding:** 
  * **Aggregate Timeline:** When evaluating cumulative revenue across all acquired customers against the total fixed acquisition cost (**$1,663,996** total CAC), the cumulative LTV curve intersects and recovers total CAC during **September 2025**.
  * **Cohort Tenure Breakdown (Payback Period):** When filtering by individual cohort year (`Cohort Year`), both the **2024 and 2025 customer cohorts** reach their CAC break-even point by **Month 3** of customer tenure (`Months Since First Purchase`). Average cumulative LTV per customer surpasses average CAC (~$178–$179) within 3 months, making each cohort net-profitable early in its lifecycle.
