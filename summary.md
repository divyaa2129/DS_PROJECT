# Market Sentiment vs. Trader Behavior on Hyperliquid

## Methodology
This analysis uses two primary datasets: the Bitcoin Fear & Greed market sentiment index and historical trade-level data from the Hyperliquid exchange.

The workflow began with basic data cleaning, including checks for missing values and duplicate records. All timestamp fields were converted into a standardized datetime format to ensure proper alignment between datasets.

Next, raw trade data was aggregated at a daily level for each trader account. This aggregation enabled the calculation of key performance and behavioral metrics such as daily PnL, trade frequency, win rate, average trade size, and long/short ratio.

These daily trader metrics were then merged with corresponding daily market sentiment labels, ranging from Extreme Fear to Extreme Greed. Finally, comparative analysis and visualizations were used to evaluate how trader behavior and performance changed across different sentiment regimes.



## Key Insights

**Fear is actually profitable**  
Average daily PnL during Fear and Extreme Fear periods was higher than during Greed regimes. This suggests that increased volatility in fearful markets can create stronger profit opportunities for traders who remain disciplined.

**Extreme Fear leads to overtrading**  
During Extreme Fear, traders significantly increased their trade frequency and showed a strong long bias. However, win rates declined, indicating emotionally driven behavior such as overtrading or attempting to time market bottoms.

**Greed has high win rates but lower returns**  
Extreme Greed periods exhibited the highest win rates, but overall profitability was lower than during Fear regimes. This implies that while trades are easier to win, price movements are smaller or most of the upside has already occurred.



## Strategy Recommendations

**Manage risk during Fear regimes**  
During Fear and Extreme Fear conditions, traders should reduce leverage and limit excessive trade frequency. High volatility increases opportunity but also amplifies downside risk if discipline is lost.

**Be selective during Extreme Greed**  
In Extreme Greed environments, focusing on fewer, high-confidence momentum trades is preferable. Higher win rates can be leveraged effectively when combined with controlled position sizing and patience.
