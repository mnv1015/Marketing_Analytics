# Marketing Analytics Report (SQL + Python + Power BI)

## Overview
This project presents an end-to-end marketing analytics solution designed to identify the key factors behind declining conversion rates and return on investment (ROI).  
It integrates multi-source marketing, customer engagement, and feedback data to generate actionable business insights through data processing, sentiment analysis, and interactive visualization.

---

## Problem Statement
Despite continuous marketing efforts, the organization is experiencing a steady decline in conversion rates and ROI.  
The absence of a unified analytical view across engagement trends, customer feedback sentiment, and seasonal demand patterns makes it difficult to determine the root causes of performance decline.

This project aims to build a comprehensive analytics pipeline that:

- Extracts and cleans multi-source marketing data  
- Analyzes customer sentiment and engagement behavior  
- Identifies seasonal and operational drivers of declining conversions  
- Delivers actionable insights through an interactive dashboard  

---

## Objectives
- Integrate marketing, engagement, and feedback datasets  
- Perform SQL-based data extraction and preprocessing  
- Conduct sentiment analysis on customer reviews using Python  
- Analyze conversion trends, engagement metrics, and ROI drivers  
- Build a Power BI dashboard for business decision support  

---

## Tech Stack
- **SQL** → Data extraction, joins, and cleaning  
- **Python** → Data processing, sentiment analysis, and trend exploration  
- **Power BI** → Interactive dashboard, KPIs, and visualization  

---

## Dataset Overview
The analytics pipeline is powered by a **star schema data model** that integrates customer, product, calendar, and multi-source marketing data.  
This structure enables efficient querying, scalable analysis, and a clear separation between **dimension** and **fact** tables.

### Dimension Tables
- **Dim_Customers** → Contains demographic and profile attributes such as age, gender, city, and country.  
- **Dim_Products** → Includes product catalog details, pricing, and category information.  
- **Dim_Calendar** → Provides standardized date attributes to support seasonal, monthly, and trend-based analysis.  

### Fact Tables
- **Fact_CustomerReviews** → Stores raw customer feedback including ratings and textual reviews.  
- **Fact_EngagementData** → Captures campaign interaction metrics such as views, clicks, and likes.  
- **Fact_CustomerJourney** → Tracks behavioral journey stages, user actions, and time spent at each stage.  
- **Fact_ReviewsSentiment** → Contains sentiment scores and sentiment categories **generated after performing sentiment analysis on customer reviews using Python**.

---

## Key Analysis Performed
- Conversion rate trend analysis across time periods  
- Customer engagement pattern evaluation  
- Sentiment classification of customer feedback  
- Identification of seasonal demand impact  
- Root cause analysis of declining ROI  

### Data Cleaning & Transformation
Raw multi-source marketing and engagement data was extracted using **SQL** and cleaned through:

- Handling missing, duplicate, and inconsistent values  
- Standardizing date formats, categorical fields, and numeric measures  
- Transforming datasets into a **star schema structure** for scalable analytical querying  

### Sentiment Analysis Methodology
Customer review data was connected to **Python** using the **pyodbc** database driver.  
Sentiment analysis was conducted using **NLTK’s VADER model**, which produced:

- Sentiment polarity scores (positive, negative, neutral, compound)  
- Aggregated sentiment categories stored in the `Fact_ReviewsSentiment` table for reporting and trend analysis  

---

## Dashboard Insights
The **Power BI** report revealed that declining conversion rates were primarily driven by:

- Seasonal drop in demand during the latter half of the year  
- Reduced campaign reach and customer engagement  
- Recurring unresolved customer concerns highlighted through sentiment trends  

These insights enable **targeted marketing optimization and improved ROI planning**.

---

## Business Impact
- Delivered a **data-driven explanation** for declining marketing performance  
- Enabled **evidence-based campaign optimization**  
- Supported **more effective marketing budget allocation**  
- Improved **customer experience monitoring through sentiment intelligence**  

---

## Power BI Dashboard Preview
The interactive Power BI report consists of **four analytical pages**:

1. **Conversion & ROI Overview**  
2. **Customer Engagement Analysis**  
3. **Sentiment & Feedback Insights**  
4. **Seasonal Trends & Root Cause Analysis**  

> *(Add Power BI dashboard screenshots below to enhance visual understanding of insights.)*

---

## Future Enhancements
- Predictive modeling for **conversion rate forecasting**  
- Customer segmentation using **machine learning techniques**  
- Real-time dashboard integration with live marketing data sources  
- Automated sentiment monitoring and alerting pipeline  

---



---

