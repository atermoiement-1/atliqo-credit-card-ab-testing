\# AtliQo Bank — Credit Card A/B Testing Project



\## Overview

An end-to-end data science project analyzing customer data for AtliQo Bank and running a statistically rigorous A/B test to evaluate whether a newly launched credit card increases average customer transaction amounts, with a focus on the underserved 18–25 age demographic.



\## Project Structure

\- \*\*Phase 1 — Data Cleaning \& EDA:\*\* Merged customer, credit profile, and transaction datasets (\~1000 customers). Handled missing values using occupation-wise medians, resolved logical inconsistencies (e.g. outstanding debt exceeding credit limit), and identified young adults (18–25) as a high-opportunity, underserved segment.

\- \*\*Phase 2 — A/B Testing:\*\* Conducted a power analysis to determine required sample size under budget constraints, launched a 2-month campaign comparing a control group (existing card) against a test group (new card), and validated results using a one-tailed two-sample Z-test — both manually implemented and cross-checked against `statsmodels`.



\## Key Findings

\- The new credit card produced a statistically significant increase in average transaction amount (Z ≈ 2.75, p ≈ 0.003) compared to the existing card.

\- Result confirmed independently via manual Z-score calculation, p-value computation, and `statsmodels.stats.ztest`.



\## Tools \& Libraries

Python · pandas · numpy · scipy · statsmodels · matplotlib · seaborn



\## Limitations

\- Campaign ran over a 2-month window; seasonal effects not controlled for.

\- Only 40% of the test group adopted the new card, introducing potential self-selection bias.

\- Result establishes statistical association, not causation.



\## Author

Sathani Vishnu Vardhan — Data Science / AI-ML (MCA)

