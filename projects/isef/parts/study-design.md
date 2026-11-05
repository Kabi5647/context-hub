# Study design

## Draft approach

- Use aligned daily adjusted prices and calculate returns. A five-trading-day absolute move of at least 10% is a proposed event definition. Choose the final definition, overlap handling and cooldown in advance.
- Estimate correlations over a window that ends before the event starts. A 126-trading-day lookback was suggested for a pilot.
- Measure responses for all comparison stocks, including small or zero moves. Compare stronger and weaker prior connections, control for broad-market moves, and include ordinary periods. Record concurrent shocks and keep event-period returns separate from subsequent returns.
- Start with returns, mean, variance, covariance and correlation. Then work through weighted networks, node strength and a simple market regression. Study network amplification with small synthetic examples if it adds a clear mathematical contribution.
- Separate method development from holdout evaluation. Shared news and sector exposure can create correlated responses, so describe conclusions as association unless the design supports more.
