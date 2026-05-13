# Food Delivery Delay Analysis and Prediction

## Project Overview

This project analyzes a food delivery dataset to understand the main factors that affect delivery time and delayed orders. The analysis includes data cleaning, KPI summary, exploratory data analysis, visualizations, and basic machine learning models for delayed delivery prediction.

## Business Problem

Food delivery businesses need to understand why some deliveries take longer than expected. The goal of this project is to identify the key drivers behind delivery delays and provide useful business recommendations for improving delivery performance.

## Dataset

The dataset contains food delivery order-level records with information about:

- Customer details
- Order time and date information
- Delivery distance
- Food preparation time
- Traffic and weather scores
- Ratings
- Order value, fees, discounts, and tips
- Cancellation, refund, promo, premium customer, and delay flags

## Tools and Libraries

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Loaded and inspected the CSV dataset
2. Checked rows, columns, data types, and missing values
3. Cleaned missing values in rating and tip columns
4. Created useful features such as delivery delay minutes and distance buckets
5. Built KPI summaries for delivery performance
6. Performed exploratory data analysis
7. Created visualizations for key business factors
8. Trained classification models to predict delayed deliveries
9. Evaluated model performance and class imbalance issues
10. Prepared final insights and business recommendations

## Key Findings

- Delivery distance is the strongest operational factor affecting delivery time.
- Longer distance orders, especially 30-40 km, take significantly more time to deliver.
- Traffic and bad weather increase average delivery time.
- Evening peak hours, especially around 8 PM to 10 PM, show slightly higher delivery times.
- City Tier 3 has the highest order volume and a slightly higher delay rate.
- The dataset is imbalanced because most deliveries are not delayed.

## Machine Learning Summary

Logistic Regression and Random Forest models achieved high accuracy, but the initial models struggled to identify delayed deliveries due to class imbalance. After applying class balancing to Logistic Regression, the model improved recall for delayed deliveries but produced more false positives.

This shows that accuracy alone is not enough for imbalanced classification problems. Recall and F1-score are more important when the goal is to detect delayed deliveries.

## Business Recommendations

- Set more realistic estimated delivery times for long-distance orders.
- Allocate more delivery partners during evening peak hours.
- Monitor bad-weather and high-traffic deliveries more closely.
- Improve restaurant preparation workflows to reduce total delivery time.
- Focus operational monitoring on City Tier 3 because it has the highest order volume.
- Use delivery efficiency score to identify strong and weak delivery operations.

## Files

- `Food_Delivery_Delay_Analysis_and_Prediction.ipynb` - Main Jupyter Notebook
- `Food_Delivery_Delay_Analysis_and_Prediction.html` - Exported HTML report
- `food_delivery_analytics_cleaned.csv` - Dataset used for analysis

## Conclusion

This project demonstrates a complete beginner-friendly data science workflow, from raw CSV inspection to business insights and basic predictive modeling. The analysis found that distance, preparation time, traffic, weather, and order hour are important factors in delivery performance.
