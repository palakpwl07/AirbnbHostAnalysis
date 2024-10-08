# Airbnb Seattle Data Analysis Project

This project was built as a part of the MA2079 Introduction to Data Science and Artificial Intelligence course at Nanyang Technological University.

## Project Overview

The aim of this project is to analyze Airbnb data from Seattle to determine which aspects or characteristics of hosts contribute to securing more bookings and generating higher revenue. By identifying these key factors, potential hosts can optimize their profiles to maximize their profits.

## Dataset

The dataset used for this analysis is the Airbnb Open Data from Seattle. It contains information on various listings, hosts, and booking details.

## Problem Statement

**Which aspect or characteristics of the host will enable them to secure more bookings resulting in higher revenue?**

By leveraging data analysis techniques, the goal is to identify the most important factors that influence bookings and revenue, providing actionable insights for Airbnb hosts.

## Steps Involved

### 1. Data Cleaning

- **Initial Predictors:** 92
- **Final Predictors After Cleaning:** 33
- **Data Cleaning Process:**
  - Converted object data types to categorical.
  - Replaced all missing values (NAs) in the dataset with 0.
  - Calculated estimated revenue for each listing using the formula:  
    `Estimated Revenue = Price x Minimum Nights`.

### 2. Exploratory Data Analysis (EDA)

We performed exploratory data analysis to understand the relationships between different variables and estimated revenue. The key analyses included:

- **Categorical Variables vs Estimated Revenue:** Analyzed the impact of variables like superhost status, host identity verification, and neighborhood on estimated revenue.
- **Numerical Variables vs Estimated Revenue:** Investigated how the number of accommodations and other numerical features affect estimated revenue.
- **Review Heatmap:** Determined which aspects of the ratings matter most to visitors.

### 3. Regression Models

To predict the price and identify key features, we applied both univariate and multivariate regression models.

- **Univariate Regression:**
  - Explored the relationship between individual features (like accommodates, neighborhood group, and number of reviews) and price.
- **Multivariate Regression:**
  - Analyzed the combined effect of multiple features on price, highlighting the most significant predictors.

### 4. XGBoost Regressor

We implemented an XGBoost regressor to further refine the predictions and understand feature importance. The model was trained on selected features and evaluated using Mean Squared Error (MSE) and R-squared (R²) scores.

## Conclusion

Through this analysis, we identified the following key factors that influence the revenue generated by an Airbnb listing:

1. **Superhost Status:** Hosts with superhost status tend to generate higher revenue.
2. **Host Identity Verification:** Verified hosts are more likely to secure bookings.
3. **Accommodation Size:** Listings with 1-4 rooms are most popular among guests.
4. **Review Scores:** Communication, cleanliness, and location ratings are crucial for attracting bookings.
5. **Neighborhood:** The location of the listing significantly impacts its revenue potential.

These insights provide Airbnb hosts with actionable strategies to optimize their listings and increase their revenue.

---

This project showcases the application of data science techniques to real-world datasets, offering valuable insights for both academic and practical purposes.
