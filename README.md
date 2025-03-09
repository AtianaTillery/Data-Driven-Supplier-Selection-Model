# Data-Driven Supplier Selection Model

## Project Overview
This project demonstrates how to use machine learning techniques to rank suppliers based on key procurement metrics such as cost, reliability, and delivery time. The goal is to help businesses optimize their supplier selection process by providing data-driven rankings.

In this model, a **Random Forest Classifier** is used to predict the ranking of suppliers based on their historical performance in terms of cost, reliability, and delivery time.

## Features
- **Data Collection**: The project uses a synthetic dataset that includes data on suppliers' costs, reliability, and delivery times.
- **Data Preprocessing**: The dataset is cleaned and normalized for better machine learning performance.
- **Model**: A Random Forest Classifier is trained on the dataset to predict supplier ranks.
- **Visualization**: Feature importance and predicted vs actual ranks are visualized to evaluate the model's performance.

## Objective
The primary objective of this project is to build a model that ranks suppliers based on the following factors:
- **Cost**: The price per unit for each supplier.
- **Reliability**: The reliability of the supplier in terms of on-time deliveries and overall quality.
- **Delivery Time**: The average delivery time for each supplier.

## Steps in the Project

### 1. **Data Collection**
   A synthetic dataset is used, which includes the following columns:
   - `Supplier`: The name of the supplier.
   - `Cost`: The price per unit of the product.
   - `Reliability`: The reliability score, indicating the percentage of on-time deliveries.
   - `Delivery Time`: The average number of days taken for delivery.

### 2. **Data Preprocessing**
   - Missing values are handled by filling them with the mean value of the respective column.
   - The features (`Cost`, `Reliability`, `Delivery Time`) are normalized using the Min-Max scaling technique.

### 3. **Model Training**
   A **Random Forest Classifier** is used to train the model on the preprocessed data. The model predicts the rank of each supplier (1 to 5) based on the given features.

### 4. **Model Evaluation**
   The model's performance is evaluated using a classification report, which includes metrics such as precision, recall, and F1-score.

### 5. **Visualization**
   - **Feature Importance**: A bar chart is displayed to show how each feature (Cost, Reliability, Delivery Time) impacts the model's predictions.
   - **Predicted vs Actual Rank**: A comparison between predicted and actual ranks for the suppliers is visualized using a bar chart.

## Requirements

Before running the project, you need to install the following Python packages:

- `pandas`: For data manipulation and analysis.
- `scikit-learn`: For machine learning algorithms and preprocessing.
- `matplotlib`: For data visualization.

You can install these dependencies using pip:

```bash
pip install -r requirements.txt
