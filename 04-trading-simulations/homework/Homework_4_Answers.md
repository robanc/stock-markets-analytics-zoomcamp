# Module 4 Homework — Trading Simulations (2026)

## Question 1 — Less Features is More
- Features: 208 (reduced from 301)
- Predictor: `pred10_rf_best_rule_55`
- CAGR multiplier: **1.135949**
- Annualized growth: **13.59%**

## Question 2 — Most Efficient Random Forest Decision Rule
- Best threshold with fewer than 5 average trades per active day: **0.56**
- Average trades per active day: 4.401667
- CAGR multiplier: 1.117791

## Question 3 — Redefining the Growth Target
- New positive-growth target: `growth_future_30d > 1.022`
- Predictor: `pred5_clf_10`
- Number of trades: **7,337**
- Multiple-choice selection: **7**
- Average trades per active day: 8.009825
- CAGR multiplier: 1.121926

## Question 4 — Ideal Trading Strategy

My ideal trading strategy would combine predictions from the Random Forest and Decision Tree models to identify stocks with the strongest potential for positive returns. I would prioritize stocks where both models predict growth, using a Random Forest probability threshold of at least 0.56.

I would select a maximum of 3–5 stocks per day, rank them by prediction confidence, and allocate my available investment capital equally among them. To manage risk, I would diversify across stocks, limit exposure to any single position, and use predefined stop-loss rules. I would also account for transaction fees and evaluate the strategy using CAGR, maximum drawdown, and risk-adjusted returns through backtesting before investing real money.

This strategy is exploratory and has not yet been independently backtested.