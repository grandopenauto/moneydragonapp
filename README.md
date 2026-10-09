# MoneyDragonApp

**Intelligence beyond the brokerage.**

This repository contains the **public-facing website** for MoneyDragonApp, an in-development financial intelligence and trading research concept from Highest Degree Priorities.

Visit the source preview by enabling GitHub Pages on this repository (Settings → Pages → Deploy from a branch → main → /root). GitHub Pages supports only static content; this repository intentionally contains **no brokerage authentication, execution backend, trading engine or secrets**.

## Product direction

- Brokerage-connected market and portfolio research
- Options strategy analysis and defined-risk scenario modeling
- Daily intelligence and evidence-based strategy review
- Human approval and strict boundaries between research, simulation and order execution
- Provider-specific integration support only where technically, contractually, and legally permitted

These are proposed capabilities. The public landing page does not connect to broker APIs or supply live market information.

## Operating architecture

| Surface | Intended location |
| --- | --- |
| Public marketing site | This GitHub repository / GitHub Pages |
| Private MoneyDragon runtime | HDP Windows VPS: `C:\HDP\MoneyDragon` |
| Deployment channel | Privately staged Google Drive artifacts + approved VPSBridge queue + audited receipts |
| Credentials, OAuth tokens and trading operations | VPS-local secure storage and controlled services only |

Never commit real tokens, keys, customer financial information, trade histories, brokerage account identifiers, or private application code here.

## Website publishing

1. Open repository **Settings → Pages**.
2. Set **Build and deployment** to **Deploy from a branch**.
3. Select **main** and **/(root)**, then Save.
4. Confirm the Pages site works before changing any custom-domain DNS.
5. Keep existing MoneyDragon/Schwab OAuth callback routing unchanged until any proposed migration has been separately validated.

## Risk notice

This website is a concept preview, not investment advice or a brokerage service. Financial instruments, especially options, involve risk. No performance is guaranteed.

© Highest Degree Priorities.