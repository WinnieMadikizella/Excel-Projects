# HealthyLife Medical Analysis 
## Unlocking Insights into Patient Demographics, Treatment Effectiveness, and Costs

**Tools Used:** Microsoft Excel (Power Query, Power Pivot, DAX, Pivot Tables & Charts)


## Introduction
In today’s healthcare landscape, leveraging data to understand patient demographics, treatment effectiveness, and costs is essential for improving outcomes and optimizing operations. This analysis examines a dataset of 5,000 patients from HealthyLife Clinics, uncovering trends in medical conditions, treatment outcomes, and seasonal visit patterns. 
Conducted entirely in **Microsoft Excel**, this project demonstrates the power of data-driven decision-making in healthcare.

## Objectives
The primary objectives of this analysis were to:
1. Identify common medical conditions treated.
2. Analyze patient demographics (age groups, gender distribution).
3. Evaluate treatment effectiveness across different conditions.
4. Assess average treatment duration and costs.
5. Uncover seasonal visit patterns.
6. Provide actionable insights for improving care and operations.

## Dataset Details
The dataset included multiple key attributes related to patients, medical conditions, and treatment outcomes:

- **Demographics:** Age, gender, location.
- **Medical Data:** Conditions, treatments, outcomes, costs, patient satisfaction.
- **Additional Fields:** Treatment duration, insurance coverage, follow-up needs.

You can view or download the dataset here:  
[health_data_case_study.xlsx](health_data_case_study.xlsx)


## Step 1: Data Cleaning & Preparation in Excel
To ensure a structured and reliable analysis, the dataset was cleaned and organized using **Excel Power Query** and **Power Pivot**:
1. Standardized text fields and formatted data types.
2. Added categorized columns:
   - Age Groups: `0–18`, `19–35`, `36–50`, `51–65`, `66+`
   - Treatment Duration Categories: `Short`, `Medium`, `Long`
   - Treatment Cost Categories: `Low`, `Medium`, `High`
   - Seasons: Derived from the visit date column
3. Built a data model with dimension and fact tables.
4. Power Pivot Enhancements:
   - Satisfaction Category: Grouped patient ratings into `Low`, `Medium`, and `High`.
   - Insurance Coverage Category: Grouped coverage levels into `Low`, `Moderate`, `Partial`, and `High`.
5. Established relationships for seamless data integration.

![Data Relationship](screenshots/data%20relationship.JPG)


## Step 2: Data Analysis & Key Metrics
The analysis focused on **Key Performance Indicators (KPIs)** and trends across different dimensions:
### 1. Common Medical Conditions Treated
- Anxiety: 584 patients
- Back Pain: 557 patients
- Arthritis: 555 patients

### 2. Demographics
- Largest age group: `66+` (1,744 patients)
- Gender distribution:
        - Female: 1,681 patients
        - Male: 1,660 patients
        - Other: 1,659 patients (balanced distribution)

### 3. Treatment Effectiveness
- Anxiety had the highest worsening rate: 206 patients.
- Depression had the most balanced improvement/worsening outcomes.

### 4. Cost & Duration Analysis
- Hypertension was the most expensive condition($2,631.38 per patient).
- Depression was the least costly condition ($2,476.97 per patient).
- Average treatment duration: `44–48 days` across conditions.

### 5. Seasonal Visit Trends
- Spring (March-May): Highest visits (1,353 patients).
- Winter (December): Lowest visits (293 patients).
- Summer & Winter show different patterns:
           - Summer: 1,224 visits
           - Winter: 1,124 visits

### 6. Follow-Ups
- Hypertension required the most follow-ups (303 patients).
- Back Pain: 276 patients did not require follow-ups.
- Counseling was the most common treatment (869 patients).
- Surgery had the highest initial success:
     - 446 patients did not need follow-ups.
     - 403 patients required follow-ups.

### 7. Patient Satisfaction Levels
- High Satisfaction: 1,993 patients
- Medium Satisfaction: 1,027 patients
- Low Satisfaction: 1,980 patients

![Pivot Table Analysis](screenshots/pivot%20tables.JPG)


## Step 3: Key Insights & Recommendations
### Key Insights
1. **Demographics:**
   - Elderly patients (`66+ years`) dominate the patient population.
   - Gender distribution is nearly equal.

2. **Treatment Effectiveness:**
   - Anxiety patients had the highest worsening rate.
   - Depression showed the most balanced outcomes.
   - COVID-19 had equal numbers of improved & worsened cases (200 each).

3. **Cost & Duration:**
   - Hypertension is the most expensive condition ($2,631.38 per patient).
   - Depression is the least costly condition ($2,476.97 per patient).
   - Treatment duration remains stable (44-48 days).

4. **Seasonal Trends:**
   - Spring (March-May) has the highest visits.
   - December has the lowest patient visits (293).

5. **Follow-ups & Satisfaction:**
   - High follow-up rate across conditions (~50%).
   - Surgery shows the highest initial success.

### Recommendations
1. **Optimize Treatments:** Improve anxiety protocols; replicate depression’s success; develop elderly-specific care programs.
2. **Manage Resources:** Increase staffing in Spring; reduce working hours in December; allocate more resources to counseling.
3. **Reduce Costs:** Investigate hypertension expenses; apply depression’s cost-effective treatments to other conditions.
4. **Enhance Follow-ups:** Implement structured follow-up programs for anxiety patients; promote preventive care to reduce re-admissions.
5. **Improve Quality:** Standardize protocols for inconsistent outcomes; closely monitor conditions with high worsening rates.  

## Step 4: Final Dashboard & Interactive Slicers
A HealthyLife Clinics Dashboard was created in Excel featuring:
- **Interactive Slicers:** Location, insurance coverage
- **Key KPIs:**
            - Total Patients: 5,000
            - Improvement Rate: 33.02%
            - Average Duration: 45 days
            - Average Cost: $2,566.04
            - Satisfaction Score: 3.0

![Clinic Performance Dashboard](screenshots/clinic%20performance%20dashboard.JPG)

## Conclusion
This analysis provides actionable insights to optimize resource allocation, improve treatment outcomes, and enhance patient satisfaction. By leveraging data-driven strategies, HealthyLife Clinics can address modern healthcare challenges and deliver better patient care.
