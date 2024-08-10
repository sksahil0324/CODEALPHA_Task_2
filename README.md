# CODEALPHA_Task_2
Here's the updated README file with the additional details:

---

# STOCK MARKET PREDICTION

**Author:** Sahil Basheer Shaik  
**Organization:** CODEALPHA  
**Batch:** JULY  

This project implements a Long Short-Term Memory (LSTM) neural network for predicting stock prices. The model is trained and evaluated on historical stock price data to forecast future prices.

## Table of Contents

- [Overview](#overview)
- [Dependencies](#dependencies)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [License](#license)

## Overview

This project uses an LSTM network to predict stock prices based on historical closing prices. The model is trained using historical data and evaluated to check its performance.

## Dependencies

Ensure you have the following Python libraries installed:

- numpy
- pandas
- sklearn
- matplotlib
- torch

You can install the required libraries using pip:

```bash
pip install numpy pandas scikit-learn matplotlib torch
```

## Dataset

The dataset used is `netflix.csv`, which contains historical stock prices for Netflix. The CSV file should include a column named `Close` representing the closing prices.

## Model Architecture

The LSTM model consists of:

- An LSTM layer with 64 hidden units.
- A fully connected (linear) layer that outputs the predicted price.

## Training

The model is trained for 100 epochs with a batch size of 1. The Mean Squared Error (MSE) is used as the loss function, and the Adam optimizer is used for training.

## Evaluation

The model's predictions are compared against the actual stock prices. The results are visualized in a plot showing the predicted prices (in red) and the real prices (in green).

## Usage

1. Place the `netflix.csv` file in the same directory as the script.
2. Run the script in a Jupyter Notebook or a Python environment.

```python
# Run the script
python lstm_stock_prediction.py
```

The script will output the training loss at every 10 epochs and display a plot of the predicted vs. real stock prices.
