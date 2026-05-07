# BLD-001 - Daily Reversal Strategy

This notebook accompanies a PortfolYou_AI Build Log video.

The idea is intentionally simple:

- If yesterday's log return was negative, the strategy is long today.
- If yesterday's log return was positive, the strategy is short today.
- If no valid lagged return exists, the strategy stays flat.

The notebook tests the rule on Ethereum and selected cross-asset proxies, then adds
benchmark comparisons, risk metrics, transaction-cost stress tests, out-of-sample checks,
yearly regime checks, and a cross-asset comparison.

## Open in Google Colab

```text
https://colab.research.google.com/github/teomancan/portfolyou-ai-notebooks/blob/main/BLD-001-daily-reversal-strategy/BLD-001_daily_reversal_strategy.ipynb
```

## Data Source

The notebook uses Yahoo Finance data through `yfinance`.

## Important Limits

This is not a trading signal. It is a research notebook. Results depend on the sample
period, data source, cost assumptions, execution assumptions, and selected assets.
The cost model is intentionally simplified and does not fully model real spreads,
slippage, funding, derivatives, taxes, shorting constraints, or exchange-specific fees.
