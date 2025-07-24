Assignment1:

📊 Project Overview

This project involves comprehensive preprocessing, analysis, and visualization of a large dataset related to electric vehicles (EVs). With over 210,000 records and 17 features, the goal was to clean, explore, and extract meaningful insights from the data using Python-based data science techniques.

📁 Dataset Information
Records: 210,165

Columns: 17

Data Types: A mix of numerical, categorical, and textual data

Main Features: Make, Model, Model Year, Electric Range, Location, MSRP, CAFV Eligibility, etc.

🛠️ Preprocessing Steps
1. Missing Value Handling
Identified missing values and calculated percentages.

Two strategies applied:

Dropping rows with missing values.

Filling missing values using appropriate methods:

Categorical: Filled with mode or 'Unknown'.

Numerical: Filled with mean (e.g., Postal Code).

Electric Utility: Filled with 'Utility Not Available'.

2. Encoding Categorical Data
Applied:

One-Hot Encoding: For unordered categories (e.g., Make, Model, City).

Label Encoding: For ordinal data.

3. Feature Normalization
Min-Max Scaling: To scale features between 0 and 1.

Standard Scaling: For standardized distribution with zero mean and unit variance.

📈 Exploratory Data Analysis (EDA)
4. Descriptive Statistics
Summarized numerical and categorical attributes (mean, median, std, unique counts, top values).

5. Spatial Distribution
Used Folium maps with marker clusters to visualize vehicle locations by Make.

6. Model Popularity
Identified most popular models (Model Y, Model 3) and dominant manufacturers.

Explored model distributions by city, county, and state.

7. Correlation Analysis
Built a correlation matrix and heatmap to investigate relationships between numeric features.

e.g., Moderate negative correlation between Electric Range and Model Year.

📊 Data Visualization Highlights
Electric Range Distribution: Most vehicles fall under 50 miles (likely PHEVs).

Base MSRP vs Electric Range: Visualized using scatter plots.

Vehicle Distribution by ZIP Code: Histogram and ranked table.

Top Cities: Pie chart showing Seattle, Bellevue, Vancouver leading.

CAFV Eligibility: Histogram comparing range across eligibility categories.

Vehicle Type by State: Bar charts for BEVs and PHEVs.

Top Makes & Models: Histograms by city, county, and state.

Log Scale Visualization: Compared top 10 brands across states.

📆 Temporal Analysis
Tracked production years of car models.

Model Trends Over Time:

Model Y peaked in 2021.

Leaf showed steady long-term growth.

Car Count Over Time: Consistent growth from 2000 to 2025 in:

Model popularity

Total EV registrations

Sales volumes

📌 Key Insights
Model Y is the most popular EV, followed by Model 3.

Seattle leads in EV adoption across all brands.

Tesla dominates the market with a significant margin.

Most electric vehicles have limited ranges, suggesting many are hybrids.

Geographic and temporal analysis highlights regional preferences and growth trends.

💻 Technologies Used
Python

Pandas, NumPy – Data preprocessing

Matplotlib, Seaborn – Visualization

Folium – Map plotting

Scikit-learn – Encoding and normalization



Assignment2:

## 📌 Overview

This project explores and analyzes a large dataset of electric vehicles registered in Washington State, USA. The dataset contains over **210,000 entries** with 17 features per record, including manufacturer, model, electric range, location, and more.

We performed data preprocessing, visualization, and feature engineering to extract insights and identify trends in EV adoption and distribution.

---

## 📁 Dataset Details

- **Records**: 210,165
- **Features**: 17 (e.g., Make, Model, Electric Range, Location, Model Year, MSRP)
- **Source**: Public EV dataset (Kaggle or open source)

---

## ⚙️ Processing Workflow

### 1. Missing Value Handling
- Identified columns with missing data.
- Handled via:
  - Dropping rows
  - Filling with statistical or custom values (mean, mode, or "Unknown")

### 2. Encoding
- Applied one-hot encoding for categorical variables.
- Used label encoding for ordinal columns.

### 3. Feature Scaling
- Used MinMaxScaler and StandardScaler from `scikit-learn`.

---

## 📊 Data Analysis & Visualization

### Geographic Distribution
- Visualized EV locations across Washington using **Folium maps** with clusters.

### Model & Brand Trends
- Identified top EV makes and models (e.g., Tesla Model Y, Nissan Leaf).
- Analyzed trends over time (2000–2025) using bar plots and histograms.

### Price & Range Analysis
- Visualized MSRP vs Electric Range.
- Found many cars with ranges < 50 miles (likely plug-in hybrids).

### Eligibility & Utility Analysis
- Examined Clean Alternative Fuel Vehicle (CAFV) eligibility.
- Filled and visualized missing electric utility data.

---

## 📈 Key Insights

- **Model Y** and **Model 3** are the most popular EVs.
- **Seattle** has the highest number of EVs.
- **Tesla** dominates the market with 4 of the top 5 models.
- EV adoption has grown steadily since 2000.
- Most EVs in the dataset are plug-in hybrids (limited electric range).

---

## 💻 Tools & Libraries

- Python  
- Pandas, NumPy – Data analysis  
- Matplotlib, Seaborn – Visualization  
- Folium – Maps  
- Scikit-learn – Preprocessing & Encoding

---
