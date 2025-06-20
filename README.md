![MIT License](https://img.shields.io/badge/license-MIT-green)
# Tesla Stock Sentiment Predictor 🚗📈

This project uses Reddit sentiment from r/wallstreetbets to predict the movement of Tesla (TSLA) stock for the next trading day.

## How it Works
1. **Data Collection**
   - Pulls TSLA stock price data using `yfinance`
   - Scrapes recent Reddit posts about "Tesla" using `praw`

2. **Sentiment Analysis**
   - Applies VADER sentiment analysis to Reddit titles

3. **Machine Learning**
   - Trains a Random Forest model to predict if Tesla stock will go up or down the next trading day based on average Reddit sentiment

## Example Output

```
📅 Tomorrow's Trading Day: 2025-06-18
📈 Prediction for 2025-06-18: 🔺 UP
```

##  Files
- `TeslaSentimentPredictor.ipynb` — Main notebook with data, ML, and prediction
- `requirements.txt` — All necessary Python packages
- `prediction_log.csv` — Daily sentiment & prediction history

## Installation

Install dependencies using pip:

```bash
pip install yfinance pandas matplotlib praw vaderSentiment scikit-learn nltk
```

Also run this in Python once:

```python
import nltk
nltk.download('vader_lexicon')
```

## Future Improvements
- Add LSTM deep learning model
- Pull more granular Reddit data (e.g., comments)
- Integrate with a daily auto-scheduler

## 👩‍💻 Author
Created by [@BadFinancial1367](https://www.reddit.com/user/BadFinancial1367)
