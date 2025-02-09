# Real Estate Market Analysis in Germany

## Overview
This project analyzes **rental listings in Germany** using data from **Immoscout24**, the country's largest real estate platform. The dataset includes **over 260,000 properties** with **49 variables**, such as rent prices, property features, and geographical information. The goal is to clean and preprocess the data, conduct exploratory data analysis (EDA), and build machine learning models to predict rental prices and categorize properties.

---

## Objectives
- **Data Cleaning**: Handle missing values, outliers, and inconsistencies.
- **Exploratory Data Analysis (EDA)**: Identify key factors influencing rental prices.
- **Feature Engineering**: Transform and select relevant variables.
- **Predictive Modeling**: Use **supervised learning** (regression) to forecast rental prices.
- **Clustering**: Apply **unsupervised learning** to group properties based on features.
- **Market Insights**: Provide actionable recommendations for real estate stakeholders.

---

## Dataset Description
The dataset consists of rental listings from **Immoscout24**, containing:

### **Main Variables**
- **Quantitative Variables**:
  - `baseRent`, `totalRent`, `serviceCharge` – Cost breakdown of rental prices.
  - `livingSpace`, `noRooms`, `floor`, `yearConstructed` – Key property characteristics.
- **Categorical Variables**:
  - `regio1`, `regio2`, `geo_krs` – Location details (state, district, city).
  - `heatingType`, `firingTypes`, `condition` – Heating systems and property condition.
  - `petsAllowed`, `balcony`, `garden`, `lift` – Amenities.
- **Boolean Variables**:
  - `newlyConst`, `cellar`, `hasKitchen` – Indicators of property features.

---

## Methodology
### **1. Data Cleaning**
- **Removed duplicates** and unnecessary columns (e.g., unique IDs, street names).
- **Handled missing values** using imputation techniques (median for numerical data, mode for categorical).
- **Addressed outliers** using statistical techniques like box plots and capping extreme values.
- **Standardized variables** to ensure consistency in analysis.

### **2. Exploratory Data Analysis (EDA)**
- **Univariate Analysis**: Examined the distribution of rental prices and property features.
- **Bivariate Analysis**: Identified correlations between pricing and location, size, amenities.
- **Geospatial Analysis**: Mapped rental prices across Germany to detect regional trends.
- **Key Findings**:
  - **Higher rental prices** in urban areas like **Berlin, Munich, and Frankfurt**.
  - **Balconies, modern heating, and proximity to city centers** increase rental value.
  - **Older properties** tend to have lower rents unless recently refurbished.

### **3. Feature Engineering**
- Created **new categorical variables** for property condition and regional rent trends.
- Engineered **binned variables** for rent ranges, floor levels, and property age.
- Normalized numerical variables for better model performance.

### **4. Machine Learning Models**
#### **Supervised Learning - Regression**
- **Linear Regression**: Achieved **R² of 0.68**, identifying key predictors of rent.
- **Random Forest Regressor**: Improved predictions with an **R² of 0.82**, showing non-linear relationships.
- **XGBoost**: Provided the highest accuracy with **R² of 0.85**, ranking features by importance.

#### **Unsupervised Learning - Clustering**
- **K-Means Clustering**: Grouped properties into distinct pricing categories.
- **PCA (Principal Component Analysis)**: Reduced dimensionality for better clustering performance.
- **Key Insights**:
  - **High-end properties** (Cluster 1) with premium amenities and central locations.
  - **Affordable housing** (Cluster 2) in suburban and rural areas.
  - **Standard apartments** (Cluster 3) with moderate rent in mid-tier cities.

---

## Key Outcomes
- **A fully cleaned and structured dataset**, ready for predictive modeling.
- **Identified major factors influencing rent**, including location, size, and property condition.
- **Developed predictive models** that estimate rent with high accuracy.
- **Provided clustering insights** to categorize properties and detect market trends.
- **Generated geospatial heatmaps** to visualize price distribution across Germany.

---

## Repository Contents
-  **cleaning_and_EDA_FV.ipynb** – Data cleaning, feature engineering, and exploratory analysis.
-  **modeling.ipynb** – Machine learning models for price prediction and clustering.
-  **Principles_and_Elementary_Models_Report.pdf** – Detailed documentation of methods and findings.
-  **Abstract** - Summary on the project and insights found.
-  **cleaned_dataset.csv** - The cleaned dataset used for modeling.
-  **immo_data.csv** – The full dataset before applyin cleaning.

---

## How to Use
### **1. Run Data Cleaning & EDA**
- Open `cleaning_and_EDA_FV.ipynb` and execute the steps to clean and explore the dataset.

### **2. Train the Machine Learning Models**
- Open `modeling.ipynb` to run regression and clustering models.

### **3. Interpret Results**
- Use regression outputs to analyze key pricing factors.
- Utilize clustering results to categorize properties effectively.

---

## Business & Market Insights
- **Investors & Developers**: Identify high-value locations for property investments.
- **Renters & Buyers**: Understand price expectations across different property types.
- **Real Estate Agencies**: Use data-driven insights for competitive pricing strategies.

---

This project provides **data-driven insights into Germany's rental market**, leveraging **machine learning and statistical analysis** to improve transparency and decision-making.

