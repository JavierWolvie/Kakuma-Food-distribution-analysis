# Kakuma Food Distribution Analysis

Data-Driven Insights for Humanitarian Food Support in Kakuma Refugee Camp

# 📌 Project Overview

This project analyzes food distribution patterns in Kakuma Refugee Camp, focusing on fairness, efficiency, and beneficiary satisfaction. Using real distribution records, the analysis identifies gaps, trends, and insights to help humanitarian organizations make more informed decisions about ration allocation and service delivery.

The project includes:

Exploratory Data Analysis (EDA)

Data cleaning and preprocessing

Zone-level distribution comparison

Household-based allocation analysis

Beneficiary satisfaction dashboards

Recommendations for improving distribution efficiency

# 🎯 Business Understanding

Food distribution is one of the most critical activities in refugee camp management. However, challenges such as unequal allocation, inconsistent service quality, and missing household data can reduce the effectiveness of humanitarian support.

This project aims to answer important questions such as:

Are food rations distributed fairly across different zones?

Do larger households receive proportionally adequate rations?

Which ration types are most common, and how do they vary over time?

What factors influence satisfaction among beneficiaries?

Are there trends or gaps that humanitarian agencies should address?

The insights generated can support:

Program monitoring

Decision-making for distribution planning

Identification of underserved areas

Enhanced accountability and transparency

# 📊 Dataset Description

The dataset contains detailed records of 1,000 household-level distribution events with the following 10 columns:

Column Name	Description
Household_ID	Unique identifier for each household.
Zone	Geographic zone within Kakuma Camp. Helps monitor fairness in distribution.
Household_Size	Number of household members. Important for ration scaling.
Distribution_Date	Date when the household received food assistance.
Ration_Type	Category of aid: Dry Rations, Cash Transfer, etc.
Ration_Amount_Kg	Total kilograms of food allocated per household.
Satisfaction_Rating	Beneficiary feedback on service delivery.
Rice_Kg	Kilograms of rice distributed.
Vegetable_Oil_L	Liters of vegetable oil distributed.
Unnamed: 0	Export index column (no analytical value).
Data Quality Notes

Some missing values in Zone, Household_Size, Distribution_Date, and ration-related columns.

Missing ration weights usually correspond to cash transfers instead of food rations.

No duplicate Household_ID entries per distribution event.

Dates are consistent and within expected distribution period.

# 🧹 Data Cleaning Steps

Key cleaning tasks performed:

Removed unnamed index column

Handled missing values using:

Mode imputation for categorical fields

Median imputation for numerical fields

Converted dates to proper datetime format

Standardized zone labels

Added new computed fields such as:

Ration per person (Kg per household member)

Total nutritional contribution from rice and oil

# 🔍 Exploratory Data Analysis (EDA)

The analysis focuses on:

1. Allocation Fairness

Comparison of ration sizes across zones

Identification of zones receiving below-average support

2. Household Size vs Ration Adequacy

Testing if larger households receive more food proportionally

3. Satisfaction Levels

Relationship between satisfaction and:

Ration type

Ration amount

Zone

Household size

4. Ration Type Trends

Proportion of Dry Rations vs Cash Transfers

Monthly distribution patterns

5. Nutritional Breakdown

Summaries of total rice and oil delivered

Zone-level nutrition comparisons

# 📈 Key Insights (Summary)

(You can expand this later once analysis is fully complete)

Some zones receive significantly lower ration amounts compared to others.

Larger households often receive less food per person than smaller households.

Beneficiaries receiving cash transfers report slightly lower satisfaction.

Dates show irregular distribution cycles, indicating possible logistical challenges.
