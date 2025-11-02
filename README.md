# Hybrid-Stock-Price-Prediction-using-LSTM-and-XGBoost

🧠 Overview

This project builds a hybrid AI model that predicts stock market price movements by combining two powerful machine learning techniques:

LSTM (Long Short-Term Memory) — learns time-based patterns and trends from sequential stock data.

XGBoost (Extreme Gradient Boosting) — refines predictions using additional technical indicators and features for better accuracy.

This hybrid approach captures both temporal dependencies (LSTM) and non-linear relationships (XGBoost) to improve decision-making for Buy/Sell predictions.

💾 About the Dataset

Dataset Name: Stock Market Dataset for AI-Driven Prediction and Trading Strategy Optimization
Format: CSV

Features include:
| Category             | Features                                 | Description                             |
| -------------------- | ---------------------------------------- | --------------------------------------- |
| Market Metrics       | `Open`, `High`, `Low`, `Close`, `Volume` | Daily trading activity                  |
| Technical Indicators | `RSI`, `MACD`, `Bollinger Bands`         | Trend and momentum indicators           |
| Sentiment            | `Sentiment_Score`                        | Market sentiment from news/social media |
| Macroeconomic        | `GDP_Growth`, `Inflation_Rate`           | Broader economic health                 |
| Target               | `Buy_Sell_Signal`                        | 1 = Buy, 0 = Sell                       |

🔄 Project Pipeline

📂 Load Dataset (CSV)
⬇️
🧹 Data Preprocessing & Scaling
⬇️
📈 Train LSTM Model → Extract Sequential Features
⬇️
🚀 Train XGBoost Model using LSTM output + Technical Features
⬇️
📊 Evaluate Model Performance
⬇️
💡 Predict Next-Day Buy/Sell Signal

🛠️ Technologies Used

Python 3.x

Libraries:

TensorFlow / Keras (for LSTM)

XGBoost

Scikit-learn

Pandas, NumPy

Matplotlib, Seaborn (for visualization)


📊 Model Evaluation

The model uses standard evaluation metrics:

Accuracy — how often the model predicts correctly

Precision, Recall, F1-score — classification quality

Confusion Matrix — detailed performance visualization

Example Output:
✅ Model Evaluation Results:
Accuracy: 0.79  
Precision: 0.82
Recall: 0.77
F1-Score: 0.79

💹 Model Suggests: BUY Tomorrow


🧩 How It Works (Real-Time Example)

Imagine you have today’s market data:
Open: 145.2, Close: 147.3, Volume: 2.5M, RSI: 65, Sentiment: 0.8
The model:

Uses LSTM to find temporal price trends.

Passes those features to XGBoost along with technical indicators.

Predicts:
→ BUY (probability 0.78)


🌟 Benefits

✅ Captures time-based trends and market patterns
✅ Integrates technical + sentiment indicators
✅ Produces actionable Buy/Sell signals
✅ Educational tool for learning financial ML systems

🚧 Future Improvements

Integrate real-time API data (e.g., Yahoo Finance, Alpha Vantage)

Use Reinforcement Learning for trade optimization

Add Deep Ensemble and Transformer-based models
