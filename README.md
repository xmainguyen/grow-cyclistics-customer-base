# Cyclistics Customer Growth Analysis

## Overview

This repository contains the analysis for the Cyclistics customer growth project. The objective of this case study is to analyze historical bike-share data to identify trends and differences in usage between "casual" riders and "annual" members. The ultimate goal is to provide recommendations on how to convert casual riders into annual members.

## Business Problem

Cyclistic’s Customer Growth Team is creating a business plan for next year. The team wants to understand how their customers are using their bikes; their top priority is identifying customer demand at different station locations. **The primary question:** How can we apply customer usage insights to inform new station growth?

The detailed problem description and goals for this project can be found in the documentation folder. 

## 🛠️ Project Structure
```
cyclistics-customer-growth-project/
├── data/                     # Saved raw and cleaned data (CSV files)
│   ├── stations.csv
│   ├── tripss.csv
│   └── trips_cleaned.csv
├── notebooks/
│   ├── 01_data_pull.ipynb                     # API fetch from Google BigQuery, raw → curated tables
│   ├── 02_clean_features.ipynb                # Cleaning, feature engineering
│   ├── 03_eda.ipynb                           # Exploratory Data Analysis
│   └── 04_causal_inference.ipynb              # Causal Model Design
├── documentation/
│   ├── 01_StakeholderRequirements.pdf         
│   ├── 02_ProjectRequirements.pdf             
│   └── 03_Strategy.pdf                        
├── dashboard/
│   └── app.py                      # Optional Streamlit dashboard
```

## Data

The data used for this analysis is located in the `data/` directory. It consists of 12 months of trip data in 2018 from Cyclistics. The data has been processed and cleaned for analysis.

This analysis is based on a combination of public datasets hosted on **Google BigQuery** and a supplementary custom data file.

The primary datasets were queried directly from BigQuery's public data repository:

* **NYC Citi Bike Trips** (`new_york_citibike`): This dataset contains detailed trip data from New York City's bike-share system for the year 2018.

* **NOAA GSOD Weather Data** (`noaa_gsod`): We used this dataset from the National Oceanic and Atmospheric Administration to source daily weather observations, such as temperature and precipitation.

* **Census Bureau US Boundaries** (`geo_us_boundaries`): This dataset provides geographical boundary data, which was used for location-based analysis.

Additionally, a supplementary **Zip Code Data** file (`.csv`) was uploaded to our BigQuery project. This file contains specific zip code information that was joined with the public datasets to enrich the analysis.

## Analysis and Findings

The core of the analysis is within the Jupyter Notebook located at `notebooks/`.

The analysis is structured as follows:

1.  **Data Loading and Cleaning:** Importing the necessary libraries and loading the datasets.
2.  **Exploratory Data Analysis (EDA):** Investigating the data to find patterns, anomalies, and initial insights.
3.  **Data Visualization:** Creating visualizations to communicate the findings effectively.
4.  **Key Findings:** Summarizing the main discoveries from the analysis, focusing on the differences between casual and member riders.

*[Optional: You can add a few key findings here as bullet points.]*

## Recommendations

Based on the analysis, the following recommendations are proposed to help convert casual riders into annual members:

  * [Recommendation 1]
  * [Recommendation 2]
  * [Recommendation 3]

A more detailed explanation of the recommendations can be found in the analysis notebook.

## Tools and Libraries

  * **Language:** Python
  * **Libraries:**
      * pandas
      * NumPy
      * Matplotlib
      * Seaborn
      * [Any other libraries you used]

## How to Run the Analysis

1.  Clone this repository:
    ```bash
    git clone https://github.com/xmainguyen/cyclistics-customer-growth-project.git
    ```
2.  Navigate to the `notebooks/` directory.
3.  Open and run the Jupyter Notebook to see the full analysis.
