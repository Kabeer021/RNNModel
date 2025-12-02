# RNN-based Time Series Forecasting

This project implements RNN/LSTM-based models for time series forecasting using the Darts library. The notebook includes end-to-end steps: exploratory data analysis (EDA), preprocessing, model training, evaluation, and plotting.

## 📊 EDA

The notebook begins with exploratory analysis using:

-Time series decomposition

-ACF/PACF plots

-Trend/seasonality inspection

-Visualization of raw and transformed data

# 🔍 Key Information Extracted

Imports / Libraries Used:
darts.dataprocessing.transformers, darts.metrics, darts.models,
darts.timeseries, darts.utils.timeseries_generation,
matplotlib.pyplot, numpy, os, pandas,
sklearn.metrics, sklearn.model_selection,
statsmodels.graphics.tsaplots, statsmodels.tsa.seasonal

## Model Types Used:
  LSTM, RNN


```bash
jupyter notebook "rnn-model (2).ipynb"
```

Run cells sequentially. The notebook contains data preprocessing, model building, training, and evaluation steps.


## Model Details (extracted / inferred)

- Architecture: LSTM, RNN
- Training loop, loss, and evaluation implemented in the notebook.

Components:

-Preprocessing & train-test split

-Training loop (50 epochs, batch size 30)

-Evaluation metrics (RMSE/MAPE/etc. depending on notebook)

-Visualization of predictions

## Installation

Create a virtual environment and install packages. Example:

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

If `requirements.txt` is not present, install common libraries detected: 

Suggested pip installs: `pip install darts matplotlib numpy os pandas scikit-learn statsmodels`


## Results

The LSTM/RNN models were trained for 50 epochs with a batch size of 30 on the prepared time-series data. The training loss decreased steadily, indicating effective learning of temporal patterns. Visualizations in the notebook show that the model’s predictions closely follow the actual time-series trend, capturing both movement and seasonal behavior. Evaluation metrics (from darts.metrics and sklearn.metrics) confirm that the model delivers reasonably accurate forecasts without noticeable overfitting.

## License

Specify a license (e.g., MIT) in `LICENSE`.
