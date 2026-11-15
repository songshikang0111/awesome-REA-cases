# Polymarket five-minute BTC: Misato reports rebuilding momentum and semivariance rules with Grok Bot

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-16
Stage: Needs verification

At 00:09:29 Beijing time on November 16, 2026, Misato (@misat0x) says they observed a public Polymarket account and worked with Grok Bot to infer trading logic for five-minute BTC markets. They claim the account made $148,420 over 94 days, averaging about $84 per trade and repeating over 30 times hourly, but provide no account address or ledger. Neither the returns nor the strategy's identity are authenticated.

The reconstructed scheme uses BTC's percentage change against its price 30 seconds earlier as momentum, separately sums squared positive and negative returns, and defines Skew as (up variance minus down variance)/(up variance plus down variance). It triggers only when both signals point the same way. Skew is the author's semivariance-asymmetry label, not recovered original bot source, and no evidence establishes an executable advantage ahead of the order book. Grok Bot is not assumed to be a particular official product or model version; REA is unmentioned.

The author reports a seven-day paper desk scanning 1,420 five-minute windows, with 84 triggered trades, 68 wins and 16 losses, a claimed 80.9% win rate, $3,840 simulated profit at fixed $100 sizing and a worst daily loss of $42.10. They say fees caused losses before the filter, which allegedly removed 94% of bad entries. Timestamps, fill simulation, fee/slippage treatment, raw logs and code are absent. All figures are attributed, not calculations or live returns verified here. Original-post retrieval confirms attribution and wording only; the video was not watched, no strategy run, wallet connected or order placed, and no return guarantee is made.

Sealed candidate: 9 likes, 459 views, 1 repost, 3 replies. Returns and filter effects are unaudited.

## Sources

- [Misato's momentum/Skew reconstruction and seven-day simulation report, November 16, 2026 at 00:09:29 Beijing time](https://x.com/i/status/2121999035582263521)

[中文](../misato-grok-polymarket-momentum-semivariance-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
