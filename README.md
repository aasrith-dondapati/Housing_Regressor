# Housing Price Regression Project

This project uses different machine learning models to predict house prices based on features like size and location. It also includes a web app for users to get price estimates.

## Project Structure

- `app.py`: Flask web application for the user interface
- `model.py`: Contains model training and evaluation code
- `templates/`: Directory containing HTML templates for the web interface
- Various `.pkl` files: Trained model files
- `USA_Housing.csv`: Dataset containing house price information

## Setup Instructions

1. Clone the repository:

```bash
git clone [repository-url]
cd Housing_Regressor
```

2. Install required dependencies:

```bash
pip install -r requirements.txt
```

## Step-by-Step Process

### 1. Data Preparation

- The dataset is loaded from `USA_Housing.csv`
- Features include:
  - House area
  - Number of bedrooms
  - Number of bathrooms
  - Number of stories
  - Year built
  - Price (target variable)

### 2. Model Training

The project implements multiple regression models:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Elastic Net
- Polynomial Regression
- Robust Regression
- SGD Regressor
- Random Forest
- XGBoost
- LightGBM
- SVM
- KNN
- Artificial Neural Network (ANN)

Each model is trained and saved as a `.pkl` file for later use.

### 3. Model Evaluation

- Models are evaluated using various metrics:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - R-squared Score
- Results are saved in `model_evaluation_results.csv`

### 4. Web Interface

The project includes a Flask web application that allows users to:

1. Input house features
2. Select a regression model
3. Get price predictions

### 5. Running the Application

1. Start the Flask server:

```bash
python app.py
```

2. Open a web browser and navigate to `http://localhost:5000`
3. Enter the house features and select a model
4. Click "Predict" to get the estimated house price

## Model Selection

Choose the model based on your needs:

- For quick predictions: Linear Regression, Ridge, or Lasso
- For better accuracy: Random Forest, XGBoost, or LightGBM
- For complex patterns: Polynomial Regression or ANN
