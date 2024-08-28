# Oil Temperature Forecasting Project

## Project Overview
This project aims to forecast the oil temperature (OT) of electricity transformers for the next 24 hours using machine learning models. The primary model used is XGBoost, a gradient boosting algorithm, known for its accuracy and performance on structured data.

## Project Structure
- `train.csv`: The training dataset containing historical data on oil temperature and related features.
- `test.csv`: The test dataset for which predictions are to be made.
- `Oil_Temperature_Forecasting_Project.ipynb`: The main script containing the data preprocessing, feature engineering, model training, and evaluation code.
- `README.md`: This documentation file.
- `requirements.txt`: A list of dependencies required to run the project.

## Dependencies
To run the project, you need the following Python packages:
- `pandas`
- `numpy`
- `scikit-learn`
- `xgboost`
- `matplotlib`
- `seaborn`

You can install these dependencies using the following command:
```bash
pip install -r requirements.txt
