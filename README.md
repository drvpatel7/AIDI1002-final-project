# Time Series Forecasting – Airline Passenger Prediction using LSTM

## Project Overview

**Dataset Used:**  
  Airline Passengers Dataset  
  [https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv](https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv)

**Inspiration Source (Tutorial):**  
  Jason Brownlee's Time Series Forecasting with LSTM  
  [https://machinelearningmastery.com/time-series-prediction-with-deep-learning-in-python-with-keras/](https://machinelearningmastery.com/time-series-prediction-with-deep-learning-in-python-with-keras/)

## Files in This Repository

| File | Description |
|------|-------------|
| `stacked_lstm_regression.ipynb` | Original reference notebook from tutorial |
| `AIDI_1002_Final_Project_Template.ipynb` | Our modified notebook with implemented changes and results |
| `README.md` | Project summary and instructions |
| *(Optional)* `airline-passengers.csv` | Dataset (if needed offline) |


## Our Contribution (Changed Model Parameters)

We selected Option A: **Change Model Parameters** and made the following improvements to the LSTM architecture:

- Increased the first LSTM layer size from 50 to **128 units**
- Added a second LSTM layer with **32 units**
- Included **Dropout layers** after each LSTM for regularization
- Changed the **learning rate** to `0.01` for faster convergence
- Used `batch_size = 32` and applied **EarlyStopping** with a patience of 15 epochs

## Results Summary

| Dataset     | RMSE  | MAE   |
|-------------|-------|-------|
| Train       | 37.48 | 28.12 |
| Validation  | 56.50 | 43.26 |
| Test        | 92.04 | 68.21 |

The model performed well on training and validation data. Although test performance was lower, the structure demonstrated the ability to learn time series patterns effectively.


## How to Run the Notebook

You can run this project using [Google Colab](https://colab.research.google.com/) or locally with Jupyter:

1. Open `AIDI_1002_Final_Project_Template.ipynb`
2. Run all cells from top to bottom
3. No need to upload the dataset — it's loaded directly from the provided public URL
4. Output includes loss plots, MAE, and forecast vs. actual visualizations

## Team Members

- **Dhruvkumar Patel ,Student ID:- 200624542**
- **Neel Chandreshkumar Patel ,Student ID:- 200628032**

## Submission Details

- **Course:** AIDI 1002 – Machine Learning Programming  
- **Instructor:** Garima Malik 
- **Term:** Summer 2025  
- **Institution:** Georgian College  
- **Project Option:** Change Model Parameters
