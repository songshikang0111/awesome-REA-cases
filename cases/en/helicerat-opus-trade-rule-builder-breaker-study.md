# Inferring SPY trading rules: helicerat's Opus builder/breaker challenges a 100% historical fit

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-11
Stage: Analysis test

At 02:08:04 Beijing time on November 11, 2026, helicerat (@helicerat0x) describes Claude Code and Opus 5.5 inferring decision rules from trade records and then trying to falsify them. The author says an initial reconstruction matched every historical trade but lost money for three months live, prompting a builder/breaker setup. This does not reverse trading-platform software or establish recovery of a trader's actual hidden algorithm.

The full post says the builder fits minimal entry/exit rules with at most one filter, while the breaker attacks unseen years and ETFs including QQQ and IWM. The example fits monthly SPY records from 1994–2012 after sealing 2013 onward to avoid future leakage from random month splits. Every test goes into research.md first; only a code harness may produce numbers, rather than agents inventing a Sharpe ratio. The author reports a three-feature rule matching 100% of old decisions and 84% of sealed ones. This is a fit decline, not return or win probability.

The final claimed rule holds SPY above its ten-month average price and cash below it. The author claims a 52% maximum decline for holding SPY since 1994 versus 18% for the rule. Full-text retrieval confirms those statements, not the linked article, agent files, prices, trades, backtest code or logs. Dividends, fees, slippage, drawdown definitions and actual advance sealing remain unchecked. All figures, the three-month live loss and the workflow are author reports, not profit guarantees or investment advice. REA is not named; no backtest or trade was run here.

Sealed snapshot: 13 likes, 393 views, 0 reposts. The 100%/84% figures are claimed rule-fit rates; 52%/18% are unchecked drawdowns, not interchangeable profit metrics.

## Sources

- [Candidate and full-text retrieval: helicerat's Opus builder/breaker rule inference and sealed testing, November 11, 2026 at 02:08:04 Beijing time](https://x.com/i/status/2120216937653260468)

[中文](../helicerat-opus-trade-rule-builder-breaker-study.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
