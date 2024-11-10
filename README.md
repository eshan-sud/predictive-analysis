# Air Quality Prediction Project

## Objective

The goal of this project is to perform **Exploratory Data Analysis (EDA)** and apply **predictive modeling** on air quality data to forecast pollutant concentrations.

## Dataset

- **Source**: [Kaggle - Air Quality Data Set](https://www.kaggle.com/datasets/fedesoriano/air-quality-data-set)
- **Description**: Contains over 200 rows with features including pollutant levels (e.g., NO2, CO), temperature, and humidity.

## Project Steps

### 1. Dataset Selection

- Chosen dataset on air quality to analyze pollutant concentrations based on sensor data.

### 2. Data Preparation

- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn.
- **Data Loading**: Used `pd.read_csv()` to import the dataset.
- **Cleaning**:
  - Handled missing values using mean imputation.
  - Removed duplicate entries with `drop_duplicates()`.
- **Feature Engineering**:
  - Created time-based features like month and day.
  - Normalized pollutant concentrations.

### 3. Exploratory Data Analysis (EDA)

- **Summary Statistics**:
  - Computed mean, median, and std using `df.describe()`.
- **Visualizations**:
  - Histograms and box plots to observe distributions and outliers.
  - Correlation heatmap to check relationships between features.
- **Insights**:
  - Identified key pollutant trends and correlations with temperature.

### 4. Predictive Modeling

- **Models Used**:
  - **Linear Regression**
  - **Decision Tree Regressor**
  - **Random Forest Regressor**
- **Train-Test Split**: 80% training, 20% testing.
- **Evaluation Metrics**: MSE, R² Score.

### 5. Results and Evaluation

- **Performance**:
  - Linear Regression: MSE = 524.19, R² = 0.77
  - Decision Tree: MSE = 645.40, R² = 0.72
  - Random Forest: MSE = 326.07, R² = 0.86
- **Conclusion**: Random Forest performed best with lowest error and highest R² score.

### 6. Conclusion and Future Work

- **Summary**: Successfully predicted NO2 levels; Random Forest model gave the best accuracy.
- **Limitations**:
  - Presence of outliers affected simpler models like Linear Regression.
- **Future Improvements**:
  - Experiment with deep learning models for better predictions.
  - Incorporate real-time weather data for improved accuracy.

## References

1. Kaggle Dataset: [Air Quality Data Set](https://www.kaggle.com/datasets/fedesoriano/air-quality-data-set)
2. [Scikit-learn Documentation](https://scikit-learn.org/stable/)
3. [Matplotlib Documentation](https://matplotlib.org/stable/index.html)
