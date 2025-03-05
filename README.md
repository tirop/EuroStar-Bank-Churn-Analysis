# ﻿Project Background

EuroStar Bank, the seventh largest financial institution in Western Europe, seeks to improve customer retention using customer data to identify and understand drivers of member attrition. While EuroStar operates across multiple countries, this institution has made  Germany, Spain, and France a priority, as these countries represent 65% of its members. 
This report uses a dataset containing 10,000 customer records. These records consist of customer demographics, behavior, and financial details. The objective is to use this data to identify the factors that drive customer churn and provide actionable insights to enhance retention strategies.

The insights and recommendations provided within this report are provided on the following key areas:
* Tenure, Location, Gender: Evaluation of patterns in length of membership, geography, and gender with a focus on rates of churn within each field.
* Retention metrics: An analysis of EuroStar Bank’s retention rates benchmarked against target rates.
* Churn Predictions: Assessing key areas such as demographics and tenure make key predictions in terms of churn

### Data Sources:
* An interactive Tableau Dashboard can be downloaded ([here](https://public.tableau.com/app/profile/joshua.kendagor/viz/BankChurn_1_v4/ChurnDashboardV2)).
* Original Dataset: ([here](https://github.com/tirop/EuroStar-Bank-Churn-Analysis/blob/main/Bank_Churn.csv)).


### Data Structure & Initial Checks:
EuroStar’s dataset contains 10,000 customer records. Each record represents a unique individual, with attributes categorized into the following dimensions:
* Demographic Data: Gender, age, geography.
* Behavioral Metrics: Tenure, number of products, credit card ownership, and activity status.
* Financial Metrics: Balance, salary estimate, credit score.
* Outcome: Churn (binary: exited or retained).
  
### Data Cleaning:
To prepare the data for analysis, the following preprocessing steps were applied:
* Addressed missing values and duplicates (e.g., replacing NULL with averages for numerical fields, and standardizing categorical data).
* Removed outliers and invalid entries.
* Ensured binary variables (has_cr_card, is_active_member) were encoded for analysis.
* Detailed cleaning of text fields like surname (removal of invalid characters).
* Dataset integrity validated after processing.
The dataset was visualized in Tableau ([here](https://public.tableau.com/app/profile/joshua.kendagor/viz/BankChurn_1_v4/ChurnDashboardV2)),
revealing trends in churn and retention by tenure, geography, and gender.

# Executive Summary

### Overview and Location Findings:

EuroBank’s current churn rate stands at 20.37%. This significantly exceeds the target rate of 15%, and signals a critical need for retention-focused interventions. 
Germany’s churn rate is 32.44% which is more than double that of Spain (16.67%) and France(16.5%). However, note that while Germany’s churn rates are higher than France or Spain, churn rates for all three countries are above the 15% target.

### Demographic Insight:
Female customers, with a churn rate of 25.07%, are at a higher risk of attrition compared to male customers (16.46%). This disparity suggests potential dissatisfaction or unmet needs among female clients, and highlights the need for tailored retention strategies. Again, note that while female churn rates exceed male churn, both genders exceed the target churn rate of 15%. 

### Tenure Analysis:
Early-tenure customers (tenure ≤1 year) face severe churn rates, with the highest churn at 23% for tenure of 0 years. These findings underscore the importance of targeted engagement strategies during the onboarding phase.

Below is the overview page from the Tableau dashboard. 

![Screenshot 2025-01-07 125939](https://github.com/user-attachments/assets/74f5fffd-49b9-44fe-a25b-921509e2e225)

The entire interactive dashboard can be downloaded([here](https://public.tableau.com/app/profile/joshua.kendagor/viz/BankChurn_1_v4/ChurnDashboardV2).
  
## Insights Deep Dive
### Demographics
Female customers are disproportionately affected, with a churn rate 25.07% compared to 16.46% in men- a disparity of  8.61 percentage points. This could indicate unmet needs or dissatisfaction among female clients that stem from product misalignment or communication gaps. To improve retention rates, this critical disparity must be addressed.

### Location
Germany's churn rate of 32.44% is more than double that of Spain (16.67%) and France (16.5%). This suggests location-specific challenges that could be linked to cultural preferences, competitive dynamics, or localized service issues. Germany's churn rate alone accounts for a substantial portion of EuroStar's customer attrition.

### Tenure
Newer customers (tenure ≤1 year) have the highest churn rates, peaking at 23% for first-year members. This trend underscores the importance of early engagement initiatives to improve retention and foster long-term loyalty. Customers with longer tenures demonstrate significantly lower churn rates. This fact highlights the value of sustained relationships, and why long term customer retention should remain a priority.

### Retention
The current retention rate stands at 79.63%. This is below the 85% target, and indicates the need for a strategic focus on at-risk segments. Our suggestion is to focus on key at-risk segments such as early-tenure customers, German clients, and female customers. Doing so will be instrumental in closing this gap.

### Recommendations
To address location, gender, and tenure related churn, we have some suggestions.
To mitigate churn and improve retention, the following targeted strategies are proposed:

Germany stands out as a clear priority, with a churn rate of 32.44%—far above the target of 15%—making swift action essential. One immediate step is to conduct customer satisfaction surveys to better understand pain points and pinpoint areas for service improvement. From there, targeted retention campaigns offering personalized discounts or incentives tailored to German customers could help reduce churn. Similar approaches should be extended to France and Spain, where churn rates (16.5% and 16.67%, respectively) also exceed the target.

In addition to location-specific strategies, gender-focused initiatives could further improve retention, particularly by designing financial products and services that address unmet needs for female customers. These efforts should be informed by feedback from surveys and focus groups, with tailored communication campaigns that emphasize empathy, transparency, and trust. Another critical focus should be tenure-based engagement, starting with stronger onboarding programs for new customers, including personalized financial consultations within the first six months, as well as loyalty incentives like fee waivers or cashback rewards during their first year.

To keep these strategies on track, EuroStar Bank should implement a retention monitoring framework, using monthly Tableau reports to track churn rates and spot emerging trends across regions and demographics. Quarterly stakeholder reviews will ensure the strategies remain effective and allow for adjustments as needed. By taking a multi-pronged approach that considers location, gender, and tenure, EuroStar Bank can better align its offerings with customer needs, reduce churn, and work toward its retention goal of 85%.
