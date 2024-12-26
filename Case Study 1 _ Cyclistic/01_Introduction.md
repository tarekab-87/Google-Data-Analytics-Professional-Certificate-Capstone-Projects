## Case Study 1: how does a bike-sharing navigate speedy success? 
**Company name: Cyclistic Bike-Share**

**Author: Tarek Abou Ismail**

**Date: 11/15/2024**

## 📝 Introducation 
Cyclistic Bike-Share, established in 2016, has become a prominent bike-sharing service in Chicago with a fleet of 5,824 GPS-enabled bicycles distributed across 692 stations. 

As a capstone project for the Google Data Analytics Professional Certificate on Coursera, this case study combines the data analysis process—ask, prepare, process, analyze, share, and act—to understand user behavior and address a critical business challenge: converting casual riders into annual members. Through this analysis, actionable insights and strategies are developed to maximize Cyclistic's growth and profitability.

## 💬 Background

**About the compnay**

Cyclistic, founded in 2016, has successfully grown its bike-sharing program into a network of 5,824 geotracked bicycles and 692 stations across Chicago, allowing users to rent bikes at one station and return them at another. 

Offering flexible pricing plans such as single-ride passes, full-day passes, and annual memberships, Cyclistic appeals to a diverse customer base, including those with disabilities through assistive bike options. 

While casual riders primarily opt for pay-per-use plans, financial analysis reveals that annual members are significantly more profitable. To drive future growth, the company seeks to convert casual riders into loyal annual members by analyzing historical bike trip data to understand usage patterns, identify motivations, and develop targeted marketing strategies that leverage digital media.

## ⚙ Approach 

### 1. Ask / Business Objectives and Key Questions

**Business Task**

Design marketing strategies aimed at converting casual riders into annual members by understanding user behavior and preferences.

> **Guiding Questions**
>
> 1. How do annual members and casual riders use Cyclistic bikes differently?
> 2. What motivates casual riders to become annual members?
> 3. How can Cyclistic use digital media to influence this conversion?

**Stakeholders**
- Cyclistic management team
- Marketing department
- Financial analysts

### 2. Prepare

Data Overview

**Source**

The data was sourced from the Chicago Department of Transportation (CDOT) and is availabe under this  [divvy_tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html). The data was made available to public under [license](https://divvybikes.com/data-license-agreement). The dataset encompassing a 12-month period (November 2023 to October 2024). This structured dataset includes:
- Ride IDs
- Ride types
- Start and end times
- Station names and IDs
- User categories (casual or member)

**Data Integrity**

The data meets the ROCCC framework:
- Relevant: Directly supports the analysis objectives.
- Original: Provided by a reliable primary source.
- Comprehensive: Covers a full year of usage.
- Current: Up-to-date through October 2024.
- Credible: Originates from a trusted authority.

**Tools**:
- Data cleaning and processing : Bigquery and PostgreSQL
- Data visualization: Power BI and Tableau.


### 3. Data Processing and Cleaning

**Steps Taken:**
1. Data Exploration and Validation: Checked for missing values, duplicates, and formatting inconsistencies.
2. Data Consolidation: Combined 12 months of ride data into a single table.
3. New Variables: Created new columns for:
    - Start and end months
    - Day of the week
    - Ride length (in minutes)
5. Outlier Removal: Used interquartile range (IQR) to filter out anomalous ride lengths.
6. Final Dataset: Excluded rows with null values and retained clean, consistent data for analysis.

### 4. Analysis and Insights

1. Usage Patterns
![image](https://github.com/user-attachments/assets/d172d756-4f9e-4605-88b2-11b23545c011)

Total Rides: Casual riders accounted for 32.96% (1,295,966) of rides, while annual members contributed 67.04% (2,644,466).

2. User perfernces
![image](https://github.com/user-attachments/assets/b6d4e114-125c-4376-b33c-7dd63b762758)
The bar chart compares ride counts of members and casual riders based on the type of rideable type: classic bikes, electric bikes, and electric scooters.

Key observations:
Classic Bikes: Dominant choice for both groups, with members recording 1.73M rides and casual riders 0.79M rides.
Electric Bikes: Members used them more (0.88M) compared to casual riders (0.48M).
Electric Scooters: Negligible usage by both groups (0.02M each).









