# Database

> 6 active facts · See also: [schema](schema.md)

## Decisions

- [2026-04-15] RedFlags table schema: severity, scope, message, status. *(telegram:@DisterX, high)*
- [2026-04-15] Snapshots table schema: as_of, equity_usd, realized_pnl, unrealized_pnl, total_pnl. *(telegram:@DisterX, high)*
- [2026-04-15] Positions table schema: market_slug, strategy_bucket, side, qty, avg_entry, mark_price, current_value_usd. *(telegram:@DisterX, high)*
- [2026-04-15] Allocations table schema: mandate_id, free_cash_usd, open_orders_usd, positions_cost_usd, equity_usd, pnl_usd. *(telegram:@DisterX, high)*
- [2026-04-15] Mandates table schema: mandate_id, token, nominal_usd, strategy_type, venue. *(telegram:@DisterX, high)*
- [2026-04-15] The database schema is Grist-ready and includes five tables: Mandates, Allocations, Positions, Snapshots, and RedFlags. *(telegram:@DisterX, high)*
