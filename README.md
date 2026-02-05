# Market Sentiment vs Trader Behavior on Hyperliquid

## Objective
Analyze how Bitcoin market sentiment (Fear & Greed Index) influences trader behavior and performance on the Hyperliquid exchange.  
The goal is to uncover behavioral patterns that can inform smarter and more risk-aware trading strategies.

---

## Datasets
This project uses two datasets:

1. **Bitcoin Market Sentiment (Fear/Greed Index)**
   - Columns: `date`, `classification`
   - Sentiment classes: Extreme Fear, Fear, Neutral, Greed, Extreme Greed

2. **Hyperliquid Historical Trader Data**
   - Fields include: `Account`, `Coin`, `Side`, `Size USD`, `Closed PnL`, `Timestamp IST`, etc.
   - Trade-level data aggregated to daily trader metrics

---

## Methodology
1. Loaded and inspected both datasets (rows, columns, missing values, duplicates)
2. Converted timestamps and aligned both datasets at a daily level
3. Created trader-level daily metrics:
   - Daily PnL
   - Trade count per day
   - Win rate
   - Average trade size
   - Long/short ratio
4. Merged trader metrics with daily market sentiment
5. Compared performance and behavior across sentiment regimes
6. Visualized results using tables and charts

---

## Key Insights
- **Fear days are not less profitable**: Average daily PnL during Fear was higher than during Greed, suggesting volatility-driven opportunities.
- **Extreme Fear triggers overtrading**: Traders showed the highest trade frequency and strongest long bias, but with lower win rates.
- **Greed days offer higher win rates but capped profits**: Extreme Greed had the highest win rate, yet lower average PnL than Fear periods.

---

## Strategy Recommendations
- **Risk control during Fear**: Reduce leverage and avoid overtrading during Fear and Extreme Fear days to manage volatility.
- **Selective momentum trading during Extreme Greed**: Fewer, higher-confidence trades can benefit from trend continuation and higher win rates.

---

## Repository Structure
