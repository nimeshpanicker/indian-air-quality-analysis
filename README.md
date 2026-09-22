# 🇮🇳 Indian Urban Air Quality Analysis

## 📌 Project Overview

An exploratory data analysis project examining air-quality observations across Indian cities.

The project uses Python-based data analysis to assess AQI distributions, AQI categories, city-level patterns, pollutant relationships, environmental variables, and overall data quality.

The dataset contains 10,000 observations across 24 Indian cities and 16 variables.

---

## 🎯 Project Objectives

- Examine the distribution of AQI observations
- Analyze AQI categories
- Compare AQI across Indian cities
- Explore relationships between AQI and pollutants
- Examine traffic and industrial activity variables
- Perform data-quality validation
- Apply statistical analysis to test apparent patterns
- Identify limitations within the dataset
- Communicate findings through visualizations and a professional report

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- scikit-learn
- Jupyter / VS Code
- GitHub

---

## 📊 Dataset

**Dataset:** `indian_aqi_health_impact_2019_2024.csv`

The dataset contains:

- 10,000 observations
- 24 Indian cities
- 16 columns
- AQI
- PM2.5
- PM10
- NO2
- CO
- SO2
- O3
- Temperature
- Humidity
- Wind Speed
- Rainfall
- Pressure
- Vehicle Count
- Industrial Activity Index
- Health Impact Score

---

## 🔄 Data Cleaning & Preparation

The analysis included:

- Missing-value checks
- Duplicate-record checks
- Data-type validation
- Column-name standardization
- Numeric conversion
- AQI range validation
- AQI category creation
- Constant-column detection
- Summary-table generation

The dataset contained no missing values, no duplicate rows, and no AQI values outside the 0–500 range.

---

## 📈 Exploratory Data Analysis

The project examines:

### AQI Distribution

The analysis found:

- Mean AQI: **273.70**
- Median AQI: **273**
- Minimum AQI: **50**
- Maximum AQI: **499**

### AQI Categories

The observations were categorized into:

- Good
- Satisfactory
- Moderate
- Poor
- Very Poor
- Severe

### City Analysis

City-level AQI averages were calculated to compare the 24 cities in the dataset.

### Pollutant Analysis

The project examines:

- PM2.5
- PM10
- NO2
- CO
- SO2
- O3

### Environmental & Activity Variables

The analysis also examines relationships involving:

- Temperature
- Humidity
- Wind Speed
- Rainfall
- Pressure
- Vehicle Count
- Industrial Activity Index

---

## 🔬 Statistical Analysis

The project goes beyond basic descriptive analysis and includes:

- Pearson correlation
- Spearman correlation
- Chi-square testing
- ANOVA
- Kruskal-Wallis testing
- Welch t-tests
- Cross-validated linear regression
- Random forest modelling

These methods were used to test whether apparent relationships in the dataset were statistically meaningful.

---

## 🔍 Key Findings

### Overall AQI Distribution

The average AQI was **273.70**, with observations distributed across the full recorded range of 50–499.

### AQI Category Distribution

Approximately **66.9% of observations were classified as Poor, Very Poor, or Severe**.

Only **10 observations (0.1%)** were classified as Good.

### City-Level Differences

Ahmedabad had the highest average AQI in the dataset at approximately **288.8**, while Ludhiana had the lowest at approximately **263.8**.

However, the statistical analysis did not identify a significant city effect.

### Relationships with AQI

The analysis found very weak relationships between AQI and the available predictor variables.

The strongest Pearson correlation with AQI was approximately **0.018**, indicating very little linear association in this dataset.

---

## ⚠️ Data Quality & Limitations

An important part of this project was identifying limitations rather than assuming that every apparent pattern represented a real-world relationship.

The dataset has:

- No date/year/month column
- A constant Health Impact Score of 10
- No documented pollutant measurement units
- No documented sampling methodology
- Variable distributions that appear unusually flat
- Limited evidence of relationships between AQI and the available predictors

Because there is no time field, a genuine 2019–2024 time-trend analysis cannot be performed from this dataset alone.

Because the Health Impact Score is constant, meaningful health-impact modelling cannot be performed from this variable.

---

## 🖼️ Visualizations

### AQI Distribution

![AQI Distribution](screenshots/aqi-distribution.png)

### AQI Categories

![AQI Categories](screenshots/aqi-categories.png)

### City AQI Analysis

![City AQI Analysis](screenshots/city-aqi-analysis.png)

### Pollutant Correlation

![Pollutant Correlation](screenshots/pollutant-correlation.png)

---

## 📁 Project Structure

```text
indian-air-quality-analysis/
│
├── data/
│   └── indian_aqi_health_impact_2019_2024.csv
│
├── python/
│   └── indian_aqi_analysis.py
│
├── reports/
│   └── Indian_Urban_Air_Quality_Analysis_Report.pdf
│
├── screenshots/
│   ├── aqi-distribution.png
│   ├── aqi-categories.png
│   ├── city-aqi-analysis.png
│   └── pollutant-correlation.png
│
└── README.md
