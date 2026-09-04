# Mahdi Aghakhani

**Finance & Operations Automation Builder** — from manual-process discovery to a system in production.

I came to software from the finance side, not the programming side: financial accountant, founder, then CFO. What I build now is the software finance and operations teams run on — accounting-system integration, bank reconciliation, treasury workflows, pricing engines, period close — and I build it AI-native: I own the requirements, architecture, data model and acceptance criteria, and direct coding agents (Claude Code, Codex) to implement, so a system ships in weeks instead of quarters.

The controls are the product; AI is only the method. A finance team does not buy AI. It buys a system that cannot corrupt the ledger and can be handed to an auditor.

## Client work (2026)

These repos are private under client contract. The claims below are the ones I can defend in a call.

| Client | Industry | What was built | Status |
|---|---|---|---|
| **Taline** | Online melted-gold sales | Read-only integration from the trading-operations system into the accounting software, three accounting modules, Persian panel with Jalali date ranges and exception reports; POS settlements auto-converted to receipt vouchers; gold & currency trial-balance export for audit | **In the client's production since 2026-06-22.** 987 tests as the acceptance gate. The process that took about a month now takes about five minutes, in the words of the system's own user. Bought four times: Phase 1, Phase 2, a supplementary scope, and now treasury & tax. |
| **Soren** | Digital-goods trading | Market-sourcing automation · pricing and marketplace stock-update engine · Torob price-competition engine for the client's storefront · health monitoring across the engines | Delivered. Build-vs-buy was decided by a coverage test, not an opinion: a vendor catalogue matched 76.7% of the client's 206 real rows, and the miss was concentrated in exactly the new launches the analysis existed for. |
| **Hamrah Mechanic** | Auto services | Branch-rollout business plan, breakeven analysis, financial projection, KPI framework with a sales-commission scheme; a competitor price-monitoring system | Delivered. |

What the Taline system guarantees, because a finance buyer should ask: it is read-only by architectural decision, with guards that hard-fail any write to a production address; re-runs cannot double-post (idempotency ledger); credentials are encrypted and access is role-based; and it shipped with a Persian user guide, an update runbook, an incident and backup procedure, signed handover minutes and ADRs.

The treasury platform for the same client — payment-rail routing by amount, an authority matrix, IBAN-versus-name verification, batch return-file handling — is **designed, not built**. Specified in full; bank connection and implementation have not happened.

## Public repos

| Repo | What it shows |
|---|---|
| [**VWare**](https://github.com/mahdincc/VWare) | The pricing and reconciliation platform I built as CFO of Viravin, in .NET/C#: ~5,500 SKU-level listings registered and under management across 16 suppliers, transaction-level reconciliation between sales channel, payment gateway and supplier, SnappShop/TapsiShop integration. 853 C# files, 37 projects, a custom CQRS/mediator framework (GiliX), a `RedactionEngine` that keeps secrets out of logs. |
| **Spider** *(product, available on request)* | Cross-supplier price discovery for the Iranian mobile market: FastAPI + HTMX, live crawlers across 14 suppliers, Dockerized, 351 tests (298 in CI). Not public because it is sold, not shown. Setup on your own systems takes about a week, and the product is under continuous development. Ask by email. |
| [**talafee**](https://github.com/mahdincc/talafee) | Prototype, instance decommissioned: real-time gold-price comparison for the Iranian market, 12 providers normalised every 30 s, cross-provider anomaly detection, trust scoring. |
| [**xPoints**](https://github.com/mahdincc/xPoints) | Explainable, self-calibrating football prediction engine: EV-optimal decisions from de-vigged odds, self-grading backtests, Brier calibration, 62 tests. |

Spider validated the idea that VWare then scaled inside Viravin; Spider is now the standalone product. Marketplace pricing and crawlers are the engineering range; finance systems are the job.

## Before this

- **Viravin** — Co-founder & CFO (2022–2024). Budgeting, forecasting, treasury planning, investor reporting, finance controls, and the tooling behind them (VWare).
- **Netmanzel** — Founder (2018–2021). Finance controls and operational reporting across online, retail and manufacturing.
- **Bamilo** (Rocket Internet) — Business development, then financial accountant (2015–2018). Product owner, from the finance side, of Crabs: the automated customer-refund engine, with a status-driven queue, bank response handling and a manual exception queue.

## How an engagement runs

1. A free 30-minute call. I listen and say honestly whether the problem is worth automating.
2. Process discovery with each stakeholder: an AS-IS map and a TO-BE requirements set.
3. A proposal for the path from one to the other, with a measurable acceptance test per step on the client's own data.
4. Build, deploy in the client's environment, hand over with training and documentation.
5. Monthly support and continuous improvement.

## Contact

[LinkedIn](https://linkedin.com/in/mahdi-aghakhani) · aghaa.mahdi@gmail.com
