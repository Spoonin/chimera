# Accounting

> 10 active facts · See also: [architecture](architecture.md), [formulas](formulas.md), [rules](rules.md), [trading](trading.md), [transparency](transparency.md)

## Decisions

- [2026-04-15] Realized and unrealized P&L must be tracked separately. *(telegram:@DisterX, high)*
- [2026-04-15] BANAL and PMM strategies cannot be mixed within the same market. *(telegram:@DisterX, high)*
- [2026-04-15] Every position must be tagged with a strategy_bucket of either BANAL or PMM. *(telegram:@DisterX, high)*
- [2026-04-15] P&L arises only from capital management, not from token issuance. *(telegram:@DisterX, high)*
- [2026-04-15] 1 token equals $1 USD obligation; token issuance does not create profit. *(telegram:@DisterX, high)*
- [2026-04-15] pnl_pct is calculated as: pnl_usd / nominal_obligation_usd × 100. *(telegram:@DisterX, high)*
- [2026-04-15] pnl_usd is calculated as: current_equity_usd − nominal_obligation_usd. *(telegram:@DisterX, high)*
- [2026-04-15] equity_usd is calculated as: free_cash_usd + reserved_collateral_usd + marked_positions_value_usd. *(telegram:@DisterX, high)*
- [2026-04-15] Accounting is structured across three layers: Obligations (capital entrusted per mandate), Allocation (where capital is sitting), and Positions (specific market entries). *(telegram:@DisterX, high)*
- [2026-04-15] Use Polymarket for tracking obligations, allocation, positions, and P&L, with versions published to the website *(web:https://echolibero.github.io, high)*
