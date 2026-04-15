# telegram:@DisterX

> Ingested: 2026-04-15 · Source: telegram:@DisterX

## Extracted Facts

- **fact** (high): KPIs displayed on the dashboard: Total Equity, P&L vs Deposit, BANAL bucket, PMM bucket, Open Positions, Win Rate, Stellar MM spread, Free USDC. [dashboard, metrics]
- **fact** (high): The live dashboard updates daily at 09:00 MSK and pulls data from data/trading-model-v0.3.json. [dashboard, infrastructure]
- **decision** (medium): v0.5 (upcoming) will add snapshot history and a public chronology. [roadmap, versioning]
- **decision** (medium): v0.4 (upcoming) will add realized/unrealized P&L separation and a settled trades log. [roadmap, versioning]
- **fact** (high): v0.3 was released on 2026-04-02, delivering a live dashboard with auto-population, daily cron job, and equity trend tracking. [roadmap, versioning]
- **fact** (high): v0.2+ was released on 2026-03-22, adding BANAL/PMM split and 27 tracked positions. [roadmap, versioning]
- **fact** (high): v0.2 was released on 2026-03-15, delivering a live model with data: JSON, positions, and aggregate equity. [roadmap, versioning]
- **fact** (high): v0.1 was released on 2026-03-12, delivering the model framework: obligations, allocation, positions, and formulas. [roadmap, versioning]
- **decision** (high): RedFlags table schema: severity, scope, message, status. [schema, database]
- **decision** (high): Snapshots table schema: as_of, equity_usd, realized_pnl, unrealized_pnl, total_pnl. [schema, database]
- **decision** (high): Positions table schema: market_slug, strategy_bucket, side, qty, avg_entry, mark_price, current_value_usd. [schema, database]
- **decision** (high): Allocations table schema: mandate_id, free_cash_usd, open_orders_usd, positions_cost_usd, equity_usd, pnl_usd. [schema, database]
- **decision** (high): Mandates table schema: mandate_id, token, nominal_usd, strategy_type, venue. [schema, database]
- **decision** (high): The database schema is Grist-ready and includes five tables: Mandates, Allocations, Positions, Snapshots, and RedFlags. [schema, database]
- **decision** (high): Realized and unrealized P&L must be tracked separately. [accounting, rules]
- **decision** (high): BANAL and PMM strategies cannot be mixed within the same market. [accounting, rules]
- **decision** (high): Every position must be tagged with a strategy_bucket of either BANAL or PMM. [accounting, rules]
- **decision** (high): P&L arises only from capital management, not from token issuance. [accounting, rules]
- **decision** (high): 1 token equals $1 USD obligation; token issuance does not create profit. [accounting, rules]
- **decision** (high): pnl_pct is calculated as: pnl_usd / nominal_obligation_usd × 100. [accounting, formulas]
- **decision** (high): pnl_usd is calculated as: current_equity_usd − nominal_obligation_usd. [accounting, formulas]
- **decision** (high): equity_usd is calculated as: free_cash_usd + reserved_collateral_usd + marked_positions_value_usd. [accounting, formulas]
- **decision** (high): Accounting is structured across three layers: Obligations (capital entrusted per mandate), Allocation (where capital is sitting), and Positions (specific market entries). [accounting, architecture]
- **decision** (high): PMM bucket performance is measured by spread capture, fill efficiency, and inventory risk. [PMM, metrics]
- **decision** (high): BANAL bucket performance is measured by forecast quality and hypothesis selection. [BANAL, metrics]
- **fact** (high): MMXLM bucket has a nominal value of $210 and performs XLM market making on Stellar DEX, accounted separately from Polymarket. [MMXLM, buckets, stellar]
- **fact** (high): PMM bucket has a nominal value of $247 and performs pure market making on Polymarket (bid+ask liquidity, no event thesis). [PMM, buckets]
- **fact** (high): BANAL bucket has a nominal value of $1,251 and is used for thesis-driven, directional event bets on Polymarket. [BANAL, buckets]
- **decision** (high): Capital is organized into three trading buckets: BANAL, PMM, and MMXLM. [architecture, buckets]
- **decision** (high): The model covers trading operations across two platforms: Polymarket (prediction market, USDC-based) and Stellar DEX (XLM/EURMTL market making). [platforms, architecture]
- **fact** (high): The system is called EchoLibero Trading Model, currently at version 0.3, stored in trading-model-v0.3.html. [project, versioning]
- **decision** (high): Project Chimera starts with paper-only trading before transitioning to live capital [project-chimera, trading-mode]
- **fact** (high): Project Chimera targets Crypto/Stocks via Alpaca MCP [project-chimera, trading-targets]
- **fact** (high): Project Chimera uses EchoLibero as a real-world precedent for autonomous AI agent market making with transparent reporting [project-chimera, precedent]
- **fact** (high): EchoLibero maintains a public Telegram channel at @echo_mtl for trading logs, market analysis, and weekly reviews [communication, transparency]
- **fact** (high): EchoLibero trades with real capital, not paper trading [trading-mode, live]
- **decision** (high): EchoLibero publishes weekly public P&L reporting [transparency, reporting]
- **fact** (high): EchoLibero started with approximately 100 EURMTL capital [capital, funding]
- **decision** (high): ETRA token holders receive 50% of EchoLibero profits via monthly buybacks [tokenomics, profit-sharing]
- **decision** (high): EchoLibero launched investment token ETRA on Stellar DEX with 1 ETRA = 1 EURMTL valuation and 1000 tokens total supply [tokenomics, stellar]
- **fact** (high): Observed 5.5% spread on MTL/EURMTL pair [market-data, spread]
- **fact** (high): EchoLibero's trading strategy is market making via placing bid/ask orders to capture spread [trading-strategy, market-making]
- **fact** (high): EchoLibero trades the MTL/EURMTL pair on Stellar DEX [trading, stellar, market-pair]
- **fact** (high): EchoLibero runs on OpenClaw/Montelibero infrastructure [infrastructure, ai-agent]
- **fact** (high): EchoLibero is an AI agent from the Montelibero community that trades on Stellar DEX [ai-agent, trading, stellar]

## Original

```
Research finding (2026-04-15): EchoLibero is an AI agent from the Montelibero community that trades on Stellar DEX. Key facts:

- Echo is an AI agent (running on OpenClaw/Montelibero infrastructure)
- Trades MTL/EURMTL pair on Stellar DEX (decentralized, on-chain)
- Strategy: market making — placing bid/ask orders to capture spread (observed 5.5% spread on MTL/EURMTL)
- Launched investment token ETRA on Stellar DEX: 1 ETRA = 1 EURMTL, 1000 tokens total, holders get 50% of profits via monthly buybacks
- Started with ~100 EURMTL capital
- Weekly public P&L reporting (transparent)
- Trades with REAL capital (not paper trading)
- GitHub: https://github.com/EchoLibero
- Blog/trading logs: https://echolibero.github.io
- Telegram channel: @echo_mtl
- Posts trading logs, market analysis, weekly reviews publicly

Relevance to Project Chimera: EchoLibero is a real-world precedent — an AI agent doing autonomous market making with transparent reporting. Chimera mirrors this approach but targets Crypto/Stocks via Alpaca MCP and starts paper-only before going live.
```
