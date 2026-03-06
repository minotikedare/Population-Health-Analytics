# Population-Health-Analytics

This project analyzes national health reporting data from Sierra Leone to evaluate healthcare service performance across facilities, districts, and chiefdoms. The analysis focuses on referral trends, reporting consistency, disease incidence, immunization coverage, and maternal health indicators to generate insights that support data-driven public health decision making.

## Project Overview
The project combines data extracted from DHIS2 with statistical analysis and visualization techniques in R to explore healthcare reporting patterns and facility performance. It includes referral trend comparisons, time-series forecasting, disease burden analysis, vaccine coverage assessment, and healthcare service comparisons across geographic regions. The project also incorporates natural language processing to analyze qualitative interpretations.

## Tools and Technologies
- **R** – Data cleaning, statistical analysis, predictive modeling, and visualization.  
- **DHIS2** – Primary data source for national health datasets including facility reporting, immunization coverage, and disease indicators.  
- **PyCharm** – Development environment to organize scripts and run analysis workflows.  
- **Time Series Models (ETS, ARIMA)** – Applied to analyze trends and forecast future referral volumes and reporting patterns.  
- **dplyr** – Efficient data manipulation, filtering, and aggregation of healthcare datasets.  
- **ggplot2** – Creation of trend plots, comparison charts, and reporting rate visualizations.  
- **Natural Language Processing (Python models integrated in R)** – Transformer-based models for sentiment analysis and named entity recognition.

## Analysis Performed

### Facility Referral Analysis
Compared referral volumes and causes between **Ngelehun CHC (Badija)** and **Jembe CHC (Baoma)** over a 24-month period.

### Referral Forecasting
Applied ETS and ARIMA time-series models to predict monthly referrals for the next year, identifying stable referral patterns in Jembe CHC and low but irregular referrals in Ngelehun CHC.

### Reporting Rate Trend Analysis
Analyzed district-level reporting rates for the **Reproductive Health dataset** from January 2024 to June 2025 and examined time-series components including trend, seasonality, and random variation.

### Dataset Reporting Comparison
Compared reporting rates across **Reproductive Health, Child Health, and PMTCT datasets**, finding strong alignment between Reproductive and Child Health reporting patterns.

### Diarrhea Incidence Rate Analysis (<5 Years)
Calculated district-level diarrhea incidence rates using DHIS2 indicator definitions and underlying case data for the previous 12 months.

### ORS Stock Requirement Estimation
Estimated the minimum **Oral Rehydration Solution (ORS)** stock required based on diarrhea incidence rates, identifying **Tonkolili district** as having the highest estimated treatment demand.

### OPV1 Coverage Mapping
Mapped chiefdom-level **OPV1 vaccination coverage for children under 1 year**, identifying top-performing chiefdoms including **Gbo, Badija, Niawa Lenga, Komboyo, and Simbaru**.

### Sherbro Island Facility Comparison
Compared OPV1 coverage across facilities located in **Sherbro Island and surrounding coastal regions**, identifying reporting gaps and uneven immunization performance.

### Facility Performance Analysis
Evaluated maternal health indicators including **ANC3 coverage** and **PHU delivery rate** across Sherbro Island facilities to assess continuity of maternal care.

### Sentiment and Topic Analysis
Applied transformer-based NLP models to analyze interpretation discussions, performing sentiment classification and named entity recognition to identify common themes.

### Dashboard Development
Developed a dashboard combining visualizations, tables, and analytical outputs to support exploration of healthcare trends and facility performance.

## Key Insights
- **Jembe CHC** shows consistently higher referral volumes (~54/month) compared to **Ngelehun CHC (~10/month)**.  
- **Reproductive Health and Child Health datasets** exhibit nearly identical national reporting trends.  
- **Tonkolili district** has the highest average diarrhea incidence among children under 5, requiring approximately **10,339 ORS packets per month** for treatment coverage.  
- Only 2 out of 5 **Sherbro Island facilities** reported OPV1 coverage, highlighting significant reporting gaps.  
- **Delken MCHP** demonstrates stronger maternal care continuity compared to other facilities in the region.
