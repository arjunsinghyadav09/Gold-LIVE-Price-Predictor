# Project 1: XAUUSD Simple Gold Price Direction Predictor

A beginner-friendly ML pipeline that predicts whether Gold will go UP or DOWN the next day.

## What it does
- Loads historical XAUUSD OHLCV data
- Engineers 25 technical indicator features (RSI, MACD, Bollinger Bands, ATR, etc.)
- Trains a **Random Forest Classifier** with chronological train/test split
- Evaluates with accuracy, precision, recall, confusion matrix
- Saves a 4-panel analysis chart

## Run it
```bash
pip install yfinance pandas numpy scikit-learn matplotlib
python gold_price_predictor.py
```

## For live data, replace the CSV loader with:
```python
gold = yf.download("GC=F", start="2018-01-01", end="2024-12-31")
```

## Tech stack
`Python` · `pandas` · `numpy` · `scikit-learn` · `matplotlib` · `yfinance`
