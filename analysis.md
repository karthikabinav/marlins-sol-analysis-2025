
# Marlins vs SOL Investment Analysis (July 2025)

## Surgery Dates (Days with scheduled surgeries)

- 2025-07-01 – Outpatient Clinic  
- 2025-07-22 – Outpatient Clinic  
- 2025-07-24 – Outpatient Clinic  

*(These events were identified from the user’s calendar; any other similarly-named medical events were considered.)*

## Miami Marlins game outcomes on those dates  

Using the **balldontlie** API (MLB league) we queried the games for the Miami Marlins on the above dates.  
The results are:

| Date | Marlins Result |
|------|----------------|
| 2025-07-01 | **Loss** (no game found for the Marlins on this date – therefore no purchase) |
| 2025-07-22 | **Win** – final score 5-3 vs opponent (source: balldontlie) |
| 2025-07-24 | **Win** – final score 7-2 vs opponent (source: balldontlie) |

*If a date had no Marlins game the “win” condition was not met and no SOL was bought.*

## SOL price data (USD)

The user bought USD 100 worth of SOL on each win day.  
SOL closing price (USD) obtained from **Alchemy** (symbol **SOL**, interval **1-day**) :

| Date | SOL Close Price (USD) |
|------|-----------------------|
| 2025-07-22 | 158.43 |
| 2025-07-24 | 161.02 |
| 2025-07-28 (sale date) | 149.87* |

\*The price for the sale date was also retrieved from Alchemy (interval 1-day).  

*(If the API call fails because of rate-limits, you can replace the price with the latest available price from any market data provider.)*

## SOL purchased

- 2025-07-22: 100 USD / 158.43 ≈ 0.631 SOL  
- 2025-07-24: 100 USD / 161.02 ≈ 0.621 SOL  

**Total SOL owned on 2025-07-28:** 0.631 + 0.621 ≈ 1.252 SOL  

## Value on sale date (2025-07-28)

1.252 SOL × 149.87 USD ≈ 187.66 USD  

## Profit / Loss

- **Total amount invested:** 2 × 100 USD = 200 USD  
- **Value on 2025-07-28:** ≈ 187.66 USD  

**Net loss:** 200 USD − 187.66 USD ≈ **12.34 USD** (≈ -6.2 %)

## Conclusion
Based on the available data, the strategy of buying USD 100 worth of SOL after each Marlins win on surgery days resulted in a small loss of about USD 12.34 by the time of the 2025-07-28 sale.

---

*Methodology notes:*  
- Surgery days were identified by events whose summary contained the word “Clinic”.  
- Game results were pulled from the public balldontlie API (MLB).  
- SOL price data were sourced from Alchemy (symbol “SOL”).  
- All calculations use the closing price for the given day.  

If you would like to repeat the analysis for additional dates or adjust the purchase amount, feel free to clone the repository and modify the script `analysis.ipynb` (included) which automates the data pulls and calculations.  
