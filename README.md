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
