# Oil Temperature Forecasting Project

## Project Overview
This project aims to forecast the oil temperature (OT) of electricity transformers for the next 24 hours using a machine learning model (XGBoost). The goal is to predict OT with high accuracy to help manage the load on transformers, prevent damage, and optimize energy distribution.

## Project Structure
The project is organized into the following files:
- `Oil_Temperature_Forecasting_Project.ipynb`: The main script containing the code for data preprocessing, feature engineering, model training, and evaluation.
- `train.csv`: The training dataset containing historical data on oil temperature and related features.
- `test.csv`: The test dataset used to evaluate the model's predictions.
- `README.md`: This documentation file.
- `requirements.txt`: A list of dependencies required to run the project.

## Assumptions
The project is based on the following assumptions:
- **No Pre-trained Models**: The XGBoost model is trained from scratch on the provided dataset.
- **No AI Models**: Traditional machine learning models were used instead of AI models.
- **Data Preprocessing**: The dataset is assumed to be clean with minimal missing values, and any missing values are handled using forward filling (`ffill`).
- **Feature Engineering**: Time-based features such as `hour`, `day_of_week`, and `month` are extracted from the `date` column. Lag features are created for the target variable `OT` to capture temporal dependencies.

## Usage
1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/yourusername/oil-temperature-forecasting.git
    cd oil-temperature-forecasting
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the `main.py` script to train the model and make predictions:
    ```bash
    python main.py
    ```

4. The script will output the model evaluation metrics and plot the predicted oil temperature for the next 24 hours.

## Results
The XGBoost model achieved the following evaluation metrics:
- **Mean Absolute Error (MAE):** 0.2967
- **Root Mean Squared Error (RMSE):** 0.4546
- **R-squared (R²):** 0.9971
- **Mean Absolute Percentage Error (MAPE):** 3.59%

These results demonstrate that the model provides highly accurate forecasts of oil temperature.

## Future Work
- **Hyperparameter Tuning**: Further tuning of the XGBoost model could improve performance.
- **Exploration of Other Models**: Consider testing other models like LightGBM or CatBoost.
- **Feature Engineering**: Additional features or time-series-specific transformations could enhance model accuracy.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
