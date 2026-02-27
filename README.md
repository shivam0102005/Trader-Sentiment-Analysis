# Trader Behavior vs Market Sentiment Analysis

## 📌 Overview

This project analyzes how Bitcoin market sentiment (Fear vs Greed Index) influences trader behavior and profitability on Hyperliquid.

The objective is to identify sentiment-driven performance patterns and derive actionable trading strategy insights.

---

## 🎯 Objective

To determine whether market sentiment affects:

- Daily Profit & Loss (PnL)
- Trade win rate
- Risk participation (position sizing)
- Trading activity levels
- Volatility patterns

---

## 📊 Methodology

1. **Data Cleaning**
   - Checked for missing values and duplicates
   - Converted timestamps to daily level
   - Validated dataset integrity

2. **Feature Engineering**
   - Daily PnL aggregation
   - Win rate calculation
   - Trade count per day
   - High Risk Participation Ratio (based on trade size quantiles)
   - 7-day rolling PnL volatility

3. **Sentiment Alignment**
   - Merged daily trading metrics with Fear/Greed classification
   - Compared regime-based performance

4. **Segmentation Analysis**
   - Risk-based segmentation (Low Risk vs High Risk)
   - Activity segmentation (Low Activity vs High Activity)
   - Sentiment-activity interaction analysis

---

## 📈 Key Insights

- **Greed regimes increase profitability**, but also expand leverage participation.
- **High-risk trade participation rises significantly during Greed periods.**
- **Fear regimes amplify downside risk**, particularly for aggressive traders.
- **High trading activity magnifies sentiment-driven performance swings.**
- Volatility clusters around extreme sentiment regimes.

---

## 🎯 Strategy Recommendations

1. Reduce leverage exposure during Fear regimes.
2. Cap high-risk participation during extreme Greed periods.
3. Apply volatility filters for high-frequency trading days.
4. Implement sentiment-aware dynamic risk management.

---

## 🛠 Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📂 Project Structure
Trader_Sentiment_Analysis/
│-fear_greed_index.csv
|-historical_data.csv
├── outputs/
│   ├── pnl_by_sentiment.png
│   ├── winrate_by_sentiment.png
│   ├── risk_ratio.png
│   ├── activity_heatmap.png
│
├── analysis.ipynb
├── README.md


✅ 📌 How to Run This Project
## ▶️ How to Run This Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/shivam0102005/Trader-Sentiment-Analysis.git
cd Trader-Sentiment-Analysis


2️⃣ Create a Virtual Environment (Recommended)

Using Anaconda:
create a new environment
conda create -n trader_env python=3.10
conda activate trader_env
3️⃣ Install Required Libraries
pip install pandas numpy matplotlib seaborn

4️⃣ Ensure Dataset Placement
Make sure the following files are inside the project folder:
historical_data.csv
fear_greed_index.csv
5️⃣ Run the Notebook
Start Jupyter Notebook:
jupyter notebook
open:
analysis.ipynb

Runs all cells sequentially

📊 Output

The notebook will:

Clean and aggregate trading data
Merge sentiment classification
Generate performance metrics
Produce visualizations
Provide regime-based insights
Suggest strategy recommendations


---



## ⚙️ Project Requirements

- Python 3.9+
- Pandas
- NumPy
- Matplotlib
- Seaborn


