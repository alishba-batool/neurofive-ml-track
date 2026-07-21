# Titanic Exploratory Data Analysis

This project performs Exploratory Data Analysis (EDA), data cleaning, and visualization on the Titanic dataset using Python, Pandas, Matplotlib, and Seaborn.

## Dataset

- **Dataset:** Titanic Dataset
- **Language:** Python
- **Libraries Used:**
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn

## Tasks Performed

### Data Exploration
- Loaded the Titanic dataset using Pandas
- Displayed the first five rows
- Checked dataset information
- Generated statistical summary
- Identified numerical and categorical columns
- Checked for missing values

### Data Cleaning
- Filled missing values in the **Age** column using the median
- Filled missing values in the **Embarked** column using the mode
- Removed the **Cabin** column due to excessive missing values

### Data Visualization
- Visualized missing values
- Plotted the Age distribution (Histogram)
- Detected outliers using a Boxplot
- Created a Survival Count Bar Chart
- Created a Correlation Heatmap
- Analyzed the relationship between passenger class and survival

## Key Findings

- Most passengers were between 20 and 40 years old.
- The Fare column contains several outliers.
- First-class passengers had a significantly higher survival rate than third-class passengers.
- Passenger Class (Pclass) appears to have the strongest impact on survival.

## Conclusion

This project demonstrates the complete data preprocessing workflow, including data exploration, handling missing values, detecting outliers, and creating visualizations. These steps help prepare the dataset for future machine learning models.
