# AQI Data Analysis Report

## Executive Summary

This report presents a comprehensive analysis of 10,000 air quality records across 24 distinct cities. The dataset contains entirely valid records with no missing data for the analyzed fields of City and AQI. 

Key observations from the data include:
* The overall average AQI across all retrieved records is 273.7, with individual readings spanning from a minimum of 50 to a maximum of 499.
* Ahmedabad recorded the highest average AQI at 288.76 (based on 435 records), while Ludhiana recorded the lowest average AQI at 263.78 (based on 453 records).
* The difference between the highest and lowest city-level average AQI is relatively narrow at 24.98.
* Every single city in the dataset experienced extreme variations in air quality, with individual readings ranging from approximately 50 to nearly 499.

## Overall AQI Statistics

| Metric | Value |
|---|---:|
| Total records retrieved | 10,000 |
| Valid AQI records | 10,000 |
| Average AQI | 273.7 |
| Minimum AQI | 50 |
| Maximum AQI | 499 |
| Total AQI | 2,736,970 |

## City-Level Analysis

The dataset covers 24 distinct cities. Ahmedabad registered the highest average AQI of 288.76, while Ludhiana registered the lowest average AQI of 263.78. The spread between the highest and lowest city average is 24.98. 

The complete breakdown of AQI statistics for all 24 cities is presented below:

| Rank | City | Average AQI | Minimum AQI | Maximum AQI | Records |
|---:|---|---:|---:|---:|---:|
| 1 | Ahmedabad | 288.76 | 50 | 498 | 435 |
| 2 | Kolkata | 283.7 | 52 | 499 | 417 |
| 3 | Thane | 283.44 | 51 | 499 | 433 |
| 4 | Jaipur | 281.57 | 50 | 497 | 398 |
| 5 | Vadodara | 279.76 | 51 | 499 | 417 |
| 6 | Lucknow | 277.36 | 55 | 499 | 442 |
| 7 | Nashik | 275.74 | 51 | 499 | 448 |
| 8 | Surat | 275.48 | 50 | 496 | 368 |
| 9 | Hyderabad | 274.56 | 51 | 498 | 418 |
| 10 | Chennai | 274.17 | 51 | 499 | 419 |
| 11 | Rajkot | 273.94 | 52 | 496 | 428 |
| 12 | Nagpur | 273.83 | 50 | 499 | 492 |
| 13 | Indore | 273.72 | 50 | 499 | 399 |
| 14 | Bangalore | 272.6 | 51 | 499 | 419 |
| 15 | Varanasi | 271.02 | 51 | 498 | 430 |
| 16 | Agra | 270.48 | 52 | 497 | 408 |
| 17 | Pune | 269.9 | 50 | 498 | 435 |
| 18 | Mumbai | 269.64 | 53 | 499 | 377 |
| 19 | Delhi | 269.05 | 51 | 499 | 377 |
| 20 | Patna | 267.16 | 50 | 499 | 373 |
| 21 | Meerut | 266.87 | 50 | 499 | 418 |
| 22 | Bhopal | 265.73 | 50 | 498 | 398 |
| 23 | Srinagar | 264.36 | 52 | 499 | 398 |
| 24 | Ludhiana | 263.78 | 51 | 498 | 453 |

## Top 5 Cities by Average AQI

The five cities with the highest average AQI values are detailed below:

| Rank | City | Average AQI | Minimum AQI | Maximum AQI | Records |
|---:|---|---:|---:|---:|---:|
| 1 | Ahmedabad | 288.76 | 50 | 498 | 435 |
| 2 | Kolkata | 283.7 | 52 | 499 | 417 |
| 3 | Thane | 283.44 | 51 | 499 | 433 |
| 4 | Jaipur | 281.57 | 50 | 497 | 398 |
| 5 | Vadodara | 279.76 | 51 | 499 | 417 |

## Lowest Average AQI Cities

The five cities with the lowest average AQI values are detailed below:

| Rank | City | Average AQI | Minimum AQI | Maximum AQI | Records |
|---:|---|---:|---:|---:|---:|
| 1 | Ludhiana | 263.78 | 51 | 498 | 453 |
| 2 | Srinagar | 264.36 | 52 | 499 | 398 |
| 3 | Bhopal | 265.73 | 50 | 498 | 398 |
| 4 | Meerut | 266.87 | 50 | 499 | 418 |
| 5 | Patna | 267.16 | 50 | 499 | 373 |

## Data Quality

The dataset exhibits high completeness and integrity for the analyzed fields, as shown in the quality check table below:

| Check | Value |
|---|---:|
| Records retrieved (full dataset) | 10,000 |
| Records with valid AQI | 10,000 |
| Records with missing/invalid AQI | 0 |
| Records with missing City | 0 |
| Records grouped by City | 10,000 |
| Distinct cities | 24 |

### Limitations & Unavailable Analyses
* **Time-based trends (daily, monthly, yearly):** The dataset contains no Date, Month, or Year column; therefore, temporal or seasonal analysis cannot be performed.
* **Pollutant and environmental correlations:** Although columns for pollutants (PM2.5, PM10, NO2, CO, SO2, O3), weather (Temperature, Humidity, Wind Speed, Rainfall, Pressure), traffic (Vehicle Count), industrial activity, and health impact exist in the raw dataset, statistics for these columns were not calculated by the Analysis Engine. Consequently, no correlation or causal analysis can be reported.

## Key Insights

* **Narrow Spread in City Averages:** The average AQI values across all 24 cities are highly concentrated. The difference between the highest average (Ahmedabad: 288.76) and the lowest average (Ludhiana: 263.78) is only 24.98.
* **Uniformly Wide Intra-City Ranges:** Every single city in the dataset recorded a minimum AQI value between 50 and 55, and a maximum AQI value between 496 and 499. 
* **Balanced Data Distribution:** The volume of records per city is relatively uniform, ranging from a minimum of 368 records (Surat) to a maximum of 492 records (Nagpur).

### Interpretation
The data indicates that air quality is not consistently "good" or "bad" in any specific city. Because every city spans nearly the entire possible AQI spectrum (from a clean 50 to an extreme 499) and the overall city averages sit within a narrow 25-point band, the variations in air quality are driven by localized or short-term fluctuations within each city rather than permanent, systemic differences between the cities themselves.

## Conclusion

This analysis of 10,000 air quality records across 24 cities reveals an overall average AQI of 273.7. City-level averages are highly consistent, ranging from a low of 263.78 in Ludhiana to a high of 288.76 in Ahmedabad. Every analyzed city experienced the full range of air quality conditions, with individual readings spanning from approximately 50 to 499. Due to dataset limitations, temporal trends and correlations with weather, traffic, or specific pollutants could not be evaluated.

---
*Generated automatically on 2026-10-01 20:58 GMT+5:30 from the complete NocoDB AQI dataset (10000 records) using the AQI Data Analysis Engine. Narrative written by Google Gemini from engine-calculated values only.*