# OIBSIP Data Science Task 5 – Sales Prediction Using Advertising Data

## Objective
The goal of this project is to build a regression model to predict **sales revenue** based on advertising expenditure across different media: **TV, Radio, and Newspaper**. This project helps businesses understand which advertising channels contribute most to product sales.

## Dataset Details

The dataset contains historical data on advertising spending and corresponding product sales:

| Column        | Description                            |
|---------------|----------------------------------------|
| TV            | Budget spent on TV advertising (in $)  |
| Radio         | Budget spent on Radio advertising (in $)|
| Newspaper     | Budget spent on Newspaper advertising (in $)|
| Sales         | Product sales (in thousands of units)  |

Dataset file: `Advertising.csv`

## Steps Performed

### 1. Data Loading and Inspection
- Loaded the dataset using pandas
- Verified the absence of missing values
- Checked statistical properties and visualized feature distributions

### 2. Exploratory Data Analysis (EDA)
- Visualized relationships using pairplots and heatmaps
- Found strong positive correlations between TV and Radio with Sales
- Newspaper had weaker correlation with Sales

### 3. Model Building
- Chose **Linear Regression** as the baseline model
- Split the dataset into training and testing sets (80-20 split)
- Trained the model using `scikit-learn`

### 4. Model Evaluation
- Evaluated using metrics:
  - R² Score
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
- Visualized the comparison between actual and predicted sales

## Tools and Libraries Used

- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- Jupyter Notebook

## Key Insights

- TV advertising had the **strongest impact** on sales, followed by Radio.
- Newspaper advertising had little to no effect on sales in this dataset.
- The Linear Regression model achieved a good R² score, showing that advertising budget is a reliable predictor of sales performance.


