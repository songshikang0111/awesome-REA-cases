# Polymarket Up/Down bots: unverified REA replay and Claude-rebuild promotions

Category: Algorithms and feature recovery · REA
Record date: 2026-11-16
Stage: Needs verification

On October 16, @slash1sol first claims REA and Opus 5.5 inspected an unnamed $49/month Electron app, tracing Export from app.asar to file output, writing SPEC.md and building a version that passed its own tests, all in 41 minutes. That unnamed introduction is not independently accepted validation. The author then specifically reports analyzing a Polymarket Up/Down bot into a loop of pulling the order book, scoring price moves and triggering at 0.40, replaying against real fills tick by tick with @Poly_Historical's five-minute BTC, ETH and SOL historical Level-2 books and saying the strategy 'survived,' while promoting that data service. Bot identity, strategy source, replay body, sample period, trade count, costs, risk and returns are absent, and the 0.40 unit is unexplained.

At 17:59:00 Beijing time on October 31, 2026, Datafengyun (@Datafengyun) claims to have dissected a Polymarket trader's terminal and had Claude reproduce a BTC UP/DOWN 5MIN scalping bot with one prompt in 20 minutes. The described design takes Binance real-time prices and five-minute candles, cross-references TradingView and CryptoQuant, and uses a Mirofish force-directed graph of 100 nodes/180 edges to detect bull/bear clusters and CLOB lag exceeding 0.3% against spot. It claims execution within 100ms, more than 1,000 orders per second and 0.3%-0.8% per trade, listing 0.5% risk per trade, a 2% daily limit, a -0.4% hard stop, skipping weak opportunities and local operation without a GPU. These are promotional design statements or claims, with no source, fill receipts, latency measurements or risk-control tests obtained. The story of $0.90 becoming $408,292 in two days concerns the studied account, not the new bot's returns, and is not independently verified account performance.

At 23:15:04 on November 16, Barnabus Notes (@BarnabusBull) says three weeks were spent studying a Polymarket bot that buys both UP and DOWN when their combined price is below $1, skipping gaps that do not cover fees. An example quotes $0.50 plus $0.47 at 11:07 and 3,860 shares on each side. The post says the operator built the bot by describing it to AI, not that AI performed this three-week reversal; no model or REA evidence is supplied. A claimed $3,231 daily profit, 38 locks, 81% hit rate, one losing window and nine misses are promotional account claims, not returns of new code or audited records.

The new post equates two fill-or-kill orders with 'both fill or neither does' without an atomic paired-order mechanism or fill records. Per-order FOK alone does not guarantee both orders succeed together; fees, slippage, leg exposure, settlement and execution risks are not eliminated by the promotion. The $0.97 quotation example does not prove locked net profit. Account identity, on-chain fills and the full build material were not obtained.

Lookup confirms the new author's identity and full text, not the video or identity behind account short links. These reports are retained together for the Up/Down strategy-research direction; they are not established as the same trader, bot or implementation. The latter two posts do not inherit the earlier REA attribution. The October 31 post also recommends Polycop copy trading and has a promotional context. Self-tests, reconstruction time, metrics, risk parameters and 'survived' do not establish live profits or safety and are not investment advice. No orders, bot execution or strategy replay occurred here.

Earlier post: October 16, 2026 at 19:00 Beijing time; then-snapshot: 44 likes, 543 views, 1 repost. Engagement proves neither replay results nor profit.
October 31 candidate: 1 like, 39 views, 0 reposts. 20 minutes, 100ms and returns are unverified; studied-account returns must not be confused with new-bot returns.
November 16 candidate: 11 likes, 57 views, 0 reposts, 1 reply. Three weeks, $3,231, 38 locks and 81% are author reports; FOK does not establish paired atomicity.

## Sources

- [@slash1sol's REA strategy-analysis and data-service promotion](https://x.com/i/status/2111049696630194596)
- [Datafengyun's Claude five-minute BTC bot-rebuild promotion, October 31, 2026](https://x.com/i/status/2116469981395439893)
- [Barnabus Notes' Up/Down paired-bot reversal and AI-build claim, November 16, 2026 at 23:15:04 Beijing time](https://x.com/i/status/2122347730408296832)

[中文](../polymarket-updown-rea-replay-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
