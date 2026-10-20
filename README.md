# 📊 Pinnacle Meta Ads Campaign Analytics & Performance Optimization

## 📌 Project Overview

This project focuses on cleaning, transforming, and analyzing Meta Ads campaign data using Microsoft Excel and Python to identify performance trends and generate actionable marketing insights.

The dataset contains **10,000+ records** and approximately **50 structured columns after preprocessing**, including campaign, ad set, advertisement, targeting, and performance metrics.

### 🎯 Project Objectives

- Clean and preprocess advertising data.
- Extract targeting information from JSON columns.
- Perform Exploratory Data Analysis (EDA).
- Analyze campaign, platform, ad set, and ad performance.
- Calculate and validate marketing KPIs.
- Identify high-performing and underperforming advertisements.
- Recommend data-driven campaign optimization strategies.

---

## 🛠️ Tools & Technologies

- **Python:** Data analysis and preprocessing
- **NumPy:** Numerical calculations
- **Pandas:** Data cleaning and manipulation
- **Matplotlib:** Data visualization
- **Seaborn:** Statistical visualization
- **Microsoft Excel:** Data cleaning and Pivot Table analysis
- **Git & GitHub:** Version control and project documentation

---

## 📂 Dataset Overview

The dataset contains advertising performance information across multiple dimensions.

| Category | Description |
|---|---|
| Dataset Size | 10,000+ records before analytical filtering |
| Analytical Columns | Approximately 50 after preprocessing |
| Campaign Data | Campaign names and performance metrics |
| Ad Set Data | Audience segments and targeting information |
| Ad Data | Ad IDs, creative names, and performance metrics |
| Performance Metrics | Impressions, clicks, spend, and CPC |
| Conversion Metrics | Payments, conversions, and landing page views |
| Targeting Data | Age ranges, interests, behaviors, and locations |
| Time-Based Data | Dates, weekdays, and monthly performance |

---

# 🧹 Phase 1: Excel Data Cleaning & Preparation

## 1. JSON Column Handling

- Extracted targeting information from nested JSON columns.
- Identified age ranges, interests, behaviors, and geographical targeting.
- Flattened relevant JSON attributes into structured columns.
- Removed unnecessary raw JSON columns after extracting useful information.

## 2. Data Standardization

- Converted date fields into appropriate date formats.
- Standardized currency and numerical fields.
- Checked Ad ID uniqueness.
- Cleaned text-based missing values, including `"NaN"` strings.
- Corrected inconsistent data types and formatting issues.

## 3. Column Reduction & Optimization

- Removed columns containing approximately 80–90% missing values when they were not analytically useful.
- Removed unnecessary hourly breakdown columns.
- Removed weekday-specific columns where the information could be derived from dates.
- Eliminated redundant or derivable metrics.
- Retained essential columns for performance analysis.

## 4. Feature Engineering

Created additional analytical features:

- Engagement Rate
- Conversion Rate
- Monthly Performance
- Date-Based Features
- Weekday Classification
- Campaign Efficiency Indicators
- Performance Benchmark Ratios

---

# 📊 Phase 2: Excel Pivot Table Analysis

## 1. Platform-Level Analysis

Analyzed advertising performance across Facebook, Instagram, Threads, and other available platforms.

**Metrics:**
- Total Spend
- Total Payments
- Average CPC
- Click-Through Rate (CTR)
- Conversion Rate
- Cost Per Landing Page View (CPLPV)

## 2. Campaign-Level Analysis

Compared campaigns using:

- Total Advertising Spend
- Total Payments
- Cost Per Landing Page View
- Click-Through Rate
- Conversion Rate
- ROI, where revenue data was available

## 3. Daily Performance Analysis

Evaluated:

- Daily Advertising Spend
- Day-Wise Payments
- Daily CPC Trends
- Daily Conversion Performance
- Weekday-Level Results

## 4. Monthly Performance Analysis

Analyzed monthly advertising expenditure and conversion trends to identify changes in campaign performance over time.

---

# 🐍 Phase 3: Python-Based Exploratory Data Analysis (EDA)

## Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
