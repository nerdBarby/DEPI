# Breast Cancer Data Analysis

## Project Overview
This project involves a comprehensive analysis of breast cancer data to identify patterns and distinguish between Malignant (M) and Benign (B) diagnoses. The analysis utilizes Python for data preprocessing and visualization, SQL for data querying and statistical comparison, and concludes with a dashboard summary[cite: 1, 6].

## Tools & Technologies
**Python Libraries:** `numpy`, `pandas`, `seaborn`, `matplotlib.pyplot`.
**Visualization:** Matplotlib, Seaborn, and Interactive Dashboard.

## Data Preprocessing (Python)
The dataset was loaded and cleaned using the Pandas library:
**Data Loading:** The dataset `breast-cancer.csv` was read into a DataFrame.
**Data Inspection:**
  The dataset contains 569 entries and 32 columns
  The `id` column was converted to an object type.
 **Cleaning:**
   Checked for duplicate rows: **0 duplicates** found.
   Checked for null values: **0 nulls** found across all columns.

## Exploratory Data Analysis (EDA)

### 1. Diagnosis Distribution
The target variable is `diagnosis`.
**Benign (B):** 357 cases (62.74%).
**Malignant (M):** 212 cases (37.26%).

### 2. Descriptive Statistics
Descriptive statistics (count, mean, std, min, 25%, 50%, 75%, max) were generated for all numerical columns to understand the data distribution.

### 3. Visualizations
Key insights were derived through various plots:
* **Boxplots:** Showed clear distinctions between diagnoses. Malignant cases consistently exhibited higher values for `radius_mean`, `perimeter_mean`, `smoothness_mean`, and `concavity_mean` compared to Benign cases[cite: 2].
  **Feature Comparisons:** Bar charts comparing "Mean" vs "Worst" values highlighted that Malignant tumors have significantly larger area, perimeter, and radius measurements.
* **Correlation Matrix:** A heatmap was generated to visualize the relationships between features. Strong positive correlations were observed between features such as `radius_mean`, `perimeter_mean`, and `area_mean`[cite: 2, 4].



## Dashboard
A visual dashboard summarizes the final analysis:
* **Diagnosis Distribution:** Pie chart confirming the 357 (B) vs 212 (M) split.

* **Scatter Plots:**
    * `perimeter_mean` vs `area_mean` shows a strong positive linear relationship.
    `concave points_mean` vs `concavity_mean` shows a positive correlation.
**Tumor Characteristics:** Bar charts reinforcing that average radius, area, and perimeter are higher in Malignant diagnoses.

![Picture1](https://github.com/user-attachments/assets/011f3b55-b655-47da-99f3-d93ce5f32d9d)
