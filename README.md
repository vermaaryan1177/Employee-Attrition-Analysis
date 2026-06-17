# Employee-Attrition-Analysis
Investigating factors that contribute to employee turnover and providing HR recommendations to improve retention.


# Table of Contents

1. [Dataset Overview](#dataset-overview)

   * [Records and Features Summary](#dataset-overview)

2. [Data Quality Checks](#data-quality-checks)

   * [Missing Values](#missing-values)
   * [Duplicate Records](#duplicate-records)
   * [Categorical Features](#categorical-features)
   * [Numerical Features](#numerical-features)
   * [Target Variable](#target-variable)
   * [Summary](#summary)

3. [Findings](#findings)

   * [Workforce Overview](#1-workforce-overview)
   * [Gender Distribution](#2-gender-distribution)
   * [Education Distribution](#3-education-distribution)
   * [Attrition by Education](#attrition-by-education)
   * [City Analysis](#4-city-analysis)
   * [Employee Distribution](#employee-distribution)
   * [Attrition by City](#attrition-by-city)
   * [Payment Tier Analysis](#5-payment-tier-analysis)
   * [Bench Status Analysis](#6-bench-status-analysis)
   * [Age Analysis](#7-age-analysis)
   * [Experience Analysis](#8-experience-analysis)

4. [Business Questions](#business-questions)

   * [What is the overall attrition rate?](#1-what-is-the-overall-attrition-rate)
   * [Which education groups have the highest turnover?](#2-which-education-groups-have-the-highest-turnover)
   * [Does attrition vary by city?](#3-does-attrition-vary-by-city)
   * [Is attrition related to age?](#4-is-attrition-related-to-age)
   * [Does employee experience affect turnover?](#5-does-employee-experience-affect-turnover)
   * [Are benched employees more likely to leave?](#6-are-benched-employees-more-likely-to-leave)
   * [Which payment tier experiences the highest attrition?](#7-which-payment-tier-experiences-the-highest-attrition)
   * [What employee profile has the highest risk of leaving?](#8-what-employee-profile-has-the-highest-risk-of-leaving)

5. [Business Insights & Recommendations](#business-insights--recommendations)

   * [Compensation May Be Driving Attrition](#1-compensation-may-be-driving-attrition)
   * [Bench Time Increases Resignation Risk](#2-bench-time-increases-resignation-risk)
   * [Early-Career Employees Are Most Vulnerable](#3-early-career-employees-are-most-vulnerable)
   * [Master's Degree Holders Require Special Retention Focus](#4-masters-degree-holders-require-special-retention-focus)
   * [Pune Is a Potential Attrition Hotspot](#5-pune-is-a-potential-attrition-hotspot)
   * [Attrition Declines with Experience](#6-attrition-declines-with-experience)
   * [High Overall Attrition Represents a Business Risk](#7-high-overall-attrition-represents-a-business-risk)

6. [Executive-Level Conclusion](#executive-level-conclusion)



# Dataset
url- https://www.kaggle.com/datasets/tawfikelmetwally/employee-dataset

# Dataset Overview

* Records: 4,653
* Features: 9
* Numerical columns: 5
* Categorical columns: 4

# Data Quality Checks

## Missing Values

* No missing values detected across all columns.

## Duplicate Records

* Duplicate rows: 1,889 (40.6% of the dataset).
* This is the primary data quality concern and should be investigated before modeling.

## Categorical Features

* Education: 3 categories (Bachelors, Masters, PhD)
* City: 3 categories (Bangalore, Pune, New Delhi)
* Gender: 2 categories (Male, Female)
* EverBenched: 2 categories (Yes, No)
* No inconsistent or unexpected category labels found.

## Numerical Features

* Age ranges from 22–41 years.
* JoiningYear ranges from 2012–2018.
* ExperienceInCurrentDomain ranges from 0–7 years.
* No obvious invalid values detected.

## Target Variable

* LeaveOrNot = 0 (Stayed)
* LeaveOrNot = 1 (Left)
* Moderate class imbalance.

# Summary

The dataset is complete and generally clean, with no missing values and valid feature ranges. The main issue is the high number of duplicate records (40.6%).





# Business Questions

## 1. What is the overall attrition rate?

* Overall Attrition Rate = 39.36%.

## 2. Which education groups have the highest turnover?

* Attrition by education level:

  * Masters: 48%
  * Bachelors: 38%
  * PhD: 26%
* Finding: Employees with a Master's degree show the highest turnover, followed by Bachelor's degree holders.

## 3. Does attrition vary by city?

* Attrition by city:

  * Pune: 51%
  * Bangalore: 35%
  * New Delhi: 34%
* Finding: Yes. Attrition varies significantly by city. Pune has the highest employee turnover, while Bangalore and New Delhi are considerably lower.

## 4. Is attrition related to age?

* Attrition is highest among employees aged 24–26 years (around 52–53%).
* Attrition gradually declines as age increases.
* Employees aged 38–41 years show the lowest attrition (around 30–34%).
* Finding: Yes. Younger employees are more likely to leave, while older employees tend to stay longer.

## 5. Does employee experience affect turnover?

* Average Attrition by experience:

  * 2–3 years: 43%
  * 0–1 years: 37–38%
  * 4 years: 39%
  * 5 years: 34%
  * 6 years: 25%
  * 7 years: 33%
* Finding: Attrition peaks around 2–3 years of experience and generally decreases as employees become more experienced.

## 6. Are benched employees more likely to leave?

* Bench status attrition:

  * Yes: 44%
  * No: 39%
* Finding: Yes. Employees who have been benched are more likely to leave than those who have not.

## 7. Which payment tier experiences the highest attrition?

* Average Attrition by payment tier:

  * Tier 2: 60%
  * Tier 1: 35%
  * Tier 3: 34%
* Finding: Payment Tier 2 experiences the highest attrition by a large margin.

## 8. What employee profile has the highest risk of leaving?

* Highest-Risk Employee Profile

  * Located in Pune
  * Holds a Master's degree
  * Aged 24–26 years
  * Has 2–3 years of experience
  * Has been benched
  * Belongs to Payment Tier 2
* This profile combines the highest-risk categories observed across all attrition drivers and would be the primary target group for retention initiatives.





# Dashboard Screenshot

<img width="1371" height="747" alt="Attrition Analysis" src="https://github.com/user-attachments/assets/90dbde17-d4e3-4366-93dd-5f46ee8bf66f" />

<img width="1262" height="697" alt="Employee Distribution" src="https://github.com/user-attachments/assets/f2b44b75-8964-4a94-983a-3e5a8acf9688" />

<img width="1357" height="755" alt="Employee Risk Factor" src="https://github.com/user-attachments/assets/f3479a35-6cd3-487b-807d-8b523635c07f" />


# Findings

## 1. Workforce Overview

* Total employee count is approximately 3,000 employees.
* Average employee age is 30.95 years.
* Average employee experience is 2.64 years.
* Overall attrition rate is 39.36%, indicating a relatively high employee turnover level.

## 2. Gender Distribution

* The workforce is relatively balanced:

  * Male: 55.3% (1.53K employees)
  * Female: 44.7% (1.24K employees)
* Male employees slightly outnumber female employees.

## 3. Education Distribution

* Employees with a Bachelor's degree constitute the majority of the workforce.
* Master's degree holders form the second-largest group.
* PhD holders represent only a small portion of employees.

### Attrition by Education

* Employees with Master's degrees show the highest attrition rate.
* Employees with PhDs show the lowest attrition rate.
* Bachelor's degree holders have moderate attrition.

## 4. City Analysis

### Employee Distribution

* Bangalore has the largest employee population.
* Pune and New Delhi have similar employee counts.

### Attrition by City

* Pune has the highest attrition rate.
* Bangalore and New Delhi have similar and lower attrition rates.

Although Pune has the highest attrition rate, Bangalore contributes almost the same number of exits because of its larger workforce.

## 5. Payment Tier Analysis

* Employees in Payment Tier 2 exhibit the highest attrition rate.
* Employees in Payment Tier 3 exhibit the lowest attrition rate.
* Payment Tier 1 employees show moderate attrition.

## 6. Bench Status Analysis

* Employees who were ever benched show a higher attrition rate.
* Employees who were never benched show a lower attrition rate.

## 7. Age Analysis

* Attrition is highest among employees aged 24–26 years.
* Attrition generally declines as age increases.
* Employees above 35 years show comparatively lower attrition.

## 8. Experience Analysis

* Employees with around 3 years of experience have the highest attrition rate.
* Employees with around 6 years of experience have the lowest attrition rate.
* Attrition tends to decrease as experience increases beyond 3 years.


# Business Insights & Recommendations

## 1. Compensation May Be Driving Attrition

**Observation:** Payment Tier-2 employees have the highest attrition rate.

### Business Insight:

* Employees in Tier-2 may perceive limited compensation growth compared to Tier-3 employees.
* This group could be receiving offers from competitors with better salary progression.

### Recommended Action:

* Conduct salary benchmarking for Tier-2 employees.
* Review promotion and compensation progression policies.
* Introduce retention bonuses or performance-based incentives.

## 2. Bench Time Increases Resignation Risk

**Observation:** Benched employees have significantly higher attrition.

### Business Insight:

* Employees without active projects may feel underutilized, uncertain about career growth, or insecure about their future within the company.
* Extended bench periods can reduce engagement and job satisfaction.

### Recommended Action:

* Minimize bench duration.
* Provide reskilling and certification programs during bench periods.
* Assign internal projects or innovation initiatives to maintain engagement.

## 3. Early-Career Employees Are Most Vulnerable

**Observation:** Highest attrition occurs among employees aged 24–26 and those with around 2–3 years of experience.

### Business Insight:

* Employees at this stage often seek faster salary growth, promotions, and learning opportunities.
* They are highly active in the job market and more willing to switch employers.

### Recommended Action:

* Create structured career progression paths.
* Offer mentorship and leadership development programs.
* Increase engagement through learning and advancement opportunities.

## 4. Master's Degree Holders Require Special Retention Focus

**Observation:** Employees with Master's degrees exhibit the highest attrition.

### Business Insight:

* Highly educated employees may have greater external opportunities.
* Their expectations regarding career growth, compensation, and challenging work may not be fully met.

### Recommended Action:

* Offer specialized career tracks.
* Increase exposure to strategic projects and leadership opportunities.
* Review compensation competitiveness for advanced-degree employees.

## 5. Pune Is a Potential Attrition Hotspot

**Observation:** Pune shows the highest attrition rate.

### Business Insight:

* The local job market may be more competitive.
* Employee satisfaction, compensation, leadership practices, or project allocation in Pune may differ from other locations.

### Recommended Action:

* Conduct location-specific employee surveys.
* Analyze manager effectiveness and workload distribution.
* Investigate local market salary competitiveness.

## 6. Attrition Declines with Experience

**Observation:** Employees with 5–6 years of experience have lower attrition rates.

### Business Insight:

* Employees who stay beyond the initial career stage tend to become more committed and invested in the organization.
* Retaining employees through the first few years can significantly improve workforce stability.

### Recommended Action:

* Focus retention efforts on employees with less than 4 years of experience.
* Implement targeted onboarding and career development programs.

## 7. High Overall Attrition Represents a Business Risk

**Observation:** Overall attrition rate is approximately 39%.

### Business Insight:

* Nearly 4 out of every 10 employees leaving can increase recruitment costs, training costs, productivity losses, and project delivery risks.
* Knowledge loss can negatively affect customer satisfaction and operational efficiency.

### Recommended Action:

* Establish an attrition reduction target.
* Monitor high-risk employee segments monthly.
* Use predictive HR analytics to identify employees likely to leave.

# Executive-Level Conclusion

Attrition is primarily concentrated among:

* Tier-2 employees
* Benched employees
* Employees aged 24–26
* Employees with 2–3 years of experience
* Master's degree holders
* Employees in Pune

These groups should be prioritized for retention initiatives because they represent the highest-risk segments and likely contribute disproportionately to employee turnover. Reducing attrition in these segments would have the greatest impact on improving workforce stability and lowering replacement costs.

