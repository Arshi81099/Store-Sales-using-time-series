# Store-Sales-using-time-series


# Project Title: Sales Forecasting with PySpark and Holt-Winters Method

## Description
This project implements a sales forecasting model using Apache Spark and the Holt-Winters exponential smoothing method. It performs data preprocessing, visualization, and forecasting on a retail sales dataset.

## Table of Contents
- [Installation](#installation)
- [Data Preparation](#data-preparation)
- [Visualization](#visualization)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [License](#license)

## Installation
To run this project, you'll need to set up the environment with the following dependencies:

1. **Apache Spark**: Install Spark and set the environment variables.
2. **Findspark**: A Python library to locate Spark installation.
3. **Pandas**: For data manipulation and analysis.
4. **Matplotlib & Seaborn**: For data visualization.
5. **Plotly**: For interactive visualizations.
6. **Statsmodels**: For time series forecasting models.
7. **scikit-learn**: For performance evaluation metrics.

Use the following command to install the required Python packages:
```bash
pip install findspark pandas matplotlib seaborn plotly statsmodels scikit-learn
```

## Data Preparation
The dataset is read from a CSV file (`train.csv`), which contains sales data with the following columns:
- `date`: Date of the sales
- `store`: Store identifier
- `item`: Item identifier
- `sales`: Number of sales

The date column is converted to a datetime format for analysis.

## Visualization
The project includes various visualizations to understand sales patterns:
- Histogram of sales frequency.
- Daily sales over time.
- Daily sales for each store.
- Daily sales for each item.
- Top 5 items by sales.

Interactive visualizations are created using Plotly for better insights.

## Modeling
The Holt-Winters exponential smoothing method is used for forecasting sales. The dataset is split into training and testing sets based on a specified date. The model is trained on the training set, and predictions are generated for the testing set.

## Evaluation
The performance of the model is evaluated using metrics such as:
- Mean Absolute Percentage Error (MAPE)
- Mean Absolute Error (MAE)

These metrics help in understanding the accuracy of the sales forecasts.

## Usage
1. Clone the repository.
2. Install the required dependencies.
3. Run the `PROJECT2.ipynb` notebook in Jupyter or Google Colab.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
