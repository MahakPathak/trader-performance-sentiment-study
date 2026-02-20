# Trader Performance vs Market Sentiment Analysis (Fear vs Greed)

## 📌 Project Overview
This project analyzes how market sentiment (Fear vs Greed) affects trader behavior and performance using historical trading data and the Bitcoin Fear & Greed Index.  
The goal is to identify patterns in profitability (PnL), win rate, trading activity, and risk behavior under different sentiment regimes and generate actionable trading insights.

---

## 🎯 Objective
- Analyze trader performance under different market sentiments (Fear vs Greed)
- Study behavioral changes such as trade frequency, position size, and long/short bias
- Identify trader segments (frequent vs infrequent, consistent vs inconsistent)
- Provide data-driven strategy recommendations

---

## 📂 Datasets
Due to large file size, the datasets are hosted on Google Drive.

### 🔗 Download Links
- Historical Trader Data (Hyperliquid):  
  👉 [Download Dataset](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)

- Bitcoin Fear & Greed Sentiment Data:  
  👉 [Download Dataset](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)

### 📥 How to Use Datasets
1. Download both CSV files from the links above  
2. Place them in the same folder as the notebook  
3. Ensure filenames are:
   - `historical_data.csv`
   - `fear_greed_index.csv`

---

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## ⚙️ Installation & Setup

### Step 1: Clone the Repository
Run the following command in your terminal:

```bash
git clone https://github.com/MahakPathak/trader-performance-sentiment-study.git
```


### Step 2: Install Required Libraries
Before running the project, install all the required Python libraries using:
```bash
pip install pandas numpy matplotlib seaborn jupyter
```
---

## ▶️ How to Run the Project

### Option 1: Using Jupyter Notebook (Recommended)
1. Open the terminal in the project folder  
2. Run the following command:
```bash
jupyter notebook
```
3. Open the notebook file (.ipynb)
4. Click Kernel → Restart & Run All to execute all cells in order

### Option 2: Using VS Code
1. Open the project folder in VS Code
2. Open the notebook file (.ipynb)
3. Select a Python kernel
4. Run all cells from top to bottom


## 📁 Project Structure

```text
trader-performance-sentiment-study/
├── notebook.ipynb
├── historical_data.csv
├── fear_greed_index.csv
└── README.md
```

## Summary

### Methodology
The project started with loading and cleaning two datasets: historical trader data and the Fear & Greed sentiment dataset.  
Missing values and duplicates were checked to ensure data quality. Timestamps were converted to datetime format, and a common daily `date` column was created to align both datasets. After merging them on the daily level, key metrics such as daily PnL, win rate, average trade size, number of trades per day, and long/short ratio were calculated.  
Exploratory data analysis and visualizations were then performed to compare trader performance and behavior across different market sentiment regimes (Fear, Greed, Neutral). Trader segmentation was also done based on trade frequency, consistency (win rate), and risk (position size proxy).

### Insights
- Trader performance (PnL) varies across different sentiment regimes, with higher variability during Fear and Extreme Greed periods.  
- Trading activity increases during Fear and Extreme Fear conditions, showing that traders become more active in volatile markets.  
- Higher drawdowns are observed during extreme sentiment phases, indicating greater risk exposure alongside higher potential returns.  
- Trader behavior, including trade frequency, position size, and directional bias (BUY/SELL), changes based on market sentiment, confirming that market psychology influences trading decisions.  

### Strategy Recommendations
- During Extreme Fear and Extreme Greed periods, traders should reduce position size and manage risk carefully due to higher volatility and larger drawdowns.  
- Traders can increase trade frequency selectively during high-volatility sentiment phases (Fear) while avoiding overtrading during Neutral market conditions.  
- Frequent and high-risk traders should apply stricter risk management rules, as larger position sizes lead to higher PnL volatility and potential losses during emotionally driven markets.
