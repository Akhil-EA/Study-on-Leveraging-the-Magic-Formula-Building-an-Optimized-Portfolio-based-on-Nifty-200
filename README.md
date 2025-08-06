# Study-on-Leveraging-the-Magic-Formula-Building-an-Optimized-Portfolio-based-on-Nifty-200
This repository showcases my internship project at Hedge Equities (2025), where I crafted an optimized investment portfolio based on the Nifty 200 Index. Conducted from May 12, 2022, to May 13, 2025, this project blends the Magic Formula for stock selection with Modern Portfolio Theory for optimization, achieving a robust risk-adjusted return.
Dubbed a "vibe coding project," the code was developed with assistance from a Large Language Model (LLM), making it a fun, AI-driven collaboration

**Run the sharpe ratio optimizer code to optimize the stocks of you choice using yfinance tickers**

**Project Details**

Stock price time Period: May 12, 2022 - May 13, 2025 (3 years)

**Methodology:**

Magic Formula: Selected 9 stocks (NMDC, Vedanta, Tata Motors, National Aluminium, Indus Towers, Hero Motocorp, Hindustan Zinc, ACC, Dr Reddy's Labs) with Earnings Yield > 7%, ROIC > 15%, and P/E < 20, sourced from Screener.in.

MPT Optimization: Implemented in Python using scipy.optimize.minimize (SLSQP) to maximize the Sharpe Ratio, utilizing 740 trading days of historical data from Yahoo Finance.

<img width="906" height="488" alt="image" src="https://github.com/user-attachments/assets/ab25b083-d1ac-4a48-888d-fd8d38fbd30a" />


**Performance Metrics:**

Annual Return: 26.84%
Annual Volatility: 17.87%
Sharpe Ratio: 1.1659 (with 6% risk-free rate)

**Optimized Weights:**

Tata Motors: 22.9%
Vedanta: 20.4%
National Aluminium: 18%
Indus Towers: 16.1%
ACC: 12.8%
Dr Reddy's Labs: 5.4%
Hindustan Zinc: 4.5%
Hero Motocorp: 0%
NMDC: 0%

**Why These Weights?**

High Weights (Tata Motors, Vedanta, National Aluminium, Indus Towers): These stocks drove the 26.84% return with returns of 29.48%, 32.92%, 21.61%, and 25.10%. Their volatilities (25.81%, 32.84%, 34.20%, 22.39%) were balanced by diversification, aided by correlations (e.g., 0.6325 for Vedanta-National Aluminium).

Zero Weights (Hero Motocorp, NMDC): Excluded due to high volatilities (25.07%, 33.59%) and correlations (0.3416 with Tata Motors, 0.5933 with Vedanta), which added risk without enough return.

ACC’s Higher Weight (12.8%): Despite a -0.48% return, its 0.4358 correlation with Indus Towers improved diversification, stabilizing the 17.87% volatility.

Lower Weights (Dr Reddy's Labs 5.4%, Hindustan Zinc 4.5%): Dr Reddy’s (35.93% return) and Hindustan Zinc (28.15% return) were limited by low correlations (0.1175 with ACC) and sector overlap (0.4715 with Vedanta), prioritizing portfolio balance.
