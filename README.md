# OHLC Model - TCN Deep Learning Model

A Temporal Convolutional Network (TCN) based deep learning model for time series forecasting with OHLC (Open, High, Low, Close) stock market data.

## Project Structure

```
ohlc_model/
├── code/
│   └── TCN_deep_learning_model.ipynb   # Main TCN model implementation
├── preprocessed_data/                   # Processed datasets
├── raw_data/                            # Raw input data
└── nifty_50_historical_data.csv        # Nifty 50 historical data
```

## Features

- Temporal Convolutional Network (TCN) architecture for time series forecasting
- OHLC data processing and normalization
- Nifty 50 stock index forecasting
- Model training and evaluation
- Trained model weights (`tcn_nifty_model.h5`)

## Requirements

- Python 3.7+
- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## Installation

```bash
pip install -r requirements.txt
```

## Usage

Open the Jupyter notebook to train and evaluate the model:

```bash
jupyter notebook code/TCN_deep_learning_model.ipynb
```

## Model

The TCN model uses dilated convolutions to capture long-range dependencies in time series data, making it effective for OHLC price forecasting.

## Author

Your Name

## License

MIT License

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests.
