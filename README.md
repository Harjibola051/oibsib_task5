# oibsib_task5
house_price_prediction
# Housing Price Prediction Project

## Project Overview
This project aims to predict housing prices using a comprehensive dataset containing various features such as price, area, bedrooms, bathrooms, stories, and parking spaces. The analysis includes data exploration, data cleaning, feature engineering, and model training using machine learning algorithms.

## Dataset
The dataset used is `Housing.csv`, which contains both numerical and categorical features related to housing attributes.

## Data Exploration and Cleaning

### Null Value Check
- No missing values were found in the dataset.

### Data Distribution
- The numerical features exhibited some skewness, particularly in price and area.
- Box plots revealed the presence of outliers in the price and area columns.

### Handling Outliers
- The Interquartile Range (IQR) method was used to remove outliers from the price and area columns.

### Encoding Categorical Variables
- One-hot encoding was applied to convert categorical features into numerical format.

## Feature Selection

### Multicollinearity Check
- The Variance Inflation Factor (VIF) was computed to detect multicollinearity.
- A correlation heatmap was plotted to visualize feature relationships.
- Lasso regression was employed for feature importance analysis.

## Model Training

### Train-Test Split
- The data was split into training and testing sets (80% training, 20% testing).

### Models Used
- Linear Regression
- Random Forest Regressor

### Model Performance
- Linear Regression:
  - Mean Absolute Error (MAE): 86524.31
  - Mean Squared Error (MSE): 12845329012.75
  - Root Mean Squared Error (RMSE): 113354.84
  - R-squared (R²): 0.72

- Random Forest Regressor:
  - Higher feature importance for area and number of bedrooms.

## Residual Analysis
- The residuals followed a normal distribution.
- Homoscedasticity was confirmed with no visible pattern in the residual plot.
- Actual vs Predicted values showed a reasonable correlation.

## Conclusion
- The Linear Regression model achieved an R² score of 0.72, explaining 72% of the variance in housing prices.
- The Random Forest Regressor showed better feature importance but was not explicitly evaluated for performance metrics.
- The model effectively handles multicollinearity and outliers, making it robust for housing price prediction.

## Future Work
- Explore additional feature engineering techniques.
- Incorporate more advanced models like XGBoost.
- Perform hyperparameter tuning for improved performance.

## Repository Structure
```
Housing_Price_Prediction/
│
├── data/
│   └── Housing.csv
├── notebooks/
│   └── Data_Exploration.ipynb
│   └── Model_Training.ipynb
├── models/
│   └── Linear_Regression.pkl
│   └── Random_Forest.pkl
├── README.md
└── requirements.txt
```

## Installation and Usage

```bash
# Clone the repository
git clone https://github.com/username/Housing_Price_Prediction.git

# Navigate to the project directory
cd Housing_Price_Prediction

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
jupyter notebook
```

## Acknowledgements
- The dataset was sourced from [Dataset Source].
- Libraries used: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, Statsmodels.

## Contact
For questions or collaborations, reach out to [Your Email] or visit my [GitHub profile](https://github.com/username).

