# 📊 Trader Performance vs Market Sentiment Analysis

## 📌 Objective

This project analyzes how market sentiment (Fear & Greed Index) influences trader behavior and profitability on Hyperliquid.
The goal is to uncover patterns in trading activity and generate actionable strategies to improve performance.

---

## 📂 Datasets

* **Bitcoin Fear & Greed Index** (daily sentiment classification)
* **Historical Trader Data** (transaction-level trading data)

---

## ⚙️ Methodology

### 1. Data Preparation

* Cleaned and audited datasets
* Converted timestamps to daily format
* Merged trader data with sentiment data

### 2. Feature Engineering

* Daily Net PnL (after fees)
* Trade count, total volume, average trade size
* Long/Short bias
* Fee ratio and PnL per trade

### 3. Exploratory Data Analysis (EDA)

* Compared profitability and win rate across sentiment phases
* Analyzed distribution of PnL using boxplots
* Evaluated mean vs median to detect outliers

### 4. Behavioral Segmentation

Traders were segmented into:

* **Scalpers** → High frequency, smaller trades
* **Whales** → Low frequency, large trades
* **Retail Traders** → Moderate behavior

### 5. Predictive Modeling 

* Random Forest Classifier used to predict profitability
* Features: sentiment value, trade_count, volume, fee_ratio
* Feature importance used to evaluate key drivers

---

## 📊 Key Insights

* Trading activity increases during **Extreme Fear**, indicating reaction to volatility
* Profitability tends to peak during **moderate Fear**, not extreme conditions
* **Execution behavior (trade frequency, fee efficiency)** impacts profitability more than sentiment alone
* PnL distribution shows high variability, meaning profits are often driven by a few large trades

---

## 🎯 Strategy Recommendations

### 1. Overtrading Alert (Greed Phase)

* Detect high activity + high fee_ratio
* Encourage trade consolidation to reduce costs

### 2. Risk Control for Retail Traders (Extreme Fear)

* Reduce position size during high volatility
* Limit exposure to downside risk

### 3. Execution Optimization

* Provide fee-awareness nudges
* Suggest optimal trading frequency
* Encourage efficient trade execution

---

## 🧠 Tech Stack

* Python (Pandas, NumPy)
* Data Visualization (Matplotlib, Seaborn)
* Machine Learning (Scikit-learn)

---

## ▶️ How to Run

1. Install dependencies:

```
pip install -r requirements.txt
```

2. Open the notebook:

```
analysis.ipynb
```

---

## 📈 Output

The notebook contains:

* Cleaned dataset
* Visualizations (barplots, boxplots, heatmaps, Time Trend)
* Insights and strategy recommendations

---


