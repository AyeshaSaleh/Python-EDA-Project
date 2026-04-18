# 🏠 USA Real Estate: Exploratory Data Analysis & Feature Engineering

This project involves a deep-dive Exploratory Data Analysis (EDA) of a massive USA Housing dataset containing over **2.2 million records**. The goal was to uncover key drivers of property characteristics and prepare the data for predictive modeling using advanced preprocessing techniques.

---

## 📊 Project Overview
The analysis explores the relationship between property features (bedrooms, bathrooms, house size) and market trends across different states and cities in the US. 

* **Dataset Size:** 2,226,382 rows × 12 columns.
* **Key Focus:** Data cleaning, handling significant missing values, and high-dimensional feature encoding.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** * `Pandas` & `NumPy`: Data manipulation and cleaning.
    * `Matplotlib` & `Seaborn`: Statistical data visualization.
    * `Scikit-Learn`: Feature scaling and categorical encoding.

---

## 🔍 Key Technical Steps

### 1. Data Cleaning & Preprocessing
* **Missing Value Strategy:** Identified columns with high null counts (Bedrooms: 21.6%, Bathrooms: 23%, House Size: 25.5%).
* **Duplicate Removal:** Streamlined the dataset to ensure unique observation counts.
* **Date Engineering:** Extracted `sold_year` and `sold_month` from the `prev_sold_date` to identify seasonal real estate trends.

### 2. Advanced Feature Engineering
* **Categorical Encoding:** * Applied **Label Encoding** and **One-Hot Encoding** for status and state variables.
    * Implemented **Frequency Encoding** for high-cardinality features like `city`, `street`, and `brokered_by`.
* **Feature Scaling:** * Utilized **MinMaxScaler** to normalize numerical ranges.
    * Applied **StandardScaler** to ensure features have a mean of 0 and a standard deviation of 1, preparing the data for distance-based algorithms.

### 3. Exploratory Insights
* **Property Distribution:** Visualized house size density and determined the average bedroom counts across top-performing cities.
* **Correlation Analysis:** Generated heatmaps to analyze the strong linear relationships between square footage and the number of bathrooms/bedrooms.
* **Sales Seasonality:** Identified peak selling months using distribution pie charts.

---

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
