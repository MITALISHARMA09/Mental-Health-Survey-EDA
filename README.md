# Mental Health in Tech – Exploratory Data Analysis

This project performs an in-depth Exploratory Data Analysis (EDA) on the **Mental Health in Tech Survey 2014** dataset to understand mental health awareness, treatment patterns, and workplace support within the technology industry.

## Project Overview

- **Project type:** Exploratory Data Analysis (EDA)
- **Domain:** Mental health, HR analytics, tech industry 
- **Contribution:** Individual  

The analysis focuses on:
- Mental health treatment-seeking behavior among tech employees.
- Impact of family history, employer benefits, and workplace culture on mental health. 
- Openness to discuss mental health with coworkers, supervisors, and potential employers. 

## Dataset

The dataset is derived from the **2014 Mental Health in Tech Survey**, which measures attitudes towards mental health and the frequency of mental health disorders in the tech workplace.

Key variables include:  
- **Demographics:** `Timestamp`, `Age`, `Gender`, `Country`, `state`  
- **Employment context:** `self_employed`, `no_employees`, `remote_work`, `tech_company`  
- **Mental health factors:** `family_history`, `treatment`, `work_interfere`  
- **Employer support:** `benefits`, `care_options`, `wellness_program`, `seek_help`, `anonymity`, `leave`  
- **Perceptions & stigma:** `mental_health_consequence`, `phys_health_consequence`, `coworkers`, `supervisor`, `mental_health_interview`, `phys_health_interview`, `mental_vs_physical`, `obs_consequence`, `comments`  

> Original data is credited to **Open Sourcing Mental Illness (OSMI)**.

## Objectives

**Problem Statement**  
Mental health issues are common among technology professionals but often remain unaddressed due to stigma, lack of awareness, and limited or poorly communicated workplace support. This can negatively affect employee well-being and organizational productivity. 

**Business Objectives** 
- Analyze mental health trends and treatment patterns among tech employees.  
- Understand how company size, benefits, wellness programs, and employer support influence mental health awareness and help-seeking.  
- Identify gaps in communication and effectiveness of organizational mental health initiatives.  
- Assess employees’ willingness to discuss mental health at work and during interviews.  
- Generate data-driven insights to guide better workplace mental health policies.  

## Methodology

### 1. Data Understanding

- Inspected shape, data types, duplicates, and missing values. 
- Summarized 27 variables covering demographics, employment, mental health, and workplace attitudes. 

### 2. Data Cleaning & Preprocessing

Key preprocessing steps: 
- Standardized and normalized text fields (e.g., `Gender`) and grouped into **Male**, **Female**, **Others**, and **Unknown** to handle noisy entries.   
- Removed unrealistic age outliers and restricted analysis to ages **18–65** to reflect working-age respondents.  
- Handled missing values, e.g., filling `self_employed` and `work_interfere` where appropriate, and dropping high-missing or less relevant columns like `comments`, `state`, and `Timestamp`. 

### 3. Exploratory Data Analysis & Visualizations

The notebook contains 20+ charts spanning **univariate**, **bivariate**, and **multivariate** analysis. 

Examples of analyses:
- Age distribution, boxplots, and age vs treatment patterns.  
- Gender distribution and gender vs treatment.  
- Family history vs treatment and work interference.  
- Company size distribution and its relation to benefits and treatment.  
- Remote work, wellness programs, and their impact on help-seeking.  
- Correlation heatmap for age, family history, remote work, and treatment.  
- Country-wise patterns and perceived mental health consequences.  

Each chart is documented with:
- Why the chart was chosen.  
- Key insights.  
- Potential positive or negative business impact.  

## Key Insights

Some high-level insights from the EDA: 

- A significant share of respondents report experiencing mental health issues, and many have sought professional treatment.  
- Individuals with a **family history of mental illness** are more likely to seek treatment.  
- Mental health conditions frequently **interfere with work performance**, pointing to productivity risks.  
- Many employees are either unaware of or unclear about available mental health **benefits and care options**.  
- Mental health is often **not treated as seriously as physical health** in workplaces, and stigma still affects willingness to talk about issues with employers.  
- Organizations with wellness programs and clear support structures show better help-seeking behavior among employees.  

## Recommendations

Based on the analysis, the following actions are suggested for organizations:  

- **Improve awareness of mental health benefits**  
  - Communicate benefits and care options clearly via onboarding, internal portals, and recurring campaigns.  

- **Normalize mental health conversations**  
  - Train leaders and managers to talk openly about mental health and reduce stigma.  

- **Strengthen wellness programs**  
  - Introduce or enhance structured initiatives such as counseling, workshops, and stress management programs.  

- **Ensure anonymity and confidentiality**  
  - Provide confidential channels for accessing mental health support to reduce fear of negative consequences.  

- **Adopt inclusive, non-segmented policies**  
  - Design mental health strategies that support all age groups and roles, as mental health challenges appear across the workforce.  

- **Monitor impact on productivity**  
  - Regularly assess employee well-being and intervene early when mental health begins to interfere with work.  
