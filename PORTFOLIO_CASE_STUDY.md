# Portfolio Case Study: Food Delivery Delay Analysis and Prediction

## Project Title

Food Delivery Delay Analysis and Prediction

## Short Summary

I analyzed a food delivery dataset to identify the main factors affecting delivery time and delayed orders. The project included data cleaning, KPI analysis, exploratory data analysis, data visualization, and basic machine learning models for delay prediction.

## Problem Statement

A food delivery business wants to understand why some deliveries are delayed and which factors have the strongest impact on delivery performance. The business also wants a basic machine learning approach to predict whether an order may be delayed.

## My Role

I worked as a data analyst/data science beginner on this project. I handled the full workflow from dataset understanding to final recommendations:

- Loaded and inspected the CSV data
- Cleaned missing values
- Created new analysis-friendly features
- Built KPI summaries
- Performed EDA
- Created charts
- Trained basic machine learning models
- Interpreted model results
- Wrote business recommendations

## Dataset Details

The dataset contains 15,000 food delivery orders and 30 columns. It includes order timing, delivery distance, preparation time, traffic level, weather severity, ratings, order values, discounts, tips, cancellation flags, refund flags, premium customer flags, and delayed delivery flags.

## Approach

First, I explored the dataset using basic Pandas commands such as shape, head, info, missing values, and descriptive statistics. Then I cleaned missing values in tip and rating columns.

After cleaning, I created new features such as delivery delay minutes, distance buckets, traffic buckets, and weather buckets. These features helped make the analysis easier to understand and more useful for business interpretation.

Then I analyzed delivery performance by distance, traffic, weather, order hour, and city tier. I also used correlation analysis to identify which numeric features had the strongest relationship with delivery time.

Finally, I trained Logistic Regression and Random Forest models to predict delayed deliveries and evaluated the results using accuracy, precision, recall, F1-score, and confusion matrix.

## Key Insights

- Delivery distance is the strongest operational factor affecting delivery time.
- Orders in the 30-40 km range take the longest time to deliver.
- Higher traffic levels increase average delivery time.
- Bad weather increases average delivery time.
- Evening hours, especially 8 PM to 10 PM, show higher delivery times.
- City Tier 3 has the highest order volume and slightly higher delay rate.
- Machine learning models struggled with delayed delivery prediction because delayed orders are a minority class.

## Machine Learning Learning Point

The first Logistic Regression and Random Forest models showed high accuracy, but they failed to detect delayed orders. This happened because the dataset was imbalanced. Most orders were not delayed, so the models learned to predict the majority class.

After applying class balancing to Logistic Regression, the model started detecting delayed deliveries, but accuracy dropped because false positives increased. This showed an important real-world lesson: accuracy is not always the best metric for imbalanced classification problems.

## Business Recommendations

- Improve estimated delivery time calculations for long-distance orders.
- Allocate more delivery partners during evening peak hours.
- Monitor high-traffic and bad-weather deliveries more closely.
- Work with restaurants to reduce food preparation time.
- Focus on City Tier 3 operations because it has the largest order volume.
- Use efficiency scores to identify operational improvement opportunities.

## Skills Demonstrated

- Python
- Pandas
- Data Cleaning
- Exploratory Data Analysis
- KPI Analysis
- Data Visualization
- Matplotlib
- Seaborn
- Scikit-learn
- Classification Modeling
- Model Evaluation
- Business Insight Writing

## Final Outcome

The project produced a complete notebook and HTML report that explain the delivery performance patterns, key delay drivers, model results, limitations, and business recommendations. This project can be used as a beginner portfolio project for data analysis and data science roles.
