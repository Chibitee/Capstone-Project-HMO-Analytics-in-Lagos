# Capstone Project: HMO Analytics in Lagos
![HMO_page-0001](https://github.com/user-attachments/assets/1638f6b2-9afd-412e-933b-c8348c1018e4)![HMO_page-0002](https://github.com/user-attachments/assets/a99cbff3-863b-42f8-8440-b1087c3b0239)
# Project Objective
The objective of this project was to analyze enrollment, revenue, and claims data for a Health Maintenance Organization (HMO) operating in Lagos, Nigeria. Using Excel, Power Query, and Power BI, the goal was to clean, model, and visualize the data to provide insights into:
•	Member distribution
•	Plan performance
•	Claims behavior
•	Financial sustainability of the HMO

# Insight-Driven Questions
The analysis was guided by key business questions, including:
1.	What is the overall loss ratio (Total Claims ÷ Total Premium), and how does it vary by plan type?
2.	Which LGAs contribute the most premiums, and which incur the most claims?
3.	How does age affect claims, and are age loadings in premiums adequate?
4.	What proportion of members made zero claims, and how does this vary across plan types?
5.	Which primary providers have the highest claims per member and loss ratios?
6.	Are higher-priced plans (Premium, Family) more costly in claims than lower-priced plans?
7.	What percentage of total claims is driven by the top 10% of members (high-cost members)?

# Data Source
The dataset was provided by the Emerging Data Analysts community as part of a capstone challenge. It simulates real-world HMO business data.

# Dataset Description
The dataset contains 670 records across 9 variables:
1.	Member_ID – Unique identifier for each enrolled member
2.	Gender – Male/Female
3.	Age – Member’s age in years
4.	Plan_Type – Health plan (Basic, Standard, Family, Premium, Corporate)
5.	Enrollment_Date – Date of enrollment
6.	LGA – Local Government Area where member resides
7.	Primary_Provider – Assigned healthcare provider
8.	Monthly_Premium_NGN – Premium amount in Naira
9.	Annual_Claims_NGN – Total annual claims in Naira

# Methodology: Data Preparation Process
To ensure accuracy and relevance in the analysis, I followed a four-stage preparation process:
# 1. Data Cleaning and Quality Checks
•	Checked for missing values, duplicates, spelling errors, and outliers.

•	No missing or duplicate records were found, confirming dataset reliability.

•	Validated each field for consistency.
# 2. Data Type Validation
•	Converted categorical fields (Member_ID, Gender, LGA, Plan_Type) to text.

•	Set Enrollment_Date to Date format.

•	Ensured Age, Premiums, and Claims were properly recognized as numeric values.

•	This step prevented calculation errors and ensured smooth analysis in Power BI.
# 3. Data Transformation
To make the dataset more analysis-friendly:
•	Created Age Groups: 18–29, 30–39, 40–49, 50–64, and 65+. This allowed easier comparison of premiums and claims by age bracket.

•	Custom Date Calendar: Built a calendar table in Power BI using DAX for time-based analysis (Year, Month, Week, Day).

•	Date Hierarchy: Enabled drill-down analysis by year and month for trends in claims and premiums.
# 4. Measure Creation with DAX
Developed key metrics for interactive analysis:
•	Total Premiums and Total Claims

•	Average Premium per Member and Average Claim per Member

•	Loss Ratio (%) = Total Claims ÷ Total Premium

•	Active Members count

•	High-Cost Member Contribution (%) (percentage of total claims driven by the top 10% of members)

These measures made the report dynamic and filter-sensitive, enabling stakeholders to view performance by plan, age group, LGA, or provider.

# Visualization and Reporting
The final step was to build an interactive Power BI dashboard designed to:
•	Clearly answer the business questions.

•	Provide drill-down capabilities for decision-makers.

•	Present trends in enrollment, revenue, and claims in a way that is both intuitive and actionable.
# 
# Health Maintenance Organization (HMO): Insights & Recommendations
# Executive Insights:
# 1.	Loss Ratio by Plan Type
o	The Basic plan recorded the highest loss ratio at 1.85, followed by Corporate (1.66) and Standard (1.57).

o	The Family plan stands at 1.44, while the Premium plan performed best with the lowest loss ratio of 1.02.

o	Implication: Premium plans are more financially sustainable, while Basic and Corporate plans may require pricing or claims management adjustments.
# 2.	Zero-Claim Members by Plan Type
o	A considerable proportion of members did not file any claims: Premium (12.63%), Standard (11.11%), and Family (10.91%).

o	Lower percentages were observed in Basic (6.49%) and Corporate (5.49%).

o	Implication: Higher-value plans have more inactive claimants, suggesting potential profitability opportunities.
# 3.	Claims and Premium by Age Group
o	Older members (50–64 years and 60+) generated the highest claims and premium contributions.

o	Younger groups (18–29 and 30–39) contributed less both in claims and premiums.

o	Implication: Older members are driving both revenue and cost, creating concentration risks if not balanced with younger enrollments.
# 4.	Premium Contributions by Location (LGA)
o	Ojo (₦1.25M), Kosofe (₦1.13M), and Ibeju-Lekki (₦1.07M) are the top-performing LGAs.

o	Mushin, Epe, Ifako-Ijaiye, and Lagos Island show the lowest premium generation.

o	Implication: Opportunities exist to increase penetration in underperforming LGAs through targeted marketing.
# 5.	Provider Performance
o	Providers with higher average claims per member include Eti-Osa Medical Suite (₦47,009, LR 1.89) and Surulere Family Clinic (₦43,353, LR 1.68).

o	Comparatively, Mainland General Hospital (₦40,783, LR 1.67) and Mushin City Clinic (₦41,501, LR 1.76) also show elevated loss ratios.

o	Implication: Provider-level loss ratios suggest possible overutilization or inefficiencies that require closer monitoring.
# 6.	Claims Monthly Trend
o	July recorded the highest claims (₦2.89M), while November showed the lowest (₦758,679).

o	Implication: There are seasonal patterns in claims behavior, which can be factored into financial planning and reserve management.
# 7.	Yearly Performance
o	Both 2024 and 2025 recorded a loss ratio of 1.49, signaling stability in overall performance.
# 8.	Membership Demographics
o	The 50–64 age group constitutes the largest membership segment (184 members).

o	The 18–29 group follows with 143 members, while the 30–39 group has the lowest enrollment at 99 members.

o	Implication: Membership is skewed toward older age groups, which increases long-term claims risk.

# Recommendations:
# 1.	Plan Optimization & Pricing Adjustments
o	Review pricing for Basic and Corporate plans to better align premiums with claims costs.

o	Consider designing tailored benefits for the Premium plan to retain its strong performance while attracting younger members.
# 2.	Target Younger Demographics
o	Develop youth-focused enrollment campaigns (e.g., affordable starter plans or digital-first health packages) to improve portfolio balance and reduce risk concentration among older members.
# 3.	Geographic Expansion
o	Strengthen market penetration in low-premium LGAs (Mushin, Epe, Ifako-Ijaiye, Lagos Island) through agent-driven outreach, employer partnerships, and digital marketing campaigns.
# 4.	Provider Management
o	Engage in provider performance reviews with high loss ratio facilities (e.g., Eti-Osa Medical Suite, Mushin City Clinic).

o	Implement claims utilization audits and negotiate improved care efficiency agreements.
# 5.	Claims Seasonality Management
o	Incorporate claims trend analysis into financial planning to ensure adequate reserves during peak months (e.g., July).

o	Explore preventive healthcare programs to reduce claim spikes.
# 6.	Portfolio Diversification
o	Introduce wellness and preventive care initiatives to reduce claim frequency.

o	Explore corporate partnerships to drive enrolment in underrepresented younger segments and locations.

# Conclusion
The analysis highlights that while the HMO demonstrates strong performance in certain plan types and locations, risks remain in high loss ratio segments, over-reliance on older members, and underperformance in some LGAs. A combination of pricing adjustments, demographic rebalancing, provider oversight, and targeted expansion will enhance both financial sustainability and market growth.

# 📊 Explore the Dashboard
👉 [View the Interactive Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiODFhOTg5YWUtOGNiNi00N2ViLThiNjUtOWNiNjc2MzhlNTBiIiwidCI6ImU2NWY2MTI3LWMyYjAtNGRiNC1hMDQxLTY4ZDk5OThkODAyNSJ9)


