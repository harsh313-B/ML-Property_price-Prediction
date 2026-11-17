# California Housing Price Prediction

This project performs Exploratory Data Analysis (EDA) and builds a baseline **Linear Regression** model to predict median house values in California based on geographical and demographic features[cite: 1].

## Repository Structure

* `Property_Price_Prediction.ipynb` — Main Jupyter Notebook containing data loading, cleaning, EDA visualizations, and model training/evaluation.
* `Data_file.csv` — Dataset containing California housing metrics (ensure this is in the root directory when running the notebook)[cite: 1].

## Dataset Overview

The dataset contains **20,640 entries** and **10 columns** representing California housing district metrics[cite: 1]:

* `longitude` & `latitude`: Geographical coordinates of the housing block[cite: 1].
* `housing_median_age`: Median age of a house within a block[cite: 1].
* `total_rooms`: Total number of rooms within a block[cite: 1].
* `total_bedrooms`: Total number of bedrooms within a block (contains 207 missing values)[cite: 1].
* `population`: Total number of people residing within a block[cite: 1].
* `households`: Total number of households for a block[cite: 1].
* `median_income`: Median income for households within a block[cite: 1].
* `median_house_value`: **Target variable** — Median house value for households within a block (in USD)[cite: 1].
* `ocean_proximity`: Categorical location of the house relative to the ocean/sea[cite: 1].

## Key Insights from EDA

* **Missing Values:** Only `total_bedrooms` has missing records (207 null values)[cite: 1].
* **Target Distribution:** `median_house_value` shows a slight right skew with a cap at `$500,001`[cite: 1].
* **Feature Correlation:** Scatter plot analysis confirms a strong positive linear relationship between `median_income` and `median_house_value`[cite: 1].

## Tech Stack

* **Python 3**
* **Data Manipulation:** `pandas`, `numpy`[cite: 1]
* **Data Visualization:** `matplotlib`, `seaborn`[cite: 1]
* **Machine Learning:** `scikit-learn` (`train_test_split`, `LinearRegression`, `mean_squared_error`, `r2_score`)[cite: 1]

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/ML-Property_price-Prediction.git
   cd ML-Property_price-Prediction
