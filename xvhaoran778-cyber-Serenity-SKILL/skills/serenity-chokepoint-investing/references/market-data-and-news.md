# Market Data and News Ingestion

Use this reference for live Serenity-style analysis across A-shares, US stocks, Hong Kong stocks, Taiwan, Japan, Europe, and other markets.

## Core Rule

Yes: include company news and official announcements for live use. Serenity-style research depends on Bayesian updates. Recent disclosures, customer wins, capex plans, subsidies, earnings calls, dilution, and negative reports can materially change the posterior probability that a company is a true bottleneck.

Do not scrape news indiscriminately. Prioritize primary sources first, then use news and social posts as leads.

## Source Priority

| Priority | Source type | Use |
|---:|---|---|
| 1 | Exchange filings, regulatory announcements, annual/interim/quarterly reports | Authoritative facts, financing, related-party transactions, customer risk, capacity plans |
| 2 | Company IR pages, investor decks, earnings calls, transcripts | Segment detail, backlog, capacity, guidance, customer language |
| 3 | Government documents, subsidies, export-control, industrial policy | Strategic criticality and capex backstop |
| 4 | Customer/vendor technical docs and product pages | BOM role, qualification, architecture specificity |
| 5 | Reputable news/industry media/research excerpts | Timely leads and market framing |
| 6 | Social posts/forums | Idea generation only; require verification |

## Market-Specific Checklist

### A-shares

Check:

- Exchange and official disclosure portals: SSE, SZSE, BSE, 巨潮资讯/CNINFO.
- Company announcements: annual reports, semiannual reports, quarterly reports, investor relations activity records, private placement/refinancing, major contracts, related-party transactions.
- Interactive platforms when relevant: 上证 e 互动, 深交所互动易. Treat management replies as useful but lower authority than filings.
- Chinese industry media and policy documents for demand shocks, subsidies, localization, export controls, and procurement.
- Liquidity, daily limit-up/down behavior, shareholder pledges, unlocks, ST risk, refinancing pressure, and retail narrative risk.

### US stocks

Check:

- SEC EDGAR: 10-K, 10-Q, 8-K, S-3/ATM, prospectuses, insider ownership when relevant.
- Company IR: earnings releases, transcripts, presentations, customer announcements.
- Customer/vendor filings and product pages for supply-chain corroboration.
- Short reports, dilution, warrants, convertibles, and going-concern language for small caps.
- Index inclusion, uplisting, Nasdaq/NYSE compliance, and liquidity.

### Hong Kong stocks

Check:

- HKEXnews / 披露易: announcements, annual/interim reports, placing, rights issue, connected transactions, inside information.
- Company IR and investor presentations.
- China/HK policy exposure, customer concentration, mainland operating subsidiaries, VIE/holding structure if relevant.
- Liquidity, ownership concentration, placing history, and related-party risk.

### Taiwan / Japan / Europe

Check:

- Local exchange disclosures and company IR.
- Annual reports, investor decks, material information filings.
- Government subsidy and industrial-policy sources.
- Customer/vendor qualification evidence.
- FX, liquidity, foreign ownership, and accounting-standard comparability.

## News-to-Evidence Triage

Classify each item:

- **Thesis-confirming:** customer qualification, backlog/revenue beat, segment growth, subsidy, capacity expansion, standard adoption, pricing power.
- **Thesis-weakening:** substitution, design-out, customer insourcing, failed ramp, margin compression, dilution, governance issue, demand fade.
- **Neutral/noise:** stock-price commentary, popularity, unsourced social claims, repeated old news.

For each important news item, write:

`Item -> source -> date -> thesis impact -> evidence strength -> follow-up check`

## Minimum Live Analysis Standard

Before issuing a current view on a company:

1. Verify ticker, exchange, market cap, and latest filing period.
2. Check recent official disclosures from the last 3-6 months; use 12 months for small caps or fast-changing sectors.
3. Check whether there are financings, dilution, customer losses, regulatory issues, or major contracts.
4. Check at least one source that can validate the supply-chain role.
5. State unresolved gaps instead of filling them with narrative.

## Output Add-On

Add this section when using live company news:

```markdown
## News and Disclosure Update
| Date | Source | Item | Thesis impact | Evidence strength | Follow-up |
|---|---|---|---|---|---|
```
