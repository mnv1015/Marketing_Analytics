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


