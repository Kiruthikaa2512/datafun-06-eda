# **US Housing Market Analysis: Supply-Demand Dynamics - EDA Project**

**Author**: Kiruthikaa NS  
**Repo Name**: `datafun-06-eda`  
**Date**: June 2025  
**GitHub Repo**: [View this project on GitHub](https://github.com/Kiruthikaa2512/datafun-06-eda)  

## **Project Introduction**  

This exploratory data analysis (EDA) project investigates the **supply-demand dynamics in the US housing market** using curated datasets. The goal is to reveal how economic indicators, pricing tiers, interest rates, and housing availability influence **both supply and demand** across different market segments.  

Using Python, Pandas, Seaborn, and Matplotlib in a Jupyter Notebook, this project develops visual data stories to highlight:  

- How interest rates shape housing demand  
- The impact of economic indicators such as GDP, mortgage rates, and consumer sentiment  
- Patterns across price tiers and time periods  
- Trends in **housing supply metrics** such as vacant units, construction spending, and permits  


## **Dataset Overview**  

- **Raw Datasets:** `demand.csv`, `supply.csv`  
- **Cleaned Datasets:** `cleaned_demand.csv`, `cleaned_supply.csv`  
- **Modified Datasets:** `modified_demand.csv`  
- **Source:** [Kaggle - Factors Influencing House Price in US](https://www.kaggle.com/datasets/utkarshx27/factors-influence-house-price-in-us)  
- **Key Variables (Demand):** `date`, `price_index`, `mortgage_rate`, `consumer_sentiment`, `interest_rate`, `median_price`, `gdp`, `year_quarter`, `price_tier`, `rate_band`  
- **Key Variables (Supply):** `construction_spending`, `vacant_units`, `metro_price_index`, `permits_issued`, `date`  
- **Goal:** Integrating both **demand-side** (sentiment, affordability, macroeconomic trends) and **supply-side** (availability, investment, permits) data for a complete housing market analysis.  

## **Project Setup Steps**  

### **Repository Creation**  
- GitHub repo created: `datafun-06-eda`  
- Initialized with a default `README.md`  

### **Clone & Development**  
git clone https://github.com/Kiruthikaa2512/datafun-06-eda.git
cd datafun-06-eda
code .


### **Python Virtual Environment & Dependencies**  
```python -m venv .venv  
source .venv/bin/activate  (Mac/Linux)  
.venv\Scripts\activate  (Windows)  
```
# Install dependencies  
```pip install pandas seaborn matplotlib jupyterlab pyarrow  
```

## **Notebook Summary**  

The notebook (`datafun-06-eda.ipynb`) follows a structured, step-by-step process with Markdown headings and Python code cells.  

### **Data Cleaning & Feature Engineering**  

- **Demand-Side Refinements:**  
  - Renamed columns (`sentiment_index` → `consumer_sentiment`)  
  - Created derived features:  
    - **`price_tier`**: Quartile bins for median housing price  
    - **`rate_band`**: Interest rate categories from low to very high  

- **Supply-Side Enhancements:**  
  - Converted `construction_spending` and `metro_price_index` to numeric formats  
  - Developed **`vacancy_rate`** to assess available housing stock  
  - Addressed missing values in `permits_issued`  

## **Exploratory Analysis Goals & Visuals**  

### **Demand Analysis**  

#### **Housing Price Tiers and Interest Rate Bands**  
- **Chart:** Clustered Bar Plot  
- **Insight:** Mid- and High-tier homes are more common under moderate interest rates, while Very High-tier homes are less frequent across all bands.  

#### **Mortgage Rate vs. Consumer Sentiment**  
- **Chart:** Scatter Plot (colored by price tier)  
- **Insight:** Consumer sentiment slightly decreases as mortgage rates increase, with variations by price tier.  

#### **GDP Trends Across Interest Rate Bands**  
- **Chart:** Heatmap using a pivot table  
- **Insight:** Periods with lower interest rates tend to show higher GDP, reinforcing the inverse relationship between borrowing costs and economic output.  

### **Supply Analysis**  

#### **Construction Spending Over Time**  
- **Chart:** Line Plot  
- **Insight:** Peaks observed in **2005 and 2019–2021**, indicating strong investment cycles, followed by a slight decline in 2022.  

#### **Distribution of Vacant Units**  
- **Chart:** Histogram  
- **Insight:** Higher vacancy rates suggest **potential oversupply**, with noticeable stock increases over time.  

#### **Issued Permits vs. Housing Availability**  
- **Chart:** Bar Chart comparing `permits_issued` vs `vacancy_rate`  
- **Insight:** High permit issuance may indicate **future housing expansions**, while vacancy rates highlight **existing availability issues**.  

## **Key Takeaways and Findings**  

1. **Interest Rate Sensitivity**  
   Housing demand shifts in response to changing rate bands, particularly for mid-range properties.  

2. **Consumer Sentiment Dynamics**  
   Economic sentiment is influenced by affordability, represented by a decline when mortgage rates rise.  

3. **GDP Correlation with Interest Rates**  
   Stronger economic performance is observed in lower rate environments, reinforcing macroeconomic trends.  

4. **Supply Expansion vs. Vacancy**  
   Permit issuance suggests future growth, but **rising vacancy rates highlight possible market saturation risks**.  

5. **Construction Spending Cycles**  
   Investment peaked during economic booms but declined post-2022, hinting at corrections or cost-driven slowdowns.  

## **Initial Storytelling Presentation**  

### **Housing Demand vs. Interest Rates**  
Mid-tier homes dominate transactions when rates are moderate, showing affordability concerns at high rates.  

### **Economic Sentiment vs. Mortgage Rates**  
Scatter plots show declining consumer confidence with rising mortgage rates, particularly in mid-price tiers.  

### **GDP Trends Across Interest Rate Bands**  
Heatmaps confirm GDP’s strength during low-interest-rate periods, reinforcing housing market stimulation through economic policy.  

### **Construction Spending Trends**  
Sharp increases in spending suggest infrastructure expansion, while declines signal cautious investment.  

### **Vacant Units Over Time**  
Higher vacancy rates suggest potential supply surplus, requiring **further demand alignment strategies**.  


## **Data Quality and Enhancements**  

- Checked for missing values and anomalies  
- Cleaned column labels  
- Added engineered features for improved segmentation  
- Used aggregation and pivot tables for multidimensional analysis  

## **Conclusion**  

This EDA uncovered **valuable insights across housing supply and demand**, highlighting:  

- Low interest rates drive higher GDP, stronger consumer sentiment, and increased demand  
- Mid- and High-tier homes are more reactive to rate fluctuations  
- Vacancy rate shifts reflect possible market saturation or demand inconsistencies  
- Construction spending spikes align with economic booms but show corrections post-2022  

These findings offer a strong basis for **forecasting models and investment strategies**.  

## **Next Steps**  

1. **Time-Series Modeling:** Forecast housing demand and supply trends using rolling averages  
2. **Correlation & Regression Analysis:** Quantify the impact of economic shifts on housing markets  
3. **Interactive Dashboard:** Develop a dynamic visualization tool for further exploration  
4. **Geospatial Deep-Dive:** Examine regional housing trends if location-based data becomes available  


## **GitHub Repository**  

[View this project on GitHub](https://github.com/Kiruthikaa2512/datafun-06-eda)  


